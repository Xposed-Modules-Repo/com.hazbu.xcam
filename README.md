# xCam - Virtual Camera Xposed Module

**xCam** is a modern Xposed module designed to replace the physical camera feed with a virtual media source (images or videos). It is specifically optimized for Android 9+ and applications using the Camera2 API (including CameraX).

## 🚀 Features

- **Universal Support**: Works with both legacy **Camera1** and modern **Camera2** APIs.
- **Image & Video Support**: Use `.mp4` videos or `.jpg`/`.png` images as your camera source.
- **Horizontal Mirroring**: Toggle mirroring to match the front-facing camera's expected behavior.
- **Auto-Rotation Correction**: Automatically forces a portrait orientation to prevent your media from appearing sideways.
- **Robust Injection**: 
    - **Videos**: Streamed via `MediaPlayer` using manual `AssetFileDescriptor` management.
    - **Images**: Rendered via a dedicated background thread for high stability.
- **Internal Storage Import**: Automatically copies media to internal storage to bypass Android URI permission restrictions.
- **Modern Material 3 UI**: Full support for Dynamic Colors and a clean, visual management interface.
- **Live Preview**: See a thumbnail of your active media and the effect of mirroring directly in the manager app.

## 🛠 Prerequisites

- A rooted Android device.
- **Xposed Framework** installed (LSPosed recommended).

## 📦 Installation

1. Download and install the **xCam APK**.
2. Open your Xposed manager (e.g., LSPosed) and **enable** the xCam module.
3. Select the **target applications** you want to hook.
4. Reboot or Force Stop the target application.

## 📖 Usage

1. Open the **xCam** app.
2. Click **Select Media** and choose your media file.
3. Use the **Mirror** toggle if your media appears flipped in the target app.
4. Open your target application. The camera preview will now display your selected media.
5. To stop using the virtual camera, click the **X** icon in the media preview box.

## ⚖️ License

This project is licensed under the **GNU General Public License v3.0**.

```text
Copyright (C) 2026 hazbu

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.
```

See the [LICENSE](LICENSE) file for the full text.

## ⚠️ Disclaimer

This module is for educational and development purposes only. Use it responsibly and at your own risk. The developer is not responsible for any misuse or violations of terms of service of third-party applications.
