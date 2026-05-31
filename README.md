# BangalirBazar Android App

BangalirBazar.com er official Android WebView App.

## Build korার 3টি পথ

### ✅ পথ ১: GitHub Actions (Recommended — সবচেয়ে সহজ)

1. GitHub-এ নতুন repository বানান
2. এই project এর সব ফাইল push করুন:
   ```
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/bangalirbazar-android.git
   git push -u origin main
   ```
3. GitHub → Actions tab → "Build BangalirBazar APK" → Run workflow
4. Build complete হলে **Artifacts** থেকে APK download করুন ✅

---

### পথ ২: Android Studio দিয়ে

1. Android Studio open করুন
2. File → Open → এই folder select করুন
3. Gradle sync হতে দিন
4. Build → Generate Signed Bundle/APK → APK → Debug
5. `app/build/outputs/apk/debug/` ফোল্ডারে APK পাবেন

---

### পথ ৩: Command Line দিয়ে

```bash
# Android SDK ইনস্টল থাকলে:
./gradlew assembleDebug

# APK পাবেন:
# app/build/outputs/apk/debug/app-debug.apk
```

---

## App তথ্য

- Package: `com.bangalirbazar.app`
- Min Android: 5.0 (API 21)
- Target Android: 14 (API 34)
- URL: https://bangalirbazar.com

## Features

- ✅ WebView (bangalirbazar.com লোড করে)
- ✅ Back button navigation
- ✅ Offline error page (বাংলায়)
- ✅ Loading progress bar
- ✅ External links → browser এ খোলে
