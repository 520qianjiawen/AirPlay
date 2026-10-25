# 电视投屏安装包 (APK)

修复了投屏过程中电视长时间无操作自动进入休眠、待机或屏保模式的 Bug。

### 安装包版本说明

| 文件名 | 适用平台 / 设备 | 说明 |
| :--- | :--- | :--- |
| **`app-universal-debug.apk`** | **全部电视与盒子 (推荐)** | 通用架构版本，内置全部 ABI，兼容性最强 |
| **`app-arm64-v8a-debug.apk`** | 64 位现代 Android TV / 电视盒子 | 适用于近年主流电视（如小米电视、索尼、外贸盒子等） |
| **`app-armeabi-v7a-debug.apk`** | 32 位老旧设备 | 适用于较早期的旧款电视芯片 |

### 安装方法

1. **U盘安装**：将 `app-universal-debug.apk` 拷贝到 U 盘，插入电视并在“文件管理器”中打开安装。
2. **ADB 无线安装**：
   ```bash
   adb connect <电视IP>:5555
   adb install -r app-universal-debug.apk
   ```
