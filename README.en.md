# ScrapeFun Client for Linux

[简体中文](./README.md) · **English**

[Product overview](https://github.com/HaoweiLi97/ScrapeFun/blob/main/README.en.md) · [Stable downloads](https://github.com/HaoweiLi97/scrapefun-client-linux/releases/latest) · [All releases](https://github.com/HaoweiLi97/scrapefun-client-linux/releases) · [Online documentation](https://scrapefun.com/?lang=en#/docs)

> Updated: 2026-09-28. Versions and assets below are the stable releases checked on this date. Follow the corresponding Release for later changes.

Linux desktop client for connecting to an existing ScrapeFun Server, browsing movie and TV libraries, playing resources, and reading comics. Server manages libraries, users, and progress.

## Downloads and environment

| Item | Current stable release |
| --- | --- |
| Version | [0.0.4](https://github.com/HaoweiLi97/scrapefun-client-linux/releases/tag/v0.0.4) |
| Architecture | x64 / amd64 |
| Packages | Debian / Ubuntu `.deb`, `.AppImage` |
| Checksums | Individual `.sha256` files, `SHA256SUMS` |

Get the package from the [stable download page](https://github.com/HaoweiLi97/scrapefun-client-linux/releases/latest). This release does not provide rpm or arm64 packages; packaging plans do not establish download availability. A graphical desktop environment is required. System dependencies follow the package manager's checks and the specific release.

## Installation

For Debian / Ubuntu, download the matching deb and run in the download directory:

```bash
sudo apt install ./scrapefun-client-electron-linux-0.0.4-stable-x64.deb
```

For AppImage, download the file and run:

```bash
chmod +x ScrapeFun-Client-0.0.4.AppImage
./ScrapeFun-Client-0.0.4.AppImage
```

If your system reports missing runtime dependencies, follow your distribution's instructions. With `SHA256SUMS` and the corresponding packages downloaded, you can first run:

```bash
sha256sum --check --ignore-missing SHA256SUMS
```

## Connect to Server

On the connection page, enter the running Server's address, such as `http://192.168.1.10:8096`, then sign in with an account from that Server. Server can run in Docker, on macOS, or on Windows. If connection fails, check the address, port, network, and service status first.

## Updates and configuration

AppImage installations support updates through GitHub Releases, or you can replace the AppImage manually. For deb installations, install the new package with your system package manager; they do not use the AppImage update method.

Installing over the existing version under the same user normally retains local connection settings. Do not delete the client's user configuration directory unless you intend to reset those settings. Back up server libraries and business data on Server separately.

## Troubleshooting

For installation failures, include your distribution, CPU architecture, package filename, and package-manager output. For playback issues, also provide Server and Client versions, media codecs, and logs with sensitive information removed.

## Support and licensing

This repository provides platform installation instructions and official release assets. Submit usage questions and feature requests to the [main repository Issues](https://github.com/HaoweiLi97/ScrapeFun/issues). For accounts, activation, or private logs, contact `scrapefun@outlook.com`. Report security issues privately according to the [security instructions](./SECURITY.en.md).

See the new [commercial license statement](./LICENSE.en.txt) and full [software license agreement](./EULA.en.md). Ordinary personal, household, and internal organizational use is allowed. Pro requires a valid entitlement. Software redistribution, resale, customer delivery, and paid hosting require separate written authorization. The statement does not retroactively change existing licenses; existing assets follow their supplied licenses, and third-party components retain their own licenses.

[Releases and compatibility](https://github.com/HaoweiLi97/ScrapeFun/blob/main/RELEASE_POLICY.en.md) · [Third-party components](https://github.com/HaoweiLi97/ScrapeFun/blob/main/THIRD_PARTY_NOTICES.en.md) · [Support](./SUPPORT.en.md)
