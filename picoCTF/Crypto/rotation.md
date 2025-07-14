# [PicoCTF - [Crypto] rotation](https://play.picoctf.org/practice/challenge/373?category=2&page=1)
## Deskripsi Tantangan
- **Kategori**: Cryptography
- **Platform**: PicoCTF 
- **Deskripsi**: Diberikan file yang berisi kode terenkripsi.

## Langkah Penyelesaian
1. File terenkripsi berisi teks: `xqkwKBN{z0bib1wv_l3kzgxb3l_25l7k61j}` Jika dilihat dari formatnya, ini adalah Caesar Cipher. 
2. Dekripsi menggunakan tool online [dcode.fr/caesar-cipher](https://www.dcode.fr/caesar-cipher), dan memilih opsi bruteforce decrypt
3. Hasilnya menunjukkan flag yang valid pada offset 8 (+18)


## Tools yang Digunakan 
- [dCode Caesar Cipher Tool](https://www.dcode.fr/caesar-cipher) (untuk brute-force Caesar Cipher) 

## Flag
`picoCTF{r0tat1on_d3crypt3d_25d7c61b}`
