# Panduan Penggunaan PRESMA

Sebelum membaca panduan, pastikan Anda memahami terlebih dahulu [arsitektur dari sistem e-voting PRESMA](architecture.md) khususnya pada alur pemilihan / voting

## Operasional

1. Panitia masuk menggunakan akun yang telah diberikan oleh developer
2. Ubah pengaturan terlebih dahulu disesuaikan dengan acara masing-masing, terutama pengaturan pemilihan kandidat (capres, caleg, atau partai)
3. Input data dalam sistem e-voting:
    - Daerah pilihan (berupa jurusan / program studi / departemen apabila di tingkat fakultas, atau fakultas apabila di tingkat universitas)
    - Mahasiswa daftar pemilih tetap
    - Jadwal pemilihan
    - Kandidat calon presiden (jika dilakukan pemilihan capres seperti pemilihan raya pada umumnya)
    - Kandidat calon legislatif (jika dilakukan pemilihan caleg)
    - Kandidat partai (jika dilakukan pemilihan partai)
4. Proses input data mahasiswa DPT dapat dilakukan dengan cara **import melalui file Excel/Spreadsheet**. File tersebut bisa didapat dengan dua cara:
    1. Menghubungi admin jurusan / fakultas / perguruan tinggi setempat untuk memohon data mahasiswa aktif dalam bentuk file Excel **(lebih aman, terhindar dari DPT fiktif, akan tetapi berpotensi terhalang birokrasi dalam mendapatkan data)**
    2. Menyebarkan formulir (umumnya Google Forms) untuk pencatatan DPT **(lebih tidak aman, rentan DPT fiktif, akan tetapi tidak terhalang birokrasi, tidak disarankan untuk metode pemilihan online melalui email institusi)**
5. File Excel wajib memiliki informasi berikut: **NIM**, **nama mahasiswa**, **angkatan** (opsional), dan **daerah pilihan**, dengan format disesuaikan supaya terbaca oleh aplikasi
6. Apabila tidak memiliki waktu untuk mendapatkan file Excel/Spreadsheet tersebut, input data mahasiswa dapat dilakukan pada saat sesi pemilihan dengan langkah-langkah sebagai berikut:
    1. Pemilihan **disarankan** untuk dilaksanakan secara *offline* (menggunakan PIN atau kode QR)
    2. Sediakan satu *booth* yang berisi panitia yang berjaga untuk input data mahasiswa DPT
    3. Mahasiswa yang akan memilih datang terlebih dahulu ke *booth* tersebut untuk mendaftarkan dirinya menggunakan **kartu identitas mahasiswa** (KTM, KRS, bukti pendaftaran / herregistrasi, dan lain sebagainya)
    4. Panitia memverifikasi kartu identitas tersebut kemudian menginputkan data mahasiswa melalui admin panel
    5. Mahasiswa dipersilakan untuk melaju ke tahap berikutnya (mendapatkan PIN dari panitia atau scan kode QR) pada *booth* pemilihan
7. Setelah selesai input semua data, maka langkah berikutnya adalah **membuka kunci sistem e-voting** melalui pengaturan supaya mahasiswa dapat melakukan voting (dilakukan menjelang hari-H acara, atau pada saat uji coba lalu dikunci kembali)
8. Apabila menjalankan uji coba, maka seluruh data surat suara **harus** dihapus (direset) melalui pengaturan supaya tidak mengganggu keberjalanan dan mempengaruhi hasil pemilihan umum
9. Setelah sesi pemilihan berakhir, maka **kunci kembali** sistem e-voting supaya tidak ada suara lagi yang masuk
10. Selain itu, panitia dapat mengumumkan hasil pemilihan secara interaktif melalui control panel
    - Pastikan juga pengaturan untuk mempublikasikan hasil pemilihan diaktifkan supaya publik dapat ikut serta memverifikasi hasilnya
11. Apabila terjadi sengketa sehingga menyebabkan hasil pemilihan tidak dapat dipercaya, maka pemilihan dapat dilaksanakan ulang dengan memerhatikan ketentuan perubahan kunci rahasia yang terdapat pada [Arsitektur Keamanan](architecture.md#keamanan)
