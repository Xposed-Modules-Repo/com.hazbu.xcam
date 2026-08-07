# xCam - Virtual Camera Xposed Module

**xCam** is a high-performance Xposed module built with the modern **LibXposed API (API 101)**. It is designed to replace the physical camera feed with a virtual media source (images or videos) using hardware-accelerated rendering for a seamless and stable injection experience.

## 🚀 Key Features

- **Modern LibXposed Architecture**: Fully utilizes the latest **LibXposed API (101)**, ensuring maximum compatibility with **LSPosed**, **Vector**, **NPatch**, and **LSPatch**.
- **Hardware-Accelerated Rendering**: Powered by a custom **OpenGL ES 2.0** engine for smooth, low-latency video and image injection.
- **Universal API Support**: Compatible with legacy **Camera1** and modern **Camera2** (including CameraX) frameworks.
- **Real-time Status Tracking**: 
    - **Instan Activation**: Direct binding to the Xposed Service for immediate status detection.
    - **Active Scopes Display**: View icons of all applications where the module is currently active directly in the manager.
- **Advanced Media Controls**:
    - **90° Rotation**: Rotate media in 90-degree steps (Left/Right) to match any target app's orientation.
    - **Horizontal Mirroring**: Flip media horizontally to simulate front-facing camera behavior.
- **Smart Aspect Ratio**: Intelligent **1:1 Center Crop** logic ensures your media never appears distorted or stretched.
- **Internal Media Management**: Automatically imports media to a secure internal directory, bypassing Android scoped storage restrictions.
- **Material 3 Interface**: Clean management app with **Dynamic Colors** and intuitive icon-based controls.

## 🛠 Compatibility

- **Rooted**: **LSPosed** or **Vector** (Recommended).
- **Non-Rooted**: **NPatch** or **LSPatch**.

## 📦 Installation

### LSPosed / Vector (Root)
1. Download and install the latest **xCam APK**.
2. Open your Xposed manager (LSPosed/Vector), find **xCam**, and **Enable** the module.
3. Select the **target applications** (scope) and restart them.
4. The status in the xCam app will change to **Active** once a target is selected.

### NPatch / LSPatch (Non-Root)
1. Install the **xCam APK**.
2. Use **NPatch** or **LSPatch** to patch your target application.
3. (Optional) For instant status detection, patch the **xCam** app itself.
4. Install and run the modified application.

## 📖 Usage

1. Launch the **xCam** manager app.
2. Tap **Select Media** to choose a video (`.mp4`) or image (`.jpg`, `.png`) from your gallery.
3. Use the **Icon Controls** below the preview:
    - 🔄 **Rotate Left/Right**: Adjust orientation.
    - ↔️ **Mirror**: Toggle horizontal flip.
4. Open your target app. The virtual media will now replace the live camera feed.
5. To stop injection, tap the **X** (close) icon on the preview card.

## ⚖️ License

This project is licensed under the **GNU General Public License v3.0**.

```text
Copyright (C) 2026 hazbu
```

## ⚠️ Disclaimer

This module is intended for **educational and development purposes only**. Use it responsibly and at your own risk. The developer is not responsible for any misuse, privacy violations, or breaches of third-party service terms.
