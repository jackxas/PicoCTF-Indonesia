nc -vz mysterious-sea.picoctf.net 62760

smbclient -L //mysterious-sea.picoctf.net -p 62760 -N

smbclient //mysterious-sea.picoctf.net/shares -p 62760 -N

ls

get flag.txt

exit

cat flag.txt
