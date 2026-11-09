# My IPTV - Android & Android TV App

Ready-to-build Android application package for [https://my-iptv-app.pages.dev/](https://my-iptv-app.pages.dev/).

## Features Configured
- **Target URL:** https://my-iptv-app.pages.dev/
- **Package Name:** `com.myiptv.player`
- **Orientation:** landscape
- **Cleartext IPTV Streams:** Allowed (HTTP / HTTPS / M3U / HLS / TS)
- **Hardware Acceleration:** Enabled (smooth 1080p/4K 60fps video decode)
- **Android TV / Leanback:** Supported with D-Pad navigation
- **Picture-in-Picture (PiP):** Supported

## How to Build the APK

### Method 1: Android Studio (Recommended)
1. Download and extract this project folder.
2. Open Android Studio and select **Open**, then choose this extracted folder.
3. Wait for Gradle sync to complete.
4. Go to **Build** > **Build Bundle(s) / APK(s)** > **Build APK(s)**.
5. Once compiled, click **locate** to get your `app-debug.apk` or `app-release.apk`.
6. Transfer to your phone or Android TV via USB, ADB, or "Send Files to TV" app.

### Method 2: GitHub Actions (Free 1-Click Cloud Build)
1. Create a new GitHub repository.
2. Push this folder to GitHub.
3. The included `.github/workflows/build-apk.yml` will automatically build the APK in the cloud.
4. Download the compiled APK directly from the **Actions** tab artifacts!

### Method 3: Command Line (Gradle)
```bash
# On Linux/macOS:
./gradlew assembleDebug

# On Windows:
gradlew.bat assembleDebug
```
The output APK will be in: `app/build/outputs/apk/debug/app-debug.apk`
