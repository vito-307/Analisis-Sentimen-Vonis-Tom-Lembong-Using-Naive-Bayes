# Analisis Sentimen Publik Terhadap Vonis Tom Lembong di Twitter
Proyek ini bertujuan untuk menganalisis sentimen warganet di platform Twitter mengenai kasus vonis Bapak Tom Lembong. Analisis ini menggunakan pemodelan Machine Learning dengan algoritma Naive Bayes untuk mengklasifikasikan opini publik ke dalam sentimen positif, negatif, atau netral.

# 📜 Deskripsi Proyek
Kasus hukum yang melibatkan tokoh publik seringkali memicu diskusi yang luas di media sosial. Proyek ini mencoba memotret dan memahami bagaimana opini publik terbentuk di Twitter terkait vonis Tom Lembong melalui pendekatan Natural Language Processing (NLP) dan machine learning.

# 🛠️ Alur Kerja Proyek
Proses analisis dalam proyek ini melalui beberapa tahapan utama:

Pengumpulan Data: Data tweet dikumpulkan dari Twitter menggunakan token autentikasi akun pribadi. Kata kunci yang digunakan antara lain "Tom Lembong", "vonis Lembong", dan kata kunci relevan lainnya.

Pra-pemrosesan Teks (Preprocessing): Teks tweet dibersihkan dari noise seperti URL, username (@), dan karakter yang tidak perlu. Dilakukan juga proses normalisasi kata tidak baku (slang) dan case folding (mengubah semua huruf menjadi kecil).

Feature Engineering: Teks yang sudah bersih diubah menjadi representasi numerik (vektor) menggunakan metode TF-IDF (Term Frequency-Inverse Document Frequency) agar dapat diproses oleh model.

Pemodelan (Modeling): Model klasifikasi Naive Bayes dilatih untuk mempelajari pola dari data teks dan mengklasifikasikan sentimennya.

Evaluasi Model: Kinerja model dievaluasi menggunakan skema 5-Fold Cross-Validation untuk mendapatkan ukuran performa yang stabil dan dapat diandalkan.

# 📊 Hasil Analisis
Distribusi Sentimen
Berdasarkan analisis terhadap 371 tweet, ditemukan bahwa sentimen warganet cenderung terbagi sebagai berikut:

Neutral: 54.1%

Negative: 31.4%

Positive: 14.5%

Mayoritas sentimen bersifat Netral, yang umumnya berisi penyampaian ulang berita dari media atau pertanyaan mengenai kasus. Sentimen Negatif banyak berisi kritik dan ketidaksetujuan, sementara sentimen Positif berisi dukungan.

<img width="761" height="559" alt="image" src="https://github.com/user-attachments/assets/c01f157d-72c7-4937-9688-a1766e18e7db" />

# 🛠️ Kinerja Model
Model Naive Bayes yang dibangun untuk klasifikasi sentimen ini mencapai kinerja (Accuracy) rata-rata sebesar 66% dari hasil 5-Fold Cross-Validation.

# ⚠️ Keterbatasan (Limitation)
Perlu dicatat bahwa kinerja model belum dapat dikatakan optimal. Skor 66% menunjukkan bahwa model sudah mampu mengenali pola sentimen, namun masih memiliki ruang besar untuk perbaikan.

Faktor utama yang memengaruhi hal ini adalah jumlah dataset yang terbatas (hanya 371 record). Dalam machine learning, kuantitas dan kualitas data sangat berpengaruh terhadap kemampuan model untuk belajar dan melakukan generalisasi. Dengan dataset yang lebih besar, performa model diharapkan dapat meningkat secara signifikan.
