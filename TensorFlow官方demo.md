# 官方demo的直接运行
### OS: Ubuntu16.04/18.04

### Android Studio: <https://developer.android.google.cn/studio/> 

### TensorFlow: <https://github.com/tensorflow/tensorflow>

### Step 1: 安装Android Studio
* 按照给的链接直接下载解压安装
* 选择一个SDK安装下载的路径，它会在路径目录下下载相应版本的SDK文件
* 点击Configure中的SDK Manager，选择SDK Platforms，找到你想下载的安卓版本，针对自己手机或其他设备进行版本下载，选择SDK Tools，勾选NDK进行下载，上述两步选择完后，点击Apply,然后Accept,点击Next进行下载。
  
### Step2: 用Android Studio打开工程文件

* tensorflow网站下载tensorflow-master文件，我将其解压到桌面，然后将Desktop\tensorflow-master\tensorflow\contrib\lite\java 目录下的demo文件夹，用Android Studio打开如下。Sync完成后接下来就是Build,期间也是漫长的等待
  
### Step3：将下载的预先训练的轻量化模型放入目录

将下载的mobilenet_quant_v1_224.tflite以及对应的标签abels_mobilenet_quant_v1_224.txt放到demo\app\src\main\assets 这个 文件夹下。之后就可以build和run了。
点击Run'app',该过程也有可能有错误产生。你需要将手机连接电脑，手机设置成开发者模式。