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

<img width="378" height="146" alt="Cuplikan layar 2026-10-26 202415" src="https://github.com/user-attachments/assets/d8dceb7e-b5a3-48c3-be47-28efc96848dc" />

### Event Click

Menggunakan `addEventListener()` untuk mendeteksi ketika tombol diklik. Program kemudian memperbarui pesan dan menampilkan waktu saat tombol ditekan.

Hasil yang diharapkan: Pesan pada halaman berubah setiap kali tombol diklik.

Code:

<img width="570" height="173" alt="Cuplikan layar 2026-10-26 202814" src="https://github.com/user-attachments/assets/6e61561e-cfc8-494d-9465-eb7ccd1c5047" />

Output:

<img width="361" height="127" alt="Cuplikan layar 2026-10-26 202834" src="https://github.com/user-attachments/assets/23e8e477-8bd1-4a7f-b826-5302ea63efd1" />

### Mengubah Class dan Gaya CSS

Menggunakan `classList.toggle()` untuk menambah atau menghapus class CSS pada elemen. Perubahan class digunakan untuk mengubah warna latar belakang, garis tepi, dan ukuran teks.

Hasil yang diharapkan: Tampilan paragraf berubah ketika tombol ditekan.

Code:

<img width="435" height="180" alt="Cuplikan layar 2026-10-26 202909" src="https://github.com/user-attachments/assets/e4c53a6c-25fa-4071-af55-d59f688c09df" />

<img width="570" height="122" alt="Cuplikan layar 2026-10-26 202920" src="https://github.com/user-attachments/assets/813f232f-f887-48a5-87a9-bf0d9bfd3c2f" />

### Event input dan penghitung karakter

Menggunakan event input untuk mendeteksi perubahan pada kolom teks. Properti `value.length` digunakan untuk menghitung jumlah karakter yang dimasukkan pengguna.

Hasil yang diharapkan: Jumlah karakter bertambah atau berkurang secara langsung ketika pengguna mengetik atau menghapus teks.

Code:

<img width="570" height="62" alt="Cuplikan layar 2026-10-26 202935" src="https://github.com/user-attachments/assets/eae08406-6cbe-4cab-a174-94c3223a6fe5" />

<img width="568" height="102" alt="Cuplikan layar 2026-10-26 202950" src="https://github.com/user-attachments/assets/088bdbda-b316-44fc-a249-758ce65e2930" />

Output:

<img width="490" height="172" alt="Cuplikan layar 2026-10-26 203128" src="https://github.com/user-attachments/assets/684546ee-1c39-4e0f-8107-4a5c8f6fdc89" />

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

<img width="570" height="180" alt="Cuplikan layar 2026-10-26 203148" src="https://github.com/user-attachments/assets/446bc109-04c2-4db0-bde4-3b7e33b2729a" />

<img width="570" height="326" alt="Cuplikan layar 2026-10-26 203203" src="https://github.com/user-attachments/assets/50be574c-03ae-4b39-a70b-4f073a223227" />

Output:

<img width="676" height="340" alt="Cuplikan layar 2026-10-26 203826" src="https://github.com/user-attachments/assets/41452a96-cb81-46da-9422-61365cab8970" />

<img width="663" height="335" alt="Cuplikan layar 2026-10-26 203904" src="https://github.com/user-attachments/assets/2e13b90b-b04d-4d28-acdc-60798749452a" />

<img width="666" height="342" alt="Cuplikan layar 2026-10-26 203930" src="https://github.com/user-attachments/assets/b1fea79b-becb-4f71-9099-1a0c6d0f976f" />

<img width="670" height="340" alt="Cuplikan layar 2026-10-26 203958" src="https://github.com/user-attachments/assets/ff075518-0c78-4d5b-a71a-5a2122247e8d" />

### To-do List

Membuat daftar tugas sederhana yang memungkinkan pengguna menambahkan tugas dan menandai tugas sebagai selesai. Program menggunakan `document.createElement()` untuk membuat elemen tugas serta `appendChild()` untuk menambahkannya ke daftar.

Hasil yang diharapkan: Tugas baru muncul pada daftar dan dapat ditandai selesai melalui tombol yang tersedia.

Code:

<img width="545" height="150" alt="Cuplikan layar 2026-10-26 204245" src="https://github.com/user-attachments/assets/c70a9f99-6725-49a9-8aae-35a318b08e03" />

<img width="558" height="50" alt="Cuplikan layar 2026-10-26 204259" src="https://github.com/user-attachments/assets/68baffcc-b342-4df2-884b-9f7ae5173e26" />

<img width="570" height="500" alt="Cuplikan layar 2026-10-26 204338" src="https://github.com/user-attachments/assets/d943234c-bf29-46d4-a920-ab676e90dec2" />
Output:

<img width="661" height="381" alt="Cuplikan layar 2026-10-26 204437" src="https://github.com/user-attachments/assets/0c156cb4-3535-4459-8e59-461886e6b2f0" />

<img width="578" height="311" alt="Cuplikan layar 2026-10-26 204517" src="https://github.com/user-attachments/assets/935204bb-ad2e-4d2d-8dd6-e698c22e8c93" />

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
