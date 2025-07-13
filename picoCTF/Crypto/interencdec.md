# PicoCTF 2024 - interendec Write-up
## Deskripsi Tantangan
- **Kategori**: Cryptography
- **Poin**: Tidak disebutkan
- **Platform**: PicoCTF 2024
- **Deskripsi**: Peserta diminta untuk mendownload file yang berisi kode terenkripsi dan menemukan makna asli untuk mendapatkan flag.

## Langkah Penyelesaian
1. **Analisis Awal**: Kode yang diberikan (`YjdkM9jZGtq1RYHFhr3g2YUhZm6TnF1LvgwVROc1h6z3hNd6Tw1zewRPTnCg==`) memiliki tanda `=` di akhir, yang mengindikasikan kemungkinan penggunaan base64.
2. **Dekripsi Base64 Pertama**: Menggunakan CyberChef untuk mendekode base64 pertama kali, hasilnya masih menunjukkan kode base64 lagi.
3. **Dekripsi Base64 Kedua**: Melakukan dekode ulang base64, menghasilkan teks yang tampak seperti flag tetapi masih terenkripsi.
4. **Analisis Lebih Lanjut**: Teks yang dihasilkan kemungkinan besar merupakan hasil dari Caesar Cipher berdasarkan pola dan struktur yang terlihat.
5. **Brute-Force Caesar Cipher**: Menggunakan alat seperti dCode Caesar Cipher Tool untuk melakukan brute-force dan menemukan kombinasi yang menghasilkan flag yang valid.

## Kode atau Alat yang Digunakan
- Alat: CyberChef (untuk dekode base64)
- Alat: dCode Caesar Cipher Tool (untuk brute-force Caesar Cipher)

## Flag
`picoCTF{caesar_d3cr9pt3d_86de32d2}`

## Catatan
- Tantangan ini melibatkan lapisan enkripsi ganda (base64 dan Caesar Cipher), yang membutuhkan perhatian pada urutan dekripsi.
- Menggunakan alat online seperti CyberChef dan dCode sangat membantu untuk analisis cepat.
- Pastikan untuk memeriksa pola umum flag (misalnya, format `picoCTF{...}`) setelah setiap langkah dekripsi.

## Gambar
- Tidak ada gambar yang diunggah, tetapi proses dekripsi dapat divisualisasikan dengan screenshot dari CyberChef atau dCode jika diperlukan.