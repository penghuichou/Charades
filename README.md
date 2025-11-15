# Charades
你比划我猜，完全使用AI开发的自用游戏App，在我的Pixel 8 Pro和一加7Pro手机上可以正常使用，其他机型没有测试过。
因为是自用，并且我没有代码知识，所以这里只是分享出来，如果有任何问题可能我没有能力处理。

## 💡 真实需求驱动AI完成

我是一名金融行业的培训师，经常需要组织团队游戏来调节气氛，比如这个我们经常玩的“你比划我猜”小游戏，我发现很难找到一款能让我方便地管理词库、组织多团队竞赛、并且没有广告干扰的应用。
虽然我对代码一窍不通，但因为之前有过通过AI制作小程序的成功经历，我决定再次借助AI的力量来解决这个痛点。

1.  **初始搭建**: 用 Google CLI 完成了项目的基础框架搭建。
2.  **转向 Android Studio**: 在打包的过程中，我发现 Android Studio 内置的有 Gemini 功能。于是，我将后续所有的开发工作全部迁移到了这里。
3.  **迭代与进化**: 整个过程全都是自然语言跟Gemini对话实现。
    *   从最开始仅有“录入”和“开始”的简单功能。
    *   到我们一起重构了数据持久化方案，让词库和队伍能够被永久保存。
    *   再到我们一次次地优化UI/UX，比如将列表改成卡片流，为按钮增加动效，为结果页加上庆祝动画...
    *   甚至连修复各种编译错误、运行时崩溃，乃至优化Gradle配置，都是通过与Gemini的对话完成的。

## 📸 应用截图

<img src="https://github.com/penghuichou/Charades/blob/79a4802a7d1ca2bd0fe3688a261823c2c1c86de3/images/Screenshot_20251114-094546.png" width="33%"><img src="https://github.com/penghuichou/Charades/blob/79a4802a7d1ca2bd0fe3688a261823c2c1c86de3/images/Screenshot_20251114-094637.png" width="33%"><img src="https://github.com/penghuichou/Charades/blob/79a4802a7d1ca2bd0fe3688a261823c2c1c86de3/images/Screenshot_20251114-094700.png" width="33%">

<img src="https://github.com/penghuichou/Charades/blob/79a4802a7d1ca2bd0fe3688a261823c2c1c86de3/images/Screenshot_20251114-094717.png" width="33%"><img src="https://github.com/penghuichou/Charades/blob/79a4802a7d1ca2bd0fe3688a261823c2c1c86de3/images/Screenshot_20251114-094918.png" width="33%"><img src="https://github.com/penghuichou/Charades/blob/79a4802a7d1ca2bd0fe3688a261823c2c1c86de3/images/Screenshot_20251114-094927.png" width="33%">

## ✨ 核心功能

*   **自定义词库管理:**
    *   **批量添加**: 支持在输入框中用空格隔开，一次性录入多个同类别词语。
    *   **分类系统**: 可为词语创建和指定分类，方便管理和筛选。
    *   **便捷选择**: 新增词语时，可从下拉菜单中快速选择已存在的分类。
    *   **筛选查看**: 在词库列表中，可按分类筛选，只查看特定类别的词语。
    *   **多选与批量删除**: 长按即可进入选择模式，支持多选、全选，并一键批量删除。

*   **动态有趣的队伍管理:**
    *   支持创建多支队伍进行对抗。
    *   每支队伍在创建时，会被自动分配一个随机的**动物Emoji头像**，增加趣味性。
    *   队伍信息会被**永久保存**，方便下次直接使用。

*   **沉浸式游戏体验:**
    *   可自由选择一个或多个词库分类组合成当轮游戏题库。
    *   支持自定义每回合的游戏时长。
    *   游戏时实时显示本轮得分。
    *   **动态倒计时**: 最后10秒，计时器会**变红变大**，并伴有沙漏图标，增加紧张感。
    *   **统一的UI风格**: 无论是词库管理还是回合总结，都使用优雅的“卡片流”来展示词语。

*   **精美且现代化的UI设计:**
    *   完全使用 **Jetpack Compose** 搭建，遵循最新的 **Material 3** 设计语言。
    *   **“边到边” (Edge-to-Edge)** 的沉浸式界面，与系统状态栏完美融合。
    *   一个极具质感、带有**“呼吸”动效**的“开始游戏”按钮。
    *   为冠军队伍准备的、带有**皇冠和烟花动画**的专属庆祝页面！

## 📲 下载与安装

您可以直接下载 `app-release.apk` 文件进行安装。

[![Download APK](https://img.shields.io/badge/Download-APK-brightgreen)](https://github.com/penghuichou/Charades/releases/download/app/app-release.apk)

