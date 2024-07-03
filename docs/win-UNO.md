# **UNO开发板--Windows**

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

![图片不存在](./media/8832e91f90a1dbf7b8e0fe976b824841.png)

点击工具，开发板，选择Arduino AVR Boards中的Arduino Uno。

![图片不存在](./media/7a3e5ae6c5df0a19922a997a0e7c0f95.png)

选择通信口。

如果有太多的端口，你不知道哪个是正确的，你可以拔下板，看看哪个消失了。如果没有COM口，请检查驱动是否安装。

![图片不存在](./media/cc7b58c15299bf0ef8d74d32d9b6e280.jpg)

此处我们的端口为COM3.

![图片不存在](./media/514f4bbbf3f265f8681d1813b543f61c.png)

安装成功后将会收到提示。

![图片不存在](./media/04f41439343bacf596fd3abaed572692.png)

点击 ![图片不存在](./media/d850ef08c2fd6b92e762108775094160.png)编译代码

![图片不存在](./media/501ae9e2281a2e82e3b4f9df88ea43a7.png)

点击 ![图片不存在](./media/3a7eab031e133625ebf71f4a0c573912.png)设置波特率为9600，串口打印“Hello Keyestudio!” 。

![图片不存在](./media/6a5c07fc4a5621b7b338c0a2417ab6a3.png)

1. 切换自动滚动：设置是否跟随打印。
2. 显示时间戳：设置是否显示打印时间。
3. 清除输出：清除输出数据。
4. 串行输入
5. 串口发送格式
6. 波特率：设置波特率。
7. 打印窗口

现在请为IDE导入库，否则会出现错误。





