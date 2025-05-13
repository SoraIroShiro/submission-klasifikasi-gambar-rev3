# 🧠 Image Classification with CNN - Cats vs Dogs

Proyek ini merupakan implementasi Convolutional Neural Network (CNN) untuk klasifikasi gambar kucing dan anjing. Model dilatih untuk mengenali dan mengklasifikasikan gambar menjadi dua kategori: **Cat** dan **Dog**.

## 📁 Struktur Folder


```plaintext

submission/
├── datasets/               # Isi datasets
│   ├── all_data/
│       ├── Cat/
│       └── Dog/
|
├── saved_model/               # Model dalam format TensorFlow SavedModel
│   ├── assets/
│   ├── variables/
│   └── saved_model.pb
│
├── tflite/                    # Model dalam format TensorFlow Lite
│   ├── model.tflite
│   └── labels.txt
│
├── tfjs_model/                # Model dalam format TensorFlow.js
│   ├── model.json
│   └── group1-shard1of1.bin
│
├── notebook.ipynb             # Notebook utama proses training dan konversi model
├── requirements.txt           # Daftar dependensi Python
└── README.md                  # Dokumentasi proyek
```


## 🧪 Dataset

- Dataset: [Dogs vs Cats](https://www.microsoft.com/en-us/download/details.aspx?id=54765)
- Total Gambar: ±25.000 gambar
- Dataset dibagi menjadi:
  - Training set
  - Validation set
  - Test set\
*NOTE : Ketika memasukkan ke datasets, harus dijadikan satu (yaitu hanya cat & dog saja)

## 🧠 Arsitektur Model

Model menggunakan arsitektur CNN sederhana berbasis TensorFlow dan Keras, dengan layer:
- Conv2D + ReLU
- MaxPooling2D
- Dropout
- Flatten
- Dense

Target akurasi:
- ✅ Training accuracy ≥ 85%
- ✅ Testing accuracy ≥ 85%

## 📊 Hasil Evaluasi

- **Training Accuracy:** 90%+
- **Validation Accuracy:** 88%+
- **Test Accuracy:** 87%+

Grafik akurasi dan loss selama training tersedia di notebook.

## 🔄 Konversi Model

Model berhasil dikonversi ke dalam 3 format:
- ✅ TensorFlow SavedModel (`saved_model/`)
- ✅ TensorFlow Lite (`tflite/`)
- ✅ TensorFlow.js (`tfjs_model/`)

## ⚙️ Cara Menjalankan

1. **Klon repositori**
```bash
git clone https://github.com/username/cats-vs-dogs-cnn.git
cd cats-vs-dogs-cnn/submission
```
2. **Menginstall dependency**\
*NOTE: gunakan environtment python versi __3.9.12__
```bash
pip install -r requirements.txt
```
