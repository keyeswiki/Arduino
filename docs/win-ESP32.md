# **ESP32开发板--Windows**

通常情况下，我们无法在工具中的开发板中找到ESP32板。因为我们还没有在Arduino IDE上安装这个板。

![图片不存在](./media/4dd77d1fb0be43fb7d235c23d2f13039.png)

安装步骤：

打开Arduino IDE，进入首选项。

复制ESP32板链接（https://espressif.github.io/arduino-esp32/package_esp32_index.json）并粘贴到其他开发板管理器地址。

![图片不存在](./media/ca069f8a7e731d48af9aeb0b023ee16a.png)

打开开发板管理器

![图片不存在](./media/23acf08c209dbb3d32268d5ed740d31f.png)

搜索并安装最新版ESP32， 等待安装完成。

**安装过程中，请确保网络稳定。如果失败，请再次操作上一步重新安装。**

![图片不存在](./media/f382602ecf5161f181ccde78ae750fff.png)

安装完成后，选择开发板类型。

![图片不存在](./media/8a9fb69b6162eaabbb7a0b50ba1ba955.png)

选择通信端口。

如果端口太多，你不知道哪个是正确的，你可以拔下板，看看哪个消失了。如果没有COM口，请检查驱动是否安装。

![图片不存在](./media/cc7b58c15299bf0ef8d74d32d9b6e280.jpg)



此处我们的通信口是 COM3， 因此我们在端口中选择 “COM3”

![图片不存在](./media/1a2a053d2146464ffcf862c077e94738.png)

如果连接成功，页面会有提示。现在您可以尝试上传代码了。这里提供了一个示例代码：每秒打印一次“Hello keystudio !”。

```c
/*
  keyes 
  打印 “Hello keyes!”
  http://www.keyes_robot.com
*/
void setup() { 
    Serial.begin(9600);  //设置波特率为9600
}

void loop() { 
    Serial.println("Hello keyes!");  //打印信息
 	delay(1000);  //延时1s
}
```

![图片不存在](./media/bcdc3a9b1259cd5bd2f6258f9384240f.png)

点击 ![图片不存在](./media/d850ef08c2fd6b92e762108775094160.png)编译上传代码。

![图片不存在](./media/11e6e317f03db274862d5fe4d72115d7.png)

上传时如果显示 “————……..————……..”，请长按开发板上的启动按钮（仅适用于keyes ESP32开发板 ，其中不包含keyes Plus ESP32）。

点击 ![图片不存在](./media/3a7eab031e133625ebf71f4a0c573912.png)设置波特率为9600， 串口打印 “Hello keyes!”。

![图片不存在](./media/9f99af8d374d355525a592340c3bba9e.png)

1. 切换自动滚动：设置是否跟随打印。
2. 显示时间戳：设置是否显示打印时间。
3. 清除输出：清除输出数据。
4. 串行输入
5. 串口发送格式
6. 波特率：设置波特率。
7. 打印窗口

现在请为IDE导入库，否则会出现错误。



