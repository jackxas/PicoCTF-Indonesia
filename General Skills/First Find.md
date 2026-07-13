Kita diberikan sebuah folder zip dan kita disuruh mencari file yang bernama uber-secret.txt

Tetapu kita bisa langsung mencari flagnya di folder tersebut dengan perintah grep

Jalankan perintah strings files.zip | grep pico dan kita mendapatkan flagnya

Perintah strings berfungsi untuk mengekstrak dan menampilkan karakter atau teks yang dapat dibaca

Simbol | (Pipe) ini berfungsi sebagai penghubung.

grep akan mencari dan hanya menampilkan baris teks yang mengandung kata "pico" dari seluruh tumpukan teks yang
