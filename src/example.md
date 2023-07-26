# Example Module

```js
let module = client.registerModule("Script Aura", "A script aura", "Combat")

let swing = module.settings.registerBoolean("Swing", true)
let keepSprint = module.settings.registerBoolean("Keep Sprint", true)

let cps = module.settings.registerNumber("CPS", 1, 20, 14, 1)
let distance = module.settings.registerNumber("Distance", 3, 6, 4.2, 0.1)

let timer = classAccess.newTimer()

module.events.onPlayerMotion((event) => {
    if (event.state != "pre")
        return

    let nearestEntity = getNearestEntity()

    if (nearestEntity == null)
        return

    let rotation = player.getRotationToEntity(nearestEntity)

    event.yaw = rotation.x
    event.pitch = rotation.y

    if (timer.hasReached(1000 / cps.get())) {
        timer.reset()

        if (swing.get())
            player.swingItem()

        if (keepSprint.get()) {
            player.network.sendAttack(nearestEntity, true)
        } else {
            player.attack(nearestEntity)
        }
    }
})

let getNearestEntity = () => {
    let nearestEntity

    for (let entity of world.getEntities()) {
        if (entity.isLocalPlayer())
            continue

        if (!entity.isPlayer())
            continue

        if (entity.isDead())
            continue

        if (player.getDistanceToEntity(entity) > distance.get())
            continue

        if (nearestEntity == null || player.getDistanceToEntity(entity) < player.getDistanceToEntity(nearestEntity))
            nearestEntity = entity
    }

    return nearestEntity
}
```
