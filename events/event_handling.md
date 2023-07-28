# Event Handling

### Listening for events:

```lua
local module = client.register_module("Name", "Description", "Category")

module.on_enable(function()

end)

module.on_disable(function()

end)

module.events.on_game_loop(function()

end)

module.events.on_game_tick(function()

end)

module.events.on_player_motion(function(event)

end)

module.events.on_player_move(function(event)

end)

module.events.on_player_move_flying(function(event)

end)

module.events.on_render(function(event)

end)
```