# WBSEDCL Roster Professional App v6

Professional Android app wrapper for the WBSEDCL Roster Generator.

## ☁️ Cloud APK build with GitHub Actions

This project includes `.github/workflows/android-apk.yml`.

1. Create a GitHub repository.
2. Upload/push this project folder to the repository.
3. Open **Actions** → **Build Android APK**.
4. On every push to `main`/`master`, GitHub Actions builds the APK automatically.
5. You can also use **Run workflow** to build manually.
6. Open the completed workflow run → **Artifacts** → download `WBSEDCL-Roster-Pro-v6-APK`.

The generated file is a debug APK intended for installation/testing. A Play Store-ready release APK should be signed with a private Android keystore.

## Local build

Open in Android Studio and build `assembleDebug`, or use Gradle 8.10.2 with JDK 21:

```bash
gradle assembleDebug
```

The roster engine remains offline-first and keeps its existing localStorage data.
