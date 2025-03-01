# **CP2102驱动安装--MAC**

将我们提供的主板连接到您的计算机上，打开Arduino IDE。

![](./media/40a968d312a8b080e52c4559201f498a.png)

点击“工具”选择**Board: Arduino Uno**中的**Port: /dev/cu.usbserial-0001**。

![](./media/3123378638d9c83554a2c90bfa436bcf.png)

点击 ![](media/98ec72440e6257e5812b408a929a37ba.png) 上传代码，如果刻录成功，您将看到完成上传。

![](./media/e97244571b69d21ff31de3b879b8b0e5.png)

注意:如果刻录不成功，需要安装CP2102驱动程序，请继续按照以下说明:

下载CP2102驱动:[https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers)

1\. 选择Mac OSX

![](./media/6e53a3dacdec57d5ee0b15b48d771a5b.png)

2\. 解压

![](./media/8dced2768d5f86d3d0c3f6076d87a9a8.png)

3\. 双击打开SiLabsUSBDriverDisk.dmg.

![](./media/61ae3e706a1c4afa7948d5fb2e797a6d.png)

4\. 你将会看到：

![](./media/3ffd0525e16492ede92bdb8c84198db9.png)

5\. 双击“安装CP210x VCP驱动程序”，勾选“不警告我”，点击“打开”。

![](./media/14f6ebb088e654abc2f0149645e34ed1.png)

6\. 继续

![](./media/a243872cdbb520e4d298c006e001fff5.png)

7\. 继续并同意

![](./media/ae367c1894df6745e46bbdfc460c1f99.png)

8\. 继续，输入你的密码

![](./media/27b7214283d7f76aba3557dd629bd965.png)

![](./media/29bbca3360d806164717733460574356.png)

9\. 选择开放安全首选项

![](./media/ca6bc6e536202f07a53c09201a0996ff.png)

10\. 点击锁定解锁安全和隐私偏好。

![](./media/379caa1889f4a45614b27c9b2b934869.png)

![](./media/88a1b169a192ee6c49e95947d6287fc2.png)

11\. 允许

![](./media/19e43624efde1b223800201c944d25e9.png)

12\. 等待安装

![](./media/bb0e17afd8bad8b8013f19d7a9da0fd9.png)

13\. 安装完成

![](./media/3bd5bb3752abf97e9bab6bf950a75bed.png)

14\. 然后进入ArduinoIDE，点击工具，选择开发板: Arduino Uno and /dev/cu.SLAB_USBtoUAPT

![](./media/73aed810d216d7da3a3ce9cc0e4dba4a.png)

15\. 点击![](./media/9c9158a5d49baa740ea2f0048f655017.png) 上传代码，显示“完成上传”。

![](./media/d918e2e31a9632f8b272a16595c46a83.png)



