# lab09

Nama : Yoga Pratama

NIM : 312210042

Kelas : TI.22.A.1


 ## Exception Handling
 - Exception (eksepsi) merupakan suatu kesalahan (error) yang terjadi saat proses eksekusi program sedang berjalan,
 - Kesalahan ini akan menyebabkan program berakhir dengan tidak normal.
## Handling
- Penanganan file adalah bagian penting dari aplikasi apa pun.
## Assertion
Assertion(pernyataan) adalah kewajaran program yang kamu bisa aktif/nonaktifkan ketika kamu selesai menjalankan program.
### The Assert Statement
- Saat menemukan pernyataan, Python mengevaluasi ekspresi yang menyertainya, yang mana semoga benar. Jika ekspresi salah, Python memunculkan pengecualian AssertionError.
##### Sintaks untuk pernyataan yaitu :

assert Expression[, Arguments]

Jika pernyataan gagal, Python menggunakan ArgumentExpression ArgumentExpression sebagai argumen argumen untuk AssertionError AssertionError.
Pengecualian AssertionError Pengecualian AssertionError dapat ditangkap dan ditangani ditangani seperti pengecualian lainnya menggunakan try-
kecuali pernyataan, tetapi jika dibiarkan, mereka akan menghentikan program dan menghasilkan backtrace.
#### Contoh
- Berikut adalah fungsi fungsi yang mengubah suhu dari derajat Kelvin menjadi derajat Fahrenheit.Karena nol derajat Kelvin dingin, fungsi fungsi menyimpannya jika melihat negatif negatif suhu.
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:
![ss1](https://user-images.githubusercontent.com/115678171/208364460-c187cd0e-9f86-430c-83b8-867541d90c1c.png)

### Menangani Pengecualian
Jika Anda memiliki beberapa kode mencurigakan yang mungkin mengeluarkan pengecualian, Anda dapat mempertahankan program Anda letakkan kode yang mencurigakan di *try: blok. Setelah coba: blok, sertakan pernyataan sertakan **except:* statemen, diikuti oleh blok kode yang menangani masalah seanggun mungkin.
#### Contoh
- Contoh-contoh ini membuka file, menulis konten file, dan keluar dengan aman karena ada tidak masalah
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:
![ss2](https://user-images.githubusercontent.com/115678171/208364533-3bebf5b2-f2f0-4a83-9d2b-ba61125b3a8c.png)

- Contoh ini mencoba membuka file yang Anda tidak memiliki izin menulis, sehingga membuat file pengecualian
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:
![ss3](https://user-images.githubusercontent.com/115678171/208364589-8553d79c-8447-49b7-9fcd-2fc36c6d577a.png)

### Fasal kecuali tanpa Pengecualian
- Anda juga dapat menggunakan pernyataan exception tanpa exception yang didefinisikan sebagai berikut:

try:
You do your operations here;
......................
except:
If there is any exception, then execute this block.
......................
else:
If there is no exception then execute this block.

Pernyataan coba-kecuali jenis ini menangkap semua pengecualian pengecualian yang terjadi. Menggunakan percobaan seperti try-expect pernyataan tidak dianggap sebagai praktik pemrograman yang baik, karena mereka menangkap semuanya pengecualian tetapi tidak membuat programmer mengidentifikasi kemungkinan penyebab masalah terjadi
### Klausa kecuali dengan Berbagai Pengecualian
- Anda juga dapat menggunakan pernyataan exception yang sama untuk menangani beberapa exception sebagai berikut:

try:
You do your operations here;
......................
except(Exception1[, Exception2[,...ExceptionN]]]):
If there is any exception from the given exception list,
then execute this block.
......................
else:
If there is no exception then execute this block.

### Klausa coba-akhirnya
#### Contoh
- Jika Anda tidak memiliki izin untuk membuka file dalam mode tulis yang dapat ditulis, maka ini akan menghasilkan hasil berikut:
![ss4](https://user-images.githubusercontent.com/115678171/208364641-aed38dfa-958b-49fe-b157-89565c837c80.png)
- Contoh yang sama dapat ditulis lebih bersih sebagai berikut:
![ss5](https://user-images.githubusercontent.com/115678171/208364686-27038c3a-82a9-44ce-a586-cc6b82d8f205.png)

Ketika exception dilempar ke dalam blok try, eksekusi segera dilanjutkan ke akhir memblok. Setelah semua pernyataan di blok akhirnya dieksekusi, pengecualian dimunculkan lagi dan ditangani dalam pernyataan kecuali jika ada di lapisan berikutnya yang lebih tinggi dari percobaan-kecuali penyataan.
### Argumen Pengecualian
#### Contoh
- Berikut adalah contoh untuk satu pengecualian
- Ketika kode di bawah dijalankan, menghasilkan hasil sebagai berikut:
![ss6](https://user-images.githubusercontent.com/115678171/208364726-06debb11-beef-426b-96e6-e2f215fdc095.png)

### Melempar Pengecualian
#### Contoh
- Pengecualian dapat berupa string, kelas, atau objek. Sebagian besar pengecualian adalah pengecualian dari inti Python menimbulkan adalah kelas, dengan argumen=argumen yang merupakan turunan dari kelas. Mendefinisikan pengecualian barucukup mudah dan dapat dilakukan sebagai berikut:
![ss7](https://user-images.githubusercontent.com/115678171/208364773-ca5be91d-7c04-42b8-849b-56869bd9b90a.png)

### Pengecualian yang Ditetapkan Pengguna
- Python juga memungkinkan Anda membuat pengecualian sendiri dengan menurunkan kelas-kelas dari yang standar pengecualian bawaan.
- Berikut adalah contoh-contoh yang terkait dengan RuntimeError. Di sini, kelas dibuat yang merupakan subkelas dari subkelas RuntimeError. Ini berguna saat Anda perlumenampilkan tampilan informasi yang lebih spesifik saat e pengecualian tertangkap.
- Di blok coba, pengecualian yang ditentukan pengguna dimunculkan dan ditangkap di blok kecuali. Itu variabel e digunakan untuk membuat instance dari kelas Networkerror.
![ss8](https://user-images.githubusercontent.com/115678171/208364817-5b812f7c-3006-4c35-ba2d-10521b51c5af.png)

### Sekian dari saya terima kasih :)
