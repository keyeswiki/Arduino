# **ESP32开发板--MAC**

通常情况下，我们无法在工具中的开发板中找到ESP32板。因为我们还没有在Arduino IDE上安装这个板。

![图片不存在](./media/2c69861be28d9585be93583b6958b3de.png)

安装步骤：

打开Arduino IDE，进入首选项。

复制ESP32板链接（https://espressif.github.io/arduino-esp32/package_esp32_index.json)并粘贴到其他开发板管理器地址。

![图片不存在](./media/f58efad46ffbf16e4b469212ee8c813b.png)

打开开发板管理器

![图片不存在](./media/cd9ff53403119ac22f1947b6cbc77ab5.png)

搜索并安装最新版ESP32， 等待安装完成。

**安装过程中，请确保网络稳定。如果失败，请再次操作上一步重新安装。**

![图片不存在](./media/6282613716362b2a217ddd5f277de20b.png)

![图片不存在](./media/c945305e8543542cce4bb12b610e05a8.png)

安装完成后，选择开发板类型。

![图片不存在](./media/bf839f0e6436da9c07d2904a12abaa73.png)

选择通信端口。

如果端口太多，你不知道哪个是正确的，你可以拔下板，看看哪个消失了。如果没有COM口，请检查驱动是否安装。

点击工具，端口并选择“/dev/cu.usbderial-0001”.

![图片不存在](./media/f50ecf2910f74466571b79dbac2155aa.png)

如果连接成功，页面会有提示。

现在您可以尝试上传代码了。这里提供了一个示例代码：每秒打印一次“Hello keystudio !”。

![图片不存在](./media/e9b7614e186a69fdffcdab2d8c46489c.png)

复制粘贴以下代码到Arduino IDE: 

```c
/*
  keyestudio 
  打印 “Hello Keyestudio!”
  http://www.keyestudio.com
*/
void setup() { 
    Serial.begin(9600);  //设置波特率为9600
}

void loop() { 
    Serial.println("Hello Keyestudio!");  //打印信息
 	delay(1000);  //延时1s
}
```

点击 ![图片不存在](./media/d850ef08c2fd6b92e762108775094160.png)编译，成功编译后显示：

![图片不存在](./media/ae56f65945157c0667f54fd4317628c9.png)

上传时如果显示 “————……..————……..”，请长按开发板上的启动按钮（仅适用于Keyestudio ESP32开发板 ，其中不包含Keyestudio Plus ESP32）。

点击 ![图片不存在](./media/3a7eab031e133625ebf71f4a0c573912.png) 设置波特率为9600， 串口打印 “Hello Keyestudio!”。

![图片不存在](./media/ca858b6e425a6752b8cdf6422a8271c4.png)

1. 切换自动滚动：设置是否跟随打印。
2. 显示时间戳：设置是否显示打印时间。
3. 清除输出：清除输出数据。
4. 串行输入
5. 串口发送格式
6. 波特率：设置波特率。
7. 打印窗口

现在请为IDE导入库，否则会出现错误。

