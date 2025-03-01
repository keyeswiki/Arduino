# **ESP32开发板环境配置和驱动安装：**

<span style="font-size: 22px;"><span style="color: rgb(255, 76, 65); font-size: 22px;">注意：Arduino IDE 软件的下载，安装与设置方法和上面的一样，就不重复说明了。</span></span>

<br>
<br>

(相关资讯：[https://github.com/earlephilhower/arduino-esp32](https://github.com/earlephilhower/arduino-esp32) )

## **A. Windows系统**

![](./media/eef95a4f71c9316e41a35813556e51da.png)

**1. 在Arduino IDE上安装ESP32：**

上面已经学习了怎么下载，安装Arduino IDE 软件和怎么安装驱动，那下面就要在Arduino IDE上安装ESP32，请执行以下步骤：

<span style="color: rgb(255, 76, 65);">特别注意：你需要Arduino IDE 1.8.5或更高版本才能在其上安装ESP32。</span>

(1)点击电脑桌面上的图标![](./media/2aa3f7ff09ff5841f1864c521af61cbd.png)，打开Arduino IDE。

![](./media/e50b14820c3bb291108dc8b9c0c12843.png)
(2)点击“文件” →“首选项”，如下图：

![](./media/339b8fc0220890b15cac94e7fefd8e7f.png)

(3)打开下图标出的按钮。

![](./media/dd6d3ea8b8ab77977ff2b2af74dbcdab.png)

(4)将这个地址：https://dl.espressif.com/dl/package_esp32_index.json ，复制粘贴到里面去再点击“**确定**”保存这个地址，如下图：

![](./media/0f4697f40d0e4c73cdaa36a15034e63b.png)
(5)再点击“**确定**”。

![](./media/11dd827f1f17588419bf7be03a47211d.png)

（6）先点击“**工具**”→“**开发版:**”，再点击“**开发版管理器...**”进入“**开发版管理器**”页面，在文本框中输入“**esp32**”，选择最新版本进行安装，安装包不大，点击“**安装**”开始安装相关安装包。如下图。

![](./media/486d22dca3d5007c0866fe0dd4b3075e.png)

![](./media/fe7700b0fc213248a7b2d09cd6fc20ae.png)

![](./media/26766efa26cbdaa8d507e52e40317158.png)

（7）点击“**工具**”→“**开发版:**”，就可以看到安装好的ESP32 Arduino，你可以在里面查看到各种不同型号ESP32开发板，选择对应的ESP32开发板型号。

![](./media/7d924f3a05df1addfd61d26a4b1f9eff.png)

![](./media/07bbc456b0cfb6f5393701025233b38b.png)

（8）设置好板型后，再选择正确的COM口（安装驱动成功后可看到对应COM口），设置如下图。

![](./media/65fcafd5ca192f1d566779a819e04d00.png)

![](./media/2cdb1757b32b480e3dac16aa8385e13c.png)

![](./media/3270b2614818b728fb3fdd4a45d239f9.png)

## B. Mac系统:

![](./media/a94b5505840316715e4bc9badd0421ba.png)

1.下载安装Arduino IDE:

进入Arduino官方网站：[https://www.arduino.cc/](https://www.arduino.cc/) ，点击“**SOFTWARE**”进入下载页面，如下图所示：

![](./media/2f1dce89630be8f6fdd23f38ab7097ec.png)

2.如何安装CP2102驱动程序：

（注意：如果已经安装了驱动程序，则不需要再安装驱动；如果没有，则需要进行以下操作）

（1）用USB线将ESP32主板连接到你的MacOS系统电脑上，并打开Arduino IDE。

![](./media/a694cc7590112b9becc48e0ad33588ea.png)

（2）CP2102驱动下载链接：
https://cn.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads

（3）点击下载MacOS 版本。

![](./media/a369c4f935f32560b84a9b3b756c7dc5.png)

（4）解压下载好的压缩包。

![](./media/43f7535e76478fc4bd3b4f7eb68ee068.png)

（5）打开文件夹，双击“SiLabsUSBDriverDisk.dmg”文件。
![](./media/e339ed4aa5a59a7ffbd426da57cc5522.png)
可以看到以下文件。

![](./media/ba80c239c55f073ad212e110898c9be5.png)

（6）双击“Install CP210x VCP Driver”，勾选“Don’t warn me when opening application on this disk image”并单击“Open”。

![](./media/b90f9fec981a67e60d6d973049c8480a.png)
（7）单击“Continue”。

![](./media/e3d154346714057c76f44a429d30bc75.png)

（8）先点击“Agree”，然后点击“Continue”。

![](./media/df1b62568fc2737d10bebe86364d6240.png)

（9）继续点击“Continue”，然后输入你的用户密码。

![](./media/8d5943e9f17648b7b345f2cb921835e8.png)

![](./media/d5caae5575fc94e8837daad3675dd164.png)

（10）选择“Open Security Preferences”。

![](./media/36fe00477b7e98da6cd3f7d4e074c489.png)

（11）点击安全锁，输入你的用户密码来授权。

![](./media/4889cc38b37c1df851c7772aa1f74fe4.png)

![](./media/85556fc015cdb38f51375ace1c498585.png)

（12）看到锁被打开了，点击“Allow”。

![](./media/bb9213f09221a88dee06bd4ff792cd4c.png)
（13）回到安装界面，根据提示等待安装。

![](./media/d49cc02c9a101542bb4a8572da600dfe.png)

（14）安装成功。

![](./media/dead537234a8ea1a9feab59bc451eebb.png)

3. 在Arduino IDE上安装ESP32：
上面已经学习了怎么下载ArduinoIDE和怎么安装驱动，那下面就要在Arduino IDE上安装ESP32，请执行以下步骤：

<span style="color: rgb(255, 76, 65);">特别注意：你需要Arduino IDE 1.8.5或更高版本才能在其上安装ESP32。</span>

(1)点击电脑桌面上的图标![](./media/2aa3f7ff09ff5841f1864c521af61cbd.png)，打开Arduino IDE。点击“Arduino IDE” →“首选项”，如下图：

![](./media/9a1550c0afb15d603b35c14fc7eb9419.png)
(2)打开下图标出的按钮。

![](./media/2021aa4872f771da0789e9d4d35c778e.png)

(3)将这个地址：https://dl.espressif.com/dl/package_esp32_index.json ，复制粘贴到里面去再点击“**确定**”保存这个地址，如下图：

![](./media/01edadc223784029595d586e60336c53.png)
(4)再点击“**确定**”。

![](./media/f88fa3fc64d0e88254ed1f1960ff20cf.png)

（5）先点击“**工具**”→“**开发版:**”，，再点击“**开发版管理器...**”进入“**开发版管理器**”页面，在文本框中输入“**esp32**”，选择最新版本进行安装，安装包不大，点击“**安装**”开始安装相关安装包。如下图。

![](./media/b190d9a92887ff3f38fd00f9ef6a7bc6.png)

![](./media/1bd7dab9f8e78713466d019451110080.png)

![](./media/032996f813d7ccb74e4c6c8a6a13486f.png)

（6）点击“**工具**”→“**开发版:**”，就可以看到安装好的ESP32 Arduino，你可以在里面查看到各种不同型号ESP32开发板，选择对应的ESP32开发板型号。

![](./media/40fb53f0ba1f781650ac404f8a25a3b6.png)

（7）设置好板型后，再选择正确的COM口（安装驱动成功后可看到对应COM口），设置如下图。

![](./media/b240beb6e80e99e17c399d6d65f03fb4.png)




