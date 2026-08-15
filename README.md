# Proyek Klasifikasi Gambar - Deep Learning (Dicoding)

Repositori ini berisi proyek akhir untuk kelas **Belajar Fundamental Deep Learning** di Dicoding. Proyek ini berfokus pada pengembangan model *Computer Vision* menggunakan Convolutional Neural Network (CNN) untuk mengklasifikasikan gambar kategori bunga secara akurat, serta mengekspor model ke berbagai format *deployment* (*SavedModel*, *TF-Lite*, dan *TensorFlow.js*).

---

## Fitur & Kriteria Proyek
Proyek ini telah memenuhi seluruh kriteria kelulusan dari Dicoding:
1. **Dataset**: Menggunakan dataset gambar dengan jumlah total data di atas minimum syarat kelulusan dan dibagi menjadi *Train*, *Validation*, serta *Test Set*.
2. **Arsitektur Model**: Menggunakan model `Sequential`, lapisan `Conv2D`, dan `Pooling Layer` yang dikombinasikan dengan *Transfer Learning* (MobileNetV2) untuk performa optimal.
3. **Akurasi Tinggi**: Model mencapai akurasi pada *Training* dan *Testing set* di atas **85%**.
4. **Visualisasi**: Menyediakan grafik plot akurasi dan *loss* selama proses pelatihan model.
5. **Multi-Format Deployment**: Model diekspor ke dalam format:
   - **SavedModel** (Standar TensorFlow untuk server/cloud).
   - **TF-Lite** (Dioptimalkan untuk perangkat mobile/edge).
   - **TensorFlow.js / TFJS** (Untuk aplikasi berbasis web/browser).

---

## Struktur Direktori Proyek

Struktur direktori berkas *submission* dirancang rapi sesuai standar yang disarankan:

```text
submission/
├───saved_model/
│   ├───assets/
│   ├───keras_metadata.pb
│   ├───saved_model.pb
│   └───variables/
│       ├───variables.data-00000-of-00001
│       └───variables.index
├───tfjs_model/
│   ├───group1-shard1of1.bin
│   └───model.json
├───tflite/
│   ├───label.txt
│   └───model.tflite
├───notebook.ipynb
└───requirements.txt

```

---

## Tech Stack & Dependencies

Proyek ini dikembangkan menggunakan bahasa **Python** dan *framework* Deep Learning populer:

* **TensorFlow / Keras** (v2.10.0)
* **TensorFlow.js Converter** (v3.18.0)
* **Split-Folders** (Untuk pembagian direktori dataset)
* **Matplotlib & Pillow** (Untuk visualisasi dan pemrosesan citra)

Daftar lengkap pustaka dan versi yang digunakan dapat dilihat pada file [`requirements.txt`](https://www.google.com/search?q=./submission/requirements.txt).

---

## Cara Menjalankan Notebook

1. Clone repositori ini ke perangkat lokal Anda:
```bash
git clone [https://github.com/Bangkah/dicoding-proyek-klasifikasi-gambar.git](https://github.com/Bangkah/dicoding-proyek-klasifikasi-gambar.git)

```


2. Masuk ke dalam direktori proyek dan aktifkan environment Python/Conda Anda (disarankan menggunakan Python 3.10):
```bash
conda activate athaganteng

```


3. Install dependensi yang dibutuhkan:
```bash
pip install -r submission/requirements.txt

```


4. Buka Jupyter Notebook (`notebook.ipynb`) menggunakan VS Code atau Jupyter Lab, lalu jalankan seluruh sel (*Run All*) untuk melihat proses pelatihan, evaluasi, hingga hasil plot grafik.

---

## Author

**Muhammad Dhiyaul Atha (Bangkah)**

* Mahasiswa Teknik Informatika — Politeknik Negeri Lhokseumawe
* GitHub: [@Bangkah](https://www.google.com/search?q=https://github.com/Bangkah)
