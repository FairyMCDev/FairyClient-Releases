# Fairylands 客户端 1.3.0

[下载完整 Windows 客户端](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.3.0/PCL-Fairylands-1.21.11-1.3.0-Windows-x64.zip) · [正式 Release](https://github.com/FairyMCDev/FairyClient-Releases/releases/tag/v1.3.0) · [下载安全检测报告（HTML）](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.3.0/Fairylands-1.3.0-Security-Report.html)

完整解压后打开 `PCL-Fairylands.exe`，保留同目录 DLL、PCL 与 `.minecraft` 文件夹。默认预装 Minecraft 1.21.11 + NeoForge，服务器地址 `fairymc.cn`；允许单人世界。26.2 / 26.3 的配套版本可在启动器中下载。

## 1.3.0 更新

三个分支的最终混淆 Mod JAR 均已嵌入完整的 `LICENSE_Fairylandsmod`，逐字节核对与工程 `LICENSE` 一致，不只是修改网页说明。元数据保持 `All Rights Reserved`。本次同步更新启动器版本、签名清单、启动器内置基线及服务端验包指纹；保留已有功能与加密图片资源。

| Minecraft | NeoForge | Mod 版本 | 内嵌许可文件 |
| --- | --- | --- | --- |
| 1.21.11 | 21.11.48 | 1.3.0 | LICENSE_Fairylandsmod |
| 26.2 | 26.2.0.93 | 1.3.0+mc26.2 | LICENSE_Fairylandsmod |
| 26.3 | 26.3.0.95 | 1.3.0+mc26.3 | LICENSE_Fairylandsmod |

[Fairylands 专有使用许可](https://github.com/FairyMCDev/FairyClient-Releases/blob/main/LICENSE)只适用于有权授权的自有部分，允许正常安装、游玩和个人备份，在法律允许范围内限制未经授权的反编译、解密、绕过校验和修改再分发。第三方许可、PCL 上游许可及法定例外不受影响。许可条款不是防破解技术措施。

已有客户端联网启动时可按签名清单更新对应 Mod。PCL 自身自动更新保持关闭；需要新版启动器时请下载完整包。若服务器开启 HandShaker 文件指纹校验，管理员须同步 1.3.0 服务端规则；本次没有自动部署线上服务器。

## 安全检测报告

**本次 Microsoft Defender 对完整解压目录和最终 ZIP 的扫描均已完成，未发现威胁。** 由发行方 DevXingMC 使用本机 Microsoft Defender Antivirus 执行并整理，不是微软安全认证、独立第三方审计或绝对安全保证。按维护者要求，未运行游戏测试，也未进行多引擎检测。

本报告覆盖默认 1.21.11 完整客户端的 5,059 个文件及其最终 ZIP，包含启动器、DLL、Mod、Java 和游戏资源。扫描器的文件格式、嵌套深度及检测能力限制仍适用。

| 项目 | 解压目录 | 最终 ZIP |
| --- | --- | --- |
| 开始时间 | 2026-10-21 11:24:44 UTC+8 | 2026-10-21 11:27:24 UTC+8 |
| 完成时间 | 2026-10-21 11:26:16 UTC+8 | 2026-10-21 11:34:40 UTC+8 |
| 平台版本 | 4.18.26090.9 | 4.18.26090.9 |
| 引擎版本 | 1.1.26090.9 | 1.1.26090.9 |
| 病毒库版本 | 1.461.118.0 | 1.461.118.0 |
| 病毒库更新时间 | 2026-10-20 15:02:06 UTC+8 | 2026-10-20 15:02:06 UTC+8 |
| 扫描退出码 | 0 | 0 |
| 原始结论 | found no threats | found no threats |

扫描命令：`MpCmdRun.exe -Scan -ScanType 3 -File <扫描目标> -DisableRemediation`。该参数使本次扫描不执行检测后处置，启用压缩档扫描并忽略文件排除规则；实时防护保持开启。完整原始输出及逐文件 SHA-256 见[可下载报告](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.3.0/Fairylands-1.3.0-Security-Report.html)。

### 完整包校验

文件：`PCL-Fairylands-1.21.11-1.3.0-Windows-x64.zip`；大小：**590607223 bytes**。扫描前、扫描后与上传前的 SHA-256 一致：

```text
2618b2b78c8501b28446041826f60c36bfb1d28c15ae837a40a464a468fc39e7
```

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath './PCL-Fairylands-1.21.11-1.3.0-Windows-x64.zip'
```

### SmartScreen 与签名状态

启动器 EXE / 配套 DLL 的 Authenticode 状态均为 `NotSigned`。新文件或未签名文件仍可能出现“Windows 已保护你的电脑 / 未知应用”，该信誉提示本身不是检出具体病毒的结论；这份扫描报告不会消除提示。请从官方发布链接下载并核对哈希，出现具体威胁名称时停止运行并反馈。

参考：[微软 SmartScreen 信誉说明](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/smartscreen-reputation)、[Defender 扫描命令](https://learn.microsoft.com/en-us/defender-endpoint/command-line-arguments-microsoft-defender-antivirus)。

## 附件与源码说明

- 完整包文件名不含 `-Glass`，包内没有独立 TXT、使用说明或安全检测报告。检测报告仅在本 README 和 Release 独立提供。
- [第三方署名、许可及启动器修改源码](https://github.com/FairyMCDev/FairyClient-Releases/blob/main/docs/third-party-notices-1.3.0.html)在公开仓库提供；Fairylands Mod 的维护源码保存在私人仓库。
- `client-index.json` 与三个 Mod JAR 用于自动更新，普通玩家下载完整包即可。独立 `SHA256SUMS.txt` 不再发布。
- GitHub 自动生成的 Source code ZIP / tar.gz 是本公开仓库的标签快照，不是私人开发仓库源码包。
