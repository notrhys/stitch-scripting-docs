# Player Move Flying Event

The `PlayerMoveFlyingEvent` is fired when the client calls the moveFlying method.

## Event Class

You can listen for this event using the `onPlayerMoveFlying` method from a module.

```js
module.events.onPlayerMoveFlying((event) => {

})
```

## Event Fields

| Field            | Type    | Description          |
|------------------|---------|----------------------|
| `event.strafe`   | `float` | The event's strafe   |
| `event.forward`  | `float` | The event's forward  |
| `event.friction` | `float` | The event's friction |
| `event.yaw`      | `float` | The event's yaw      |

## Event Methods

| Method                           | Return Type | Description                       |
|----------------------------------|-------------|-----------------------------------|
| `event.cancel()`                 | `void`      | Cancels the event                 |
| `event.silentStrafe(yaw: float)` | `void`      | Strafes towards the specified yaw |
