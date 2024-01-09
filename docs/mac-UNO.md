# **UNO开发板--Mac**

上传代码：这里提供了一个示例代码，每秒打印一次“Hello keystudio !”

将以下代码复制粘贴到Arduino IDE中

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

![](./media/image-20230531163632939.png)

点击工具，开发板，选择Arduino AVR Boards中的Arduino Uno。

![9a473649d5e8d5920ebda8a0624f1fa9](./media/9a473649d5e8d5920ebda8a0624f1fa9.png)

选择通信口。

如果有太多的端口，你不知道哪个是正确的，你可以拔下板，看看哪个消失了。如果没有COM口，请检查驱动是否安装。

点击工具，端口，选择“/dev/cu.usbderial-0001”.

![](./media/1721f18ce120baa9a09440d9887c5cff-1685526089268-109.png)

安装成功后将会收到提示。

![](./media/11111111-1685530379800-113.png)

点击 ![image-20230531164208065](./media/image-20230531164208065.png)编译。 

![](./media/848beee386ba83971f66615b76e66629.png)

点击 ![image-20230601084422847](./media/image-20230601084422847.png)设置波特率为9600，串口打印“Hello Keyestudio!” 。

![](./media/421d25a177740e6f6390035b16b256f6-1685581181278-12.png)

1. 切换自动滚动：设置是否跟随打印。
2. 显示时间戳：设置是否显示打印时间。
3. 清除输出：清除输出数据。
4. 串行输入
5. 串口发送格式
6. 波特率：设置波特率。
7. 打印窗口

现在请为IDE导入库，否则会出现错误。



