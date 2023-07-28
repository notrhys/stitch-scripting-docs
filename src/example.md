# Example Module

```lua
local module = client.register_module("Script Aura", "Aura made with a lua script", "Combat")

local swing = module.settings.register_boolean("Swing", true)
local keep_sprint = module.settings.register_boolean("Keep Sprint", true)

local cps = module.settings.register_number("CPS", 1, 20, 14, 1)
local distance = module.settings.register_number("Distance", 3, 6, 4.2, 0.1)

local click_timer = Timer.new()

module.events.on_player_motion(function(event)
    if not event.state == "pre" then
        return
    end

    local target = get_target()

    if target then
        local rotation = local_player().get_rotation_to_entity(target)

        event.yaw = rotation.x
        event.pitch = rotation.y

        if click_timer.has_reached(1000 / cps.get()) then
            click_timer.reset()

            if swing.get() then
                local_player().swing_item()
            end

            if keep_sprint.get() then
                local_player().network.send_attack(target, true)
            else
                local_player().attack(target)
            end
        end
    end
end)

function get_target()
    local target

    local i = 1
    local entities = world.get_entities()

    while entities[i] do
        local entity = entities[i]

        if not entity.is_local_player() then
            if entity.is_player() then
                if not entity.is_dead() then
                    local target_distance = local_player().get_distance_to_entity(entity)

                    if target_distance <= distance.get() then
                        if not target or target_distance < local_player().get_distance_to_entity(target) then
                            target = entity
                        end
                    end
                end
            end
        end

        i = i + 1
    end

    return target
end
```