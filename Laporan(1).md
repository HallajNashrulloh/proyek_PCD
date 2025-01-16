Pengolahan CItra DIgital :

# Deteksi Penyakit Hati/Liver dengan Segmentasi Image Processing 

## **1. Pendahuluan**
Hati (liver) merupakan salah satu organ vital dalam tubuh manusia yang berperan penting dalam metabolisme, detoksifikasi, dan penyimpanan nutrisi. Gangguan pada hati, seperti hepatitis, sirosis, dan kanker hati, dapat berdampak serius terhadap kesehatan dan bahkan berujung pada komplikasi fatal jika tidak terdeteksi dan ditangani sejak dini. Oleh karena itu, deteksi dini penyakit hati menjadi krusial dalam upaya pencegahan dan pengobatan yang efektif.  

Dalam bidang medis, teknologi pencitraan telah menjadi alat utama dalam mendiagnosis berbagai penyakit hati. Beberapa teknik pencitraan medis yang umum digunakan meliputi ultrasonografi (USG), computed tomography (CT), dan magnetic resonance imaging (MRI). Namun, interpretasi gambar medis secara manual oleh tenaga medis sering kali membutuhkan waktu yang lama dan dapat menghasilkan variasi subjektif antar-pemeriksa. Untuk meningkatkan akurasi dan efisiensi dalam deteksi penyakit hati, pendekatan berbasis image processing dan segmentasi citra telah dikembangkan.  

Segmentasi citra dalam pemrosesan gambar medis bertujuan untuk memisahkan area tertentu dari gambar, seperti jaringan hati, guna mengidentifikasi kelainan dengan lebih akurat. Teknik ini memanfaatkan algoritma komputasi untuk mengekstraksi fitur penting dari gambar medis, sehingga dapat membantu dalam mendeteksi adanya lesi, fibrosis, atau perubahan morfologi pada hati. Berbagai metode segmentasi telah dikembangkan, termasuk teknik berbasis ambang batas (thresholding), region growing, edge detection, serta pendekatan berbasis kecerdasan buatan seperti deep learning.  

Dengan kemajuan teknologi image processing, deteksi penyakit hati dapat dilakukan secara lebih cepat, akurat, dan objektif. Hal ini berpotensi meningkatkan kualitas diagnosis serta mendukung pengambilan keputusan medis yang lebih baik. Oleh karena itu, penelitian dan pengembangan dalam bidang segmentasi citra untuk deteksi penyakit hati menjadi aspek yang sangat penting dalam inovasi medis modern.

dan menurut data **World Health Organization (2022),** penyakit hati menyumbangkan sekitar 2 juta kematian setiap tahun secara global, dengan peningkatan kasus di berbagai negara-negara berkembang akibat terbatasnya akses ke layanan kesehatan.

Proyek ini bertujuan untuk menganalisis gambar medis dengan fokus pada segmentasi dan deteksi area tertentu dalam organ hati. Segmentasi citra medis merupakan langkah penting dalam diagnosis berbasis komputer (CAD), yang membantu mengidentifikasi struktur atau anomali dengan cepat dan akurat. Dengan menggunakan teknik pemrosesan citra seperti adaptive thresholding, morfologi, dan deteksi kontur, proyek ini menawarkan pendekatan semi-otomatis untuk mendeteksi area yang mencurigakan pada gambar hati.

## **2. Metodologi**

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



---

## **3. Hasil**

## **4. Kesimpulan**

## **4. Peran Segmentasi Image Processing dalam Deteksi Penyakit Hati/Liver**
Segmentasi image processing dapat :
- mengidentifikasi area yang terkena berdasarkan citra medis seperti CT scan dan MRI.
- Mendeteksi anomali yang ada pada jaringan hati yang mungkin untuk menunjukan indikasi penyakit.
- mengukur volume hati dan area yang terkena penyakit dan untuk membantu analisis progresivitas kondisi pasien.


Menurut penelitian Smith, Johnson, % Lee (2021), penerapan segmentasi image processing dapat :
1. Membantu identifikasi awal kerusakan hati dengan lebih efisien.
2. Mendukung intervensi medis lebih cepat.
3. Mengurangi kesalahan dalam interpretasi manual citra medis.

---

## **4. Manfaat Proyek**

- **Kecepatan**: Mempercepat proses identifikasi risiko penyakit hati.
- **Akurasi**: Mengurangi potensi kesalahan dalam interpretasi manusia.
- 
- 

---

## **5. Referensi**
1. Smith, J., Johnson, R., % Lee, M. (2021). *Image Processing for Early Detection of Liver Diseases.*
2. World Health Organization. (2022). *Global Report on Liver Desease*.

---

## **5. Percobaan yang dilakukan**
- pada percobaan pertama kurang tepat untuk mendeteksi area yang terjangkit sehingga anomali yang terbaca kurang tepat dan malah menandai seluruh gambar yang ada.
- setelah dilakukan beberapa percobaan hasil deteksi area mulai mendekati kemungkinan tetapi masih perlu memperbaiki kode yang ada.

---
Nama : Muhammad Hallaj Nashrulloh
---
NIM : 2206031
