# Tugas 

**1.Jelaskan Struktur Antar Hubungan dan Beri Contohnya?**

Struktur Antar Hubungan
Struktur antar hubungan adalah pola keterkaitan atau keterhubungan antara berbagai elemen dalam suatu sistem, organisasi, atau kelompok sosial. Hubungan ini dapat bersifat hierarkis, fungsional, atau timbal balik, tergantung pada konteksnya.

**Contoh Struktur Antar Hubungan**

1.Dalam Organisasi Perusahaan

**Hierarkis:** CEO → Manajer → Supervisor → Karyawan

**Fungsional:** Departemen Produksi berhubungan dengan Departemen Pemasaran untuk memastikan produk yang dibuat sesuai dengan kebutuhan pasar.

2.Dalam Ekosistem

Hubungan antara produsen (tumbuhan), konsumen pertama (herbivora), dan konsumen kedua (karnivora).

3.Dalam Masyarakat

Hubungan antara pemerintah dan rakyat dalam bentuk kebijakan yang dibuat dan implementasinya terhadap kesejahteraan masyarakat.

**Sumber**

Soekanto, S. (2009). Sosiologi Suatu Pengantar. Jakarta: Rajawali Pers.

**2.Bila terlalu banyak modul atau perangkat dihubungkan pada bus maka akan terjadi penurunan kinerja, sebutkan penyebabnya?**

Penurunan kinerja pada bus ketika terlalu banyak modul atau perangkat dihubungkan disebabkan oleh beberapa faktor, antara lain:

**1.Kontensi (Contention) Bus**

Banyak perangkat yang mencoba mengakses bus secara bersamaan dapat menyebabkan kemacetan, sehingga perangkat harus menunggu giliran untuk mentransmisikan data.

**2.Waktu Propagasi (Propagation Delay)**

Semakin banyak perangkat yang terhubung, semakin panjang jalur komunikasi, sehingga waktu yang dibutuhkan untuk mengirim dan menerima data meningkat.

**3.Penurunan Bandwidth Efektif**

Kapasitas bus terbatas, dan semakin banyak perangkat yang menggunakannya, semakin kecil bagian bandwidth yang tersedia untuk masing-masing perangkat.

**4.Meningkatnya Waktu Akses**

Karena bus bersifat berbagi (shared), perangkat harus menunggu akses yang lebih lama ketika jumlah perangkat meningkat, menyebabkan latensi yang lebih tinggi.

**Sumber**
Stallings, W. (2017). Computer Organization and Architecture. Pearson.

**3.Umumnya perangkat berprioritas paling rendah memiliki waktu tunggu rata-rata yang paling singkat. Dengan dasar ini biasanya CPU diberi perioritas tertinggi pada SBI. Sebutkan alasan perangkat berprioritas 16 memiliki waktu tunggu rata-rata paling rendah? Dibawah kondisi seperti apa keadaan diatas tidak berlaku?**
   
**Alasan Perangkat Berprioritas 16 Memiliki Waktu Tunggu Rata-Rata Paling Rendah**

Dalam sistem bus terstruktur seperti **Synchronous Bus Interconnect (SBI)**, perangkat dengan prioritas lebih rendah sering kali memiliki waktu tunggu rata-rata lebih singkat karena mekanisme penjadwalan **round-robin** atau **fair queuing**. Berikut adalah alasannya:

**1.Intervensi Lebih Jarang**

-Perangkat dengan prioritas lebih tinggi sering kali memiliki waktu pemrosesan yang lebih lama atau frekuensi permintaan yang lebih tinggi, sehingga bisa mengalami antrean lebih panjang.

-Sebaliknya, perangkat dengan prioritas lebih rendah (misalnya prioritas 16) biasanya memiliki jumlah permintaan lebih sedikit, sehingga dapat diproses lebih cepat dalam sistem yang berbasis fair queuing.

**2.Distribusi Akses yang Merata**

-Jika sistem menerapkan penjadwalan berbasis rotasi, maka setiap perangkat akan mendapat giliran akses yang hampir sama, mengurangi kemungkinan perangkat berprioritas rendah mengalami antrean panjang.

**Kondisi di Mana Keadaan Ini Tidak Berlaku**

**1.Sistem dengan Skema Prioritas Ketat (Strict Priority Scheduling)**

-Jika sistem menerapkan skema prioritas ketat, perangkat dengan prioritas lebih tinggi akan selalu mendapatkan akses lebih dulu, menyebabkan perangkat dengan prioritas lebih rendah mengalami kelaparan sumber daya (starvation) dan waktu tunggu yang lebih lama.

**2.Tingkat Beban yang Sangat Tinggi**

-Jika lalu lintas data sangat tinggi dan perangkat dengan prioritas lebih tinggi terus-menerus mengajukan permintaan, maka perangkat berprioritas rendah mungkin tidak mendapat kesempatan akses, menyebabkan waktu tunggu meningkat drastis.

**3.Preemption oleh Perangkat Prioritas Tinggi**

-Jika sistem mengizinkan preemption (di mana perangkat berprioritas tinggi bisa menghentikan perangkat lain yang sedang berjalan), maka perangkat dengan prioritas rendah akan mengalami waktu tunggu yang lebih panjang.

**Sumber**

Tanenbaum, A. S. (2016). Structured Computer Organization. Pearson
