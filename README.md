# xCam - Universal Virtual Camera Xposed Module

**xCam** is a high-performance, universal Xposed module built with the modern **LibXposed API (API 101)**. It allows users to replace live camera feeds and actual photo/video captures with virtual media sources (videos or images) across a wide range of Android applications.

## 🚀 Key Features

- **Full Capture Injection**: Replaces both the live preview and the **actual captured photo data** using JPEG (0x21/HAL_PIXEL_FORMAT_BLOB) injection techniques.
- **Universal Dual-Engine**:
    - **Advanced Legacy Engine**: High-performance OpenGL rendering and Byte Array hijacking for modern applications using legacy camera layers.
    - **Classic Camera Engine**: Advanced Surface Redirection and Direct MediaPlayer playback for applications using older camera APIs.
- **Synchronized Orientation**: Any rotation (90° steps) or horizontal mirroring applied to the preview is **perfectly synced** to the final captured result.
- **Smart Aspect Ratio**: Intelligent **Center Crop** logic ensures your media matches the target application's aspect ratio, preventing distorted or "stretched" results.
- **Hardware-Accelerated Rendering**: Powered by **OpenGL ES 2.0** for low-latency, battery-efficient video injection.
- **Modern LibXposed Architecture**: Fully compatible with modern Xposed environments like **LSPosed**, **Vector**, and **LSPatch**.
- **Process-Aware Hooking**: Intelligently identifies main application processes vs. sub-processes to prevent loops and ensure system stability.

## 📦 Installation

### Rooted Environments
1. Install the **xCam APK**.
2. Enable the module in your Xposed manager.
3. Select the **target applications** in the scope/manager.
4. Force stop and restart the selected applications.

### Non-Rooted Environments
1. Install the **xCam APK**.
2. Patch your target application using a compatible patching tool.
3. Install and run the patched application.

## 📖 Usage

1. Launch the **xCam** manager app.
2. Tap **Select Media** to choose a video (`.mp4`) or image (`.jpg`, `.png`).
3. Adjust the orientation using the **Rotate** and **Mirror** icons until the preview looks correct.
4. Open your target application. The virtual media will now replace the live camera feed.
5. Perform a capture operation; the result will be your virtual media, perfectly aligned and rotated.

## ⚖️ License

This project is licensed under the **GNU General Public License v3.0**.

```text
Copyright (C) 2026 hazbu
```

## ⚠️ Disclaimer

This module is intended for **educational and development purposes only**. Use it responsibly and at your own risk. The developer is not responsible for any misuse, privacy violations, or breaches of third-party service terms.
