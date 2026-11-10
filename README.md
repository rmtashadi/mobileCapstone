# Campus Mart

Aplikasi Marketplace sederhana untuk mahasiswa yang ingin menjual dan membeli barang kebutuhan kuliah. Menggunakan (Flutter + Provider), simulasi dua akun pada satu perangkat.
Tanpa Firebase, backend, atau internet. Data disimpan lokal dengan `shared_preferences`.

## Cara menjalankan

```bash
Ekstrak proyek, lalu jalankan perintah
flutter pub get
kemudian jalan aplikasi 
flutter run
```

(Alternatif pubspec: `flutter pub add provider shared_preferences`.)

## Akun demo

| Username | Password |
|---|---|
| demo1 | butuhkopi |
| demo2 | naspadseporsi |

## Skenario uji

1. Login `penjual` -> menu Jual -> Tambah Barang (Headphone, Rp150000) -> Simpan.
2. Profil -> Logout. Login `pembeli`. Home -> buka Headphone -> Chat Penjual -> kirim pesan.
3. Logout. Login `penjual` -> menu Chat -> buka percakapan -> balas.
4. Logout. Login `pembeli` -> baca balasan -> Ajukan Pembelian -> Ajukan (status Menunggu).
5. Logout. Login `penjual` -> Chat -> Terima atau Tolak.
6. Logout. Login `pembeli` -> status terbaru tampil di Chat dan Detail Barang.



## Batasan
1. Data hanya tersimpan di satu perangkat dan tidak tersinkron antar perangkat.
2. Tidak ada pembayaran
3. Login hanya simulasi, yg tersimpan sebagai teks biasa di kode. Sehingga tidak ada registrasi


## 📱 Tampilan Aplikasi


### 1. Beranda & Login

<p align="center">
  <img src="https://github.com/user-attachments/assets/ee8acef4-cfc2-4eae-bac4-f92d1c2608f6" width="280" alt="Halaman Login">
</p>


<p align="center">
  <img src="https://github.com/user-attachments/assets/01e7b8f7-3fc9-44c8-a25d-5fa752e05554" width="280" alt="Tampilan Beranda">
</p>




### 2. Fitur Pendukung (Profil & Chat)

<p align="center">
  <img src="https://github.com/user-attachments/assets/d12e5e7f-0f17-4790-9ff9-01c268b87171" width="280" alt="Tampilan Profil">
</p>


<p align="center">
  <img src="https://github.com/user-attachments/assets/4cb238da-863b-4c5b-9d3d-fdfab03a6b0f" width="280" alt="Tampilan Chat">
</p>

### 3. Katalog & Favorit

<p align="center">
  <img src="https://github.com/user-attachments/assets/f58b1c2d-6ab0-4f13-a629-6b6428e51238" width="280" alt="Tampilan Barang yang Dijual">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/11649cdf-fc99-479c-bc87-33b04e8d72d1" width="280" alt="Tampilan Halaman Favorit">
</p>

