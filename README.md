# Ian - 定量停充
**这是一个在安卓设备上工作的Magisk模块。**

当您设备的电量为“停止充电电量”时，此模块会为您的设备停止充电。

当您设备的电量为“恢复充电电量”时，此模块会为您的设备恢复充电。

**配置文件**：/data/adb/modules/Ian-QuantitativeStopCharging/**config.conf**

**日志文件**：/data/adb/modules/Ian-QuantitativeStopCharging/**log.log**

**原理**：通过Shell脚本(此模块中的main.sh)循环检测设备当前电量，当设备的电量为“停止充电电量”或“恢复充电电量”时修改设备的控制充电文件(/sys/class/power_supply/battery/input_suspend)，以此实现自动停止/恢复充电的功能。
