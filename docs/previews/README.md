# 预览图片

图片来自沃TV v1.1.10 的 Flutter 界面组件，按对应平台能力、窗口尺寸和主题生成，使用本地示例内容；用于展示实际组件布局，不代表系统桌面或原生播放器的实机截图。

源码版本：`698e0776957bbce8ccbfe516acbd3e2520b91368`。更新日期：2026-10-27。

| 文件前缀 | 平台布局 | 尺寸 |
| --- | --- | --- |
| `android` | Android 手机：首页、找片、详情、播放、直播、我的 | 390 × 844 |
| `desktop` | 桌面版：浅色、深色首页 | 1440 × 900 |
| `android-tv` | Android TV，包含遥控器焦点 | 1280 × 720 |

Android 使用 `android-<页面>.png`；桌面版和 TV 版分别使用 `<平台>-light-home.png`、`<平台>-dark-home.png`。仅保留这三类界面预览。

生成入口：Android 为 `test/mobile_cinema_test.dart` 的原生组件截图；桌面版与 TV 版为 `test/ui_redesign_test.dart` 的 `desktop` / `tv` 首页截图，启用本地海报素材。预览不启动视频解码或远程视频流。

`wotv.png` 为应用图标。
