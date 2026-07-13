# Animeko TV 版下载

[![Latest Release](https://img.shields.io/github/v/release/GrahamZen/animeko-tv-releases?include_prereleases&label=%E4%B8%8B%E8%BD%BD&labelColor=06599d&color=043b69)](https://github.com/GrahamZen/animeko-tv-releases/releases/latest)

这是 [**GrahamZen/animeko**](https://github.com/GrahamZen/animeko)（[open-ani/animeko](https://github.com/open-ani/animeko) 的 **Android TV 适配 Fork**）的**发布分发仓库**。

本仓库**不含源代码**，只做一件事：每天自动从上面的 Fork 拉取最新 Release 并原样发布到这里，方便直接下载 TV 版 APK，而无需进入完整的源码仓库。

## 📥 下载

👉 **[前往 Releases 下载最新版 APK](https://github.com/GrahamZen/animeko-tv-releases/releases/latest)**

不确定架构时请下载 `universal` 版本，它同时适用于手机、平板和电视盒子（如 NVIDIA Shield）。

## 📺 关于 TV 版

- 在原版功能之上增加了 **Android TV / Google TV 遥控器适配**，可在电视盒子上用遥控器操作，并在电视主屏幕（LEANBACK 启动器）显示图标。
- 详情页等界面针对电视大屏专门重新设计（TMDB 横版剧照背景、Prime Video 式选集轮播等）。
- 遥控器使用说明、系统版本要求与已知问题，请见源仓库的
  [「📺 Android TV 版说明」](https://github.com/GrahamZen/animeko#-android-tv-版说明)。

> **推荐 Android 11（API 30）及以上**；Android 10 及以下可能无法正确请求焦点，导致遥控器功能不可用。

## 🔗 相关链接

| | |
|---|---|
| 源代码（TV Fork） | https://github.com/GrahamZen/animeko |
| 上游原项目 | https://github.com/open-ani/animeko |
| 官网（上游） | https://animeko.org/ |

---

*本仓库的 Release 由 [GitHub Actions 定时任务](.github/workflows/mirror-release.yml) 自动从源 Fork 镜像，通常每天同步一次。*
