GGMPXDONGHUB - Prototype mapping Android

FITUR YANG SUDAH ADA
- Tombol mapping dapat digeser dalam area uji.
- Ketuk tombol saat EDIT untuk mengganti fungsi.
- UKURAN - / UKURAN + mengubah ukuran tombol terakhir.
- SIMPAN / MUAT menyimpan layout dengan SharedPreferences.
- Input keyboard eksternal dapat terdeteksi saat aplikasi sedang fokus.
- Mode MAIN menguji tombol hanya di dalam aplikasi.

BATASAN PENTING
Ini belum mengontrol Free Fire. Overlay permission hanya mengizinkan tampilan di atas aplikasi lain, bukan menyuntikkan touch ke game. Android AccessibilityService dapat melakukan gesture dalam batas API dan kebijakan yang berlaku, tetapi kompatibilitas game tidak dijamin. Jangan gunakan untuk melewati anti-cheat atau ketentuan game.

MEMBUKA PROYEK
1. Buka folder proyek di IDE Android yang mendukung Gradle.
2. Gunakan JDK 17 dan Android Gradle Plugin 8.6.1.
3. Sinkronkan Gradle lalu Build APK.
4. Jika IDE HP tidak mendukung versi Gradle ini, gunakan versi AIDE/Android IDE yang mendukung project Gradle modern atau buat project Java baru dan salin MainActivity.java serta resource manifest/theme.

BUILD APK OTOMATIS VIA GITHUB ACTIONS
1. Buat repository baru di GitHub dari browser HP.
2. Ekstrak ZIP ini, lalu upload semua isi folder (termasuk folder .github) ke repository dan commit ke branch main.
3. Buka tab Actions pada repository. Jalankan workflow "Build GGMPXDONGHUB APK" jika belum otomatis berjalan.
4. Buka hasil run yang berhasil, scroll ke bagian Artifacts, unduh GGMPXDONGHUB-debug-apk.
5. Ekstrak artifact ZIP yang diunduh untuk mendapatkan APK debug.

Catatan: workflow menggunakan Gradle yang tersedia di runner. Jika build gagal karena konfigurasi Gradle/Android plugin, lihat log Actions untuk pesan error dan sesuaikan versi toolchain.
