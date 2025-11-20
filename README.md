# 🚌 Analisis Pola Penumpang Transjakarta untuk Optimalisasi Layanan Akhir Pekan

## 1\. Project Overview

Proyek ini menganalisis data transaksi *tap-in* Transjakarta untuk mengidentifikasi pola pergerakan penumpang, dengan fokus khusus pada Koridor dengan volume tertinggi dan terendah saat **Akhir Pekan** (*Weekend*).

**Problem Statement:** Optimalisasi alokasi armada dan penjadwalan layanan untuk memenuhi permintaan penumpang secara efisien, terutama untuk Koridor kritis pada hari Sabtu dan Minggu.

**Key Objectives:**

1.  **Membersihkan, memformat, dan menghapus duplikasi** data transaksi Transjakarta.
2.  **Membangun fitur** untuk mengidentifikasi transaksi yang terjadi pada **akhir pekan** (`akhir_pekan`).
3.  **Mengidentifikasi** Top 5 dan Bottom 5 Koridor berdasarkan volume penumpang di akhir pekan.
4.  **Menyajikan *insight* yang *actionable*** melalui visualisasi interaktif di Tableau.

-----

## 2\. Data Sources

| Dataset | Deskripsi | Ukuran/Periode |
| :--- | :--- | :--- |
| **`Transjakarta.csv`** | Data transaksi *tap-in* yang mencakup ID transaksi (`transID`), waktu *tap-in* (`tapInTime`), koridor (`corridorName`), dan jumlah tarif yang dibayarkan (`payAmount`). | \[Sebutkan jumlah baris atau periode data, misal: Data Transaksi April 2023\] |

-----

## 3\. Technologies Used

  * **Programming Language:** Python (Pandas untuk Data Cleaning dan Feature Engineering)
  * **Visualization:** Matplotlib (untuk EDA), Tableau (untuk Dashboard interaktif)
  * **Interactive Dashboard:** Tableau Public
  * **Version Control:** Git & GitHub
  * **Environment:** Jupyter Notebook

-----

## 4\. Project Structure

Struktur direktori proyek yang direkomendasikan:

```
├── README.md                               <- File dokumentasi ini.
├── data
│   ├── raw                                 <- File mentah: Transjakarta.csv
│   └── cleaned                             <- Data setelah dibersihkan (opsional)
│
├── notebooks                               <- File Jupyter Notebook (.ipynb) berisi kode:
│   └── 1.0-Data-Cleaning-FE-EDA.ipynb
│
├── reports
│   ├── slide                               <- File Presentasi (Link: [Masukkan link Slide Presentasi Anda])
│   └── figures                             <- Gambar atau grafik yang diekstrak.
│
└── Ridership & Weekend Optimization.twbx    <- File Tableau Workbook.
```

-----

## 5\. Summary of Finding

### 5.1 Business Insight

Berdasarkan analisis Koridor Top N dan Bottom N pada saat *weekend*:

  * **Top 5 Koridor:** Koridor-koridor ini secara kolektif menyumbang \[**Masukkan Persentase**\] total penumpang di akhir pekan, menunjukkan adanya kebutuhan fokus operasional di titik-titik ini.
  * **Perbandingan Layanan:** Layanan **\[Sebutkan Layanan Paling Dominan\]** mendominasi volume penumpang, mengindikasikan bahwa \[**Sebutkan hasil: layanan utama (Rp 3500) adalah *revenue generator* terbesar, atau Mikrotrans (Rp 0) adalah layanan penting untuk *feeder***\].
  * **Kesenjangan Kinerja:** Kesenjangan volume antara Koridor teratas dan terbawah mencapai sekitar \[**Masukkan Angka Kesenjangan**\] transaksi.

### 5.2 Actionable Recommendation

1.  **Optimalisasi Jadwal (Top 5):** Merekomendasikan **penambahan frekuensi** bus pada Top 5 Koridor di luar jam sibuk *weekend* untuk menjaga kualitas layanan.
2.  **Evaluasi Ulang (Bottom 5):** Lakukan **studi mendalam** terhadap Bottom 5 Koridor untuk mempertimbangkan penggabungan rute, pengurangan jadwal, atau kampanye pemasaran di area tersebut.
3.  **Peningkatan Data:** Perlu adanya pengumpulan data *tap-out* yang lebih lengkap untuk analisis *load factor* dan kepadatan bus yang lebih akurat.

-----

## 6\. Contact

  * **Name:** Fahrezy Maulana Haz
  * **Email:** farez007100@gmail.com
  * **LinkedIn:** [linkedin.com/in/fahrezy-maulana-haz](https://www.google.com/search?q=https://linkedin.com/in/fahrezy-maulana-haz)
