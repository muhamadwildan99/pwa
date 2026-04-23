1. Point (Titik Utama)
Sistem operasi mobile modern dirancang untuk mengelola sumber daya secara ketat melalui manajemen memori yang hierarkis, komunikasi antar-komponen yang terstruktur, dan sistem keamanan data yang terenkripsi. Fokus utamanya adalah menjaga performa perangkat tetap optimal meskipun memiliki keterbatasan baterai dan memori.
2. Reason (Alasan)
Manajemen ini diperlukan karena perangkat mobile beroperasi dalam lingkungan yang dinamis. OS harus bisa menentukan prioritas aplikasi mana yang harus tetap berjalan dan mana yang harus dihentikan (low memory killer), serta bagaimana data dibagikan secara aman antar aplikasi tanpa mengekspos seluruh sistem.
3. Evidence (Bukti/Detail dari Gambar)
Berdasarkan catatan di papan tulis, berikut adalah rincian teknisnya:
• Manajemen Memori (Memory Management):
Sistem membagi status aplikasi menjadi tiga kategori utama:
• Foreground: Aplikasi yang sedang berinteraksi langsung dengan pengguna.
• Background: Aplikasi yang berjalan di balik layar (misalnya proses sinkronisasi).
• Cache: Data aplikasi yang disimpan sementara untuk mempercepat akses kembali.
• Catatan khusus: Terdapat mekanisme Low Memory yang akan mematikan proses tertentu jika RAM penuh.
• Komunikasi & Komponen (IPC & Content Provider):
• Intent (IPC): Digunakan untuk komunikasi antar-proses (Inter-Process Communication).
• Content Provider: Mekanisme untuk mengelola dan berbagi basis data antar aplikasi secara standar.
• WorkManager: Digunakan untuk menjadwalkan tugas di latar belakang (deferrable tasks) yang harus tetap berjalan meskipun aplikasi ditutup.
• Keamanan Data (Data Security):
• FBE (File-Based Encryption): Papan tulis mencatat penggunaan File-Based Encryption, di mana file yang berbeda dienkripsi dengan kunci yang berbeda pula, memungkinkan fitur seperti Direct Boot.
• EDA: Merujuk pada arsitektur data atau enkripsi tingkat lanjut lainnya untuk perlindungan privasi pengguna.
• Alur Kerja & Notifikasi:
Terdapat diagram di bagian bawah yang mengilustrasikan alur Request dan Broadcast. Ini menunjukkan bagaimana sistem mengirimkan sinyal (seperti status baterai 10%) ke berbagai aplikasi atau modul terkait melalui broadcast receiver.
4. Point (Kesimpulan)
Secara keseluruhan, catatan tersebut merangkum fondasi penting dalam pengembangan aplikasi mobile. Dengan memahami klasifikasi memori (Foreground/Background), cara kerja WorkManager, serta implementasi keamanan seperti FBE, seorang pengembang dapat membangun aplikasi yang efisien, tidak boros baterai, dan aman bagi data pengguna.
