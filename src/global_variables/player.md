# player

The player global variable gives access to client local player functions.

## Fields

| Field                          | Type            | Description                    |
|--------------------------------|-----------------|--------------------------------|
| [network](./player_network.md) | `PlayerNetwork` | The player's networking access |

## Methods

| Method                                                     | Return Type                      | Description                                         |
|------------------------------------------------------------|----------------------------------|-----------------------------------------------------|
| `player.exists()`                                          | `boolean`                        | Whether or not the player exists                    |
| `player.getMotionX()`                                      | `double`                         | Gets the player's motion X                          |
| `player.getMotionY()`                                      | `double`                         | Gets the player's motion Y                          |
| `player.getMotionZ()`                                      | `double`                         | Gets the player's motion Z                          |
| `player.setMotionX(motionX: double)`                       | `void`                           | Sets the player's motion X                          |
| `player.setMotionY(motionY: double)`                       | `void`                           | Sets the player's motion Y                          |
| `player.setMotionZ(motionZ: double)`                       | `void`                           | Sets the player's motion Z                          |
| `player.getYaw()`                                          | `float`                          | Gets the player's rotation yaw                      |
| `player.setYaw(yaw: float)`                                | `float`                          | Sets the player's rotation yaw                      |
| `player.getPitch()`                                        | `float`                          | Gets the player's rotation pitch                    |
| `player.setPitch(pitch: float)`                            | `float`                          | Sets the player's rotation pitch                    |
| `player.setSpeed(speed: double)`                           | `void`                           | Sets the player's speed                             |
| `player.getSpeed()`                                        | `double`                         | Gets the player's speed                             |
| `player.getHealth()`                                       | `float`                          | Gets the player's health                            |
| `player.jump()`                                            | `void`                           | Makes the player jump                               |
| `player.getCurrentItemIndex()`                             | `int`                            | Gets the current item index                         |
| `player.setCurrentItemIndex()`                             | `void`                           | Sets the current item index                         |
| `player.getName()`                                         | `string`                         | Gets the player's name                              |
| `player.getUniqueID()`                                     | `string`                         | Gets the player's UUID                              |
| `player.getID()`                                           | `int`                            | Gets the player's entity id                         |
| `player.hasEffect(id: int)`                                | `boolean`                        | Whether or not the player has an effect with the id |
| `player.getEffect(id: int)`                                | [Effect](../types/effect.md)     | Gets the effect with the id                         |
| `player.getActiveEffects()`                                | [Effect](../types/effect.md)\[]  | Gets all the player's active effects                |
| `player.addEffect(id: int, duration: int, amplifier: int)` | `void`                           | Adds an effect to the player                        |
| `player.attack(entity: Entity)`                            | `void`                           | Attacks an entity                                   |
| `player.isSneaking()`                                      | `boolean`                        | Whether or not the player is sneaking               |
| `player.isSprinting()`                                     | `boolean`                        | Whether or not the player is sprinting              |
| `player.swingItem()`                                       | `void`                           | Swings the player's item                            |
| `player.isBlocking()`                                      | `boolean`                        | Whether or not the player is blocking a sword       |
| `player.isDead()`                                          | `boolean`                        | Whether or not the player is dead                   |
| `player.getDistanceToEntity(entity: Entity)`               | `double`                         | Gets the distance to an entity                      |
| `player.getRotationToEntity(entity: Entity)`               | [Vector2f](../types/vector2f.md) | Gets the rotation to an entity                      |