# XAU Console — Proyek Android WebView APK

Proyek Android Kotlin + Gradle ini dihasilkan otomatis oleh WebView APK Studio dari file HTML Anda.

## Identitas Aplikasi
- Nama Aplikasi: XAU Console
- Package Name: `com.xauconsole.webview`
- Versi: 1.0.0 (code 1)
- Target SDK: Android 35 (Min SDK 24)
- Mode Aset Lokal: WebViewAssetLoader (https://appassets.androidplatform.net/assets/index.html)

## Cara Menjadikan File .APK

### Opsi 1 — Build Otomatis di Cloud (Tanpa Install Android Studio)
1. Buat repository baru di GitHub (bisa Private/Public).
2. Ekstrak seluruh isi file ZIP ini dan upload ke repository tersebut.
3. Buka tab **Actions** di GitHub, pilih **Build Android WebView APK**, lalu klik **Run workflow** (atau otomatis berjalan saat push).
4. Setelah selesai (~2 menit), unduh file `app-debug.apk` pada bagian **Artifacts**.

### Opsi 2 — Build Menggunakan Android Studio
1. Buka **Android Studio** -> **Open** -> pilih folder hasil ekstrak ZIP ini.
2. Tunggu proses Gradle Sync selesai.
3. Klik menu **Build** -> **Build Bundle(s) / APK(s)** -> **Build APK(s)** (atau **Generate Signed Bundle / APK** untuk versi rilis Play Store).
4. File APK tersedia di `app/build/outputs/apk/debug/app-debug.apk`.

### Opsi 3 — Build Via Terminal (Membutuhkan JDK 17 + Android SDK + Gradle 8.10+)
```bash
gradle assembleDebug
```
