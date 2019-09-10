Debugging Longan Nano
======

## Connect the debugger
| Development board | Debugger |
| :----: | :----: |
|  JTDO  |  TDO   |
|  JTDI  |  TDI   |
|  JTCK  |  TCK   |
|  JTMS  |  TMS   |
|  3V3   |  3V3   |
|  GND   |  GND   |

## Modify the configuration file
Modify the project configuration file `platformio.ini`, add `debug_tool = jlinkit` below , and select it according to the actual debugger model. Currently supports Jlink, GD-LINK, and other debuggers to be added.

## One-click debugging

VSCode switch to the left side of the `DEBUG` screen, click the green arrow to debug.

![](assets/../../../assets/longan_pio_debug.jpg).