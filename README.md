# Fairylands 客户端下载

## FairyClient 1.3.1

新增独立 Fabric 客户端；NeoForge 和 Fabric 均支持 Minecraft **1.21.11、26.2、26.3**。两个完整包都预装 1.21.11 和 Java 21，26.2、26.3 的游戏文件及 Java 25 在下载页另行安装。

| 加载器 | 完整客户端下载 | 大小 |
| --- | --- | --- |
| Fabric | [下载 Windows x64 完整包](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.3.1/PCL-Fairylands-Fabric-1.21.11-1.3.1-Windows-x64.zip) | 598.7 MiB |
| NeoForge | [下载 Windows x64 完整包](https://github.com/FairyMCDev/FairyClient-Releases/releases/download/v1.3.1/PCL-Fairylands-NeoForge-1.21.11-1.3.1-Windows-x64.zip) | 620.1 MiB |

### 更新内容

- 打开 PCL 后后台检查新版，成功发现新版时弹出更新内容，提供“下载新版客户端”和“稍后”。下载按钮前往发布页，不静默覆盖玩家目录。
- 检查失败或超过 8 秒直接跳过，不影响已有完整客户端启动。
- 随包缓存三个游戏版本的配套 Mod；安装与修复从本地复制，不在启动前强制访问 GitHub。
- 新增三个独立构建的 Fabric Fairylandsmod，保留星空菜单、圆角材质、Logo、HUD、按键和聊天功能。
- 保留单人世界；多人列表 20 个条目均连接 fairymc.cn。
- 六个专属 Mod JAR 都嵌入完整自有代码许可，保留第三方原有许可。

### 使用

完整解压后打开 `PCL-Fairylands.exe`，按提示选择离线用户名或微软账号。两个包分别安装，不要混装 NeoForge 和 Fabric 的 Mod。已有存档升级前自行备份。

首次安装游戏、微软登录及服务器连接仍需要相应网络服务。本地必需文件与缓存同时损坏时，请重新完整解压。

仅完成编译与静态文件核对，按维护者要求未启动 PCL、游戏或服务端测试。

### 其他附件

`client-index.json` 与 `client-index-fabric.json` 是签名更新清单；单独 JAR 用于相应游戏/加载器版本，不是完整客户端。只想游玩的玩家下载上表 ZIP 即可。

PCL 原作者：龙腾猫跃；本客户端是第三方美化版，非官方版本。第三方许可与启动器修改源码：[NeoForge 说明](https://github.com/FairyMCDev/FairyClient-Releases/blob/main/docs/third-party-notices-1.3.1-neoforge.html)、[Fabric 说明](https://github.com/FairyMCDev/FairyClient-Releases/blob/main/docs/third-party-notices-1.3.1-fabric.html)。

## 完整包 SHA-256

`PCL-Fairylands-Fabric-1.21.11-1.3.1-Windows-x64.zip`

```text
1941980dbeb5221e9014d716fbd972c13bfc8efe1d1d118115d8e7a4459c13fa
```

`PCL-Fairylands-NeoForge-1.21.11-1.3.1-Windows-x64.zip`

```text
a95864b07b476e6fa6ed95ddfb9b7ee0d7f8b524da67fd4d95da60ee45283df1
```

Fairylandsmod 自有部分适用本仓库 [专有使用许可](LICENSE)。第三方组件保留各自作者和许可。
