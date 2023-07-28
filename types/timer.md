# Timer

The `Timer` class is used to keep track of time. It can be used to check if a certain amount of time has passed since
the last time it was reset.

## Methods

| Method                      | Return Type | Description                                                              |
|-----------------------------|-------------|--------------------------------------------------------------------------|
| `has_reached(time: double)` | `boolean`   | Returns true if the given amount of time has passed since the last reset |
| `reset()`                   | `void`      | Resets the timer                                                         |
