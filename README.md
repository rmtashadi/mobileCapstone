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
   
