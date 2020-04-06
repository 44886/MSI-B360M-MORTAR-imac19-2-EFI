# 微星 B360M 迫击炮 + i7 8700 + AMD 独显黑苹果 EFI

此EFI fork自 [andot/MSI-B360M-MORTAR-IMACPRO-EFI](https://github.com/andot/MSI-B360M-MORTAR-IMACPRO-EFI) 感谢原作者的贡献！

改动说明：我用原作者的efi,出现了长时间睡眠后，无法唤醒的问题，强制重启后，出现五国界面。然后再开机后看到系统的错误报告是和核显及缓冲帧有关系。

这才注意到，原EFI是选择的 imacPro1,1 ，但我改成了 imac19,2 ，EFI中缺少缓冲帧补丁。

原作者是 i7-8700 CPU，为什么不开核显呢？

## 实现功能
✅ 开启核显，打好缓冲帧补丁（硬件解码）

✅ 睡眠/唤醒

✅ 其他功能和原EFI一样


## 我的配置

|         硬件       |                   型号                  | 
|-------------------:|:----------------------------------------|
|               主板 | 微星 B360M 钛金版                       |
|                CPU | Intel Core i7-8700                      |
|               显卡 | 蓝宝石 RX560 4G   |
|              硬盘1 | 东芝 RC500                |
|              硬盘2 | 三星 860 EVO 1T                |
|               内存 |  DDR4 2400Mhz 8G*2   |
|        无线 + 蓝牙 | fenvi T919   |
|    麦克风 | blue yeti usb 接口   |
|               键盘 | 苹果二代无线                             |
|               鼠标 | 罗技 M220                               |
|            显示器1 | 21寸 1080p ASUS V229          |



## 更新注意事项

除了下面日志中列出的内容，其余的全是使用的原EFI东西

## 更新日志

### 2020年4月6日

* 新增了缓冲帧补丁。
* 修复长时间睡眠无法唤醒的问题。



![图片加载失败](/44886/MSI-B360M-MORTAR-imac19-2-EFI/ScreenShot/framebuffer.jpg)

![图片加载失败](/44886/MSI-B360M-MORTAR-imac19-2-EFI/ScreenShot/framebufferpatch.jpg)