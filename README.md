<div align="center">

  <!-- PROJECT LOGO / BANNER PLACEHOLDER -->
  <img src="assets/banner.png" alt="LiquidGlass LSPosed Banner" width="100%" />

  # LiquidGlass for WhatsApp & Instagram (LSPosed Module)

  **Transform your WhatsApp & Instagram UI on Samsung devices into a sleek, modern LiquidGlass aesthetic dynamically—without modifying the original APKs.**

  [![Android](https://img.shields.io/badge/Android-16%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://www.android.com/)
  [![Device](https://img.shields.io/badge/Samsung-Rooted-1428A0?style=for-the-badge&logo=samsung&logoColor=white)](https://www.samsung.com/)
  [![LSPosed API](https://img.shields.io/badge/LSPosed%20API-101%20--%20103-blue?style=for-the-badge)](https://github.com/LSPosed/LSPosed)
  [![WhatsApp](https://img.shields.io/badge/WhatsApp-Beta%20Support-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://www.whatsapp.com/)
  [![Instagram](https://img.shields.io/badge/Instagram-Coming%20Soon-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/)
  [![License](https://img.shields.io/badge/License-GPLv3-orange?style=for-the-badge)](LICENSE)

  <p align="center">
    <a href="README.md">🇺🇸 English</a> •
    <a href="README_ID.md">🇮🇩 Bahasa Indonesia</a> •
    <a href="README_ES.md">🇪🇸 Español</a>
  </p>

</div>

---

## 📖 Overview

**LiquidGlass** is an advanced Xposed/LSPosed module designed specifically for rooted Samsung devices running modern Android versions. By hooking directly into the application's UI rendering pipeline at runtime, this module applies real-time **translucent blur, glassmorphism, and fluid refraction effects** (LiquidGlass) to **WhatsApp** (currently in Beta) and **Instagram** (coming soon).

Because it operates purely via Xposed hooking, **no APK patching, repackaging, or signature spoofing is required**. Your apps remain 100% original, safe, and eligible for official updates via the Google Play Store.

---

## 🎬 Preview

> *Replace the placeholder paths below with your actual `.gif` or `.mp4` files inside your repository's `assets/` folder.*

<div align="center">
  <table>
    <tr>
      <td align="center"><b>WhatsApp (Beta)</b></td>
      <td align="center"><b>Instagram (Coming Soon)</b></td>
    </tr>
    <tr>
      <td><img src="assets/preview_whatsapp.gif" alt="WhatsApp LiquidGlass Preview" width="320"/></td>
      <td><img src="assets/preview_instagram.gif" alt="Instagram LiquidGlass Preview" width="320"/></td>
    </tr>
  </table>
</div>

---

## ✨ Key Features & Roadmap

- **Zero APK Modification:** Hooks directly into UI views at runtime; preserves original app signatures and avoids third-party modded APK bans.
- **Dynamic Real-Time Blur:** Hardware-accelerated translucent backgrounds with customizable blur radius, tint opacity, and corner radius.
- **WhatsApp Integration (🧪 Beta):** Applies translucent chat backgrounds, frosted navigation/top bars, and glass modals on the latest Global WhatsApp builds.
- **Instagram Integration (⏳ Coming Soon):** Support for Instagram feeds, DMs, and translucent navigation bars is currently in active development.
- **Lightweight & Battery Friendly:** Uses native Android `RenderEffect` and Samsung's proprietary blur APIs to ensure smooth scrolling and minimal battery overhead.

---

## 📱 Supported Devices & Requirements

To ensure optimal performance and stability, please verify that your device meets the following requirements:

| Component | Requirement / Compatibility |
| :--- | :--- |
| **Device Brand** | Rooted Samsung Galaxy Devices (S-Series, Z-Series, Note, A-Series) |
| **OS Version** | **Android 16+** (OneUI 8.0 / 8.1 or newer) |
| **Root Solution** | Magisk (v27+), KernelSU, or APatch |
| **Framework** | **LSPosed** (Zygisk / NeoZygisk) supporting **API 101 – 103** |
| **Target Apps** | **WhatsApp (Latest Global - Beta)** & **Instagram (Coming Soon)** |

> **⚠️ Note:** Non-Samsung devices or AOSP-based Custom ROMs are **not officially supported**, as this module utilizes Samsung's native blur rendering APIs.

---

## 🚀 Installation & Usage

1. **Prerequisites:** Ensure your Samsung device is rooted and has the latest **LSPosed (API 101–103)** installed and active.
2. **Download:** Grab the latest `LiquidGlass-vX.X.apk` from the [Releases](../../releases) page.
3. **Install:** Install the downloaded APK onto your device like a normal app.
4. **Activate Module:**
   - Open the **LSPosed Manager**.
   - Navigate to the **Modules** tab and enable **LiquidGlass**.
   - In the module scope list, check **WhatsApp** *(and **Instagram** once supported)*.
5. **Apply Changes:**
   - **Force Stop** WhatsApp from your device settings, then reopen it to see the LiquidGlass effect.
6. **Customize (Optional):** Open the **LiquidGlass** companion app from your launcher to tweak blur intensity, glass tint, and border highlights.

---

## 🛠️ Troubleshooting

<details>
<summary><b>1. The LiquidGlass effect is not showing up in WhatsApp.</b></summary>
<br>
- Verify that **WhatsApp** is checked inside the **LSPosed Module Scope**.
- Make sure you **Force Stopped** WhatsApp after enabling the module.
- Check if your LSPosed framework is running **API 101 to 103**. Outdated LSPosed forks may fail to hook Android 16+ views.
</details>

<details>
<summary><b>2. WhatsApp crashes or glitches after a Play Store update (Beta Notice).</b></summary>
<br>
- Because WhatsApp support is currently in **Beta** and WhatsApp frequently obfuscates its internal view classes on new updates, a new Global update may occasionally break hooks. If a crash occurs, temporarily uncheck WhatsApp in LSPosed Scope and check the [Releases](../../releases) or [Issues](../../issues) tab for an updated hook mapping.
</details>

<details>
<summary><b>3. UI lags or frame drops when scrolling through chats.</b></summary>
<br>
- Open the **LiquidGlass Companion App** and reduce the **Blur Radius** or disable **Real-time Refraction** on older/mid-range Galaxy A-series GPUs.
- Ensure *Disable HW Overlays* is **not** enabled in Android Developer Options.
</details>

<details>
<summary><b>4. Module states "LSPosed API Mismatch" or fails to initialize.</b></summary>
<br>
- This module strictly targets **LSPosed API 101–103** for Android 16+. Please update your Zygisk and LSPosed builds to the latest compatible versions.
</details>

---

## 🤝 Contributing & Bug Reports

Contributions, feature requests, and bug reports are welcome!
- Found a bug in the WhatsApp Beta? Open an [Issue](../../issues) and attach your **LSPosed Logs** along with your exact **Device Model, OneUI Version, and WhatsApp Version**.

---

## 📜 Disclaimer & License

- **Disclaimer:** This module is provided *"as is"*. Rooting your Samsung device voids Samsung Knox warranty. The developer is not responsible for bootloops, system instability, or third-party app issues.
- **License:** Distributed under the **GNU General Public License v3.0 (GPLv3)**. See `LICENSE` for more information.