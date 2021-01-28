# 神舟炫龙A3S 黑苹果EFI
Hackintosh for Shinelon_A3S (HM86)

### 兼容性

此 EFI 适用于神舟炫龙A3S，主板型号E479，需要刷入加入了微码的魔改BIOS，且只在该平台测试使用。

### 笔记本配置

| 规格     | 详细信息                                                |
| -------- | ----------------------------------------------------- |
| 电脑型号 | 神舟炫龙A3S (HM86)                                  |
| 主板型号 | E479XL54                                  |
| 操作系统 | macOS Big Sur 11.1                                 |
| 处理器   | Intel Core i3-4000M (ig-platform-id:0x0A260006 device-id:0x04128086)                  |
| 内存     | 8 GB 1600 MHz DDR3                        |
| 显卡     | Intel HD Graphics 4600 2048 MB    |
| 有线网卡     | Realtek  8111E-VL                     |
| 无线网卡     | Intel AC3160                     |
| 蓝牙     | Intel Bluetooth                     |
| 声卡     | Realtek ALC269 (layout-id 76)                                |
| SMBIOS | MacBookPro11,2     |


### 正常工作的功能

- CPU 睿频、变频
- 核显
- 亮度调节
- 有线网卡
- 无线网卡
- 声音以及麦克风
- 原生电源管理
- 电池状态
- 蓝牙
- USB 3.0x1 USB 2.0x2
- 睡眠唤醒(由于此机器的电源键实在难用，所以未禁用 USB 唤醒)
- Fn 快捷键
- 触摸板
- 摄像头
- Facetime/iMessage 等白苹果功能 (自行注入五码进行洗白)
- 隔空投送
- OTA 更新

### 如何刷入加入了微码的魔改BIOS

- 所需文件都在 `E479BIOS_EC` 中
- 已注入最新微码，不注入不能启动 macOS
- 务必使用我提供的 FPTW64
- 使用 AMIBCP4 进行 BIOS 高级菜单解锁
- 刷入命令：
```bash
fptw64.exe -f BIOS_E479_Unlocked.bin -bios
```

### 未测试的功能

- HDMI 无显示器无法测试

### 现存问题

- 电池若不被识别，需要手动重启一次
- 处理器 i3 被识别为 i7/i5 (注入 ProcessorType 但是无效，也许 Apple 没有 i3 的机器？不过不影响使用)
- 开机输入密码阶段有时会有些许卡顿延迟 (Azul4600Patcher 未能解决该问题)
- nVIDIA GeForce 940M 独立显卡 (没有任何解决方案)
- VGA (没有任何解决方案)

### 截图一览

![desktop.jpg](https://github.com/bavelee/Shinelon_A3S-Hackintosh/raw/master/Screenshots/desktop.jpg)

![usb.jpg](https://github.com/bavelee/Shinelon_A3S-Hackintosh/raw/master/Screenshots/usb.jpg)

![wifi.jpg](https://github.com/bavelee/Shinelon_A3S-Hackintosh/raw/master/Screenshots/wifi.jpg)

![bluetooth.jpg](https://github.com/bavelee/Shinelon_A3S-Hackintosh/raw/master/Screenshots/bluetooth.jpg)

# 如果我的辛勤工作对您有所帮助的话，感谢您的捐赠鼓励

![alipay.png](https://github.com/bavelee/Shinelon_A3S-Hackintosh/raw/master/Screenshots/alipay_250x250.png)

![wechat.png](https://github.com/bavelee/Shinelon_A3S-Hackintosh/raw/master/Screenshots/wechat_250x250.png)

