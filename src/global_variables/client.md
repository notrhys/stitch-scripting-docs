# client

The client global variable gives access to important client-side functions.

## Methods

| Method                                                                        | Return Type                     | Description                                                   |
|-------------------------------------------------------------------------------|---------------------------------|---------------------------------------------------------------|
| `client.register_module(name: string, description: string, category: string)` | [Script](../types/script.md)    | Registers a module on the client and gives the instance of it |
| `client.get_module(name: string)`                                             | [Module](../types/module.md)    | Gets a module by name                                         |
| `client.get_all_modules()`                                                    | [Module](../types/module.md)\[] | Gets all modules                                              |
| `client.get_protocol_version()`                                               | `int`                           | Gets the current protocol version (ViaVersion Protocol)       |
| `client.get_name()`                                                           | `string`                        | Gets the client name                                          |
| `client.get_build_id()`                                                       | `string`                        | Gets the client build ID                                      |
| `client.get_username()`                                                       | `string`                        | Gets the client user username                                 |
| `client.get_user_id()`                                                        | `string`                        | Gets the client user userID                                   |
| `client.is_client_user(minecraftName: string)`                                | `boolean`                       | Whether or not the minecraft username is a client user        |
| `client.get_fps()`                                                            | `int`                           | Gets the client FPS                                           |
| `client.current_time_millis()`                                                | `int`                           | Gets the current time in milliseconds                         |
| `client.nano_time()`                                                          | `int`                           | Gets the current time in nanoseconds                          |