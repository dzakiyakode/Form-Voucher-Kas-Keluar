# Voucher Entri Kas Keluar

Aplikasi web sederhana untuk mencatat voucher kas keluar dan memeriksa keseimbangan debit-kredit. Aplikasi berjalan langsung di browser dan tidak memerlukan proses build atau server backend.

Lihat tampilan dan coba aplikasinya secara langsung di [Voucher Entri Kas Keluar](https://dzakiyakode.github.io/Form-Voucher-Kas-Keluar/). Website memiliki tampilan responsif yang memudahkan pencatatan voucher dari desktop maupun ponsel.

## Menjalankan secara lokal

Buka `index.html` di browser, atau jalankan server statis lokal dari folder proyek:

```bash
python -m http.server 8000
```

Kemudian buka `http://localhost:8000`.

## Fitur

- Mengisi tanggal, nomor bukti, dan deskripsi voucher.
- Menambah atau menghapus baris jurnal (minimal dua baris).
- Memvalidasi akun, nilai debit/kredit, dan keseimbangan total secara langsung.
- Menampilkan payload JSON yang dapat disalin atau diunduh.
- Tampilan responsif untuk layar desktop maupun ponsel.

> Aplikasi ini berjalan di sisi browser. Tombol buat payload tidak menyimpan data ke database; integrasi Supabase memerlukan konfigurasi backend tersendiri. Tailwind CSS dan font dimuat dari CDN, sehingga koneksi internet diperlukan untuk tampilan optimal.

## Publikasi menggunakan GitHub Pages

1. Buat repository GitHub, lalu unggah `index.html` dan `README.md` ke root repository.
2. Buka **Settings → Pages** pada repository.
3. Pada **Build and deployment**, pilih **Deploy from a branch**.
4. Pilih branch `main` dan folder `/ (root)`, lalu tekan **Save**.
5. Buka URL GitHub Pages yang ditampilkan setelah proses deployment selesai.
