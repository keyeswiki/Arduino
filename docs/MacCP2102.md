# **CP2102驱动安装--MAC**

将我们提供的主板连接到您的计算机上，打开Arduino IDE。

![File:====9.png](./media/542px-%253D%253D%253D%253D9.png)

点击“工具”选择**Board: Arduino Uno**中的**Port: /dev/cu.usbserial-0001**。

![File:====10.png](./media/768px-%253D%253D%253D%253D10.png)

点击 ![image-20230601153931790](media/image-20230601153931790.png) 上传代码，如果刻录成功，您将看到完成上传。

![File:====11.png](./media/534px-%253D%253D%253D%253D11.png)

注意:如果刻录不成功，需要安装CP2102驱动程序，请继续按照以下说明:

下载CP2102驱动:[https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers)

1\. 选择Mac OSX

![File:====12.png](./media/800px-%253D%253D%253D%253D12.png)

2\. 解压

![====13.png](./media/700px-%253D%253D%253D%253D13.png)

3\. 双击打开SiLabsUSBDriverDisk.dmg.

![====14.png](./media/700px-%253D%253D%253D%253D14.png)

4\. 你将会看到：

![====15.png](./media/700px-%253D%253D%253D%253D15.png)

5\. 双击“安装CP210x VCP驱动程序”，勾选“不警告我”，点击“打开”。

![====16.png](./media/700px-%253D%253D%253D%253D16.png)

6\. 继续

![====17.png](./media/700px-%253D%253D%253D%253D17.png)

7\. 继续并同意

![====18.png](./media/700px-%253D%253D%253D%253D18.png)

8\. 继续，输入你的密码

![====19.png](./media/700px-%253D%253D%253D%253D19.png)

![====20.png](./media/700px-%253D%253D%253D%253D20.png)

9\. 选择开放安全首选项

![====21.png](./media/700px-%253D%253D%253D%253D21.png)

10\. 点击锁定解锁安全和隐私偏好。

![====22.png](./media/700px-%253D%253D%253D%253D22.png)

![====23.png](./media/700px-%253D%253D%253D%253D23.png)

11\. 允许

![====24.png](./media/700px-%253D%253D%253D%253D24.png)

12\. 等待安装

![====25.png](./media/700px-%253D%253D%253D%253D25.png)

13\. 安装完成

![====26.png](./media/700px-%253D%253D%253D%253D26.png)

14\. 然后进入ArduinoIDE，点击工具，选择开发板: Arduino Uno and /dev/cu.SLAB_USBtoUAPT

![====27.png](./media/700px-%253D%253D%253D%253D27.png)

15\. 点击![0486-23.png](./media/0486-23.png) 上传代码，显示“完成上传”。

![====28.png](./media/700px-%253D%253D%253D%253D28.png)



