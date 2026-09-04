# GTS AI — Build APK langsung dari HP

Project ini sudah dilengkapi GitHub Actions untuk membangun `app-debug.apk` di cloud, sehingga tidak perlu Android Studio di laptop.

## Langkah singkat dari HP

1. Buat/login akun GitHub.
2. Buat repository baru, misalnya `gts-ai-android`.
3. Upload **isi folder project ini** ke repository (bukan file ZIP di dalam repository).
4. Pastikan folder `.github/workflows/build-apk.yml` ikut ter-upload.
5. Buka tab **Actions** di repository.
6. Pilih workflow **Build GTS AI APK**.
7. Tekan **Run workflow**.
8. Tunggu sampai status selesai.
9. Buka hasil run → bagian **Artifacts** → download `gts-ai-debug-apk`.
10. Ekstrak ZIP artifact, lalu install `app-debug.apk` di HP Android untuk pengujian.

## Catatan
- Ini adalah build debug untuk testing.
- APK memakai project GTS AI Android v4 dan backend Supabase yang sama.
- Build dilakukan GitHub Actions; HP hanya untuk mengelola repository dan mengunduh hasil.
- Untuk rilis Play Store/release, diperlukan signing key dan konfigurasi release terpisah.
- Aplikasi ini tetap digunakan sebagai sandbox/demo, bukan sistem investasi uang nyata atau jaminan keuntungan.
