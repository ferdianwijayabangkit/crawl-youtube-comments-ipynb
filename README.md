# 📊 Sistem Crawling Komentar YouTube

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![API](https://img.shields.io/badge/API-YouTube%20Data%20v3-red?logo=youtube)

Sebuah skrip Python untuk mengekstrak komentar video YouTube secara sistematis menggunakan YouTube Data API v3. Dirancang untuk penelitian akademik dan analisis data.

## ✨ Fitur Utama

- **Ekstraksi Otomatis**: Mengambil semua komentar dan balasannya dari video YouTube target.
- **Pengumpulan Metadata Video**: Mengumpulkan informasi penting seperti judul, durasi, jumlah tayangan, dan kategori.
- **Analisis Sentimen**: Melakukan analisis sentimen dasar (positif, negatif, netral) pada setiap komentar.
- **Ekspor Multi-Format**: Menyimpan hasil ke dalam format **Excel (.xlsx)**, **JSON (.json)**, dan **Teks (.txt)**.
- **Antarmuka Interaktif**: Menggunakan widget Jupyter untuk konfigurasi API Key dan URL video tanpa mengubah kode.
- **Manajemen Quota API**: Dirancang untuk efisiensi dan dilengkapi pemantauan penggunaan kuota API.

## 🔧 Tumpukan Teknologi (Tech Stack)

- **API**: `Google API Python Client` (untuk YouTube Data API v3)
- **Analisis Data**: `Pandas`
- **Analisis Teks**: `TextBlob` atau library sejenis untuk sentimen
- **Antarmuka Pengguna**: `IPython Widgets`
- **Lingkungan**: `Jupyter Notebook`

## 🚀 Cara Memulai

### Prasyarat
- **Python 3.x** sudah terinstal di sistem Anda.
- **Kunci API (API Key)** dari Google Cloud Console yang telah mengaktifkan **YouTube Data API v3**.
- Koneksi internet yang stabil.

### Instalasi & Penggunaan

1.  **Clone Repositori**
    Gunakan `git` untuk mengunduh proyek ke komputer lokal Anda.
    ```bash
    git clone [https://github.com/ferdianwijayabangkit/crawl-youtube-comments-ipynb](https://github.com/ferdianwijayabangkit/crawl-youtube-comments-ipynb)
    cd crawl-youtube-comments-ipynb
    ```

2.  **Buat & Aktifkan Virtual Environment** (Sangat Direkomendasikan)
    ```bash
    # Untuk Windows
    python -m venv venv
    venv\Scripts\activate

    # Untuk macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Jalankan Notebook**
    Buka file `.ipynb` menggunakan Jupyter, Google Colab, atau VS Code.
    ```bash
    jupyter notebook Youtube_Komentar_v1.0.ipynb
    ```

4.  **Eksekusi di dalam Notebook**
    - **Jalankan sel instalasi** untuk mengunduh semua pustaka yang diperlukan secara otomatis.
    - **Masukkan Kunci API Anda** pada widget yang tersedia.
    - **Masukkan URL video YouTube** yang ingin Anda analisis.
    - **Mulai Proses Crawling** dengan menjalankan sel eksekusi utama.

## 📊 Struktur Data Output

Data yang berhasil diekstrak akan memiliki kolom-kolom informatif, seperti:

| Field           | Deskripsi                                    | Contoh                                     |
| --------------- | -------------------------------------------- | ------------------------------------------ |
| `video_id`      | ID unik dari video YouTube                   | "AbCdEfGhIjK"                              |
| `video_title`   | Judul lengkap video                          | "Tutorial Analisis Data dengan Python"     |
| `comment_id`    | ID unik dari setiap komentar                 | "Ugw...9fl"                                |
| `author_name`   | Nama channel dari pemberi komentar           | "Data Enthusiast"                          |
| `comment_text`  | Isi teks dari komentar                       | "Sangat bermanfaat, terima kasih banyak!"  |
| `published_at`  | Waktu komentar dipublikasikan                | "2025-08-06T01:30:00Z"                     |
| `like_count`    | Jumlah suka yang diterima komentar           | 125                                        |
| `reply_count`   | Jumlah balasan untuk komentar tersebut       | 5                                          |
| `sentiment`     | Hasil analisis sentimen (Positif/Negatif/Netral) | "Positif"                              |


## ⚖️ Lisensi & Penafian

- Proyek ini dilisensikan di bawah **Lisensi MIT**.
- Pengguna bertanggung jawab penuh atas penggunaan tool dan data yang dikumpulkan. Pastikan penggunaan Anda mematuhi [Persyaratan Layanan YouTube API](https://developers.google.com/youtube/terms/api-services-terms-of-service) dan tidak melanggar privasi.
- Gunakan Kunci API Anda dengan bijak untuk menghindari penggunaan kuota berlebih.

## 👨‍💻 Author

- **Ferdian Bangkit Wijaya**
- Universitas Sultan Ageng Tirtayasa (UNTIRTA)
- Versi: 1.0.0

---

> Tool ini dirancang untuk memfasilitasi penelitian berbasis data dari platform YouTube dengan cara yang etis dan efisien.
