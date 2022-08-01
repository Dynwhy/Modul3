##### Nama: Dio Firmansyah
##### Kelas: XII RPL 1
# Project ke 3
sebelum lanjut ke modul selanjutnya, langkah sebaiknya lihat modul 1 dan 2 terlebih dahulu:
## Link Modul sebelumnya dibawah ini:
```
https://github.com/Dynwhy/test_readme/blob/main/README.md
```
langkah pertama cari _web.php_  difolder _routes_ seperti dibawah ini diVSCode:

![image](https://user-images.githubusercontent.com/109930420/182093944-6cefdd8e-3cb3-481f-a444-6fd94b26106a.png)

kemudian ubah script sebagai berikut:
```
<?php

use Illuminate\Support\Facades\Route;
use App\Http\Controllers\BarangController;
use App\Http\Controllers\KategoriController;

Route::get('/barang', [BarangController::class, 'aku']);
Route::get('/barang/kamu', [BarangController::class, 'kamu']);

Route::get('/kategori', [KategoriController::class, 'home']);
Route::get('/kategori/add', [KategoriController::class, 'add']);
```
tampilan seperti bawa ini:

![image](https://user-images.githubusercontent.com/109930420/182093708-6d6d8d9e-5a0e-481e-abea-071d41d2e700.png)

lalu buat folder KategoriController dengan dibawah ini:

*saran menggunakan fitur terminal diVSCODE
```
php artisan make:controller KategorigController
```
hasilnya:

![image](https://user-images.githubusercontent.com/109930420/182103635-128b2886-b98d-4a69-b7ae-39f855f326c0.png)


