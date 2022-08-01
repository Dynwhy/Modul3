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

![image](https://user-images.githubusercontent.com/109930420/182103635-128b2886-b98d-4a69-b7ae-39f855f326c0.png)

Hasilnya ada difordel _App/Http/Controllers_: 

![image](https://user-images.githubusercontent.com/109930420/182105214-a4dea60c-d88a-4516-82c9-5e56fbd462d4.png)


lalu ubah script seperti ini:
```
<?php

namespace App\Http\Controllers;

use Illuminate\Http\Request;

class KategoriController extends Controller
{
        Public function home(){
        return 'Mengakses Fungsi di controller menggunakan
        route add';
        }
        Public function add()
        {
        return 'Ini Adalah Halaman add';
        }
    
        
}

```
contoh gambar:

![image](https://user-images.githubusercontent.com/109930420/182105656-2a7c96c8-e089-4509-b194-53775ec202d5.png)

lalu untuk cek project yang kita buat buka fitur terminal VSCODE:
```
php artisan serve
```

![image](https://user-images.githubusercontent.com/109930420/182106336-9d41f9f7-83cd-4933-9ee8-42eef3da7674.png)

hasilnya

![image](https://user-images.githubusercontent.com/109930420/182106479-0d201164-01a9-40b6-840f-bbd0c63892a3.png)


lalu salin dan search dicrome/google 
```
http://127.0.0.1:8000
```
tampilan seperti ini:

![image](https://user-images.githubusercontent.com/109930420/182106857-70c3b663-3b9b-418d-aa93-cccf1b033745.png)

jika ingin memanggil _Route_ yang kita buat hasil dari search tambahkan dengan nama _Route_ sebagai berikut:

![image](https://user-images.githubusercontent.com/109930420/182107400-e657ff0b-e7d8-4987-8d10-d06ea0243f11.png)

Hailnya:

![image](https://user-images.githubusercontent.com/109930420/182107577-10f4016f-2469-49f5-be1c-d232f0a28b4d.png)


selesailah project _Modul 3_ tersebut.
# SEKIAN TERIMA KASIH>.<
