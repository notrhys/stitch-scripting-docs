# Module

The module class provides access to client modules.

## Methods

| Method                                 | Return Type | Description                            |
|----------------------------------------|-------------|----------------------------------------|
| `toggle(state: boolean)`               | `void`      | Toggles the module on or off           |
| `isEnabled()`                          | `boolean`   | Returns true if the module is enabled  |
| `getName()`                            | `string`    | Returns the name of the module         |
| `getBooleanSettingValue(name: string)` | `boolean`   | Returns the value of a boolean setting |
| `getNumberSettingValue(name: string)`  | `double`    | Returns the value of a number setting  |