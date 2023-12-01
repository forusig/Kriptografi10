# Kriptografi10
pembahasan tentang one time pad

<table>
<th>nama</th>
<th>prodi</th>
<th>kelas</th>
<tr>
<th>Ade Maulani Bilgis</th>
<th>Teknik Informatika</th>
<th>TI.21.A1</th>
</tr>
</table>

## Alur Algoritma
1.	Tentukan plainteks
2.	Tentukan kunci
   ```
plaintext = input("Plaintext: ")
key = input("kunci: ")
```
3.	Ubahk plainteks ke ascii
4.	Ubah kunci ke ascii
```
asci = konversiascii(text)
key_A = konversiascii(key)
```  
5.	Ubah planinteks ascii (Desimal) ke biner
6.	Ubah Kunci ascii (Desimal) ke biner
```
textb = konversibiner(asci)
keyb = konversibiner(key_A)
```
7.	Lakukan Xor hasil biner Plainteks dan Kunci
    ```
    result = xor_biner(textb, keyb)
    ```
12.	Hasil XOR kembalikan ke decimal
13.	Desimal hasil Xor ambil kode asciinya jadilah Eckeripsi OTP

```
decrypted_result = xor_biner(result, keyb)
hasil_deskripsi_karakter = [kodeascii(biner_ke_desimal(biner)) for biner in decrypted_result]
decimal_results = [biner_ke_desimal(b) for b in result]
ascii_results = [kodeascii(d) for d in decimal_results]
```

## contoh hasil
![Screenshot 2023-11-30 234804](https://github.com/forusig/Kriptografi10/assets/92717505/0ab5bf3a-c1ec-4552-99b0-37aca41d1cb6)
![Screenshot 2023-12-01 004610](https://github.com/forusig/Kriptografi10/assets/92717505/d7075b1e-5680-4d52-bfa7-d6fc4ed4cdab)
