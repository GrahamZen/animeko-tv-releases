# Animeko TV 版下载

[![Latest Release](https://img.shields.io/github/v/release/GrahamZen/animeko?include_prereleases&label=%E4%B8%8B%E8%BD%BD&labelColor=06599d&color=043b69)](https://github.com/GrahamZen/animeko/releases/latest)

这是[open-ani/animeko](https://github.com/open-ani/animeko) 的 **第三方 Android TV 适配 Fork**的**发布分发仓库**，源代码见[**GrahamZen/animeko**](https://github.com/GrahamZen/animeko)。

## 📺 Android TV 版说明

本项目在上游基础上完成了大部分 Android TV 遥控器适配，并让应用图标显示在电视主屏幕（LEANBACK 启动器）上。安装后在更新 release 之后会在主页提醒，在设置里可以直接更新。

除遥控器焦点适配外，部分页面针对电视大屏**专门重新设计**：

| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/tv-home.png" alt="TV 主页 - 热门动画介绍轮播" width="600"/> |
|:---------------------------------------------------------------------------------------------------:|

| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/tv-home2.png" alt="TV 主页 - 推荐" width="600"/> |
|:---------------------------------------------------------------------------------------------------:|

| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/tv-home3.png" alt="TV 主页 - 继续观看" width="600"/> |
|:---------------------------------------------------------------------------------------------------:|



| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/tv-collection.png" alt="TV 主页 - 追番" width="600"/> |
|:---------------------------------------------------------------------------------------------------:|

| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/tv-search.png" alt="TV 主页 - 搜索" width="600"/> |
|:---------------------------------------------------------------------------------------------------:|

| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/subject-details1.png" alt="TV 动画详情页" width="600"/> |
|:--------------------------------------------------------------------------------------:|

| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/subject-details2.png" alt="TV 动画详情页 - 选集轮播" width="600"/> |
|:---------------------------------------------------------------------------------------------------:|

| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/subject-details3.png" alt="TV 动画详情页 - 作品信息" width="600"/> |
|:---------------------------------------------------------------------------------------------------:|


还提供两项电视系统级功能：

- **主屏预览频道**：电视主屏幕显示"热门动画"频道和"继续观看"行，点击卡片直达详情页（首次启动时按系统提示允许添加频道）。

| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/tv_preview_channels.png" alt="TV 主屏预览频道" width="600"/> |
|:----------------------------------------------------------------------------------------------:|

- **屏保**：轮播在看与热门动画的横版剧照，按确定键直达该动画详情页，左右键切换（需在系统设置 → 屏保中选择 Animeko）。

| <img src="https://raw.githubusercontent.com/GrahamZen/animeko/main/.readme/images/features/tv_screen_saver.png" alt="TV 屏保" width="600"/> |
|:------------------------------------------------------------------------------------:|

### 下载

| 平台          | 下载                                                                                                            |
|-------------|---------------------------------------------------------------------------------------------------------------|
| Android / 电视 | [前往 Releases 下载最新版 APK](https://github.com/GrahamZen/animeko/releases/latest)（推荐 `universal` 版本） |

> 不确定架构时请直接下载 `universal` 版本。该 APK 同时适用于手机、平板和电视盒子。

### ⚠️ 系统版本要求

- **推荐 Android 11（API 30）及以上**。
- 在 **Android 10 及以下** 的系统里很可能无法正确请求焦点，导致遥控器功能不可用。遇到遥控器无法操作的问题时，请先确认系统版本。
- NVIDIA Shield 等主流电视盒子的较新系统一般可正常使用。

### 遥控器使用说明

播放时如果焦点丢失，**按住确认键**可以找回焦点（在播放器界面会回到弹幕设置按钮，其他界面会回到左上角按钮）。

遥控器按钮支持：

- 播放 / 暂停键
- 左右键控制后退 / 前进
- 上一首 / 下一首键控制上一集 / 下一集
- 确认键唤出播放器组件，再按确认键将焦点移到弹幕设置按钮

以上功能在焦点位于"播放器任意按钮的上一级"时生效；焦点在播放器中任意按钮时，按返回键回到上一级。

> 最开始的登录部分如果焦点丢失，请接入鼠标完成登录，之后即可继续使用遥控器。

### 手动完成验证码页面的操作

| 操作              | 效果                                  |
|-----------------|-------------------------------------|
| 方向键             | 移动光标（先按一下方向键唤出光标）          |
| 确认键（短按）        | 在光标位置模拟触摸点击（用于通过验证码）      |
| 确认键（长按 ~500ms） | 点击"✓"（大部分情况通过验证码后会自动关闭）  |
| 返回键             | 取消，关闭对话框                          |

### 已知问题

- 右侧数据源侧边栏可能出现按返回键不关闭等问题，建议只使用播放器内的"选择数据源"按钮。
- 在 Android 10 及以下系统中可能无法正确请求焦点，从而无法使用遥控器功能（见上方系统版本要求）。

## 🔗 相关链接

| | |
|---|---|
| 源代码（TV Fork） | https://github.com/GrahamZen/animeko |
| 上游原项目 | https://github.com/open-ani/animeko |

---

*本仓库的 Release 由 [GitHub Actions 定时任务](.github/workflows/mirror-release.yml) 每天自动从源 Fork 镜像。*
