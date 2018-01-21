# esp8266-for-mac
20元制作一个 简单物联网小灯
esp8266加5v继电器 制作一个简单的物联网小灯
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/psb.gif?raw=true)
# 步骤
* 1、设备购买
* 2、电脑环境配置（for mac）
* 3、代码调试
* 4、代码上传，设备调试

### 1、设备购买

#### 物件一、
ESP8266串口wifi模块 物联网 V3开发板 兼容 ModeMCU Lua CH340
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/1.png?raw=true)
#### 物件二、
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/2.png?raw=true)
#### 物件三、
若干个不杜邦线

### 1、设电脑环境配置（for mac）
新买的Arduino开发板 USB转串口使用了CH340芯片，在Mac OS X Yosemite上正常安装驱动后，才能正常使用
开发板背后有写需要什么驱动 购买时可以仔细看看
##### CH341SER_MAC.zip （mac 驱动文件）
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/3.png?raw=true)
* 1.安装CH340驱动
>（驱动下载地址：http://www.wch.cn/download/CH341SER_MAC_ZIP.html）
* 2.打开终端运行以下命令：
>sudo nvram boot-args="kext-dev-mode=1"<br>
>sudo Reboot
* 3.安装Arduino IDE
>https://www.arduino.cc/en/Main/OldSoftwareReleases
* 4.配置Arduino IDE 参数
##### ![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/4.png?raw=true)
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/5.png?raw=true)
在设置里配置附加开发板管理网址
>http://arduino.esp8266.com/stable/package_esp8266com_index.json
##### 打开工具选项 选择开发板中开发板管理器 添加esp8366 并安装
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/6.png?raw=true)
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/7.png?raw=true)
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/8.png?raw=true)
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/9.png?raw=true)
##### 选择 文件>示例>ESP8266WebServer>HelloServer
![图片](https://github.com/YYBT/esp8266-for-mac/blob/master/10.png?raw=true)
### 3、代码调试 
##### 直接打开我上传的文件已经修改好了只有修改路由器信息就行
##### 连接路由器填入你加的路由器密码
>const char* ssid = "wifi名称";<br>
>const char* password = "wifi密码";

#### 4、代码上传，设备调试
##### 点击上传按钮，上传代码

#### 5、设备连线
> 3v->vcc<br>
> G->GND<br>
> D4->IN

#### 视频可参考网友
##### 不想下床关灯？20元改造一个“物联网灯”——ESP8266
> https://www.bilibili.com/video/av16491098/






