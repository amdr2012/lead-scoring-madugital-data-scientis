# lead-scoring-madugital-data-scientis
Mini Project Lead Scoring Machine Learning using Random Forest

# Lead Scoring Prediction - Madugital

Proyek *Machine Learning* untuk memprediksi potensi konversi pelanggan (*lead scoring*) berdasarkan kebiasaan kunjungan website dan profil interaksi, guna membantu tim sales memprioritaskan prospek terbaik.

## 🚀 Alur Kerja Proyek (Workflow):
1. **Data Preparation & Cleaning:** Menyiapkan dataset dan membersihkan data dari nilai yang tidak valid.
2. **Preprocessing:** 
   - Melakukan pembagian data **Train-Test Split (80:20)** dengan parameter `stratify=y` untuk menjaga keseimbangan rasio kelas target.
   - Menyamakan skala fitur numerik menggunakan **StandardScaler** (mencegah *data leakage* dengan melakukan *fit* hanya pada data latihan).
3. **Model Training:** Menggunakan algoritma **Random Forest Classifier** (`n_estimators=100`, `random_state=42`) sebagai pendekatan berbasis ensambel (*decision tree voting*) untuk mengenali pola konversi pelanggan.
4. **Prediction & Ranking:** Menghasilkan probabilitas konversi (`predict_proba`) untuk mengurutkan daftar *lead* paling potensial yang harus segera dihubungi.

## 🛠️ Teknologi yang Digunakan:
* Python
* Pandas & NumPy
* Scikit-Learn (StandardScaler, RandomForestClassifier, Train-Test Split)
* Google Colab
