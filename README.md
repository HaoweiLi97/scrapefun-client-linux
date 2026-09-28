# ScrapeFun Client for Linux

**简体中文** · [English](./README.en.md)

[产品主页](https://github.com/HaoweiLi97/ScrapeFun) · [稳定版下载](https://github.com/HaoweiLi97/scrapefun-client-linux/releases/latest) · [全部发行](https://github.com/HaoweiLi97/scrapefun-client-linux/releases) · [在线文档](https://scrapefun.com/#/docs)

> 文档更新：2026-09-28。下列版本和资产为核对当日的稳定版；后续以对应 Release 为准。

Linux 桌面客户端，连接已有 ScrapeFun Server，浏览影视媒体库、播放资源和阅读漫画。媒体库、用户及进度由 Server 管理。

## 下载与系统环境

| 项目 | 当前稳定版 |
| --- | --- |
| 版本 | [0.0.4](https://github.com/HaoweiLi97/scrapefun-client-linux/releases/tag/v0.0.4) |
| 架构 | x64 / amd64 |
| 安装包 | Debian / Ubuntu `.deb`、`.AppImage` |
| 校验文件 | 单文件 `.sha256`、`SHA256SUMS` |

从[稳定版下载页](https://github.com/HaoweiLi97/scrapefun-client-linux/releases/latest)获取所需文件。当前 Release 未提供 rpm 或 arm64 包；不要根据打包计划推定下载支持。需要图形桌面环境，系统依赖以包管理器检查和当前 Release 为准。

## 安装

Debian / Ubuntu 用户下载匹配的 deb 后，在下载目录执行：

```bash
sudo apt install ./scrapefun-client-electron-linux-0.0.4-stable-x64.deb
```

AppImage 用户下载后执行：

```bash
chmod +x ScrapeFun-Client-0.0.4.AppImage
./ScrapeFun-Client-0.0.4.AppImage
```

如系统报告缺少运行依赖，请按发行版说明处理。下载了 `SHA256SUMS` 和相应包时，可先运行：

```bash
sha256sum --check --ignore-missing SHA256SUMS
```

## 连接 Server

在连接页面填写运行中的 Server 地址，例如 `http://192.168.1.10:8096`，然后使用该 Server 的账号登录。Server 可以部署在 Docker、macOS 或 Windows 上；连接失败时先确认地址、端口、网络及服务状态。

## 更新与配置

AppImage 安装支持基于 GitHub Release 的更新，也可以手动替换 AppImage。deb 安装使用系统包管理器安装新版，不使用 AppImage 的更新方式。

同一用户下覆盖安装通常保留本地连接设置。不要主动删除客户端用户配置目录；删除它会重置连接配置。服务端媒体库和业务数据需在 Server 侧备份。

## 故障排查

安装失败时记录发行版、CPU 架构、安装包名和包管理器输出。播放问题请同时提供 Server 与 Client 版本、媒体编码及脱敏日志。

## 支持与授权

本仓库提供平台安装说明和官方发行资产。使用问题与功能建议请提交到[主仓库 Issues](https://github.com/HaoweiLi97/ScrapeFun/issues)；账号、激活或私密日志请联系 `scrapefun@outlook.com`。报告安全问题请按[安全说明](./SECURITY.md)私密提交。

新的商业许可声明见 [LICENSE](./LICENSE)，完整条款见[软件使用许可协议](./EULA.md)。个人、家庭及组织内部可正常使用；Pro 需有效授权，软件再分发、转售、客户交付和收费托管须单独书面授权。该声明不追溯改变既有授权；现有资产以其随包许可为准，第三方组件继续适用各自许可证。

[发行与兼容性说明](https://github.com/HaoweiLi97/ScrapeFun/blob/main/RELEASE_POLICY.md) · [第三方组件说明](https://github.com/HaoweiLi97/ScrapeFun/blob/main/THIRD_PARTY_NOTICES.md) · [支持流程](./SUPPORT.md)
