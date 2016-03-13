#第三次作业
###1 反编译任意apk，并且截图

###2 使用aapt的命令查询权限，并且截图

###3 编写3种不同切入点的Android monkey的命令，并成功运行，同时说明切入点是什么
#### 切入点:多系统按键事件的验证
adb -s 123456 shell monkey -p com.adroid.mms --pct-syskeys 30 --ignore-timeouts --ignore-crashes --throttle 500 -s 123456 -v -v -v 10000
#### 切入点:多Activiy切换事件的验证
adb -s 123456 shell monkey -p com.adroid.mms --pct-appswitch 30 --ignore-timeouts --ignore-crashes --throttle 500 -s 123456 -v -v -v 10000
####切入点:多点击事件的验证
adb -s 123456 shell monkey -p com.adroid.mms --pct-touch 30 --ignore-timeouts --ignore-crashes --throttle 500 -s 123456 -v -v -v 10000
###4 请找出Android monkey中motion和touch对应的源码里的方法，并找出monkey工具实现点击的最基础发方法是什么
###5 找到任意一个apk or ipa，然后去寻找里面的db，并打开，上传截图

