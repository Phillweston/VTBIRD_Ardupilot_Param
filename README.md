# VTBIRD_Ardupilot_Param

## 注意

- VTBIRD 官方的初始参数仅作参考，不要直接导入
- 原始参数一定要做备份
- 修改好的参数一定记得导出保存一份

## 修改的参数（Tilt-VTOL）

### 垂起相关

|Param_Name|New_Value|Restart?|
|-|-|-|
|Q_ENABLE|1|Y|
|Q_TILT_MASK|5|N|
|Q_TILT_TYPE|2|N|
|Q_TILT_MAX|60|N|
|Q_TILT_RATE_DN|30|N|
|Q_TILT_RATE_UP|80|N|
|Q_TRAN_PIT_MAX|5|N|
|Q_TILT_YAW_ANGLE|10|N|
|Q_TILT_FIX_ANGLE|10|N|
|Q_ASSIST_SPEED|8|N|
|Q_ASSIST_ANGLE|60|N|
|Q_RTL_MODE|1|N|
|Q_RTL_ALT|30|N|
|Q_LAND_FINAL_ALT|8|N|

### 空速和油门相关

|Param_Name|New_Value|Restart?|
|-|-|-|
|ARSPD_FBW_MIN|15|N|
|Airspeed Cruise|18|N|
|Throttle Max|80|N|

### 降落和返航相关

|Param_Name|New_Value|Restart?|
|-|-|-|
|RTL_RADIUS|-90|N|
|WP_LOITER_RAD|-90|N|
|ARSPD_AUTOCAL|1|N|

## 输出通道定义

|Param_Name|New_Value|Restart?|
|-|-|-|
|SERVO3_FUNCTION|0|N|
|SERVO4_FUNCTION|0|N|
|SERVO5_FUNCTION|75|N|
|SERVO6_FUNCTION|76|N|
|SERVO7_FUNCTION|33|N|
|SERVO8_FUNCTION|34|N|
|SERVO9_FUNCTION|35|N|
|SERVO10_FUNCTION|36|N|
|SERVO1_REVERSED|1|N|
|SERVO2_REVERSED|1|N|

## PID 自动调参相关

|Param_Name|New_Value|Restart?|
|-|-|-|
|AUTOTUNE_LEVEL|10|N|

## 倾转舵机限幅

|Param_Name|New_Value|Restart?|
|-|-|-|
|AUTOTUNE_LEVEL|10|N|

> 注意：**Q_AUTOTUNE_AXES** 参数需要室外分别轴向调参，默认参数7放在一起调试时间会比较长，可以先调1再调2再调4

## 备注

有几个参数找不到，应该是固件版本的问题

**ARMING_CHECK** 注意自检参数

## 文档作者

Phillweston

2022.4.20
