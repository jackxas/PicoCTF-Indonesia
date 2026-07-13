Kita diberikan sebuah folder zip dan kita disuruh mencari sebuah flag 

Jalankan perintah unzip -p big-zip-files.zip | grep "picoCTF"

unzip -p: Mengekstrak seluruh isi file zip dan langsung mengeluarkan hasilnya ke layar terminal (standard output) secara bergantian tanpa membuat folder baru di komputer Anda.

| grep "picoCTF": Menyaring keluaran tersebut dan hanya menampilkan baris yang berisi kata "picoCTF".
