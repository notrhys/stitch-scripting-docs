# Player Move Event

The `PlayerMoveEvent` is fired when the player moves.

## Event Class

You can listen for this event using the `onPlayerMove` method from a module.

```js
module.events.onPlayerMove((event) => {

})
```

## Event Fields

| Field     | Type     | Description           |
|-----------|----------|-----------------------|
| `event.x` | `double` | The player's X motion |
| `event.y` | `double` | The player's Y motion |
| `event.z` | `double` | The player's Z motion |

## Event Methods

| Method                          | Return Type | Description           |
|---------------------------------|-------------|-----------------------|
| `event.cancel()`                | `void`      | Cancels the event     |
| `event.setSpeed(speed: double)` | `void`      | Sets the player speed |
