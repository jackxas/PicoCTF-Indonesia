Ketika kita menjalankan programy yang dikasih di deskripsi,kita diminta menjawab sebuah ascii decimal dari suatu angka

Ketika sudah menjawab benar,program belum memberikan flag

Di soal diberikan sebuah source code program tersebut

Didalam program terdapat 

    if user_input == "\x65"*1751:
      print(open("./flag.txt", "r").read())
      break

\x65 adalah notasi heksadesimal.
Nilai heksadesimal 0x65 sama dengan 101 dalam desimal.
Nilai desimal ASCII 101 sesuai dengan karakter e.

Jadi kita perlu memasukkan huruf e sebanyak 1751 ke input

python3 -c 'print("e"*1751)' (program python cepat untuk menampilkan e sebanyak 1751)
