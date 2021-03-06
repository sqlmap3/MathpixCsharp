### 使用官方API教程

1. 首先到 https://dashboard.mathpix.com/ 注册一个账户并登录。然后到[这里](https://accounts.mathpix.com/ocr-api/new)创建OCR API，在设置Biliing的时候需要用到**国外的信用卡**，可能会暂时扣1美元验证信用卡有效性。
2. 之后在账户主页点击OCR APIs，就可以看到你的API keys列表，把 app_id 和 app_key 这两个字段复制出来，如下图：

![apiPic.png](https://i.loli.net/2021/02/19/iDofHx6bZFmqvVB.png)

3. 按照[安装教程](https://github.com/itewqq/MathpixCsharp/blob/master/README.md)装好客户端。安装完之后如果没找到在哪儿启动请打开```开始```进行查找。
4. 第一次打开会弹出在名为```login```的窗口，在里面填入之前的app_id和app_key，**下方的复选框选择```官方Key```**，**注意不要选错**，选错了会导致无法使用。然后点击确认。只需要填一次之后再打开就不用填了。如果填错了或者要更换Key可以在主界面点击```菜单->重置Key```。
   
![image.png](https://i.loli.net/2021/02/19/HAKMjmYhplwqez4.png)

5. 客户端主界面如下图：

![image.png](https://i.loli.net/2021/02/19/8eqmzvsGDKUJh9d.png)

6. 使用时需要先截屏选择要识别的公式。点击**截屏按钮**或者使用**快捷键Ctrl+Alt+M**开始截屏。截屏过程类似QQ的截屏功能，鼠标按下开始截屏，拖动选择区域，松开完成截屏。
7. 截屏完成后客户端会自动完成识别，并将识别结果置于文本框内，点击文本框对应的按钮可以复制到剪贴板。完整的演示流程参考下图：
![使用演示](/images/demo1.gif)

8. 当点击关闭窗口的时候，MathpixCsharp会自动最小化到系统托盘，**如果要退出客户端，请右键系统托盘上的客户端图标再选择退出。**
9. **关于Office Word中的公式**：Word用户请点击**复制MathML**按钮，然后在word文档里**右键->粘贴->仅粘贴文本**。有时候Ctrl+V会有问题，但是现在这个问题貌似很少出现了。另外，由于Word自身处理公式的问题，有时候一些带括号的公式可能会出现这种情况：
![image.png](https://i.loli.net/2021/02/19/yKu7RCmknDGNz8V.png)这时候只需要把**光标放在公式最后面，敲一下回车**就好了。如果还有问题，就把**光标放在异常的括号后面，点一下空格**就好了。

注： 使用**多个显示器**时，MathpixCsharp将选择**其窗体当前所在的屏幕**进行截屏。