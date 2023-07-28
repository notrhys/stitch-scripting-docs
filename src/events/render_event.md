# Render Event

The `RenderEvent` is fired when the client renders anything to the screen.

## Event Class

You can listen for this event using the `on_render` method from a module.

```lua
module.events.on_render(function(event)

end)
```

## Event Fields

| Field                 | Type     | Description                                                                                                                                    |
|-----------------------|----------|------------------------------------------------------------------------------------------------------------------------------------------------|
| `event.scaled_width`  | `double` | The window's scaled width                                                                                                                      |
| `event.scaled_height` | `double` | The window's scaled height                                                                                                                     |
| `event.partial_ticks` | `float`  | The client's render partial ticks                                                                                                              |
| `event.state`         | `string` | The state of the event, can be `before_overlay`, `overlay`, `world_pass`, `screen`, `view_bobbing`, `hurt_cam`, `world`, `camera`, `main_menu` |

## Event Methods

| Method           | Return Type | Description       |
|------------------|-------------|-------------------|
| `event.cancel()` | `void`      | Cancels the event |