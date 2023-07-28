# Module

The module class provides access to client modules.

## Methods

| Method                                    | Return Type | Description                            |
|-------------------------------------------|-------------|----------------------------------------|
| `toggle(state: boolean)`                  | `void`      | Toggles the module on or off           |
| `is_enabled()`                            | `boolean`   | Returns true if the module is enabled  |
| `get_name()`                              | `string`    | Returns the name of the module         |
| `get_boolean_setting_value(name: string)` | `boolean`   | Returns the value of a boolean setting |
| `get_number_setting_value(name: string)`  | `double`    | Returns the value of a number setting  |