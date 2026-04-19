# Aplikasi Sistem Pakar: Diagnosa Medis THT

Program ini merupakan implementasi sistem pakar (Expert System) berbasis desktop yang dirancang untuk mengidentifikasi gangguan pada Telinga, Hidung, dan Tenggorokan (THT). Aplikasi dikembangkan menggunakan Python dan library Tkinter.

## Arsitektur Sistem

Aplikasi ini mengadopsi tiga komponen utama sistem pakar:
1. **Basis Pengetahuan (Knowledge Base):** Menyimpan data relasi antara 23 jenis penyakit dan 37 indikator gejala klinis yang bersumber dari modul praktikum.
2. **Mesin Inferensi (Inference Engine):** Menggunakan metode Forward Chaining (Penalaran Maju). Sistem akan mengevaluasi jawaban user menggunakan logika konjungsi (AND) untuk mencapai kesimpulan diagnosa yang valid.
3. **Antarmuka (User Interface):** GUI interaktif yang memudahkan pengguna dalam melakukan sesi konsultasi secara mandiri.

## Panduan Instalasi & Penggunaan
* Python versi 3.x terinstal di sistem Anda.
* Library `tkinter` (umumnya sudah tersedia dalam instalasi standar Python).

## Langkah Menjalankan
1. Clone atau unduh repositori ini ke penyimpanan lokal Anda.
2. Buka terminal/command prompt pada folder proyek.
3. Eksekusi program dengan perintah:
   python tugasTHT.py
4. Tekan tombol "MULAI DIAGNOSA" pada jendela utama.
5. Berikan respon "YA" atau "TIDAK" terhadap setiap pertanyaan yang ditanyakan.
6. Hasil analisis medis akan muncul secara otomatis melalui pop-up message box di akhir sesi.

## Komponen Kode
* 'database_tht': Objek dictionary yang menyimpan jenis penyakit dengan kombinasi kode gejala (G1-G37).
* 'daftar_gejala': Sekumpulan data berisi daftar pertanyaan yang telah disesuaikan agar mudah dipahami.
* 'AplikasiPakarTHT': Kelas utama yang menghandle seluruh logika program, mulai dari manajemen state antarmuka hingga proses eksekusi mesin inferensi.
