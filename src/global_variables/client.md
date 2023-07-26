# client

The client global variable gives access to important client-side functions.

## Methods

| Method                                                                       | Return Type                     | Description                                                   |
|------------------------------------------------------------------------------|---------------------------------|---------------------------------------------------------------|
| `client.registerModule(name: string, description: string, category: string)` | [Script](../types/script.md)    | Registers a module on the client and gives the instance of it |
| `client.getModule(name: string)`                                             | [Module](../types/module.md)    | Gets a module by name                                         |
| `client.getEnabledModules()`                                                 | [Module](../types/module.md)\[] | Gets all enabled modules                                      |
| `client.getProtocolVersion()`                                                | `int`                           | Gets the current protocol version (ViaVersion Protocol)       |
| `client.getName()`                                                           | `string`                        | Gets the client name                                          |
| `client.getBuildID()`                                                        | `string`                        | Gets the client build ID                                      |
| `client.getUsername()`                                                       | `string`                        | Gets the client user username                                 |
| `client.getUserID()`                                                         | `string`                        | Gets the client user userID                                   |
| `client.isClientUser(minecraftName: string)`                                 | `boolean`                       | Whether or not the minecraft username is a client user        |
| `client.getFPS()`                                                            | `int`                           | Gets the client FPS                                           |
| `client.currentTimeMillis()`                                                 | `int`                           | Gets the current time in milliseconds                         |
| `client.nanoTime()`                                                          | `int`                           | Gets the current time in nanoseconds                          |