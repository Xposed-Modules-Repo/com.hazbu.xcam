# xCam - Virtual Camera Xposed Module

**xCam** is a high-performance Xposed module designed to replace the physical camera feed with a virtual media source (images or videos). Leveraging hardware-accelerated rendering, xCam provides a seamless and stable injection experience for modern Android applications.

## 🚀 Key Features

- **Hardware-Accelerated Rendering**: Powered by **OpenGL ES 2.0** and the **Egloo** library for smooth, low-latency video and image injection.
- **Universal API Support**: Fully compatible with legacy **Camera1** and modern **Camera2** (including CameraX) frameworks.
- **Advanced Media Controls**:
    - **90° Rotation**: Manually rotate your media in four directions to match the target app's orientation.
    - **Horizontal Mirroring**: Flip your media horizontally to simulate front-facing camera behavior.
- **Smart Aspect Ratio**: Features a **1:1 square preview** and intelligent "Center Crop" logic to ensure your media never appears distorted or stretched in the target application.
- **Unified Pipeline**: Both images (`.jpg`, `.png`) and videos (`.mp4`) are processed through the same high-performance GPU pipeline.
- **Internal Media Management**: Automatically imports media to a secure internal directory, bypassing modern Android scoped storage and URI permission restrictions.
- **Material 3 Interface**: A clean, modern management app with support for **Dynamic Colors** and intuitive icon-based controls.

## 🛠 Prerequisites

- **Rooted**: A device with **LSPosed Manager** (recommended).
- **Non-Rooted**: A device with **LSPatch** installed to patch target applications.

## 📦 Installation

### For Rooted Users (LSPosed)
1. Download and install the latest **xCam APK**.
2. Open **LSPosed Manager**, find **xCam**, and **Enable** the module.
3. Select the **target applications** (scope) and restart them.

### For Non-Rooted Users (LSPatch)
1. Install the **xCam APK** on your device.
2. Open the **LSPatch Manager** app.
3. Choose the target application you want to use.
4. Select **Embed Module** and choose **xCam**.
5. Patch, install, and run the modified application.

## 📖 Usage

1. Launch the **xCam** manager app.
2. Tap **Select Media** to choose a video or image from your gallery.
3. Use the **Icon Controls** below the 1:1 preview:
    - 🔄 **Rotate Left/Right**: Adjust the orientation in 90-degree steps.
    - ↔️ **Mirror**: Flip the image/video horizontally.
4. Transformations are saved automatically and reset when you pick a new media file.
5. Open your target app. The virtual media will now replace the live camera feed.
6. To stop injection, tap the **X** (close) icon on the preview card in the xCam app.

## ⚖️ License

This project is licensed under the **GNU General Public License v3.0**.

```text
Copyright (C) 2026 hazbu
```

## ⚠️ Disclaimer

This module is intended for **educational and development purposes only**. Use it responsibly and at your own risk. The developer is not responsible for any misuse, privacy violations, or breaches of third-party service terms.
