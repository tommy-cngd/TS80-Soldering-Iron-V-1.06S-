# TS80-Soldering-Iron-V-1.06S-
在官方发布的1.06固件基础上，做了一个能解决TS80电焊笔在接移动电源下无法使用的问题的固件，把它命名为1.06s，问题解决方法如下

在开机后，进入设置模式，找到设置项source，这个呢决定启不启动移动电源模式，ON为启动，OFF为关闭，设置操作和其它设置项一样，开启时电焊笔多跑一个唤醒程序

移动电源模式开启时
待机状态下，唤醒程序每0.5s加热一次每次加热2.5ms，无操作10min后不再执行唤醒程序

移动电源模式关闭时
待机状态下，唤醒程序每0.5s加热一次每次加热2.5ms，无操作30s不再执行唤醒程序

移动电源模式开启/关闭
设置模式下，唤醒程序每0.5s加热一次每次加热3.5ms，无操作重复执行唤醒程序20次，操作会重新计数，执行满20次返回待机模式

另外还做了其它一些小的修改和bug优化

On the basis of 1.06 firmware issued by the government, a firmware was made to solve the problem that TS80 solder pen can not be used under the mobile power supply. It was named 1.06s. The solution is as follows.

After booting, enter the settings mode, find the settings item source, this decision to start or not start the mobile power mode, ON to start, OFF to close, set the operation and other settings, open the welding pen run an additional wake-up program

When mobile power mode is switched on
In standby state, the wake-up program is heated once every 0.5s for 2.5ms, and no wake-up program is executed after 10 minutes without operation.

When the mobile power mode is off
In standby state, the wake-up program is heated once every 0.5s for 2.5ms, and no wake-up program is executed after 30 s without operation.

Mobile power mode on / off
In the setting mode, the wake-up program is heated 3.5ms every 0.5s, and the wake-up program is executed 20 times without repetition. The operation counts again and returns to standby mode 20 times after execution.

Some other minor modifications and bug optimization are also made.
