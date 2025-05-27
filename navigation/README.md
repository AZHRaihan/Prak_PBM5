# Navigation
![navigation utama (pre)](https://github.com/user-attachments/assets/210e9e52-db80-4f4c-bf0b-07c344659de9)

![nav detail](https://github.com/user-attachments/assets/ea7b5c7e-7de7-412d-870e-c1127c2e9e44)

![detail route](https://github.com/user-attachments/assets/4f92751c-4847-47ab-a424-9f3224a5be40)

![nav setting screen](https://github.com/user-attachments/assets/18f18c0b-84d4-44bf-bfab-287d6418fede)

![navigation utama](https://github.com/user-attachments/assets/3c655fb4-2624-4b5c-aa34-c456d060d651)

![about page](https://github.com/user-attachments/assets/6f60fa40-a227-4249-b01c-f234a4a1a929)


## Struktur Aplikasi

- **MyApp**  
  Root widget aplikasi yang menggunakan `MaterialApp` dengan tema dan pengaturan route.

- **HomeScreen**  
  Layar utama aplikasi dengan tiga tombol untuk navigasi ke layar lain:
  - Navigasi menggunakan `Navigator.push` dengan `MaterialPageRoute`.
  - Navigasi menggunakan **named route** ke `DetailScreen`.
  - Navigasi menggunakan **named route** ke `SettingsScreen` dengan mengirimkan argumen.

- **DetailScreen**  
  Menerima dan menampilkan data string dari layar sebelumnya.  
  Terdapat tombol untuk kembali ke layar sebelumnya.

- **SettingsScreen**  
  Menerima argumen `username` dari navigasi dan menampilkannya.  
  Terdapat tombol untuk kembali ke layar sebelumnya.

---

## Fitur Navigasi

- **Navigasi Push (MaterialPageRoute)**  
  Menavigasi ke halaman baru dengan data dikirim langsung melalui konstruktor widget.

- **Named Routes**  
  Navigasi menggunakan nama route yang sudah didefinisikan di `MaterialApp`.  
  Data dapat dikirim lewat parameter `arguments`.

- **Mengambil Argumen pada Halaman Tujuan**  
  Menggunakan `ModalRoute.of(context)?.settings.arguments` untuk mengambil data yang dikirim lewat `arguments`.

---

## Cara Menjalankan

1. Pastikan Flutter SDK sudah terinstall dan environment sudah siap.
2. Clone repo ini atau salin file `main.dart`.
3. Jalankan perintah berikut di terminal:
   flutter run
