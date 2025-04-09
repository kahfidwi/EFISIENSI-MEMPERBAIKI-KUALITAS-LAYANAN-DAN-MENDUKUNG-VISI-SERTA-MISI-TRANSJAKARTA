# EFISIENSI MEMPERBAIKI KUALITAS LAYANAN DAN MENDUKUNG VISI SERTA MISI TRANSJAKARTA

## Latar Belakang
Sebuah perusahaan yang bergerak di bidang transportasi milik pemerintah daerah yakni TransJakarta, ingin merekrut data analis. Perusahaan ini ingin meningkatkan efisiensi, memperbaiki kualitas layanan, dan mendukung visi serta misinya dalam menyediakan transportasi yang memudahkan dan membahagiakan warga Jakarta. 
Untuk mencapai hal ini, analisis data perjalanan dan transaksi pengguna menjadi kunci. Data seperti rute, pemberhentian, waktu perjalanan, dan profil penumpang dapat memberikan wawasan mendalam terkait kebutuhan penumpang, pola perjalanan, serta efisiensi rute. Dengan menganalisis data tersebut, TransJakarta dapat mengoptimalkan efisiensi, memperbaiki kualitas layanan, dan mendukung visi serta misinya dalam menyediakan transportasi yang memudahkan dan membahagiakan warga Jakarta.

## Rumusan Masalah
Meskipun TransJakarta telah menjadi tulang punggung transportasi publik di Jakarta, masih terdapat berbagai tantangan dalam menyediakan layanan yang efektif, efisien, dan memuaskan bagi semua pengguna. Seiring dengan meningkatnya jumlah penumpang dan perluasan jaringan rute, TransJakarta perlu mengoptimalkan operasionalnya untuk memenuhi kebutuhan mobilitas masyarakat dengan lebih baik. 
Oleh karena itu, diperlukan analisis data yang lebih mendalam untuk efisiensi, memperbaiki kualitas layanan, dan mendukung visi serta misinya dalam menyediakan transportasi yang memudahkan dan membahagiakan warga Jakarta.

## Tujuan Analisis
- Efisiensi, memperbaiki kualitas layanan, dan mendukung visi serta misinya dalam menyediakan transportasi yang memudahkan dan membahagiakan warga Jakarta dengan:
- Meningkatkan efisiensi dengan penjadwalan dinamis berdasarkan waktu sibuk dan jalur prioritas
- Memperbaiki kualitas layanan dengan menjamin kenyamanan dan keamanan penumpang wanita dan menyesuaikan fasilitas Halte TransJakarta.
- Memudahkan dan membahagiakan warga Jakarta disesuaikan berdasarkan usia penumpang dan biaya TransJakarta.

## Kondisi Data
- Dataset transjakarta memiliki 22 kolom dan 37.900 baris
- Beberapa kolom, yaitu, `corridorID`, `corridorName`, `tapInStops`, `tapOutStops`, `tapOutStopsName`, `tapOutStopsLat`, `tapOutStopsLon`, `stopEndSeq`, `tapOutTime` dan `payAmount` memiliki data kosong. Data kosong pada kolom-kolom tersebut diwakili dengan data NaN.
- Kolom `transID` berisikan id unik untuk tiap penumpang transjakarta, sehingga penumpang akan mendapatkan transID baru setiap menaiki tranjakarta yang pertama atau yang kesekian kalinya.
- Kolom `payCardID` dan `stopEndSeq` memiliki data tipe numerik. Dari penjelasannya, kolom ini seharusnya berisikan data object dengan tujuan agar bisa dianalisis sebagai primary key atau foreign key.
- Kolom `payCardBirthDate`, `tapInTime`, `tapOutTime` memiliki data tipe object. Dari penjelasannya, kolom ini seharusnya berisikan data datetime dengan tujuan agar bisa dianalisis sebagai patokan waktu.
- Kolom `tapOutStopsName`, `tapOutStopsLat`, `tapOutStopsLon`, `stopEndSeq`, `tapOutTime` memiliki data kosong yang jumlahnya sama diperkirakan bahwa data dengan kosong dalam kolom tersebut adalah data yang sama jadi bisa dihapuskan nilai/value yang kosong.
Untuk pengertian tiap kolom bisa dilihat di link dibawah:
https://docs.google.com/document/d/1e-Q6S2RviDPrio6KCKA2EFg_54q51j036dp3pnwtTuw/edit?tab=t.0

## Kesimpulan
- Perilaku Penumpang Berdasarkan Waktu
Jam paling sibuk terjadi pada pagi hari (05:00–07:00) dan sore hari (16:00–18:00).
Ini berlaku untuk seluruh jenis layanan (BRT, Non-BRT, Mikrotrans, Royaltrans) dan konsisten pada semua kelompok usia dan gender.

- Koridor Prioritas
Koridor 9D (Pasar Minggu - Tanah Abang) dan JAK.36 (Cilangkap - Cililitan) merupakan koridor dengan volume tertinggi pada pagi dan sore hari.
Koridor lain seperti 2E(Rusun Rawa Bebek - Kodamar), 8C(Kebayoran Lama - Tanah Abang), 1T (Cibubur - Balai Kota), JAK.06(Kampung Rambutan - Pondok Gede), dan S21(Ciputat - CSW) juga menunjukkan aktivitas tinggi dan dapat dikategorikan sebagai koridor sekunder prioritas.

- Segmentasi Berdasarkan Usia dan Gender
Usia 25–40 tahun adalah kelompok penumpang terbesar (45,8%), diikuti oleh usia <25 tahun (28,3%) dan >40 tahun (26%).
Perempuan menunjukkan volume signifikan, terutama di titik-titik seperti Penjaringan, Tendean, Tanah Abang, Bundaran Senayan, dan Terminal Senen pada jam 06:00 dan 17:00–18:00.

- Pola Titik Naik dan Turun
Titik tap-in populer: Garuda Taman Mini, SMKN 56, Penjaringan, Grand Sahid.
Titik tap-out populer: BKN, Bundaran Senayan, Tendean, Terminal Senen, JPO Blok G.
Titik-titik ini menunjukkan keterkaitan antara permukiman, perkantoran, pendidikan, dan terminal transit.

## Rekomendasi
- Peningkatan Efisiensi Operasional
Terapkan penjadwalan dinamis berdasarkan waktu sibuk dan jalur prioritas.
Fokus penambahan armada di jam 05:00–07:00 dan 16:00–18:00 untuk koridor seperti 9D(Pasar Minggu - Tanah Abang), JAK.36 (Cilangkap - Cililitan) , dan 2E(Rusun Rawa Bebek - Kodamar).

- Penguatan Mikrotrans dan Non-BRT
Karena banyak perjalanan berasal dari layanan feeder dan non-BRT, perluasan dan peningkatan kualitas Mikrotrans dan Non-BRT akan meningkatkan aksesibilitas dan kenyamanan.

- Layanan Ramah Gender
Titik-titik seperti Penjaringan, GBK, dan Tendean perlu pencahayaan, CCTV, dan fasilitas keamanan tambahan, terutama di sore dan malam hari.
Perluas inisiatif “Zona Aman Perempuan” di halte dan dalam armada diseluruh halte.

- Segmentasi Layanan Berdasarkan Usia
<25 tahun: Program "Transjakarta Goes to School/University", kerjasama dengan Dinas Pendidikan.
25–40 tahun: Paket langganan commuter, integrasi layanan kerja (kantor/kawasan industri).
>40 tahun: Fasilitas halte ramah lansia, sosialisasi hak prioritas, dan integrasi dengan layanan kesehatan/jemputan lansia.

