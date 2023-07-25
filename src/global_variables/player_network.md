# player.network

The player.network global variable gives access to the player's networking access.

## Methods

| Method                                                                                                                                         | Return Type | Description                             |
|------------------------------------------------------------------------------------------------------------------------------------------------|-------------|-----------------------------------------|
| `player.network.sendTransaction(windowID: int, action: short, accepted: boolean, triggerEvent: boolean)`                                       | `void`      | Sends a transaction packet              |
| `player.network.sendKeepAlive(key: int, triggerEvent: boolean)`                                                                                | `void`      | Sends a keep alive packet               |
| `player.network.sendPlayer(ground: boolean, triggerEvent: boolean)`                                                                            | `void`      | Sends a player packet                   |
| `player.network.sendPlayerPosition(x: double, y: double, z: double, ground: boolean, triggerEvent: boolean)`                                   | `void`      | Sends a player position packet          |
| `player.network.sendPlayerRotation(yaw: float, pitch: float, ground: boolean, triggerEvent: boolean)`                                          | `void`      | Sends a player rotation packet          |
| `player.network.sendPlayerPositionRotation(x: double, y: double, z: double, yaw: float, pitch: float, ground: boolean, triggerEvent: boolean)` | `void`      | Sends a player position rotation packet |
| `player.network.sendAttack(entity: Entity, triggerEvent: boolean)`                                                                             | `void`      | Sends an attack packet                  |