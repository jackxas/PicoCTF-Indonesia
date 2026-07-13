## Deskripsi : 
We intercepted a suspicious file from a system, but instead of the password itself, it only contains its SHA-1 hash. Using OSINT techniques, you are provided with personal details about the target. Your task is to leverage this information to generate a custom password list and recover the original password by matching its hash.
Download the following files:
userinfo: Contains the personal details.
hash: Contains the SHA-1 hash of the password.
check_password: Script to test passwords against the hash.
<br>

## Petunjuk :

1.CUPP is a Python tool for generating custom wordlists from personal data.

<br>

## Pengerjaan
Soal ini menguji penggunaan OSINT + password profiling. Dari deskripsinya, pembuat soal mengharapkan kita membuat wordlist menggunakan CUPP (Common User Passwords Profiler) berdasarkan data korban, lalu mencocokkannya dengan hash SHA-1.

Pertama install CUPP terlebih dahulu jika belum

git clone https://github.com/Mebus/cupp.git
cd cupp

Lalu jalankan dengan cara menjalankan perintah python3 cupp.py -i

Lalu isi sesuai dengan userinfo.txt

Nanti akan menghasilkan alice.txt

Dalam file check_password.py disebutkan WORDLIST_FILE = "passwords.txt"

Jadi ganti nama file alice.txt.

mv alice.txt passwords.txt

passwords.txt harus satu direktori dengan file check_password.py

jalankan check_password.py

python3 check_password.py
