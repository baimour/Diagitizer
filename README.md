#  Diagitizer - 诊断启动程序

请注意，我们不会提供诊断文件！您可以从@1nsane_dev 的紫色工具中获取它们

特点：
+ 在启动时自动设置 usbserial bootarg
+ 一键启动诊断（正确设置后）


用法：

将引导链放在 ~/Documents/diagitizer_bootchain/

如果您使用 Purple 的引导链，您可能需要编辑文件名
您可以在 TheiPhoneWiki 和 supportedDevices.json 中查找的 DeviceModel 值

一个完整有效的引导链如下所示：


- iBSS.DeviceModel.img4
- iBoot.DeviceModel.img4
- diag.DeviceModel.img4

iPhone X 型号 D221 的示例：
- iBSS.D221.img4
- iBoot.D221.img4
- diag.D221.img4


如果只有 iBoot 和 diags 文件，则需要创建 iBSS 文件并将 DEADBEEF 字节放入其中。它应该如下所示：

![Image of DEEDBEED](https://github.com/j4nf4b3l/Diagitizer-Open-Source/blob/master/DEADBEEF_Example.png)

如果添加新模型，则需要修改supportedDevices.json并添加缺少的信息

这个工具在 MIT 许可下，所以随意贡献和修改你想要的 :)
