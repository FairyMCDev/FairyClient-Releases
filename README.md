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
| 最终 ZIP 扫描 | 2026-10-21 10:26:37 UTC+8 至 2026-10-21 10:34:52 UTC+8 |
| 两次退出码 | 0 |
| 扫描结论 | 均明确返回 `found no threats` |
| 实时防护 | 扫描期间保持开启 |
| 启动器 EXE / 配套 DLL 的 Authenticode 状态 | `NotSigned`（尚未正式签名） |

扫描范围为完整解压目录的 **5060 个文件**，包含启动器、DLL、Mod、Java 运行时、游戏资源及使用说明；随后生成内置报告并打包，再对最终 ZIP 扫描。最终包有 5061 个文件。嵌套格式、深度及扫描器本身的能力限制仍适用。

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

文件：`PCL-Fairylands-1.21.11-1.2.9-Windows-x64.zip`，大小：**591909252 bytes**。最终 ZIP 扫描前、扫描后及上传前的 SHA-256 一致：

```text
a7d9b4aac429a930031bd71f707f2e83421c4e46249a14ba54d62ddf388997fd
```

玩家可用 PowerShell 核对下载文件：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath './PCL-Fairylands-1.21.11-1.2.9-Windows-x64.zip'
```

[下载完整 HTML 报告](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.2.9/Fairylands-1.2.9-Security-Report.html)，其中包含全部目录扫描文件的 SHA-256 清单、原始扫描记录和签名状态。完整包内也附有目录扫描报告。

### 关于 SmartScreen 提示

“Windows 已保护你的电脑 / 未知应用”是 SmartScreen 文件与发布者信誉提示，本身不是检出具体病毒的结论。本版启动器 EXE 和配套 DLL 尚未正式签名，仍可能显示此提示；附加报告不会消除它。请从本页官方链接下载并核对哈希。如出现具体威胁名称，应停止运行并反馈。

微软资料：[SmartScreen 信誉说明](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/smartscreen-reputation)、[Defender 命令行扫描](https://learn.microsoft.com/en-us/defender-endpoint/command-line-arguments-microsoft-defender-antivirus)。

## 下载文件说明

- 普通玩家下载完整 ZIP 即可；包名已去掉 `-Glass`，独立 TXT 文件已移除。
- 必要的第三方署名、完整许可和启动器修改源码保留在包内 `使用说明.html`。
- `client-index.json` 和三个 Mod JAR 是自动更新所需文件，请保留；独立 `SHA256SUMS.txt` 不再发布，校验值见上方与报告。
- GitHub 自动显示的 `Source code (zip/tar.gz)` 是本公开仓库的标签快照，不是私人开发仓库的源码包；客户端开发源码继续保存在私人仓库。
