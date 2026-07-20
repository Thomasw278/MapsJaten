# Peta Digital Rumah Warga Jaten

Sebuah aplikasi peta digital berbasis web (*Web GIS*) interaktif yang dirancang khusus untuk memetakan sebaran lokasi tempat tinggal warga di Dusun Jaten. Proyek ini dikembangkan sebagai bagian dari program kerja **KKN ISL UKDW 2026 — Kelompok Jaten**.

Aplikasi ini menggunakan integrasi Google Sheets sebagai sumber *database* (melalui konversi publikasi CSV), sehingga memudahkan pengurus dusun atau anggota tim KKN untuk memperbarui data secara langsung tanpa perlu menyentuh kode program.

---

## Fitur Utama

*   **Peta Interaktif Leaflet.js**: Navigasi responsif dengan dukungan kontrol perbesaran (*zoom*) dan pergeseran.
*   **Ganti Lapisan Peta (Layer Toggle)**: Pilihan tampilan peta standar (OSM), Satelit Google, atau Peta Hybrid.
*   **Sidebar Daftar Warga**: Menampilkan seluruh daftar warga lengkap dengan bilah pencarian (*live search*) berdasarkan nama atau alamat.
*   **Penanda Kustom (Custom Markers)**: Desain penanda peta dinamis, termasuk penanda khusus berlambang `🐦` untuk warga yang memiliki mata pencaharian sebagai pengrajin sangkar burung.
*   **Pop-up Detail Informatif**: Menampilkan informasi lengkap warga (nama, alamat, pekerjaan) saat penanda diklik, lengkap dengan tombol pintasan menuju Google Maps.
*   **Desain Responsif**: Antarmuka modern yang optimal baik saat diakses via komputer (*desktop*) maupun *smartphone* (*mobile*).

---

## Struktur File Proyek

Proyek ini menggunakan pemisahan kode yang bersih demi kemudahan pemeliharaan (*clean code*):

```text
├── index.html        # Struktur utama web dan logika JavaScript (Leaflet & Fetch API)
├── style.css         # Seluruh aturan desain, layout, tata letak, dan media queries
└── peta.jpg      # Aset gambar penunjuk arah mata angin (kompas)