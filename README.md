# ScrapeFun Client for Linux

> 最后更新：2026 年 7 月 26 日

ScrapeFun Client 是用于连接现有 ScrapeFun Server 的 Linux 桌面客户端。

## 下载

从 [Releases](https://github.com/HaoweiLi97/scrapefun-client-linux/releases/latest) 选择与你的发行版和处理器匹配的安装包：

- Debian / Ubuntu：`.deb`
- Fedora / RHEL 兼容发行版：`.rpm`
- 架构：`x64` 或 `arm64`，以文件名为准

每个版本会同时提供单文件 `.sha256` 和汇总的 `SHA256SUMS`。

## 安装

Debian / Ubuntu：

```bash
sudo apt install ./scrapefun-client-electron-linux-*.deb
```

Fedora / RHEL：

```bash
sudo dnf install ./scrapefun-client-electron-linux-*.rpm
```

## 连接服务器

首次打开客户端后，填写 ScrapeFun Server 地址，例如：

```text
http://192.168.1.10:8096
```

服务器可以来自 Docker、macOS Server 或 Windows Server。

## 更新

有新版本时，从 Releases 下载并安装同架构的新包即可，客户端连接配置会保留。

## 相关链接

- [部署 ScrapeFun Server](https://github.com/HaoweiLi97/ScrapeFun)
- [产品网站](https://mightly.store/)
