# **Pico开发板--Mac**

通常情况下，我们无法在工具中的开发板中找到Pico板。因为我们还没有在Arduino IDE上安装这个板。

![](./media/2c69861be28d9585be93583b6958b3de.png)

安装步骤：

启动Arduino IDE， 进入![](./media/25204e75256579ce37b2e10029bbb246.png):

![](./media/9381b569c1ee1a2e79d28ab1f55b8690.png)

搜索**Pico**并安装 **Arduino Mbed OS RP2040 Boards**. 

![](./media/368b1281ad27465d827f7069061d44c0.png)

安装完成会有弹出窗口提示。

![](./media/d1ee80401c0108a6e7453c99ad30eb7f.png)

选择pico板。

![](./media/b9663a1803953e6348facb0118737550.png)

重要步骤：上传与arduino兼容的Pico固件， 否则arduino IDE不能在Pico板上刻录程序。

请参考以下配置:

(1) 断开Raspberry Pi Pico与计算机的连接。按住树莓派Pico上的白色按钮(BOOTSEL)，直到板连接到PC。(一定要记得按住按钮，直到连接完成，否则固件下载失败。)



![](./media/03d4f75c5de184fa2b9ee153f25b83ff.jpg) 

（2）启动Arduino IDE， 点击文件，示例，01.Basics，Blink

![](./media/fdccbfa62236fe55246dec2f9dcb3d8f.png) 

（3）点击工具，开发板，选择**Arduino Mbed OS RP2040 Boards** 中的 **Raspberry Pi Pico**.

![](./media/4dc0152ad415243edc574a73180d4de6.png) 

（4）上传 **Blink** 到Pico板并点击 ![](./media/83d2ea9b45a89ad6088dcd3318b85fc8.png)编译。

![](./media/7ef3907d1dfb7186ef2363ecc7242b5f.png) 

板上指示灯开始闪烁，间隔为一秒。

![](./media/124ad033d76beea4110fba100fb84601.png)

点击工具，串口，选择 **/dev/cu.sudmodem14101(Raspberry Pi Pico)**. 

![](./media/9f27106ea4cf61d90daf9feeefa26ab5.png)

**注意**

* 第一次通过Arduino上传，不需要选择端口。但此后每次都需要检查端口是否选中；否则可能导致下载失败
* 由于固件缺失，Pico板可能无法工作。此时，请重新上传固件

