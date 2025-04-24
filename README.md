# 🥦 Submission Klasifikasi Gambar : Vegetable Image Dataset

## ✨ Deskripsi
Repositori ini berisi proyek akhir dari pembelajaran Machine Learning yang fokus pada klasifikasi gambar sayuran menggunakan Convolutional Neural Network (CNN). Model dikembangkan dengan TensorFlow dan Keras, serta dievaluasi dengan berbagai metrik akurasi dan visualisasi hasil prediksi.

## ✨ Ringkasan
Model dikembangkan untuk mengenali beberapa jenis sayuran berdasarkan gambar. Dataset citra yang digunakan telah dibagi menjadi data pelatihan, validasi, dan pengujian. Proses augmentasi dilakukan untuk memperkaya variasi data, dan model dioptimalkan menggunakan `Adam Optimizer `.

## 🔍 Fitur Utama
- **Klasifikasi Gambar Multikategori**: Memprediksi label dari gambar sayuran secara otomatis.
- **Augmentasi Data**: Termasuk rotasi, flip horizontal, zoom, dan transformasi lainnya untuk meningkatkan kemampuan generalisasi model.
- **CNN Arsitektur Sederhana**: Dirancang menggunakan `Sequential API` dengan lapisan `Conv2D`, `MaxPooling2D`, dan `Dense`.
- **Evaluasi Model**: Menggunakan confusion matrix, classification report, dan visualisasi hasil akurasi/loss.
- **Inference**: Pengujian pada gambar individual menggunakan model `TFSMLayer` dan `TFLite Interpreter`.

## 📦 Dataset
- Nama Dataset: Vegetable Image Dataset
- Sumber: https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset?utm_source=chatgpt.com
- Jumlah Kelas: 15 kelas 
- Total gambar: 21000
- Ukuran citra: Gambar-gambar memiliki ukuran awal yang bervariasi, namun seluruhnya di-resize ke ukuran 128x128 piksel sebelum digunakan dalam pelatihan dan pengujian model
- Dataset dibagi menjadi: 70% training, 20% validation, 10% testing

## 🧠 Arsitektur Model
- Jenis Model: CNN (Sequential)
- Lapisan Utama:
  - Conv2D → MaxPooling2D
  - Flatten → Dense
- Aktivasi: ReLU untuk hidden layers, Softmax untuk output
- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Metrik Evaluasi: Accuracy

## 📈 Hasil Evaluasi & Visualisasi
Hasil Evaluasi
Kode tersebut mengevaluasi model yang dilatih menggunakan data uji dan menampilkan akurasi dan loss.
- Akurasi Training: Model mencapai akurasi 98.25% pada data training. Ini ditunjukkan oleh output dari kode:
```
print(f"Akurasi Train: {train_accuracy[-1] * 100:.2f}%")
```
- Akurasi Testing: Model mencapai akurasi 93.54% pada data testing. Ini ditunjukkan oleh output dari kode :
```
print(f'Test Accuracy: {test_accuracy}')
```
- Loss: Kode juga menghitung dan menampilkan loss pada data testing. Nilai loss menunjukkan seberapa besar kesalahan model dalam prediksinya. Semakin rendah loss, semakin baik model tersebut.

Hasil Visualisasi
Kode tersebut juga membuat plot untuk memvisualisasikan akurasi dan loss model selama proses training.

Plot Akurasi: Menampilkan akurasi model pada data training dan validasi selama proses training. Plot Loss: Menampilkan loss model pada data training dan validasi selama proses training.

## 💻Cara Penggunaan
Menjalankan di Google Colab
1. Upload file `.ipynb` ke Colab
https://colab.research.google.com/drive/1HZw_IvMDD-n17Q4O9YPdTbzqMvBVDdyx#scrollTo=9ICO2-E0YxzD 
2. Upload folder dataset ke runtime
https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset?utm_source=chatgpt.com
3. Jalankan setiap sel dari atas ke bawah sesuai urutan

Menjalankan di Lokal (Jupyter Notebook)
1. Clone repositori ini
https://github.com/maylina-may/Submission-Proyek-Klasifikasi-Gambar-Vegetable
2. Install dependensi menggunakan `pip install -r requirements.txt`
3. Buka dan jalankan notebook secara berurutan

Akses File lengkapnya
GoogleDrive
https://drive.google.com/drive/folders/1uksNRNCvpOuAwCCUN8BPwudkCAyjbtK8?usp=sharing

## 💾 Format Model
- .Keras
- SavedModel
- TensorFlow Lite
- TensorFlow.js

## 👩‍💻 Kontributor
| Nama Lengkap      | Email                        | ID Dicoding             |
|-------------------|------------------------------|--------------------------|
| Maylina Nur'aini  | maylinanuraini@gmail.com     | mc444d5x0679             |
