PIO 配置
=====

## 安装 VS-CODE
VS CODE 是一款比较常用的开发工具。前往[VScode官网](https://code.visualstudio.com/ "VScode官网")，下载安装对应操作系统版本的安装包即可。

## 安装 PIO 插件
打开 VSCode -> 点击左侧扩展 -> 搜索 PlatformIO -> 点击安装插件 -> 等待安装完成

![](http://blog.sipeed.com/wp-content/uploads/2019/04/0d501a8515a735fba54e2f5de908cd1e.png)

## 安装 GD32V 平台定义

点击左侧PIO标志 -> 点击左下方的新建终端 -> 在终端窗口中执行下面的安装指令

* 开发版（与Github同步）
```
platformio platform install https://github.com/sipeed/platform-gd32v
```
![](http://blog.sipeed.com/wp-content/uploads/2019/04/c79100e1ed1747988f001d7471cd1064.png)
 
注：受国内网络环境影响，安装过程需要较长时间，请耐心等待。
