# Fairylands 客户端下载

## FairyClient 1.3.2

NeoForge 和 Fabric 两个完整包现在均内置 **Minecraft 1.21.11、26.2、26.3**，包括游戏文件、资源、对应加载器、优化 Mod 和 Java 21/25。在启动器的版本选择中直接切换，无需再次安装这三个版本。默认选择 1.21.11；文件名保留此默认版本，包内实际包含三个版本。

| 加载器 | 完整客户端下载 | 大小 |
| --- | --- | --- |
| Fabric | [下载 Windows x64 完整包](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.3.2/PCL-Fairylands-Fabric-1.21.11-1.3.2-Windows-x64.zip) | 976.5 MiB |
| NeoForge | [下载 Windows x64 完整包](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.3.2/PCL-Fairylands-NeoForge-1.21.11-1.3.2-Windows-x64.zip) | 1085.4 MiB |

### 本次修改

- Fabric 下载页从本地签名基线自动选择配套 Loader 0.19.5，避免手动选择其他版本后被拦截；提示中的 Loader 版本也从基线读取。
- 26.2、26.3 各自内置 Java 25，1.21.11 内置 Java 21；每个游戏配置都使用自己版本文件夹中的运行环境。
- 游戏窗口标题统一为 `Fairylands Network | 玩家QQ社群: 677371713`。
- 六个 Fairylandsmod JAR 沿用 1.3.1，内容和服务端文件指纹未改变。这次升级的是客户端、启动器与完整包。
- 保留后台新版提示；检查失败或 8 秒超时跳过，不阻塞本地游戏启动。发现新版时显示更新内容，可下载新版或稍后处理。
- 保留单人世界；多人列表 20 个条目均连接 `fairymc.cn`。

### 使用

完整解压后打开 `PCL-Fairylands.exe`，选择离线用户名或微软账号，在“版本选择”中选择 1.21.11、26.2 或 26.3。NeoForge 和 Fabric 分开解压，不混装两个加载器的 Mod。更新前备份已有存档。

微软登录和多人服务器连接仍需联网；手动重新安装或修复损坏的游戏文件也可能访问下载服务。配套 Mod 可以从随包缓存修复。

仅完成启动器编译和文件、哈希、依赖配置核对，按维护者要求未运行 PCL、Minecraft 或服务器测试。本次不提供检测报告。

### 更新附件和许可

玩家只需下载上表的完整 ZIP。`client-index.json`、`client-index-fabric.json` 是签名更新清单；单独 JAR 是相应游戏和加载器的 Mod，不能作为完整客户端。

PCL 原作者：龙腾猫跃。本客户端是 Fairylands 第三方美化版，非 PCL 官方版本。第三方署名、许可及启动器修改源码单独提供：[NeoForge 说明](https://github.com/FairyMCDev/FairyClient-Releases/blob/main/docs/third-party-notices-1.3.2-neoforge.html)、[Fabric 说明](https://github.com/FairyMCDev/FairyClient-Releases/blob/main/docs/third-party-notices-1.3.2-fabric.html)。客户端 ZIP 不包含使用说明或检测报告。

### 完整包 SHA-256

`PCL-Fairylands-Fabric-1.21.11-1.3.2-Windows-x64.zip`

```text
627c62ff5b2023772956e1db58fc0bcb680a4d99a664a11d15299772d3eac0e9
```

`PCL-Fairylands-NeoForge-1.21.11-1.3.2-Windows-x64.zip`

```text
4e2a30d372bdf963113adf936860858cd450ad7747761eaaf82bd8917231e99d
```

Fairylandsmod 自有部分适用 [专有使用许可](LICENSE)；第三方组件保留各自许可。
