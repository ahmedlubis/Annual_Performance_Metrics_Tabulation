Deskripsi Data

1. Data Pendaftar (admisi.csv)
Tabel ini merekam proses bisnis admisi pendaftar di universitas. Di dalamnya terdapat atribut registrasi yang berfungsi sebagai indikator status akhir dari setiap pendaftar. Pendaftar yang dinyatakan lulus seleksi dan diterima secara resmi dapat diidentifikasi melalui penerbitan Nomor Induk Mahasiswa (NIM). NIM ini dirancang sebagai smart key.

2. Data Aktivitas Kuliah (aktivitas-perkuliahan.csv)
Tabel ini merekam proses bisnis aktivitas akademik perkuliahan mahasiswa, mulai dari aktivitas pada semester reguler hingga program remedial. Tabel ini mencakup komponen penilaian dalam bentuk indeks huruf, yang ditransformasikan lebih lanjut menjadi Indeks Prestasi Kumulatif (IPK) dengan formulasi standar sebagai berikut:
--------------------------------
IPK = (Σ(bobot × SKS)) / (Σ SKS)
--------------------------------
Format Kode Semester:[4_digit_tahun_akademik][1_digit_kode_semester]
(Contoh: 20251 -> Semester Ganjil Tahun Akademik 2025/2026)
Kode Semester --> Klasifikasi
1 --> Semester Ganjil
2 --> Semester Genap
3 --> Remidi Ganjil
4 --> Remidi Genap

Konversi Nilai Huruf ke Bobot Angka:
Nilai --> Bobot
A --> 4,00
A- --> 3,70
B+ --> 3,30
B --> 3,00
B- --> 2,70
C+ --> 2,30
C --> 2,00
D --> 1,00
E --> 0,00

3. Data Kelulusan (peserta-wisuda-tervalidasi.csv)
Tabel ini merekam proses bisnis kelulusan mahasiswa yang telah menyelesaikan seluruh beban studi akademik dan secara resmi terdaftar sebagai peserta wisuda.

4. Data Induk Program Studi (homebase.csv)
Tabel ini merupakan data acuan (master data) klasifikasi fakultas, jenjang, dan program studi.
