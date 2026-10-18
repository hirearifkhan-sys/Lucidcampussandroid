# Lucid Campus Android project

**App:** Lucid Campus  
**Package:** `com.lucidcampus.app`  
**Version:** `1.0.0`  
**Mode:** Offline-first WebView wrapper

## Included
- Android Studio project source
- Existing Lucid Campus HTML dashboard and graphics bundled in app assets
- LocalStorage-backed study progress and persistent student display name
- GitHub Actions workflow that builds a debug APK and publishes it as an artifact

## Build the APK
Open this folder in Android Studio with Android SDK Platform 35 installed, sync Gradle, then run **Build > Build Bundle(s) / APK(s) > Build APK(s)**. Or push this project to a GitHub repository and run **Actions > Build Lucid Campus APK > Run workflow**. Download the `Lucid-Campus-APK` artifact after a successful run.

## Important limitations
- This environment has Java but no Android SDK, Gradle installation/wrapper, or `adb`, so a compiled APK could not be produced here. The source project and CI workflow are included to build it in Android Studio or GitHub Actions.
- The requested “login” currently means a local student profile/name stored on this device. It is not secure account authentication and will not sync across devices. Real login requires an authentication backend and privacy/security design.
- The app is offline-first for the bundled dashboard and locally saved data. Official exam links and current notifications require internet.
- Sample practice questions are not a verified 50,000+ PYQ bank.
