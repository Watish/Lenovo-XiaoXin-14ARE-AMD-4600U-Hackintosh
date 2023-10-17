# 联想小新Air14 ARE（2020）Hackintosh

| 处理器         | R5 4600U (6c 12t)                           |
| -------------- | ------------------------------------------- |
| 内存           | ddr4 16G 3200mhz （板载）                   |
| 主硬盘         | 梅捷nvme固态500G （原三星硬盘不支持，需换） |
| 副硬盘（2242） | 西数SN750 256G                              |
| 无线           | AX200（原无线网卡不支持，需换）             |
| 蓝牙           | （已驱动）                                  |

### 当前系统版本

MacOS **Monterey**（12.6）



### 测试正常的功能

1. 摄像头
2. 所有USB口
3. 麦克风（需要在安装完成后进行操作，见下方教程）
4. 触控板正常
5. iCloud，iMessage，Facetime
6. 无线及蓝牙



### 已知问题

1. 无法睡眠（准确的说是无法进入睡眠，盖上盖子后屏幕熄灭，但cpu以及风扇仍然在转）
2. NootedRed的已知问题，如Chrome硬件加速，新版QQ卡死



### 注意

1. 已对本机进行USB定制，对应kext为 **UTBMap.kext** 
2. 本EFI带intel网卡驱动（Monterey版），安装其它系统请删除更换对应驱动文件



### 安装前

1. 更改**三码**
2. 开机狂按F2进BIOS修改**显存**至2G
3. BIOS关掉Secure Boot

（得益于**GenericUSBXHCI.kext**，我们不再需要屏蔽xhci口，现在所有的插口都可以使用！）



### 安装后：麦克风阵列的驱动

请参考此仓库 https://github.com/qhuyduong/AMDMicrophone





### 参考链接

1. https://github.com/W2725730722/Lenovo-R7000P-2020-Hackintosh
2. https://github.com/Zrc00/Lenovo-Xiaoxin-15ARE-AMD-4800U-Hackintosh
3. https://github.com/zabdottler/Lenovo-Yoga-16S-hackintosh
4. https://github.com/wubiao1998/Lenovo-Xiaoxin-Pro13-AMD-hackintosh
5. https://github.com/qhuyduong/AMDMicrophone
6. https://github.com/ChefKissInc/NootedRed

