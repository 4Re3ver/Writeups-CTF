# [PicoCTF - [Crypto] interendec](https://play.picoctf.org/practice/challenge/418?category=2&difficulty=1&page=1)
## Deskripsi Tantangan
- **Kategori**: Cryptography
- **Platform**: PicoCTF 
- **Deskripsi**: Diberikan file yang berisi kode terenkripsi.

## Langkah Penyelesaian
1. **Analisis Awal**: Kode yang diberikan (`YidkM0JxZGtwQlRYdHFhR3g2YUhsZmF6TnFlVGwzWVROclh6ZzJhMnd6TW1zeWZRPT0nCg==
`) memiliki tanda `=` di akhir, yang mengindikasikan kemungkinan penggunaan base64.
2. **Dekripsi Base64 Pertama**: Menggunakan CyberChef untuk mendekode base64 pertama kali, hasilnya masih menunjukkan kode base64 lagi (`d3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrXzg2a2wzMmsyfQ==`)
3. **Dekripsi Base64 Kedua**: Melakukan dekode ulang base64, menghasilkan teks yang tampak seperti flag tetapi masih terenkripsi (`wpjvJAM{jhlzhy_k3jy9wa3k_86kl32k2}`)
4. **Analisis Lebih Lanjut**: Teks yang dihasilkan kemungkinan besar merupakan hasil dari Caesar Cipher berdasarkan pola dan struktur yang terlihat.
5. **Brute-Force Caesar Cipher**: Menggunakan alat seperti dCode Caesar Cipher Tool untuk melakukan brute-force dan menemukan kombinasi yang menghasilkan flag yang valid.

## Alat yang Digunakan
- Alat: [CyberChef](https://cyberchef.io/) (untuk dekode base64) 
- Alat: [dCode Caesar Cipher Tool](https://www.dcode.fr/caesar-cipher) (untuk brute-force Caesar Cipher) 

## Flag
`picoCTF{caesar_d3cr9pt3d_86de32d2}`
