# Kiln Launcher

> 轻量的 Minecraft Java 版启动器。把「装版本」这件事变成一次点击。

一个 Windows 平台上的 Minecraft Java 启动器：单文件、免安装、内置运行环境，
不需要另外装 Java 或 Node。界面走 macOS 风格的三色点 + 圆角卡片，没有广告，也没有账号体系。

## 下载

- 官网：https://kilnlaun.asia
- 直链：https://kilnlaun.asia/downloads/KilnLauncher-Setup.exe
- 本仓库 Releases 页也会同步上传安装包

## 功能

**版本管理**
- 原版一键安装，指定任意版本
- Fabric 一键安装，可选加载器版本
- 自定义版本名；有其它版本依赖时拒绝删除底座，避免删坏

**模组**
- 内置 Modrinth 搜索：中文名、图标、下载量
- 中文关键词也能搜（输入「钠」= Sodium、「小地图」= Xaero's Minimap）
- 自动补齐依赖，可启停、删除

**整合包**
- 支持 `.mrpack` 导入，自动创建独立实例
- 实例的 mods / 存档 / 配置互不污染
- 也能直接从 Modrinth 搜整合包安装

**账户**
- **微软正版登录**：内置登录窗口，登录后自动加入账户列表，可直接进正版服
- **换皮肤**：账户页上传 PNG（64×64 / 64×32），不用去官网
- **皮肤站登录**：LittleSkin、Blessing Skin 等 Yggdrasil 外置登录
- **离线账户**：填个昵称即可

**其它**
- 内存按本机物理内存给档位，上限留足系统余量
- 下载源自动切换（官方 / BMCLAPI 镜像）
- 内置更新检查：发现新版本会提示，点一下自动下载并静默覆盖安装

## 系统要求

| 项目 | 要求 |
|---|---|
| 系统 | Windows 10 1809+ / Windows 11（64 位） |
| 运行库 | Microsoft Edge WebView2 运行时（Win11 自带，Win10 一般已装） |
| Java | 自动检测；缺失时可在设置页一键下载 Temurin JRE |
| 磁盘 | 约 40 MB（游戏本体另算） |

## 安装

1. 下载 `KilnLauncher-Setup.exe`
2. 双击运行，选择安装目录与数据位置
3. 首次启动会自动解包运行时（几秒钟，有进度条）

也可以只用单文件 `KilnLauncher.exe`，解包即用，不需要安装。

## 关于正版登录

如果登录后提示「没有 Xbox 档案」，说明这个微软账号还没创建过 Xbox 账号：

1. 用同一个账号打开一次 https://www.xbox.com 登录
2. 回到启动器重新点「用微软账号登录」

## 常见问题

**需要先装 Java 吗？**
不需要。启动器会扫描本机已有的 Java，按版本要求自动选择。

**会动我原来的存档吗？**
不会。默认使用独立目录（`%LOCALAPPDATA%\Kiln`），不碰官方启动器的 `.minecraft`。

**支持 Forge / NeoForge 吗？**
目前只支持 Fabric。界面上会明确标「即将支持」，不会装出半成品。

**被杀毒软件拦了怎么办？**
启动器会把内嵌的 Node 运行时解压到本地执行，行为类似自解压程序，容易被误判。加入信任即可。

**怎么卸载？**
系统设置里卸载，或运行安装目录里的 `Uninstall.exe`。卸载默认保留数据。

## 声明

本项目是非官方项目，与 Mojang Studios / Microsoft 无关。
Minecraft 是 Mojang Studios 的商标。使用本启动器需要拥有正版游戏或遵守相应服务条款。

## 反馈

问题与建议请提 Issue，或到官网查看联系方式。
