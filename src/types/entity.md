# Entity

| Method                      | Return Type                     | Description                                    |
|-----------------------------|---------------------------------|------------------------------------------------|
| `isDead()`                  | `boolean`                       | Whether or not the entity is dead              |
| `isPlayer()`                | `boolean`                       | Returns true if the entity is a player         |
| `isLocalPlayer()`           | `boolean`                       | Returns true if the entity is the local player |
| `getMotionX()`              | `double`                        | Gets the entity's motion X                     |
| `getMotionY()`              | `double`                        | Gets the entity's motion Y                     |
| `getMotionZ()`              | `double`                        | Gets the entity's motion Z                     |
| `getYaw()`                  | `float`                         | Gets the entity's rotation yaw                 |
| `getPitch()`                | `float`                         | Gets the entity's rotation pitch               |
| `getName()`                 | `string`                        | Gets the entity's name                         |
| `getUniqueID()`             | `string`                        | Gets the entity's UUID                         |
| `getID()`                   | `int`                           | Gets the entity's entity id                    |
| `getHealth()`               | `float`                         | Gets the entity's health                       |
| `hasEffect()`               | `boolean`                       | Whether or not the entity has an effect        |
| `player.getEffect(id: int)` | [Effect](../types/effect.md)    | Gets the effect with the id                    |
| `player.getActiveEffects()` | [Effect](../types/effect.md)\[] | Gets all the entity's active effects           |