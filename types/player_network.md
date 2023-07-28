# network

## Methods

| Method                                                                                                                             | Return Type | Description                             |
|------------------------------------------------------------------------------------------------------------------------------------|-------------|-----------------------------------------|
| `send_transaction(windowID: int, action: short, accepted: boolean, triggerEvent: boolean)`                                         | `void`      | Sends a transaction packet              |
| `send_keep_alive(key: int, triggerEvent: boolean)`                                                                                 | `void`      | Sends a keep alive packet               |
| `send_player(ground: boolean, triggerEvent: boolean)`                                                                              | `void`      | Sends a player packet                   |
| `send_player_position(x: double, y: double, z: double, ground: boolean, triggerEvent: boolean)`                                    | `void`      | Sends a player position packet          |
| `send_player_rotation(yaw: float, pitch: float, ground: boolean, triggerEvent: boolean)`                                           | `void`      | Sends a player rotation packet          |
| `send_player_position_rotation(x: double, y: double, z: double, yaw: float, pitch: float, ground: boolean, triggerEvent: boolean)` | `void`      | Sends a player position rotation packet |
| `send_attack(entity: Entity, triggerEvent: boolean)`                                                                               | `void`      | Sends an attack packet                  |