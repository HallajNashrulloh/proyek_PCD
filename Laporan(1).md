Pengolahan CItra DIgital :

# Deteksi Penyakit Hati/Liver dengan Segmentasi Image Processing 

## **1. Domain Proyek**
Penyakit hati merupakan salah satu masalah kesehatan utama di dunia yang dapat memicu komplikasi serius seperti:
- **Sirosis hati** yang merupakan jaringan perut pada hati akibat kerusakan kronis, menyebabkan gangguan fungsi hati.
- **Hepatitis Kronis** yang disebabkan oleh infeksi virus atau konsumsi alkohol berlebihan, yang dapat berkembang menjadi siroris atau kanker hati.
- **Kanker Hati** ini yang sering kali terdeteksi pada tahap lanjut, sehingga sulit untuk diobati dengan sukses.

dan menurut data **World Health Organization (2022),** penyakit hati menyumbangkan sekitar 2 juta kematian setiap tahun secara global, dengan peningkatan kasus di berbagai negara-negara berkembang akibat terbatasnya akses ke layanan kesehatan.


---

## **2. Peran Segmentasi Image Processing dalam Deteksi Penyakit Hati/Liver**
Segmentasi image processing dapat :
- mengidentifikasi area yang terkena berdasarkan citra medis seperti CT scan dan MRI.
- Mendeteksi anomali yang ada pada jaringan hati yang mungkin untuk menunjukan indikasi penyakit.
- mengukur volume hati dan area yang terkena penyakit dan untuk membantu analisis progresivitas kondisi pasien.


Menurut penelitian Smith, Johnson, % Lee (2021), penerapan segmentasi image processing dapat :
1. Membantu identifikasi awal kerusakan hati dengan lebih efisien.
2. Mendukung intervensi medis lebih cepat.
3. Mengurangi kesalahan dalam interpretasi manual citra medis.

---

## **3. Manfaat Proyek**

- **Kecepatan**: Mempercepat proses identifikasi risiko penyakit hati.
- **Akurasi**: Mengurangi potensi kesalahan dalam interpretasi manusia.
- 
- 

---

## **4. Referensi**
1. Smith, J., Johnson, R., % Lee, M. (2021). *Image Processing for Early Detection of Liver Diseases.*
2. World Health Organization. (2022). *Global Report on Liver Desease*.

---

## **5. Percobaan yang dilakukan**
- pada percobaan pertama kurang tepat untuk mendeteksi area yang terjangkit sehingga anomali yang terbaca kurang tepat dan malah menandai seluruh gambar yang ada.
- setelah dilakukan beberapa percobaan hasil deteksi area mulai mendekati kemungkinan tetapi masih perlu memperbaiki kode yang ada.

## **6. Percobaan yang dilakukan**
Proyek ini bertujuan untuk menganalisis gambar medis dengan fokus pada segmentasi dan deteksi area tertentu dalam organ hati. Segmentasi citra medis merupakan langkah penting dalam diagnosis berbasis komputer (CAD), yang membantu mengidentifikasi struktur atau anomali dengan cepat dan akurat. Dengan menggunakan teknik pemrosesan citra seperti adaptive thresholding, morfologi, dan deteksi kontur, proyek ini menawarkan pendekatan semi-otomatis untuk mendeteksi area yang mencurigakan pada gambar hati.

Aplikasi utama dari metode ini meliputi:
- Membantu radiolog dalam menganalisis citra medis.
- Mendeteksi dan memantau penyakit hati seperti tumor atau kista.
- Memberikan dasar untuk pengembangan sistem CAD lebih lanjut.

Metodologi

Metodologi yang digunakan dalam proyek ini mencakup beberapa tahapan berikut:

1. Pengumpulan Data: Gambar input diimpor dalam format digital menggunakan pustaka OpenCV. Citra input harus berupa citra medis hati yang relevan.
2. Preprocessing Gambar:
   - Konversi gambar ke skala abu-abu (grayscale).
   - Equalisasi histogram untuk meningkatkan kontras.
   - Gaussian blur untuk mengurangi noise dan artefak.

3. Segmentasi Hati:
   - Menggunakan adaptive thresholding (Gaussian) untuk membedakan area hati dari latar belakang.
   - Operasi morfologi (closing) untuk menghilangkan noise kecil dan menyempurnakan batas area hati.

4. Ekstraksi dan Deteksi Anomali:
   - Deteksi kontur area hati yang tersegmentasi.
   - Memfilter area kecil yang tidak signifikan untuk menghindari deteksi palsu.
   - Menyoroti area mencurigakan pada gambar asli dengan kontur berwarna.

5. Visualisasi Hasil: Menampilkan gambar input, hasil preprocessing, segmentasi, dan deteksi pada satu kanvas menggunakan Matplotlib untuk evaluasi.

6. Evaluasi: Menilai hasil segmentasi dan deteksi dengan membandingkannya terhadap ground truth jika tersedia.

Dengan pendekatan ini, proyek diharapkan dapat memberikan hasil segmentasi dan deteksi yang dapat digunakan sebagai langkah awal dalam diagnosis berbasis komputer. Pustaka utama yang digunakan meliputi OpenCV untuk pemrosesan gambar dan Matplotlib untuk visualisasi.

