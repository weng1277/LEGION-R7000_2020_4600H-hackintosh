# LEGION-R7000_2020_4600H-hackintosh

本EFI适用于拯救者R7000 2020 4600H机型，EFI改自Q群“OpenCore黑苹果”内大佬制作的EFI文件

正常工作：
AMD核显
AX200（WLAN+蓝牙）
键盘
触控板（轮询模式）
短时间睡眠（长时间会黑屏）
右侧及背部的USB-A接口（XHCI1控制器下的设备）
扬声器输出

不正常工作：
隔空投送
左侧USB-A、背部Type-C及摄像头（XHCI0控制器下设备）
内置麦克风
GTX1650（废话，包括其他N卡）
PM981a
有线网卡（支持但用的少，所以懒得加，后期可能会更新）

注意⚠️：
由于本人新增有硬盘，故将主盘位的PM981A屏蔽掉了，在EFI/OC文件夹内可以看到有无硬盘屏蔽版本，如果出现问题请将该配置重命名为“Config.plist”进行替换使用
由于默认屏蔽了XHCI0控制器，请  不要  把启动盘插在左侧USB口内
由于一些系统问题，建议在安装前将显存改到1GB及以上以保证系统流畅度
本EFI使用MOD版OC，请在进入macOS后使用OpenCore Configurator进行编辑修改， 不要  使用OCAT修改EFI，可能会导致配置损坏，win下建议学习使用ProperTree
受显卡驱动的限制，本EFI默认关闭核显驱动以保证安装过程的顺利，请在安装完成后勾选启用NootedRed.kext来驱动核显


在此感谢群内各位大佬们的技术支持和Nooted大佬的核显驱动，让我们吃上了AMD的黑苹果