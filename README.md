# Deployment Model CNN (Jeruk Nipis vs Sirih)

## Deskripsi singkat

Repository ini berisi semua file yang dibutuhkan untuk melakukan deployment model Machine Learning Image Classification menggunakan CNN (Convolutional Neural Network). Adapun model yang digunakan merupakan model untuk memprediksi gambar daun jeruk nipis atau daun sirih.

#

## Sekilas mengenai input model

Agar dapat memprediksi daun jeruk nipis atau daun sirih, data input model harus mengikuti format sebagai berikut:

-   Gambar dengan format umum seperti .jpeg, .png, .webp, dsb.
-   Gambar dikonversi ke dalam bentuk array/tensor
-   Nilai pixel gambar memiliki rentang nilai 0-1 dengan cara membagi semua nilai pixelnya dengan 255.0

#

## Folder, file, dan kegunaannya

-   static/
    -   uploads/ --> Berisi gambar yang diunggah untuk diprediksi.
-   templates/
    -   index.html --> Berisi template website.
-   app.py --> Berisi konfigurasi route dan proses prediksi model untuk API.
-   jeruknipis_sirih_class_model.h5 --> Model Image Classification CNN yang sudah di-training.
-   requirements.txt --> Berisi daftar dependency/package Python yang diperlukan untuk menjalankan API dan model Image Classification CNN.

#

## Cara menjalankan API pada komputer Anda

1. Pastikan Anda sudah menginstall Anaconda.
1. Buka terminal/command prompt/power shell.
1. Buat virtual environment dengan\
   `conda create -n <nama-environment> python=3.9`
1. Aktifkan virtual environment dengan\
   `conda activate <nama-environment>`
1. Install semua dependency/package Python dengan\
   `pip install -r requirements.txt`
1. Jalankan API menggunakan perintah\
   `python app.py`

## Akses melalui Website

1. Anda akan diberikan URL untuk membuka website berupa `localhost:5000/` atau `127.0.0.1:5000/`.
1. Buka URL dengan browser, coba masukkan gambar daun jeruk nipis atau daun sirih yang ingin di prediksi.
1. Anda akan diberikan prediksi bahwa pada gambar tersebut adalah daun jeruk nipis atau daun sirih pada halaman website.
