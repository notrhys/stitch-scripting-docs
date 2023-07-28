# Player Move Event

The `PlayerMoveEvent` is fired when the player moves.

## Event Class

You can listen for this event using the `on_player_move` method from a module.

```lua
module.events.on_player_move(function(event)

end)
```

## Event Fields

| Field     | Type     | Description           |
|-----------|----------|-----------------------|
| `event.x` | `double` | The player's X motion |
| `event.y` | `double` | The player's Y motion |
| `event.z` | `double` | The player's Z motion |

## Event Methods

| Method                           | Return Type | Description           |
|----------------------------------|-------------|-----------------------|
| `event.cancel()`                 | `void`      | Cancels the event     |
| `event.set_speed(speed: double)` | `void`      | Sets the player speed |
