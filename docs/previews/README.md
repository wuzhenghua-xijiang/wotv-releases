# 版本截图

更新日期：2026-11-05。所有画面均由 Flutter 组件在受控示例数据下渲染，未启动视频解码或远程视频流。

## v1.1.32

手机、桌面和 TV 深浅色截图由沃TV v1.1.32 源码生成，源码提交为 `70678d3a7c7acdd903bf6a5bfbb16fb7db67b7f5`。截图用于展示对应平台的实际组件布局，不代表系统桌面或原生播放器的实机截图。影片、账号和播放记录为示例数据。

| 文件 | 页面 | 尺寸 |
| --- | --- | --- |
| `android-{home,search,detail,player,live,account}.png` | Android 手机：首页、搜索、详情、播放、直播、我的 | 390 × 844 |
| `desktop-{light,dark}-home.png` | 桌面版：浅色、深色首页 | 1440 × 900 |
| `android-tv-{light,dark}-home.png` | TV 版：浅色、深色首页，包含遥控器焦点 | 1280 × 720 |

Android 使用 `test/mobile_cinema_test.dart` 的原生组件截图入口，限定 `phone cinema pages retain media actions and fit the viewport` 场景，开启 `CAPTURE_MOBILE_CINEMA`。

桌面和 TV 使用 `test/ui_redesign_test.dart` 的平台配置、本地素材缓存和示例控制器，在独立截图入口中挂载生产 `AppShell`，选择「为你精选」栏目，并在 TV 上显示遥控器焦点。

图片均采用无损 PNG 压缩，输出像素与 Flutter 原图一致；来源、尺寸和文件 SHA-256 见 [manifest.json](manifest.json)。`wotv.png` 为现有应用图标，与当前源码一致。
