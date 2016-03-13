#第三次作业
###1 反编译任意apk，并且截图
![image](https://github.com/Test-Seven/TangJixu/blob/master/3rd/1.png)
###2 使用aapt的命令查询权限，并且截图
![image](https://github.com/Test-Seven/TangJixu/blob/master/3rd/2.png)
###3 编写3种不同切入点的Android monkey的命令，并成功运行，同时说明切入点是什么
#### 切入点:多系统按键事件的验证	
adb -s 123456 shell monkey -p com.adroid.mms --pct-syskeys 30 --ignore-timeouts --ignore-crashes --throttle 500 -s 123456 -v -v -v 10000
#### 切入点:多Activiy切换事件的验证
adb -s 123456 shell monkey -p com.adroid.mms --pct-appswitch 30 --ignore-timeouts --ignore-crashes --throttle 500 -s 123456 -v -v -v 10000
####切入点:多点击事件的验证
adb -s 123456 shell monkey -p com.adroid.mms --pct-touch 30 --ignore-timeouts --ignore-crashes --throttle 500 -s 123456 -v -v -v 10000
###4 请找出Android monkey中motion和touch对应的源码里的方法，并找出monkey工具实现点击的最基础发方法是什么
![image](https://github.com/Test-Seven/TangJixu/blob/master/3rd/4_1_motion.png)
![image](https://github.com/Test-Seven/TangJixu/blob/master/3rd/4_2_touch.png)
![image](https://github.com/Test-Seven/TangJixu/blob/master/3rd/4_3.png)
###5 找到任意一个apk or ipa，然后去寻找里面的db，并打开，上传截图
![image](https://github.com/Test-Seven/TangJixu/blob/master/3rd/5.png)
###6 github上去找monkey.js 去instruments运行，给出instruments运行的结果图
###7 安装idevicestaller，获取iOS日志
![image](https://github.com/Test-Seven/TangJixu/blob/master/3rd/7.png)

