# counter_7

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

