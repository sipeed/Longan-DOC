Blink 闪灯程序
=====

## 创建 Blink 工程

* 打开 PIO 主页 选择 `Project Examples`

![](http://blog.sipeed.com/wp-content/uploads/2019/04/d977e844490e6ccc4625f701883a29f5.png)

* 选择 `arduino blink` 点击 `Import` 导入示例程序 （初次导入需要下载架构文件及工具，需要等待较长时间）
![](http://blog.sipeed.com/wp-content/uploads/2019/04/82943a6b74077e6210e2d9421cb5438f.png)

* 导入成功后即可见到示例工程
![](http://blog.sipeed.com/wp-content/uploads/2019/04/1262373ca7b0b483e30dac1124adaabf.png)

## 工程配置文件


* 我们首先需要编辑工程配置文件 `platformio.ini` 根据自己的开发板型号，删掉其他开发板环境。

![](assets/../../../assets/pio_ini_cfg.png)

配置示例
```ini
[env:sipeed-longan-nano]
platform = gd32v          ;平台，选择gd32v
framework = arduino       ;可选 gd32vf103_firmware_library 或 arduino
board = sipeed-longan-nano ; 开发板
monitor_speed = 115200     ; 串口监视器botelv
upload_tool = serial       ; 下载工具 默认串口， 可选jlink、gd-link、dfu等
debug_tool = jlink         ; 调试工具 默认jlink ，可选gd-link
```

## 一键编译

点击左下角的 `Build` 即可构建项目
![](http://blog.sipeed.com/wp-content/uploads/2019/04/a826bb03ebfe5226fa3bcc336179e763.png)

## 连接开发板
### 串口 ISP 下载
* 准备USB 转 串口下载器
* 连接开发板与下载器
* 开发板按住 `BOOT` 键，再按 `RESET` 键重启开发板后再松开 `BOOT` 键，开发板进入下载模式。
  
### JTAG 下载
* 准备J-link 或 GD-Link 
* 连接开发板
  
### USB DFU 下载
* 待添加

## 一键下载

点击左下角的 `Upload` 即可上传程序。

