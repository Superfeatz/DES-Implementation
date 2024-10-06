# Tugas Implementasi Data Encryption Standard (DES)

## Nama  :  Muhammad Hafidz Harridil Mahali
## NRP  :  5025221030


Repositori ini berisi implementasi algoritma **Data Encryption Standard (DES)** dalam Python. Algoritma ini mendukung proses enkripsi dan dekripsi teks dengan menggunakan kunci sepanjang 8 karakter yang diberikan oleh pengguna. Algoritma DES beroperasi pada blok data 64-bit dan menggunakan struktur Feistel dengan 16 ronde untuk enkripsi.

## Fitur
- **Enkripsi**: Mengubah plaintext menjadi ciphertext menggunakan DES dengan kunci yang diberikan oleh pengguna.
- **Dekripsi**: Mengubah ciphertext kembali menjadi plaintext asli dengan menggunakan kunci yang sama.
- **Key Generation**: Menghasilkan 16 sub-kunci dari kunci 8 karakter yang digunakan untuk setiap ronde enkripsi dan dekripsi.

## Daftar Isi
- [Cara Kerja](#cara-kerja)
- [Cara Menggunakan](#cara-menggunakan)
- [Contoh](#contoh)
- [Kebutuhan](#kebutuhan)


## Cara Kerja

Algoritma DES bekerja dengan membagi teks yang akan dienkripsi menjadi blok-blok 64-bit. Setiap blok akan melalui beberapa tahapan proses, yaitu:

1. **Initial Permutation (IP)**: Sebelum enkripsi dimulai, data awal diacak menggunakan tabel permutasi awal.
2. **16 Ronde Feistel**: Pada setiap ronde, data dibagi menjadi dua bagian (left dan right). Setiap bagian akan mengalami operasi Feistel (expansion, substitusi menggunakan S-box, permutasi, dan XOR).
3. **Final Permutation (FP)**: Setelah 16 ronde selesai, data yang telah diproses akan diacak lagi menggunakan tabel permutasi akhir untuk menghasilkan ciphertext.
4. **Key Generation**: Kunci 8 karakter yang diberikan akan diproses untuk menghasilkan 16 sub-kunci yang berbeda. Setiap sub-kunci digunakan di setiap ronde Feistel.

Dekripsi dilakukan dengan mengikuti proses yang sama, tetapi sub-kunci diterapkan dalam urutan yang terbalik.

## Cara Menggunakan

### 1. Enkripsi
Untuk mengenkripsi teks, pengguna akan diminta untuk memasukkan plaintext dan kunci sepanjang 8 karakter. Setelah proses enkripsi selesai, hasilnya akan diberikan dalam format **hexadecimal**.

### 2. Dekripsi
Untuk mendekripsi ciphertext, pengguna harus memasukkan ciphertext dalam format **hexadecimal** dan kunci yang sama dengan yang digunakan saat enkripsi. Hasil dekripsi akan berupa plaintext asli.

## Contoh

![Screenshot (75)](https://github.com/user-attachments/assets/0a8d05a5-f847-4eb2-a2f8-a18649e23422)


