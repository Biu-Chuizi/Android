**安装配置 TensorFlow on Android**

首先先根据提示把Demo跑起来，后面的工作在此基础上进行。

1）安装 Android Studio

去官网下载安装即可。

2）在Github上 clone TensorFlow 
git clone https://github.com/tensorflow/tensorflow

3）搭建 Android Studio环境

打开Android Studio，选择 “Open an existing Android Studio project”，在“Open File or Project ”，选择在2）中对应的 tensorflow/examples/android 文件夹，OK。如果需要“Gradle Sync”，选择OK。第一次启动可能需要安装或更新很多模块，耐心等待。

4） 在 build.gradle 文件中（在左侧 1:Project 面板  Android 下面 Gradle Scripts/build.gradle ），找到  nativeBuildSystem 这个变量，设置等于 “none”:
```
// set to 'bazel', 'cmake', 'makefile', 'none'
def nativeBuildSystem = 'none'
```
5) 点击上方菜单 Run -> Run 'android'  命令， 在弹出菜单选择 右侧的 Proceed Without Instant Run。

6）同时，打开手机的开发者模式与USB调试，用USB连接电脑。不同手机方法不同，自行百度。

成功连接后运行命令时会识别对应手机型号，选择后继续，将会在手机上安装4个不同的APP，期间注意查看手机，允许安装（默认会拒绝）。

ref: 

> https://blog.csdn.net/dy_guox/article/details/80192343

> https://www.tensorflow.org/mobile/android_build

> https://www.tensorflow.org/lite
