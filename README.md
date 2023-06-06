# UAS_PBO_Kel3
Kode yang kami buat adalah sebuah skrip Python yang membuat antarmuka pengguna grafis (GUI) menggunakan pustaka Tkinter. GUI ini memungkinkan pengguna untuk menghasilkan, memvalidasi, menyimpan, melihat, menghapus, dan mengedit password. Berikut adalah penjelasan dari apa yang dilakukan oleh kode tersebut:

1. Kode mengimpor modul-modul yang diperlukan: `random`, `string`, `tkinter`, `messagebox`, `simpledialog`, dan `os`.
2. Fungsi `generate_password` digunakan untuk menghasilkan sebuah password dengan panjang tertentu (`panjang`). Password yang dihasilkan menggunakan kombinasi huruf (baik huruf kecil maupun huruf besar), angka, dan tanda baca. Password yang dihasilkan harus memenuhi persyaratan tertentu (setidaknya terdapat satu huruf kecil, satu huruf besar, satu angka, dan satu tanda baca).
3. Fungsi `generate_password_button` dipanggil ketika tombol "Generate Password" ditekan. Fungsi ini mengambil panjang password dari entri `panjang_entry`, kemudian memanggil fungsi `generate_password` untuk menghasilkan password baru. Password tersebut ditampilkan di entri `password_entry`.
4. Fungsi `validate_password` dipanggil ketika tombol "Validate Password" ditekan. Fungsi ini mengambil password dari entri `password_entry`, kemudian memeriksa apakah password tersebut memenuhi persyaratan yang sama dengan fungsi `generate_password`. Jika password memenuhi persyaratan, sebuah kotak pesan ditampilkan dengan informasi bahwa password memenuhi persyaratan, dan password tersebut disimpan menggunakan fungsi `save_password`. Jika password tidak memenuhi persyaratan, sebuah kotak pesan peringatan ditampilkan.
5. Fungsi `save_password` digunakan untuk menyimpan password ke dalam file "passwords.txt". Password disimpan dalam format teks, satu password per baris.
6. Fungsi `view_passwords` dipanggil ketika tombol "View Passwords" ditekan. Fungsi ini membaca isi file "passwords.txt" jika file tersebut ada. Jika ada password yang tersimpan, daftar password ditampilkan dalam kotak daftar (`listbox`). Jika tidak ada password yang tersimpan, sebuah kotak pesan ditampilkan dengan informasi bahwa tidak ada password yang tersimpan.
7. Fungsi `delete_password` dipanggil ketika tombol "Delete Password" ditekan. Fungsi ini menghapus password yang dipilih dari kotak daftar (`listbox`) dan juga dari file "passwords.txt". Sebelum menghapus password, pengguna diminta konfirmasi terlebih dahulu.
8. Fungsi `edit_password` dipanggil ketika tombol "Edit Password" ditekan. Fungsi ini memungkinkan pengguna untuk mengedit password yang dipilih dalam kotak daftar (`listbox`). Pengguna diminta memasukkan password baru melalui kotak dialog, dan password yang lama diganti dengan password baru tersebut.
9. Kode kemudian membuat window Tkinter dengan judul "Generator & Penyimpanan Password".
10. Label dan entri dibuat untuk memasukkan panjang password yang diinginkan.
11. Tombol "Generate Password" dibuat untuk memanggil fungsi `generate_password_button` saat

 ditekan.
12. Label dan entri dibuat untuk menampilkan password yang dihasilkan.
13. Tombol "Validate Password" dibuat untuk memanggil fungsi `validate_password` saat ditekan.
14. Tombol "View Passwords" dibuat untuk memanggil fungsi `view_passwords` saat ditekan.
15. Kotak daftar (`listbox`) dibuat untuk menampilkan daftar password yang telah disimpan.
16. Tombol "Delete Password" dibuat untuk memanggil fungsi `delete_password` saat ditekan.
17. Tombol "Edit Password" dibuat untuk memanggil fungsi `edit_password` saat ditekan.
18. Terakhir, aplikasi dijalankan dengan memanggil `window.mainloop()`.

Dengan menggunakan GUI ini, pengguna dapat menghasilkan password acak, memvalidasi password, menyimpan password, melihat daftar password yang telah disimpan, menghapus password yang tidak diperlukan, dan mengedit password yang ada. Semua password disimpan dalam file "passwords.txt" untuk referensi dan penggunaan selanjutnya.
