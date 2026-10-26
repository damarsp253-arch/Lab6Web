# Praktikum 6 JavaScript DOM dan Event Handling

## Nama: Damar Satryo Pambudi<br>
## NIM: 312510189<br>
## Kelas: I251B<br>
## Mata Kuliah: Pemrograman Web<br>
## Pertemuan: 7<br>

## Tujuan Praktikum

Praktikum ini bertujuan untuk memahami penggunaan Document Object Model (DOM) dalam JavaScript, memilih dan memanipulasi elemen HTML, menangani event pengguna, mengubah tampilan halaman menggunakan CSS, serta melakukan validasi form. Praktikum juga bertujuan mengembangkan halaman web interaktif melalui latihan dan mini project.

## Langkah Kerja Praktikum

Membuat folder Lab6Web yang berisi file HTML, CSS, dan JavaScript. File HTML digunakan untuk membangun halaman, CSS untuk mengatur tampilan, sedangkan JavaScript digunakan untuk menambahkan interaksi.

### Mengubah Teks dengan DOM

Memilih elemen HTML berdasarkan id menggunakan document.`getElementById()`. Selanjutnya, properti textContent digunakan untuk mengubah teks judul dan paragraf secara langsung.

Hasil yang diharapkan: Judul dan paragraf berubah sesuai teks yang ditentukan pada JavaScript.

Code:

<img width="627" height="332" alt="Cuplikan layar 2026-10-26 202326" src="https://github.com/user-attachments/assets/20f02e9d-1e1b-4853-b719-487dac096d99" />

<img width="562" height="105" alt="Cuplikan layar 2026-10-26 202351" src="https://github.com/user-attachments/assets/8b6e5434-2f1d-4fc9-a551-48e2ca99e640" />

Output:

![alt text](gambar/gambar1.png)

### Event Click

Menggunakan `addEventListener()` untuk mendeteksi ketika tombol diklik. Program kemudian memperbarui pesan dan menampilkan waktu saat tombol ditekan.

Hasil yang diharapkan: Pesan pada halaman berubah setiap kali tombol diklik.

Code:

![alt text](gambar/code3.png)

Output:

![alt text](gambar/gambar2.png)

### Mengubah Class dan Gaya CSS

Menggunakan `classList.toggle()` untuk menambah atau menghapus class CSS pada elemen. Perubahan class digunakan untuk mengubah warna latar belakang, garis tepi, dan ukuran teks.

Hasil yang diharapkan: Tampilan paragraf berubah ketika tombol ditekan.

Code:

![alt text](gambar/code4.png)

![alt text](gambar/code5.png)

### Event input dan penghitung karakter

Menggunakan event input untuk mendeteksi perubahan pada kolom teks. Properti `value.length` digunakan untuk menghitung jumlah karakter yang dimasukkan pengguna.

Hasil yang diharapkan: Jumlah karakter bertambah atau berkurang secara langsung ketika pengguna mengetik atau menghapus teks.

Code:

![alt text](gambar/code6.png)

![alt text](gambar/code7.png)

Output:

![alt text](gambar/gambar3.png)

### Validasi Form Pendaftaran

Membuat form yang terdiri dari nama lengkap, email, dan usia. JavaScript memeriksa setiap input dan menampilkan pesan berdasarkan hasil validasi.

Pengujian dilakukan terhadap lima kondisi:

1. Semua input kosong.
2. Nama kosong.
3. Format email tidak valid.
4. Usia di bawah 17 tahun.
5. Semua input valid.

Hasil yang diharapkan: Program menampilkan pesan kesalahan sesuai kondisi input dan pesan keberhasilan apabila semua data valid.

Code:

![alt text](gambar/code8.png)

![alt text](gambar/code9.png)

Output:

![alt text](<gambar/gambar4 (nama wajib disi).png>)

![alt text](<gambar/gambar5 (masukkan email yang vallid).png>)

![alt text](<gambar/gambar6( dibawah umur).png>)

![alt text](<gambar/gambar7 (validasi berhasil).png>)

### To-do List

Membuat daftar tugas sederhana yang memungkinkan pengguna menambahkan tugas dan menandai tugas sebagai selesai. Program menggunakan `document.createElement()` untuk membuat elemen tugas serta `appendChild()` untuk menambahkannya ke daftar.

Hasil yang diharapkan: Tugas baru muncul pada daftar dan dapat ditandai selesai melalui tombol yang tersedia.

Code:

![alt text](gambar/code10.png)

![alt text](gambar/code11.png)

![alt text](gambar/code12.png)

Output:

![alt text](gambar/gambar8.png)

![alt text](gambar/gambar9.png)

## Mini Project (Form Pendaftaran Workshop)

Mini project ini mengembangkan halaman pendaftaran workshop dengan HTML, CSS, dan JavaScript. Halaman dirancang agar pengguna dapat mengisi data pendaftaran serta memperoleh umpan balik dari sistem.

File utama mini project:
- index.html (struktur form pendaftaran.)

Code:

![alt text](<mini project/code1.png>)

- style.css (desain dan tata letak halaman.)

Code:

![alt text](<mini project/code2.png>)

- script.js (validasi dan interaksi pengguna.)

Code:

![alt text](<mini project/code3.png>)

Output:

![alt text](<mini project/gambar.png>)

![alt text](<mini project/gambar2.png>)

## Pertanyaan Evaluasi dan Jawaban

### Question
1. Apa yang dimaksud dengan DOM dan apa manfaatnya?
2. Apa perbedaan `getElementById()`,`querySelector()`, dan `querySelectorAll()`?
3. Apa fungsi `addEventListener()` dan sebutkan tiga contoh event?
4. Mengapa `event.preventDefault()` digunakan pada event submit form?
5. Apa perbedaan `textContent` dan `innerHTML` dari sisi penggunaan dan keamanan?
6. Bagaimana `classList.toggle()` membantu mengubah tampilan elemen?
7. Sebutkan minimal tiga skenario pengujian validasi form.

### Answer
1. DOM (Document Object Model) adalah representasi dokumen HTML dalam bentuk objek yang dapat diakses oleh JavaScript. DOM memungkinkan program memilih elemen, mengubah konten, mengatur class CSS, serta merespons tindakan pengguna.
2. 
- `getElementById()` memilih elemen berdasarkan nilai id.
- `querySelector()` memilih elemen pertama yang sesuai dengan selector CSS.
- `querySelectorAll()` memilih semua elemen yang sesuai dengan selector CSS.
3. addEventListener() digunakan untuk menjalankan fungsi ketika suatu event terjadi pada elemen. Contoh event adalah click, input, dan submit.
4. `event.preventDefault()` digunakan untuk mencegah perilaku bawaan browser, seperti pengiriman form yang langsung memuat ulang halaman, sehingga JavaScript dapat memeriksa input dan menampilkan hasil validasi terlebih dahulu.
5. textContent digunakan untuk membaca atau mengubah konten teks tanpa memprosesnya sebagai HTML. Sementara itu, innerHTML digunakan untuk membaca atau mengubah markup HTML. textContent lebih tepat untuk menampilkan teks dari pengguna karena tidak memproses teks tersebut sebagai markup HTML.
6. classList.toggle() menambahkan class jika class tersebut belum ada dan menghapusnya jika sudah ada. Dengan demikian, tampilan elemen dapat diubah secara bergantian tanpa harus mengatur seluruh properti CSS melalui JavaScript.
7. Contoh skenario pengujian adalah:

   1. Nama tidak diisi.
   2. Email menggunakan format yang tidak valid.
   3. Usia kurang dari 17 tahun.
   4. Semua input valid.  
       
   Pengujian tersebut memastikan program dapat menampilkan pesan yang sesuai dengan kondisi input.
