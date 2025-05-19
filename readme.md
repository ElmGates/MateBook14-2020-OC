# Matebook 14(2020) MacOS 11-15 配置文件

### 特别说明
国内网络环境比较糟糕，push半天push不上来，OC直接放在Release里面了，点击下方链接前往下载。  


### 机型配置信息
| 项目 | 详细参数|
| :--: | :-------------------- |
| 型号 | Matebook 14 2020    |
| CPU  | Intel i7-10510U |
|内存| DDR3L 16G|
| 显卡 | UHD620（MacOS识别为iris plus655）&MX350|
| 硬盘 | WD SN750 512G|
| 声卡 | Realtek ALC256 |
|LCD| 2160*1440|
  
### 已经驱动
* CPU睿频
* 唤醒
* 录音
* 扬声器/耳麦
* 触摸板/手势
* USB3.0/2.0（已定制USB，所有接口工作均正常）
* HiDPI
* HDMI正常
* 蓝牙
* WIFI(INTEL AC9560无线网卡)

### 无法驱动：
* Camera
* MX350及其他规格独立显卡

### 补充说明
* HiDIP 用RDM切换,[设置方法](#hidip-设置方法)见下面
* config.plis默认机型为 Macbookpro15,2 **必须**自行使用工具生成新的序列号，不建议修改机型,默认序列号全是0，无法正常使用！
* MacOS15及以上**需要使用OCLP破解intel-WiFi**，破解后会导致Realtek USB网卡无法驱动，如有需要请使用MacOS15 OC 附带的驱动进行驱动！
* 可以使用Tools中的3.5接口修补来修复3.5接口识别异常问题。
* MacOS15 破解后有概率会出现某些系统进程大量占用CPU导致电脑发热严重，请自行搜索「进程名称」+异常占用CPU，寻找解决方案。

### HiDIP 设置方法
* 使用HiDIP脚本进行设置 [Github](https://github.com/xzhih/one-key-hidpi) ，选择开启HiDPI（不注入EDID），图标自选，自定义几个3:2的分辨率，如1680x1120 1500x1000 1350x900等

### 声卡偶尔外放出现噪音的解决方法
* 偶尔外放播放出现底噪[声音沙哑]问题，进入声音设置->声音控制偏好->将输入与输出选项进行切换一下即可恢复外放正常播放

### 写在最后
* `OpenCore`版本不是最新就最好，合适的版本达到稳定即可，若要升级`OpenCore`版本推荐使用，[OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools/blob/master/READMe-cn.md)

### 致谢
Apple's macOS
[frezs的Matebook 14/13 (2019/2020/2021) MacOS Monterey & Bigsur 黑苹果安装教程](https://github.com/frezs/MateBook14-Hackintosh)，本OC的13版本基于此OC基础上修改而来。
[Acidanthera](https://github.com/acidanthera)'s [OpenCore](https://github.com/acidanthera/OpenCorePkg)
[B站UP主win10Q的MacOS15WiFi驱动教程](https://www.bilibili.com/video/BV1r5WyeyE3k/?vd_source=c3e90c8c0d8c4b38cb0f32fc94494c46)
[xzhih](https://github.com/xzhih)'s [hidpi](https://github.com/xzhih/one-key-hidpi)
[Dortania](https://github.com/dortania) 和 OpenCore Legacy Patcher 贡献者
[laobamac](https://github.com/laobamac)'s [OCLP-Mod](https://github.com/laobamac/OCLP-Mod)
还有其他一切对Hackintosh提供支持的人！
