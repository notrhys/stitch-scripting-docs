# local_player()

The local_player() global method gives access to the local player instance.

## Fields

| Method                   | Return Type                                 | Description                        |
|--------------------------|---------------------------------------------|------------------------------------|
| `local_player().network` | [PlayerNetwork](../types/player_network.md) | The local player's network access. |

## Methods

| Method                                  | Return Type | Description                           |
|-----------------------------------------|-------------|---------------------------------------|
| `local_player().jump()`                 | `void`      | Jump.                                 |
| `local_player().attack(entity: Entity)` | `void`      | Attacks an entity.                    |
| `local_player().swing_item()`           | `void`      | Swings the item in the player's hand. |
| `set_speed(speed: double)`              | `void`      | Sets the player's speed               |
| `get_speed()`                           | `double`    | Gets the player's speed               |