# Janji
Saya Elsa Nurjanah dengan NIM 2306026 mengerjakan Tugas Praktikum 4 dalam mata kuliah Desain dan Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

# Alur Program
## **1. Kelas**
Kelas Mahasiswa merepresentasikan data seorang mahasiswa dengan atribut berikut:
- `nim: str` -> Nomor Induk Mahasiswa
- `nama: str` -> Nama mahasiswa
- `jenisKelamin: str` -> Jenis kelamin mahasiswa
- `jalurMasuk: str` -> Jalur penerimaan mahasiswa (SNBP/SNBT/Mandiri)

## **2. Menu**
Program `Menu.java` adalah aplikasi GUI berbasis Java Swing yang memungkinkan pengguna untuk mengelola data mahasiswa. Aplikasi ini memungkinkan pengguna untuk menambahkan, memperbarui, dan menghapus data mahasiswa yang disimpan dalam `ArrayList`. Data mahasiswa ditampilkan dalam `JTable`, yang diperbarui setiap kali ada perubahan.

Program terdiri dari beberapa komponen utama:
- **JFrame**: Sebagai jendela utama aplikasi.
- **JTable**: Untuk menampilkan daftar mahasiswa.
- **JTextField**: Untuk menginput NIM dan Nama mahasiswa.
- **JComboBox**: Untuk memilih jenis kelamin mahasiswa.
- **JRadioButton**: Untuk memilih jalur masuk mahasiswa (SNBP, SNBT, Mandiri).
- **JButton**: Untuk menambahkan, memperbarui, menghapus, dan membatalkan aksi input.

## **3. Fitur**

### **a. Menampilkan Data Awal**
Pada saat program dijalankan, data awal mahasiswa diisi melalui `populateList()`, yang menambahkan beberapa data awal ke dalam `ArrayList<Mahasiswa>`.

### **b. Menambahkan Data Mahasiswa**
1. Pengguna mengisi **NIM**, **Nama**, memilih **Jenis Kelamin**, dan **Jalur Masuk**.
2. Klik tombol **"Add"**, data baru ditambahkan ke `ArrayList`.
3. Tabel diperbarui dengan memanggil `setTable()`.
4. Form input dikosongkan dengan `clearForm()`.
5. Notifikasi sukses ditampilkan.

### **c. Memperbarui Data Mahasiswa**
1. Pengguna memilih baris dalam `JTable`, yang secara otomatis mengisi formulir input.
2. Tombol **"Add"** berubah menjadi **"Update"**.
3. Pengguna dapat mengubah data dan klik **"Update"**.
4. Data dalam `ArrayList` diperbarui dan tabel direfresh.
5. Notifikasi sukses ditampilkan.

### **d. Menghapus Data Mahasiswa**
1. Pengguna memilih baris dalam `JTable`.
2. Tombol **"Delete"** muncul.
3. Jika diklik, akan muncul konfirmasi.
4. Jika konfirmasi "Yes", data dihapus dari `ArrayList` dan tabel diperbarui.

### **e. Membatalkan Aksi Input**
1. Klik tombol **"Cancel"** akan mengosongkan form input.
2. Tombol **"Update"** kembali menjadi **"Add"**.
3. Tombol **"Delete"** disembunyikan kembali.

## **4. Implementasi Event Handling**
- `ActionListener` digunakan pada tombol **Add/Update**, **Delete**, dan **Cancel**.
- `MouseAdapter` digunakan untuk menangani klik pada tabel, memungkinkan pemilihan dan pengisian otomatis form input.

# Dokumentasi
## Tampilan Awal
![Main](https://github.com/elsanrj/TP4DPBO2025C1/blob/main/Dokumentasi/1_select.png?raw=true)
## Add
![Main](https://github.com/elsanrj/TP4DPBO2025C1/blob/main/Dokumentasi/2_add.png?raw=true)
## Update
![Main](https://github.com/elsanrj/TP4DPBO2025C1/blob/main/Dokumentasi/3_update.png?raw=true)
## Delete
![Main](https://github.com/elsanrj/TP4DPBO2025C1/blob/main/Dokumentasi/4_confirmDelete.png?raw=true)
![Main](https://github.com/elsanrj/TP4DPBO2025C1/blob/main/Dokumentasi/5_delete.png?raw=true)
