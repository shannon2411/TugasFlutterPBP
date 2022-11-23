<details>
<summary> Tugas 7 </summary>
<pre>

## counter_7

##  **Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.** 

Stateless widget adalah widget yang tidak dapat berubah contohnya Icon, IconButton, dan text. Sedangkan stateful widget adalah  widget yang sifatnya dinamis atau dapat berubah-ubah, contohnya mengubah nilai variable, warna, dll.

##  **Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya**

- AppBar : display toolbar widgets, seperti title dan actions
- Material App : sebagai root dari aplikasi
- Scaffold : menyediakan struktur dasar dan styling dalam aplikasi
- Column : Display children dalam format vertikal
- Row : Display children dalam format horizontal
- Text : Display string dalam satu baris


##  **Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.**

berfungsi untuk memberitahu framework bahwa ada object yang berubah pada State, kemudian akan melakukan build ulang pada Widget tersebut. Variabel yang akan terdampak adalah variable yang diganti pada fungsi tersebut (tergantung fungsi tersebut ingin mengubah apa)

##  **Jelaskan perbedaan antara const dengan final.**

final dapat digunakan untuk deklarasi variabel immutable yang nilainya sudah ataupun belum diketahui pada saat waktu kompilasi berjalan. Sedangkan Const dapat digunakan untuk deklarasi variabel immutable yang nilainya bersifat konstan dan harus sudah diketahui pada saat waktu kompilasi (Compile time) berjalan, artinya adalah nilai dari variabel tersebut harus sudah di berikan value secara langsung.

## **Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.**

1. Melakukan perintah ```flutter create counter_7```

2. Mengimplementasikan widget - widget yang diperlukan pada program dan melakukan styling 

3. Membuat fungsi untuk logika penambahan dan pengurangan angka.

4. Menambahkan variabel dan fungsi berikut untuk mengubah text dan warna text ketika angka berubah

5. Mengimplementasikan Bonus yaitu dengan menambahkan kondisi tersebut sebelum button - agar button - hilang ketika angka 0.

</pre>
</details>

<details> 
<summary> Tugas 8 </summary>
<pre>
1. Jelaskan perbedaan Navigator.push dan Navigator.pushReplacement

Navigator.push menambahkan rute ke tumpukan rute yang dikelola oleh Navigator. Navigator.pushReplacement menambahkan rute ke tumpukan rute yang dikelola oleh Navigator saat ini dengan mendorong rute yang diberikan dan kemudian membuang rute sebelumnya setelah rute baru selesai dianimasikan.

2. Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.

* Card -> Untuk membentuk sebuah component Ketru seperti container dan diloop untuk tiap" data
* Drawer -> Panel untuk melakukan perpindahan tampilan atau navigator
* TextFormField -> Component untuk ask input text
* Form -> Membuat sebuah container untuk dijadikan parent dari input input yang dideklarasikan
* ListTile -> component yang didalamnya juga bisa digunakan widget
* Column, Padding, Row -> positioning
* DropDownButton -> Membuat fields untuk memilih input
* DatePicker -> pilih tanggal
* TextStyle -> Styling text
* Container -> menampung beberapa komponen 
* TextButton -> membuat tombol berbasis text untuk trigger datepicker

3. Sebutkan jenis-jenis event yang ada pada Flutter (contoh: onPressed).
* OnPressed
* OnChange
* OnSaved
* OnTap
* OnComplete

4. Jelaskan bagaimana cara kerja Navigator dalam "mengganti" halaman dari aplikasi Flutter.
Navigator pada Flutter menggunakan implementasi stack. Navigator menyediakan metode untuk mengubah tumpukan dengan push to stack atau dengan keluar dari tumpukan. Metode Navigator.push adalah untuk menavigasi ke halaman yang lebih baru dan Navigator.pop untuk kembali dari halaman saat ini.

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Membuat file drawer yang berisi route untuk masing masing class untuk counter, show_Budget, atau form.
2. Membuat file form.dart untuk membuat form untuk dimasukkan kedalam List di budget.
3. File budget akan diset untuk memiliki fungsi untuk menambahkan obj pada atribut classnya untuk menampung data yang diinput.
4. Membuat show_Budget dan melakukan loop dari budget.len untuk diloop dan ditampilan sebagaimananya dengan Card view. Menggunakan ListView.Builder

</pre>
</details>

<details> 
<summary> Tugas 9 </summary>
<pre>
##  **Apakah bisa kita melakukan pengambilan data JSON tanpa membuat model terlebih dahulu? Jika iya, apakah hal tersebut lebih baik daripada membuat model sebelum melakukan pengambilan data JSON?.** 

Ya bisa, kita dapat menggunakan manual serialization yaitu dengan menggunakan built-in JSON decoder dari dart:convert. Kita akan passing raw JSON String ke jsonDecode(), kemudian hasilnya akan ada pada Map<String, dynamic>. Namun membuat model akan lebih baik sebelum melakukan pengambilan data JSON, karena jika kita mengambil banyak akan lebih error-prone dan susah untuk di manage, jika JSON field typo / tidak ada maka akan error saat runtime.

##  ** Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.** 

- Material App : sebagai root dari aplikasi
- Scaffold : menyediakan struktur dasar dan styling dalam aplikasi
- Text : Display string dalam satu baris
- AppBar : display toolbar widgets, seperti title dan actions
- Padding : widget yang insets child dengan memberikan padding
- Drawer : Panel Desain Material yang meluncur secara horizontal dari tepi Scaffold  untuk menampilkan tautan navigasi dalam aplikasi.
- ListView : Display children satu persatu dalam scrolling direction
- SizedBox : Sebuah kotak dengan ukuran tertentu. Jika diberikan anak, widget ini memaksa anaknya untuk memiliki lebar dan/atau tinggi tertentu
- Container : Widget kenyamanan yang menggabungkan lukisan umum, penentuan posisi, dan widget ukuran.
- Column : Display children dalam format vertikal

##  ** Jelaskan mekanisme pengambilan data dari json hingga dapat ditampilkan pada Flutter.** 

1. Menambahkan dependensi http ke proyek, dependency ini digunakan untuk bertukar data melalui HTTP request, seperti GET, POST, PUT, dan lain-lain.

2. Membuat model sesuai dengan respons dari data yang berasal dari web service tersebut.

3. Membuat http request ke web service menggunakan dependency http.

4. Mengkonversikan objek yang didapatkan dari web service ke model yang telah kita buat di langkah kedua.

5. Menampilkan data yang telah dikonversi ke aplikasi dengan FutureBuilder.

##  ** Cara Implementasi.** 

1. Menambahkan drawer untuk watchlist
2. Membuat model yang sesuai untuk data json mywatchlist
3. Membuat function untuk fetch data dari mywatchlist/json
4. Menampilkan data pada widget
5. Membuat page detail untuk data

</pre>
</details>
