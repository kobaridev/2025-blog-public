> 如何激活 Windows / Office / 扩展更新（ESU）？

## 方法 1 - PowerShell ❤️
### 1、打开 PowerShell
点击开始菜单 ，输入 PowerShell，然后打开它。
### 2、复制粘贴下面的代码，然后按下回车键。

- 针对 Windows 8、10、11： 📌
```bash
irm https://get.activated.win | iex
```

- 如果上述设置被 ISP/DNS 阻挡，试试这个（需要更新 Windows 10 或 11）：
```bash
iex (curl.exe -s --doh-url https://1.1.1.1/dns-query https://get.activated.win | Out-String)
```

- 适用于 Windows 7 及更高版本：
```bash
iex ((New-Object Net.WebClient).DownloadString('https://get.activated.win'))
```
- 脚本无法启动❓使用方法 2。
### 3、激活菜单会出现。
 **选择绿色高亮选项**来激活 Windows 或 Office。
### 4、Done! 

## 方法2 - 传统（Windows Vista 及更高版本）
### 下载脚本
[**MAS_AIO.cmd**](https://dev.azure.com/massgrave/Microsoft-Activation-Scripts/_apis/git/repositories/Microsoft-Activation-Scripts/items?path=/MAS/All-In-One-Version-KL/MAS_AIO.cmd&download=true) 或完整 [**ZIP**](https://dev.azure.com/massgrave/Microsoft-Activation-Scripts/_apis/git/repositories/Microsoft-Activation-Scripts/items?$format=zip)。
### 运行名为 MAS_AIO.cmd 的文件。

>你会看到激活选项。请按照屏幕上的指示作。
>就这样。