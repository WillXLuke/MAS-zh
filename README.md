## This is a fork of MAS providing Simplified Chinese support.


<h1 align="center">Microsoft  Activation  Scripts (MAS)</h1>

<p align="center">开源的 Windows 和 Office 激活工具，支持 HWID、Ohook、TSforge 和 Online KMS 激活方式，并提供高级故障排除功能。</p>

<hr>
  
## 如何激活 Windows / Office / 扩展安全更新（ESU）？

### 方法 1 - PowerShell ❤️

1. 点击**开始菜单**，输入 `PowerShell`，然后打开它。

2. 复制并粘贴下面的代码，然后按 **Enter**。  
   - 适用于 **Windows 8.1、10 和 11**：
     ```
     irm https://get.activated.win | iex
     ```
	 如果上述命令被阻止（由 ISP/DNS 造成），请尝试以下命令（需要较新版本的 Windows 10 或 11）：  
	 ```
	 iex (curl.exe -s --doh-url https://1.1.1.1/dns-query https://get.activated.win | Out-String)
	 ```
	 - **脚本无法启动？请使用下面列出的方法 2。**

3. 在出现的菜单中，输入对应**绿色**选项的数字。

---

### 方法 2 - 传统方式（Windows Vista 及更高版本）

1.   下载脚本：
      *   [**MAS_AIO.cmd**](https://dev.azure.com/massgrave/Microsoft-Activation-Scripts/_apis/git/repositories/Microsoft-Activation-Scripts/items?path=/MAS/All-In-One-Version-KL/MAS_AIO.cmd&download=true)（直接下载脚本）
      *   [**MAS_AIO.zip**](https://dev.azure.com/massgrave/Microsoft-Activation-Scripts/_apis/git/repositories/Microsoft-Activation-Scripts/items?$format=zip)（如果直接下载的脚本被浏览器阻止）
2.   运行 `MAS_AIO.cmd` 文件。
3.   在出现的菜单中，输入对应**绿色**选项的数字。

---

> [!TIP]
> - 某些 ISP/DNS 提供商会阻止访问我们的域名。你可以通过在浏览器中启用 [DNS-over-HTTPS (DoH)](https://developers.cloudflare.com/1.1.1.1/encryption/dns-over-https/encrypted-dns-browsers/) 来绕过此限制。 
> - **遇到问题？** 请访问我们的[故障排除页面](https://massgrave.dev/troubleshoot)，或在 [GitHub](https://github.com/massgravel/Microsoft-Activation-Scripts/issues) 上提交 issue。

> [!NOTE]
>
> - PowerShell 中的 `irm` 命令用于从指定 URL 下载脚本，`iex` 命令用于执行该脚本。
> - 在执行命令之前，请务必仔细检查 URL；手动下载文件时，请确认来源可信。
> - 请警惕第三方通过篡改 PowerShell 命令中的 URL 来传播伪装成 MAS 的恶意软件。

---

<div align="center">
	
### 主页 - [https://massgrave.dev/](https://massgrave.dev/)
