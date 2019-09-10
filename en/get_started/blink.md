Getting to Blinky
=====

## Create a LED Blink project

* Open the PIO home page selection `Project Examples`

![](http://blog.sipeed.com/wp-content/uploads/2019/04/d977e844490e6ccc4625f701883a29f5.png)

* Select `arduino blink` Click `Import` Import sample program (first need to download the schema file and import tool, It may take long time to download)
![](http://blog.sipeed.com/wp-content/uploads/2019/04/82943a6b74077e6210e2d9421cb5438f.png)


* You can see the sample project after the import is successful.
![](http://blog.sipeed.com/wp-content/uploads/2019/04/1262373ca7b0b483e30dac1124adaabf.png)

## Project configuration file


* We first need to edit the configuration file works `platformio.ini` according to their own development board model, delete the other development board environments.

![](assets/../../../assets/pio_ini_cfg.png)

Configuration example
```ini
[env:sipeed-longan-nano]
platform = gd32v          ;Platform, choose gd32v
framework = arduino       ;Optional gd32vf103_firmware_library or arduino
board = sipeed-longan-nano ; Development board
monitor_speed = 115200     ; Serial monitor baudrate
upload_tool = serial       ; Download tool Default serial port, optional jlink, gd-link, dfu, etc.
debug_tool = jlink         ; Debugging tool default jlink, optional gd-link
```

## One-click compilation

Click on the lower left corner `Build` to build the project
![](http://blog.sipeed.com/wp-content/uploads/2019/04/a826bb03ebfe5226fa3bcc336179e763.png)

## Connect to the development board
### Serial ISP download
* Prepare the USB to serial downloader
* Connect development board and downloader
* Development board hold down the `BOOT` key, then press the `RESET` button to restart development board and then release the `BOOT` button to enter download mode development board.

### JTAG download
* Prepare J-link or GD-Link
* Connection development board

### USB DFU download
Download the DFU tool：http://dl.sipeed.com/LONGAN/Nano/Tools/GD32_MCU_Dfu_Tool_V3.8.1.5784_1.rar

Unzip two folders：

GD32 MCU Dfu Drivers_v1.0.1.2316 and GD32 MCU Dfu Tool_v3.8.1.5784

First enter the driver folder, install the corresponding driver file, pay attention to run with administrator privileges

![](../../zh/examples/assets/how_to_install_dfu.png)

Run GD32 MCU Dfu Tool.exe Insert Longan Nano into the computer, press and hold the Boot0 key, short press the Reset key, then release the Boot0 key, you can see that the GD32VF chip is recognized in the DFU tool.

Select the corresponding firmware file, and check the checksum after burning. Click OK to burn.

After the burning is completed, it will not be reset automatically. You need to manually press the reset button to check the running effect.

![](../../zh/examples/assets/how_to_use_dfu.png)

## One click download

Click on the lower left corner `Upload` to upload program.
