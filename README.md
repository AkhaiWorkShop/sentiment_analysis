# Sentiment Analysis: Analisis Sentimen Publik terhadap Capres-Cawapres 2019

Proyek ini bertujuan untuk membangun sistem **Sentiment Analysis** berbasis NLP (Natural Language Processing) untuk mengklasifikasikan sentimen tweet terhadap pasangan calon presiden dan wakil presiden (capres-cawapres) dalam konteks Pilpres 2019. Model akan mengklasifikasikan teks ke dalam tiga kategori: **positif**, **negatif**, dan **netral**.

Proyek ini membandingkan performa berbagai pendekatan:
- **Machine Learning tradisional** (Logistic Regression, Naive Bayes, SVM)
- **Deep Learning** (LSTM, IndoBERT)

Hasil evaluasi digunakan untuk menentukan metode terbaik berdasarkan akurasi, F1-score, dan efisiensi.

---
## 🛠️ Cara Menjalankan

### 1. Clone atau buka repositori ini
Jika Anda sudah di folder lokal yang terhubung ke GitHub, lanjut ke langkah berikutnya.

### 2. Buat virtual environment (opsional tapi direkomendasikan)
```bash
python3 -m venv venv
source venv/bin/activate    # Linux/macOS
# atau
venv\Scripts\activate       # Windows


📦 Dependensi Utama
pandas – manipulasi data
numpy – komputasi numerik
re – regular expression
emoji – konversi emoji ke teks
Sastrawi – stopword removal & stemming untuk bahasa Indonesia
jupyter – untuk menjalankan notebook
📌 Catatan Penting
Emoji tidak dihapus, melainkan dikonversi ke teks emosional (misal: 😂 → [tertawa]) untuk mempertahankan informasi sentimen.
Slang bahasa gaul Indonesia dinormalisasi menggunakan kamus eksternal (indo_slang_new.csv).
Dataset berisi 1.815 tweet dengan distribusi sentimen yang seimbang (~33% per kelas).
📎 Referensi
Dataset: Google Drive
IndoBERT: Hugging Face - indobenchmark/indobert-base-p1
Library Sastrawi: https://github.com/sastrawi/sastrawi



---

### ✅ Langkah Selanjutnya:
1. Simpan teks di atas sebagai `README.md` di **root folder** proyek Anda.
2. Pastikan file `requirements.txt` sudah ada (jika belum, buat dengan `pip freeze > requirements.txt`).
3. Lakukan **commit & push** ke GitHub:

```bash
git add .
git commit -m "feat: add README and project structure"
git push origin main