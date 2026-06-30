## Deskripsi : 
A message has been encrypted using RSA. The public key is gone… but someone might have been careless with the private key. Can you recover it and decrypt the message?
<br>

## Petunjuk :
1.Metadata can tell you more than you expect.
2.Hex can be turned back into a key file.
<br>

## Pengerjaan

Kita diberikan sebuah teks encript dan sebuah gambar

Gambarnya masukkan ke cyberchef dan beri from hex pada recipe

Salin outputnya dan buat ke sebuah file di linux

Lalu decrypt rsa di command line

openssl pkeyutl -decrypt -inkey privatekey -in flag.enc -out decryptedfile.txt

(privatekey : hasil output dari hex)
(flag.enc : teks enkripsi yang kasih)
(decryptedfile.txt : hasilnya)

cat decrypted_file.txt,akan menampilkan flag
