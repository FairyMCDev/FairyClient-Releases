# Fairylands 客户端

[下载完整 Windows 客户端](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.2.9/PCL-Fairylands-1.21.11-1.2.9-Windows-x64.zip) · [查看 Release](https://github.com/FairyMCDev/FairyClient-Releases/releases/tag/v1.2.9) · [下载安全检测报告（HTML）](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.2.9/Fairylands-1.2.9-Security-Report.html)

完整解压后打开 `PCL-Fairylands.exe`，保留同目录 DLL、PCL 与 `.minecraft` 文件夹。默认预装 Minecraft 1.21.11 + NeoForge；启动器也提供 26.2 / 26.3 的配套版本。服务器地址：`fairymc.cn`。

## 安全检测报告 · 1.2.9

**Microsoft Defender 对完整解压目录及最终 ZIP 的扫描均已完成，本次未发现威胁。**

此报告由发行方 **DevXingMC** 使用本机 Microsoft Defender Antivirus 执行并整理，记录特定时间与病毒库版本的扫描结果。它不是微软安全认证或独立第三方审计，也不构成绝对安全保证。未执行多引擎检测或启动游戏验证。

| 检测项目 | 记录 |
| --- | --- |
| 扫描器 | Microsoft Defender Antivirus |
| 平台版本 | 4.18.26090.9 |
| 引擎版本 | 1.1.26090.9 |
| 病毒库版本 | 1.461.118.0 |
| 病毒库更新时间 | 2026-10-20 15:02:06 UTC+8 |
| 完整目录扫描 | 2026-10-21 10:24:10 UTC+8 至 2026-10-21 10:25:44 UTC+8 |
| 最终 ZIP 扫描 | 2026-10-21 11:03:30 UTC+8 至 2026-10-21 11:10:55 UTC+8 |
| 两次退出码 | 0 |
| 扫描结论 | 均明确返回 `found no threats` |
| 实时防护 | 扫描期间保持开启 |
| 启动器 EXE / 配套 DLL 的 Authenticode 状态 | `NotSigned`（尚未正式签名） |

原目录扫描覆盖 5,060 个文件（包含当时的使用说明）。此次只从完整包移除使用说明和随后生成的内置报告，保留的 **5059 个文件**逐一核对 SHA-256，与原来已扫描的文件一致。当前 ZIP 共 5059 个文件，并已重新单独扫描。嵌套格式、深度及扫描器本身的能力限制仍适用。

两次均使用自定义扫描命令：

```powershell
MpCmdRun.exe -Scan -ScanType 3 -File <扫描目标> -DisableRemediation
```

`-DisableRemediation` 只禁止此次扫描的检测后处置，同时启用压缩档扫描并忽略文件排除规则；不会关闭系统实时防护。

两次命令输出如下（目标路径已脱敏）：

```text
完整解压目录：
Scan starting...
Scan finished.
Scanning <release-target> found no threats.
最终 ZIP：
Scan starting...
Scan finished.
Scanning <release-target> found no threats.
```

### 文件校验

文件：`PCL-Fairylands-1.21.11-1.2.9-Windows-x64.zip`，大小：**590706144 bytes**。最终 ZIP 扫描前、扫描后及上传前的 SHA-256 一致：

```text
1fa12e9ef24ee4637761d9fd5add4cc99a0ce2190b21123b4f78fdbeebd1fd2b
```

玩家可用 PowerShell 核对下载文件：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath './PCL-Fairylands-1.21.11-1.2.9-Windows-x64.zip'
```

[下载完整 HTML 报告](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.2.9/Fairylands-1.2.9-Security-Report.html)，其中包含全部目录扫描文件的 SHA-256 清单、原始扫描记录和签名状态。完整包内不附使用说明或检测报告。

### 关于 SmartScreen 提示

“Windows 已保护你的电脑 / 未知应用”是 SmartScreen 文件与发布者信誉提示，本身不是检出具体病毒的结论。本版启动器 EXE 和配套 DLL 尚未正式签名，仍可能显示此提示；附加报告不会消除它。请从本页官方链接下载并核对哈希。如出现具体威胁名称，应停止运行并反馈。

微软资料：[SmartScreen 信誉说明](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/smartscreen-reputation)、[Defender 命令行扫描](https://learn.microsoft.com/en-us/defender-endpoint/command-line-arguments-microsoft-defender-antivirus)。

## Fairylands 自有代码许可

Fairylandsmod 自有代码采用 [Fairylands 专有使用许可](https://github.com/FairyMCDev/FairyClient-Releases/blob/main/LICENSE)（All Rights Reserved），不是 MIT 或其他开源许可证。允许正常安装、游玩和个人备份；在法律允许范围内，禁止未经授权的反编译、解密、绕过校验、修改再分发和冒充官方。第三方组件及 PCL 衍生部分继续适用各自上游许可，法定例外与既有合法授权不受影响。许可条款不是防破解技术措施。


