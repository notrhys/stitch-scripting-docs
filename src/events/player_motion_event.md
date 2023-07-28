# Player Motion Event

The `PlayerMotionEvent` is fired when the player sends movement packets.

## Event Class

You can listen for this event using the `on_player_motion` method from a module.

```lua
module.events.on_player_motion(function(event)

end)
```

## Event Fields

| Field             | Type      | Description                                  |
|-------------------|-----------|----------------------------------------------|
| `event.x`         | `double`  | The player's X position                      |
| `event.y`         | `double`  | The player's Y position                      |
| `event.z`         | `double`  | The player's Z position                      |
| `event.yaw`       | `float`   | The player's yaw                             |
| `event.pitch`     | `float`   | The player's pitch                           |
| `event.on_ground` | `boolean` | Whether or not the player is on the ground   |
| `event.state`     | `string`  | The state of the event, can be `pre`, `post` |

## Event Methods

| Method                        | Return Type | Description           |
|-------------------------------|-------------|-----------------------|
| `event.cancel()`              | `void`      | Cancels the event     |