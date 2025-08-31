# IBM-granite
# Identifikasi Tren Gambar Timpa Teks 

## Deskripsi
Proyek ini bertujuan untuk mendeteksi teks yang menempel pada gambar, yang sering digunakan untuk menyebarkan hoaks melalui meme. Sistem ini memanfaatkan **IBM Granite-3.3-8b-instruct LLM** untuk mengklasifikasikan status gambar menjadi:  
- `Asli` 
- `Meme / Dimodifikasi`   
- `Tidak Terbaca` 

Dengan pendekatan ini, pengguna dapat secara cepat menilai apakah gambar tertentu mengandung konten yang berpotensi menyesatkan.

---

## Fitur Utama
- **Ekstraksi OCR**: Mengambil teks dari gambar.  
- **Pembersihan Data**: Normalisasi teks agar siap diproses.  
- **Prompt Engineering**: Aturan klasifikasi menggunakan LLM Granite.  
- **Loop Evaluasi**: Prediksi label pada batch data.  
- **Post-Processing**: Validasi label akhir (`asli`, `meme`, `tidak terbaca`).  
- **Analisis Hasil**: Distribusi label dan insight terkait tren gambar.

---

## Teknologi yang Digunakan
- **Bahasa Pemrograman**: Python  
- **Library & Tools**:  
  - `pytesseract` untuk OCR  
  - `Pandas` untuk manipulasi data  
  - IBM Granite-3.3-8b-instruct LLM untuk klasifikasi teks  

