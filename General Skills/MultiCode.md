Kita diberikan sebuah file yang berisi teks yang sudah enkripsi

NjM3NjcwNjI1MDQ3NTMyNTM3NDI2MTcyNjY2NzcyNzE1ZjcyNjE3MDMwNzE3NjYxNzQ1ZjM4MzIzNDM5Mzk3MTZlNzEyNTM3NDQ= merupakan format Base64. Jika kita mendekodenya, kita akan mendapatkan string angka dan huruf berikut:

637670625047532537426172666772715f72617030717661745f3832343939716e71253744

String dari langkah pertama adalah kode Hexadecimal. Jika kita mengubah nilai hex tersebut menjadi teks ASCII standar, hasilnya adalah:

cvpbPGS%7Barfgrq_rap0qvat_82499qnq%7D

Pada teks di atas, terdapat karakter %7B dan %7D. Ini adalah format URL Encoding untuk tanda kurung kurawal.%7B = {%7D = }

Setelah disesuaikan, formatnya mulai terlihat jelas:cvpbPGS{arfgrq_rap0qvat_82499qnq}.Teks tersebut sekarang menggunakan sandi ROT13 (menggeser setiap huruf sebanyak 13 posisi pada alfabet).

cvpbPGS menjadi picoCTF,arfgrq menjadi nested,rap0qvat menjadi enc0ding,82499qnq menjadi 82499dad (Angka tetap sama, qnq menjadi dad)

picoCTF{nested_enc0ding_82499dad}
