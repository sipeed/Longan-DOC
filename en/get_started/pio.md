PIO configuration
=====

## Install VSCode
VS CODE is a more common development tool. Go to the VSCode official website and download and install the installation package for the corresponding operating system version.

## Install the PIO plugin
Open VSCode -> click on the left extension -> search for PlatformIO -> click install plugin -> wait for the installation to complete

![](http://blog.sipeed.com/wp-content/uploads/2019/04/0d501a8515a735fba54e2f5de908cd1e.png)

## Install the GD32V platform definition

Click the PlatformIO logo on the left -> click New Terminal at the bottom left -> execute the following installation command in the terminal window

* Development version (synchronized with Github)
```
platformio platform install https://github.com/sipeed/platform-gd32v
```
![](http://blog.sipeed.com/wp-content/uploads/2019/04/c79100e1ed1747988f001d7471cd1064.png)
 
Note: Due to the domestic network environment, the installation process takes a long time, please be patient.
