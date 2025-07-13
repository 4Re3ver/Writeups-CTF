# PicoCTF - [Crypto] interendec 
## Deskripsi Tantangan
- **Kategori**: Cryptography
- **Poin**: Tidak disebutkan
- **Platform**: PicoCTF 2024
- **Deskripsi**: Diberikan file yang berisi kode terenkripsi.

## Langkah Penyelesaian
1. **Analisis Awal**: Kode yang diberikan (`YjdkM9jZGtq1RYHFhr3g2YUhZm6TnF1LvgwVROc1h6z3hNd6Tw1zewRPTnCg==`) memiliki tanda `=` di akhir, yang mengindikasikan kemungkinan penggunaan base64.
2. **Dekripsi Base64 Pertama**: Menggunakan CyberChef untuk mendekode base64 pertama kali, hasilnya masih menunjukkan kode base64 lagi.
3. **Dekripsi Base64 Kedua**: Melakukan dekode ulang base64, menghasilkan teks yang tampak seperti flag tetapi masih terenkripsi.
4. **Analisis Lebih Lanjut**: Teks yang dihasilkan kemungkinan besar merupakan hasil dari Caesar Cipher berdasarkan pola dan struktur yang terlihat.
5. **Brute-Force Caesar Cipher**: Menggunakan alat seperti dCode Caesar Cipher Tool untuk melakukan brute-force dan menemukan kombinasi yang menghasilkan flag yang valid.

## Alat yang Digunakan
- Alat: CyberChef (untuk dekode base64)
- Alat: dCode Caesar Cipher Tool (untuk brute-force Caesar Cipher)

## Flag
`picoCTF{caesar_d3cr9pt3d_86de32d2}`
