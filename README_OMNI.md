# 📱 OMNI Terminal — Custom Android Terminal Workstation

This is your branded fork of Termux configured to run **OMNI** directly out of the box.

---

### What's Configured:
1. **Branding:** Rebranded to **OMNI Terminal** (`TERMUX_APP_NAME = "OMNI Terminal"`).
2. **OMNI Payload:** Pre-packaged `omni-suite.tar.gz` embedded in `app/src/main/assets/`.
3. **Java Version:** Locked to Java 21 LTS via `mise` (`.mise.toml`).

---

### How to Build the Standalone APK:

#### Option A: Build with Android Studio (Recommended / Easiest UI)
1. Open **Android Studio** on your desktop.
2. Select **Open** and choose `/home/jpi/projects/omni-terminal`.
3. Allow Gradle to sync.
4. Click **Build ➜ Build Bundle(s) / APK(s) ➜ Build APK(s)**.
5. Your installer will be ready at:
   `app/build/outputs/apk/debug/app-debug.apk`

#### Option B: Build via CLI with Android SDK
If you have `cmdline-tools` / Android SDK installed:
```bash
export ANDROID_HOME="/path/to/android-sdk"
cd /home/jpi/projects/omni-terminal
./gradlew assembleDebug
```

---

### Installation on Phone:
1. Once built, send the APK to your phone:
   ```bash
   adb install app/build/outputs/apk/debug/app-debug.apk
   # or
   scp -P 8022 app-debug.apk u0_a501@100.118.50.88:~/downloads/
   ```
2. Tap the **OMNI Terminal** icon to launch your custom branded workspace!
