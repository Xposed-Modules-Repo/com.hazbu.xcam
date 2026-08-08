# xCam - Universal Virtual Camera Xposed Module (v17.5-Stable)

**xCam** is a high-performance, universal Xposed module built with the modern **LibXposed API (API 101)**. It allows users to replace live camera feeds and actual photo captures with virtual media sources across a wide range of Android applications, from legacy devices to the latest Android 16.

## 🚀 Key Features

- **Universal OS Support (Android 9 - 16)**: Built with a hybrid architecture that automatically adapts to the device's API level (API 28 to API 37).
- **Dual-Engine Pipeline**:
    - **Legacy Engine (API 28-30)**: Uses high-stability Camera1 hooks and Legacy Camera2 `produceFrame` hijacking for Android 9, 10, and 11.
    - **Modern Engine (API 31-37)**: Features **Surgical Diversion** and **OutputConfiguration Swapping** to bypass the strict security of Android 12 through Android 16.
- **The Hunter Hook (Universal Capture)**: A revolutionary `BitmapFactory` interception system that ensures 100% success in replacing captured photo data across almost any application.
- **Surgical Target Diversion**: Intelligently redirects only the preview streams to a dummy source while allowing the actual capture data flow to reach our interceptors, preventing app hangs during photo sessions.
- **Hardware-Accelerated Rendering**: Powered by **OpenGL ES 2.0** for low-latency, battery-efficient video injection.
- **Perfect Orientation Sync**: Synchronizes rotation (90° steps) and mirroring between the preview and the final capture automatically.
- **Intelligent Center Crop**: Prevents distorted or stretched images by automatically adjusting the virtual media to the target app's aspect ratio.

## 📦 Installation

### Rooted Environments
1. Install the **xCam APK**.
2. Enable the module in your Xposed manager (e.g., **LSPosed**, **Vector**).
3. Select the **target applications** in the module scope.
4. Force stop and restart the selected applications.

### Non-Rooted Environments
1. Patch your target application using a tool like **LSPatch**.
2. Install the patched application and the xCam manager.

## 📖 Usage

1. Launch the **xCam** manager app.
2. Tap **Select Media** to choose a video (`.mp4`).
3. Adjust the orientation using the **Rotate** and **Mirror** icons.
4. Open your target application. The live camera feed will be replaced by your video.
5. Take a photo; xCam will intercept the process and save your virtual media as the result.

## ⚖️ License

This project is licensed under the **GNU General Public License v3.0**.

```text
Copyright (C) 2026 hazbu
```

## ⚠️ Disclaimer

This module is intended for **educational and development purposes only**. Use it responsibly and at your own risk. The developer is not responsible for any misuse or breaches of third-party service terms.
