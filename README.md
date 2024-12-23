# **UAS Deep Learning: Chatbot Layanan Akademik UNIB**

## **Nama Kelompok**

| **Nama**                      | **NPM**      |
|-------------------------------|--------------|
| Muhamad Rifqi Afriansyah       | G1A021023    |
| Vilda Aprilia                  | G1A021033    |
| Muhamad Iqbal                  | G1A021073    |

---

## **Deskripsi Proyek**
Proyek ini bertujuan untuk membangun model **Long Short-Term Memory (LSTM)** yang dapat digunakan untuk tugas klasifikasi teks. Model dilatih menggunakan dataset teks yang telah diolah sebelumnya, termasuk proses tokenisasi, padding, dan encoding label.

---

## **Langkah-Langkah Proyek**
1. **Pengolahan Data:**
   - Tokenisasi teks menggunakan `Tokenizer`.
   - Padding untuk menyamakan panjang semua urutan.
   - Encoding label menggunakan `LabelEncoder`.

2. **Arsitektur Model:**
   - **Embedding Layer:** Untuk representasi kata ke dalam bentuk vektor.
   - **LSTM Layer:** Untuk memproses data berurutan dan menangkap hubungan antar kata.
   - **Flatten Layer:** Untuk meratakan keluaran dari LSTM.
   - **Dense Layer dengan Softmax:** Untuk klasifikasi menjadi beberapa kelas.

3. **Kompilasi Model:**
   - **Loss Function:** Sparse Categorical Crossentropy.
   - **Optimizer:** Adam.
   - **Metrics:** Accuracy.

4. **Pelatihan Model:**
   - Model dilatih selama 300 epoch.
   - Dataset dibagi menjadi training dan testing untuk validasi performa.

---

## **Hasil Pelatihan**
Setelah melakukan proses pelatihan model LSTM, berikut adalah hasil yang dicapai:

### **Parameter Pelatihan**
- **Jumlah epoch:** 300

### **Hasil Akhir Pelatihan**
- **Accuracy pada epoch terakhir:** 0,9968
- **Loss pada epoch terakhir:** 0,0178

### **Visualisasi Grafik**
Berikut adalah grafik yang menunjukkan **Akurasi** dan **Loss** model selama proses pelatihan:

### **Grafik Akurasi**
![grafik_accuracy](https://github.com/user-attachments/assets/f826135c-471d-4705-8315-33cc65af8b99)

### **Grafik Loss**
![grafik_loss](https://github.com/user-attachments/assets/0dfb0e51-cfa2-4564-8817-24439fe9fa2b)

### **Hasil Chatbot**
![image](https://github.com/user-attachments/assets/9a8ec092-dd75-491d-9267-37e70721cf5c)

---

## **Kesimpulan**
Model LSTM yang telah dilatih menunjukkan hasil yang sangat memuaskan:
- **Accuracy akhir** yang sangat tinggi (**99.68%**).
- **Loss akhir** yang sangat rendah (**0.0178**), menunjukkan error yang kecil dalam prediksi model.

Model ini siap untuk diimplementasikan dalam berbagai tugas klasifikasi teks seperti chatbot, analisis sentimen, atau tugas lainnya yang melibatkan teks.

---

## **Cara Menjalankan**
1. Clone repositori ini:
   ```bash
   git clone https://github.com/rifqiafr/Chatbot-Layanan-Akademik-UNIB.git
2. Di Colab, jalankan kode berikut untuk mengakses file dari Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
3. Upload dataset dan file proyek ke Google Drive Anda. Pastikan file dataset berada di direktori yang tepat, seperti `/content/drive/MyDrive/Dataset Chatbot/intents.json`

