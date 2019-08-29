Debug 调试
======

## 连接调试器
| 开发板 | 调试器 |
| :----: | :----: |
|  JTDO  |  TDO   |
|  JTDI  |  TDI   |
|  JTCK  |  TCK   |
|  JTMS  |  TMS   |
|  3V3   |  3V3   |
|  GND   |  GND   |

## 修改配置文件
修改工程配置文件 `platformio.ini`， 在下面添加 `debug_tool = jlink` ，根据实际调试器型号选择。目前支持Jlink 、GD-LINK ，其他调试器待添加。

## 一键调试

切换到 VS CODE 左侧的 `DEBUG` 界面， 点击绿色箭头即可进行调试。

![](assets/../../../assets/longan_pio_debug.jpg).