# Executive Performance Dashboard: Service Unit Analysis & Customer Segmentation

## 📌 Project Overview
Proyek ini mengimplementasikan **Dashboard Analisis Kinerja Operasional dan Segmentasi Pelanggan** yang dirancang untuk memonitor, mengevaluasi, dan mengoptimalkan produktivitas unit servis (bengkel) serta strategi retensi pelanggan. Menggunakan pendekatan berbasis data (*data-driven approach*), dashboard ini memberikan visibilitas penuh terhadap metrik utama seperti *Unit Entry*, pencapaian target kerja (*CPUS*), komposisi jenis pekerjaan, hingga segmentasi perilaku pelanggan (*Effort, Inisiatif, New*).

![Executive Dashboard](Executive%20Dashboard.png)

Melalui visualisasi yang interaktif dan komprehensif, manajemen dapat mengidentifikasi bottleneck operasional, mengukur efektivitas program loyalitas (seperti *TCare*), dan merumuskan strategi pemasaran yang lebih presisi untuk meningkatkan *revenue* bisnis *aftersales*.

---

## 🎯 Project Objectives (Tujuan Proyek)
1. **Operasional Efisiensi:** Memantau volume kendaraan yang masuk (*Unit Entry*) dan tingkat utilitas kapasitas servis (*CPUS vs Non-CPUS*) secara real-time vs target perusahaan.
2. **Optimalisasi Produktivitas Mekanik:** Menganalisis komposisi jenis pekerjaan (SBE, GR, TWC, SBI, RTJ) untuk mengoptimalkan alokasi *manpower* dan *stall utilization*.
3. **Peningkatan Retensi Pelanggan:** Mengklasifikasikan basis pelanggan berdasarkan kategori interaksi (*Effort, Inisiatif, New*) serta status keikutsertaan program *TCare* untuk menekan angka *churn rate*.
4. **Strategi Pemasaran Tersegmentasi:** Mengidentifikasi kelompok data potensial (seperti kategori *Next* dan *Late Service*) untuk kampanye *re-call* atau promosi servis yang lebih tertarget.

---

## 📊 Detailed Dashboard Breakdown & Section Analysis

### 1. Main KPI Blocks: Unit Entry & CPUS
* **Komponen:**
    * **Unit Entry:** Mencapai **10.252 unit** (91,2% dari Target Astrido Unit Entry sebesar 11.239).
    * **CPUS (Capacity Productive Unit Service):** Mencapai **8.951 unit** (92,2% dari Target Astrido CPUS sebesar 9.713, atau 126,1% dari Target TAM CPUS).
    * **Non-CPUS:** Sebesar **1.301 unit**.
* **Penjelasan Teknikal:** Bagian ini berfungsi sebagai *high-level health indicator* dari volume bisnis. Rasio CPUS yang tinggi (87,3% dari total *Unit Entry*) menandakan mayoritas kendaraan yang masuk berkontribusi langsung pada produktivitas bengkel utama.

### 2. Komposisi Jenis Pekerjaan (Job Type Composition)
* **Komponen:** Analisis volume berdasarkan jenis pekerjaan:
    * **SBE (Service Body & Paint / Express):** 6.764 unit (89,6% dari Target).
    * **GR (General Repair):** 2.187 unit (100,8% dari Target - *Exceeded*).
    * **TWC (Two Wheel / Quick Service):** 900 unit.
    * **SBI & RTJ:** Kontribusi minoritas (395 dan 6 unit).
* **Penjelasan Teknikal:** Grafik batang ini memecah beban kerja bengkel. Keberhasilan GR menembus target (100,8%) menunjukkan performa tim teknikal yang solid pada perbaikan berat, sementara SBE tetap menjadi volume driver terbesar.

### 3. Komposisi TCare & Tipe Pelanggan (Loyalty & Customer Fleet Profile)
* **Komponen:** * **Proporsi TCare:** Didominasi oleh **Non-TCare (87,7%)** dibandingkan **TCare (12,3%)**.
    * **Tipe Pelanggan:** Mayoritas adalah **Retail (80,6%)**, sedangkan **Fleet** berkontribusi **19,4%**.
    * **Matriks TCare vs Fleet/Retail:** Visualisasi bertingkat (*stacked bar chart*) memperlihatkan distribusi pelanggan Retail dan Fleet di dalam segmen TCare dan Non-TCare. Pelanggan Retail mendominasi kedua kategori tersebut secara masif (7.147 di Non-TCare dan 1.115 di TCare).

### 4. Komposisi Kategori Customer (Customer Engagement Behavior)
* **Komponen:** Segmentasi perilaku pelanggan yang dibagi menjadi tiga kategori utama:
    * **Effort:** Pelanggan yang membutuhkan tindak lanjut/edukasi intensif (Dominan di segmen Non-TCare sebesar 4.512 unit).
    * **Inisiatif:** Pelanggan proaktif yang melakukan servis atas kesadaran sendiri (3.356 di Non-TCare, sangat kecil di TCare).
    * **New:** Pelanggan baru yang berhasil diakuisisi (1.126 di Non-TCare).
* **Penjelasan Teknikal:** Grafik ini memberikan sinyal penting bagi CRM (*Customer Relationship Management*). Tingginya angka segmen *Effort* di kelompok Non-TCare menandakan perlunya otomatisasi pengingat servis (misalnya via WhatsApp API atau telemarketing).

### 5. Komposisi Tipe Data (Funneling & Follow-Up Priority)
* **Komponen:** Distribusi database pelanggan berdasarkan status *lifecycle* mereka:
    * **Non Utilisasi (3.931):** Data pelanggan yang belum dioptimalkan.
    * **Next (2.693):** Target utama untuk prospek servis berikutnya.
    * **Late Service (1.908):** Pelanggan yang terlambat melakukan servis berkala (risiko *churn*).
    * **TCare (1.258) & First (233):** Pelanggan dalam program berkala dan servis pertama.

---

## 📈 Business Impact & Value Proposition (Dampak & Nilai Bisnis)

Dengan mengintegrasikan dashboard ini ke dalam sistem manajemen bengkel, perusahaan dapat mentransformasi data mentah menjadi keputusan strategis yang berdampak langsung pada:

* **Peningkatan Revenue Aftersales:** Dengan memetakan **1.908 pelanggan Late Service** dan **2.693 data Next**, tim marketing dapat meluncurkan kampanye *pemberian insentif/diskon khusus* secara presisi untuk menarik mereka kembali ke bengkel, langsung mengonversi data menjadi *Unit Entry*.
* **Efisiensi Biaya Operasional (Opex):** Manajemen dapat menyesuaikan jumlah mekanik dan ketersediaan suku cadang (*spare parts*) berdasarkan tren *Komposisi Jenis Pekerjaan*. Kelebihan kapasitas pada lini yang underperform dapat dialihkan untuk mendukung lini *General Repair (GR)* yang sedang mengalami lonjakan permintaan (100,8% target).
* **Peningkatan Customer Retention Rate:** Visualisasi ini membantu tim CRM melacak efektivitas konversi *TCare*. Rendahnya angka TCare saat ini (12,3%) menjadi dasar pembuatan strategi *cross-selling* saat penyerahan unit baru (*New Car Delivery*) agar loyalitas pelanggan jangka panjang meningkat.
* **Data-Driven Decision Making untuk Ekspansi:** Profiling pelanggan *Retail vs Fleet* memberikan arah strategis yang jelas bagi manajemen jika ingin membuka cabang baru atau memperluas layanan khusus korporasi (*Fleet service contract*).

---

## 🛠️ Tech Stack & Tools Used
* **Data Analytics & Visualization:** Google Looker Studio / Power BI
* **Data Warehouse / Backend:** Google Sheets / BigQuery / SQL Server
* **Data Integration:** Google Apps Script / ETL Pipeline

---
💡 *Dashboard ini merupakan bagian dari portofolio profesional saya dalam bidang Data Analytics, Project Management, dan Aftersales Business Strategy di industri otomotif.*
