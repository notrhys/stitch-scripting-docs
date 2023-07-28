# Entity

| Method                                               | Return Type                     | Description                                     |
|------------------------------------------------------|---------------------------------|-------------------------------------------------|
| `is_dead()`                                          | `boolean`                       | Whether or not the entity is dead               |
| `is_player()`                                        | `boolean`                       | Returns true if the entity is a player          |
| `is_local_player()`                                  | `boolean`                       | Returns true if the entity is the local player  |
| `get_motion_x()`                                     | `double`                        | Gets the entity's motion X                      |
| `get_motion_y()`                                     | `double`                        | Gets the entity's motion Y                      |
| `get_motion_z()`                                     | `double`                        | Gets the entity's motion Z                      |
| `set_motion_x(motionX: double)`                      | `void`                          | Sets the player's motion X                      |
| `set_motion_y(motionY: double)`                      | `void`                          | Sets the player's motion Y                      |
| `set_motion_z(motionZ: double)`                      | `void`                          | Sets the player's motion Z                      |
| `get_yaw()`                                          | `float`                         | Gets the entity's rotation yaw                  |
| `get_pitch()`                                        | `float`                         | Gets the entity's rotation pitch                |
| `set_yaw(yaw: float)`                                | `float`                         | Sets the player's rotation yaw                  |
| `set_pitch(pitch: float)`                            | `float`                         | Sets the player's rotation pitch                |
| `get_name()`                                         | `string`                        | Gets the entity's name                          |
| `get_unique_id()`                                    | `string`                        | Gets the entity's UUID                          |
| `get_id()`                                           | `int`                           | Gets the entity's entity id                     |
| `get_health()`                                       | `float`                         | Gets the entity's health                        |
| `get_max_health()`                                   | `float`                         | Gets the entity's max health                    |
| `get_armor()`                                        | `int`                           | Gets the entity's armor                         |
| `get_hurt_time()`                                    | `int`                           | Gets the entity's hurt time                     |
| `has_effect(id: int)`                                | `boolean`                       | Whether or not the entity has an effect         |
| `get_effect(id: int)`                                | [Effect](../types/effect.md)    | Gets the effect with the id                     |
| `get_active_effects()`                               | [Effect](../types/effect.md)\[] | Gets all the entity's active effects            |
| `add_effect(id: int, duration: int, amplifier: int)` | `void`                          | Adds an effect to the player                    |
| `get_held_item_index()`                              | `int`                           | Gets the index of the item in the player's hand |
| `set_held_item_index(slot: int)`                     | `void`                          | Sets the index of the item in the player's hand |
| `is_blocking()`                                      | `boolean`                       | Whether or not the entity is blocking           |
| `get_distance_to_entity(entity: Entity)`             | `double`                        | Gets the distance to the given entity           |
| `get_distance_to(x: double, y: double, z: double)`   | `double`                        | Gets the distance to the given position         |
| `get_rotation_to_entity(entity: Entity)`             | [Entity](../types/entity.md)    | Gets the rotation to the given entity           |
| `is_sneaking()`                                      | `boolean`                       | Whether or not the entity is sneaking           |
| `is_sprinting()`                                     | `boolean`                       | Whether or not the entity is sprinting          |