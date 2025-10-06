# 🧠 Text Classification on BBC News Dataset

## 📖 Deskripsi
Proyek ini melakukan **klasifikasi teks berita BBC** ke dalam kategori seperti *business*, *sports*, *politics*, *entertainment*, dan *tech* menggunakan dua metode representasi teks: **TF-IDF** dan **Word2Vec**, serta algoritma klasifikasi **KNN**.

---

## ⚙️ Alur Proyek
1. **Setup & Import Data**  
   - Menggunakan Google Colab dan dataset `bbc.csv`.  
   - Visualisasi distribusi kategori dengan `matplotlib`.

2. **Preprocessing Teks**  
   - Lowercasing, hapus tanda baca, tokenisasi (`nltk`), ganti slang, hapus stopwords, dan stemming.  
   - Hasil disimpan di kolom `clean_text`.

3. **Feature Extraction**  
   - **TF-IDF**: `TfidfVectorizer(max_features=1000)`  
   - **Word2Vec**: `Word2Vec(sentences, vector_size=100, window=5, min_count=2)`

4. **Training Model**  
   - Split data 80:20 dengan `train_test_split`.  
   - Model: `KNeighborsClassifier(n_neighbors=5)`

5. **Evaluasi**  
   - Mengukur akurasi, confusion matrix, dan classification report.  
   - Bandingkan performa TF-IDF vs Word2Vec.

---

## 🧰 Library Utama
`pandas`, `matplotlib`, `nltk`, `scikit-learn`, `gensim`

---

## 📁 Struktur Folder
