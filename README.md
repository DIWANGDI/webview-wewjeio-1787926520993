# wewjeio - Android WebView APK

## 配置信息
- 应用名称：wewjeio
- 网址：https://www.baidu.com
- 包名：com.baiduapp.app
- 版本：2.1
- 屏幕方向：自适应

## 构建方式

### 方式一：Android Studio
1. 下载安装 [Android Studio](https://developer.android.com/studio)
2. 打开 Android Studio → File → Open → 选择本项目根目录
3. 等待 Gradle 同步完成
4. Build → Build Bundle(s) / APK(s) → Build APK(s)
5. APK 输出：app/build/outputs/apk/debug/app-debug.apk

### 方式二：命令行
```bash
# Windows
gradlew.bat assembleDebug

# Mac / Linux
chmod +x gradlew && ./gradlew assembleDebug
```
APK 输出：app/build/outputs/apk/debug/app-debug.apk

### 方式三：GitHub Actions 自动构建（推荐，零成本）
1. 在 GitHub 创建新仓库（Public 仓库免费）
2. 将本项目所有文件推送到该仓库
3. 推送后自动触发编译（约 5-10 分钟）
4. 在仓库 Actions 页面找到对应的 workflow run
5. 在 Artifacts 区域下载 app-debug-apk.zip，解压即得 APK

> 已内置 .github/workflows/build-apk.yml，推送到 GitHub 即自动编译。
> GitHub 免费额度：Public 仓库无限分钟，Private 仓库每月 2000 分钟。
