# Panduan Instalasi Linux

## Langkah-Langkah Instalasi Mengunduh VirtualBox

1. Kunjungi [situs resmi VirtualBox](https://www.virtualbox.org/wiki/Downloads).
2. Pilih versi yang sesuai dengan sistem operasi Anda.
3. Unduh file instalasi VirtualBox.

### Instalasi Linux Mint pada VirtualBox

1. Buka VirtualBox dan klik "New".
   ![Langkah 1](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/1.png)

2. Atur base memory sesuai kapasitas laptop Anda.
   ![Langkah 2](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/2.png)

3. Buat disk virtual dengan ukuran 25,00 GB.
   ![Langkah 3](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/3.png)

4. Atur pengaturan display:
   - Video memory: 128 MB
   - Monitor Count: 1
   - Scale Factor: 100%
   ![Langkah 4](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/4.png)

5. Lengkapi Machine Name dan OS Type.
   ![Langkah 5](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/5.png)

6. Mulai instalasi Linux Mint.
   ![Langkah 6](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/6.png)

7. Pilih opsi untuk memasang codec multimedia.
   ![Langkah 7](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/7.png)

8. Lanjutkan proses instalasi.
   ![Langkah 8](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/8.png)

9. Pilih zona waktu Anda.
   ![Langkah 9](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/9.png)

10. Buat username, nama host, dan password.
    ![Langkah 10](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/10.png)

11. Tunggu proses instalasi selesai.
    ![Langkah 11](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/11.png)

12. Nyalakan ulang sistem.
    ![Langkah 12](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/12.png)

13. Instalasi selesai! Selamat menggunakan Linux Mint.
    ![Langkah 13](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/13.png)

## Analisis Mount Point "/"

![Mount Point](https://github.com/tritusmita31/09011182328114_TriTusmita_TugasSO/blob/main/soal%202.png)

Mount point "/" dipilih saat instalasi karena:
Mount point adalah direktori dalam sistem file yang berfungsi sebagai titik akses untuk sistem file lain. Ketika sistem file terpasang pada mount point, isi dari sistem file tersebut dapat diakses seolah-olah menjadi bagian dari struktur direktori yang lebih besar. Ini memungkinkan pengguna untuk mengintegrasikan berbagai sistem file ke dalam satu hierarki direktori yang koheren, yang sangat pentingdalam sistem operasi seperti Unix, Linux, dan macOS.
1. **Hierarki Sistem File**: "/" adalah titik paling atas dalam struktur direktori Linux.
2. **Titik Mulai Sistem**: Sistem operasi mencari file-file penting di direktori root.
3. **Konvensi**: Standar yang umum digunakan di hampir semua distribusi Linux.

Hal yang terjadi jika salah memilih Mount Point.

•	Sistem Tidak Bisa Boot: Jika kita salah memilih mount point, sistem operasi tidak akan bisa menemukan file-file penting yang dibutuhkan untuk berjalan.

•	Data Hilang: Jika kita secara tidak sengaja menimpa partisi yang sudah berisi data dengan partisi yang kita pilih sebagai root, data pada partisi yang sebelumnya bisa hilang.


Struktur direktori dasar:
```
/
├── bin
├── etc
├── home
├── usr
└── var
```
•	bin: Berisi program-program dasar yang dibutuhkan sistem.

•	etc: Berisi file-file konfigurasi.

•	home: Berisi direktori home untuk masing-masing pengguna.

•	usr: Berisi program-program pengguna, pustaka, dan data.

•	var: Berisi file-file log, cache, dan data yang sering berubah.

Jadi, memilih "/" sebagai mount point saat instalasi Linux sangat penting karena ini menentukan di mana sistem operasi akan menyimpan semua file dan programnya. Tujuannya kita memastikan bahwa sistem operasi dapat berjalan dengan baik dan semua data kita tersimpan dengan aman.

## Penjelasan Sistem File

### Sistem File Linux
- **ext4**: Sistem file modern untuk Linux dengan kinerja tinggi dan fitur canggih.
- **ext3**: Pendahulu ext4, masih digunakan pada sistem lama. Menawarkan journaling untuk melindungi data dari kerusakan, tetapi memiliki beberapa keterbatasan dibandingkan ext4. Secara bertahap digantikan oleh ext4 karena fitur-fitur yang lebih canggih.
- **swap**: Area untuk memori virtual, bukan sistem file sebenarnya. Ketika RAM penuh, sistem operasi akan memindahkan data yang tidak sering digunakan ke swap untuk membebaskan RAM. 

### Sistem File Windows
- **NTFS**: Sistem file default Windows modern dengan fitur keamanan dan enkripsi. Ideal untuk hard disk utama pada komputer Windows.
- **FAT32**: Sistem file lama,masih digunakan pada perangkat penyimpanan eksternal seperti flash drive dan kartu memori. Memiliki keterbatasan ukuran file dan partisi, tetapi kompatibel dengan berbagai sistem operasi.

### Sistem File Modern
- **BTRFS**: Sistem file baru dengan fitur canggih seperti snapshot dan checksum.
