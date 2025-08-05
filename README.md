# Sistem Crawling Komentar YouTube v1.0.0

Sebuah skrip Python dalam format Jupyter Notebook yang dirancang untuk melakukan ekstraksi (crawling) komentar dari video YouTube menggunakan YouTube Data API v3. Proyek ini dikembangkan oleh **Ferdian Bangkit Wijaya** dari **Universitas Sultan Ageng Tirtayasa** untuk keperluan penelitian akademik dan analisis data.

## 📝 Deskripsi Proyek

Tool ini memungkinkan peneliti untuk mengumpulkan data kualitatif dan kuantitatif dari kolom komentar video YouTube secara sistematis. Data yang dikumpulkan mencakup teks komentar, metadata penulis, jumlah suka, balasan, serta informasi detail dari video itu sendiri.

## ✨ Fitur Utama

- **Ekstraksi Otomatis**: Mengambil komentar dan balasan dari satu atau lebih video YouTube.
- **Pengumpulan Metadata**: Mengumpulkan informasi penting video seperti judul, durasi, jumlah tayangan, dan kategori.
- **Analisis Sentimen**: Melakukan analisis sentimen dasar (positif, negatif, netral) pada teks komentar.
- **Ekspor Data**: Menyimpan hasil crawling ke dalam format **Excel (.xlsx)**, **JSON (.json)**, dan **Teks (.txt)** untuk analisis lebih lanjut.
- **Antarmuka Interaktif**: Menggunakan widget Jupyter untuk memudahkan konfigurasi tanpa mengubah kode.
- **Manajemen Quota API**: Dirancang untuk efisiensi dan dilengkapi monitoring penggunaan API.

## ⚙️ Persyaratan

Sebelum menjalankan notebook, pastikan Anda memiliki:

1. **Python 3.x** terinstal.
2. **API Key** dari Google Cloud Console.
3. **YouTube Data API v3** yang sudah diaktifkan pada proyek Google Cloud Anda.
4. Koneksi internet yang stabil.

## 🚀 Instalasi & Cara Penggunaan

1. **Clone Repositori**

    ```bash
    git clone https://github.com/ferdianwijayabangkit/crawl-youtube-comments-ipynb
    cd crawl-youtube-comments-ipynb
    ```

2. **Buat Virtual Environment (Sangat Disarankan)**

    ```bash
    # Untuk Windows
    python -m venv venv
    venv\Scripts\activate

    # Untuk macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Jalankan Jupyter Notebook**
    Buka notebook menggunakan Jupyter, Google Colab, atau Visual Studio Code.

    ```bash
    jupyter notebook Youtube_Komentar_v1.0.ipynb
    ```

4. **Konfigurasi dan Eksekusi**
    - Jalankan sel-sel notebook secara berurutan dari atas ke bawah.
    - Masukkan **API Key** Anda pada widget di **Bagian 4**.
    - Masukkan URL video yang ingin di-crawl pada widget di **Bagian 3**.
    - Konfigurasikan atribut yang ingin diambil di **Bagian 6**.
    - Mulai proses crawling di **Bagian 7**.

## ⚖️ Lisensi

Proyek ini dilisensikan di bawah **Lisensi MIT**. Lihat file `LICENSE` untuk detail lengkap. Harap gunakan tool ini secara etis dan hanya untuk tujuan penelitian akademik sesuai dengan kebijakan penggunaan yang dijelaskan dalam notebook.

## ⚠️ Disclaimer

Pengguna bertanggung jawab penuh atas penggunaan tool dan data yang dikumpulkan. Pastikan penggunaan Anda mematuhi [Persyaratan Layanan YouTube API](https://developers.google.com/youtube/terms/api-services-terms-of-service) dan regulasi privasi data yang berlaku.
