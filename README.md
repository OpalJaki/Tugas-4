* Nama: Muhammad Naufal Zaki
* Kelas: SKU2B
* Mata Kuliah: Organisasi dan Arsitektur Komputer

# 1. Jelaskan struktur antar hubungan dan beri contohnya!
Struktur hubungan antar komponen dalam komputer dikenal sebagai sistem BUS. BUS merupakan subsistem yang berperan dalam mentransfer data atau daya listrik antara komponen-komponen di dalam komputer atau antar komputer. Dalam sistem komputer, BUS mencakup perangkat internal dan memiliki kecepatan tinggi dalam mentransmisikan informasi.  

**Contoh BUS:**  
- **PCI (Peripheral Component Interconnect)**  
  PCI adalah bus yang dirancang untuk menghubungkan berbagai perangkat keras. Bus ini memiliki bandwidth tinggi dan tidak bergantung pada prosesor, sehingga dapat digunakan sebagai bus mezzanine atau bus periferal. Standar PCI dikembangkan oleh PCI Special Interest Group, yang dibentuk oleh Intel Corporation bersama beberapa perusahaan lainnya pada tahun 1992. PCI hadir untuk menggantikan Bus ISA/EISA yang sebelumnya digunakan pada komputer IBM PC dan kompatibelnya.  

- **USB (Universal Serial Bus)**  
  USB adalah teknologi yang memungkinkan koneksi perangkat eksternal seperti scanner, printer, mouse, keyboard, perangkat penyimpanan (flash drive), kamera digital, dan lainnya ke komputer. USB mendukung kecepatan transfer data hingga 12 Mbps (juta bit per detik). Saat ini, hampir semua komputer telah dilengkapi dengan port USB, biasanya minimal dua port. Dibandingkan dengan port paralel dan serial, port USB lebih praktis dan mudah digunakan.  

- **BUS PCI**  
  BUS PCI adalah bus yang independen dari prosesor dan berfungsi sebagai bus mezzanine atau bus periferal. Standar PCI memiliki 64 jalur data dengan kecepatan 33 MHz, memungkinkan transfer data hingga 263 MB per detik atau 2,112 Gbps. Selain menawarkan kecepatan tinggi, PCI juga memiliki keunggulan dalam efisiensi biaya karena menggunakan jumlah komponen yang lebih sedikit.  

- **BUS ISA (Industry Standard Architecture)**  
  BUS ISA dikembangkan sebagai standar industri untuk komputer pribadi. Pada dasarnya, ISA merupakan bus PC/AT yang beroperasi pada frekuensi 8,33 MHz. Keunggulan utama bus ISA adalah kemampuannya untuk tetap kompatibel dengan perangkat keras dan kartu ekspansi yang telah ada sebelumnya.
  
# 2. Bila terlalu banyak modul atau perangkat dihubungkan pada bus maka akan terjadi penurunan kinerja, sebutkan penyebabnya!
Kapasitas transfer bus yang terbatas dapat menyebabkan perlambatan dalam pengiriman data. Setiap bus memiliki lebar jalur data tertentu, sehingga jika kapasitas transfer data melebihi batas yang tersedia, proses transfer akan menjadi lebih lambat. Selain itu, semakin banyak perangkat yang menggunakan bus secara bersamaan, antrean akses akan semakin panjang, yang berdampak pada lambatnya proses transfer data. Selain itu, waktu tunda (delay propagasi) dalam koordinasi penggunaan bus juga semakin besar, sehingga mempengaruhi efisiensi transfer data secara keseluruhan.

# 3. Umumnya perangkat berprioritas paling rendah memiliki waktu tunggu rata-rata yang paling singkat. Dengan dasar ini biasanya CPU diberi perioritas tertinggi pada SBI. Sebutkan alasan perangkat berprioritas 16 memiliki waktu tunggu rata-rata paling rendah? Dibawah kondisi seperti apa keadaan diatas tidak berlaku?
Perangkat dengan prioritas 16 memiliki waktu tunggu rata-rata paling rendah karena penggunaan bus data. Bus data berfungsi sebagai jalur yang menyalurkan data antara berbagai komponen dalam sistem, terdiri dari 8, 16, 32, atau lebih jalur sinyal paralel. Jalur-jalur ini bersifat dua arah (bidirectional), memungkinkan CPU untuk membaca dan mengirim data dari atau ke memori maupun port. Meskipun banyak perangkat terhubung ke bus data, hanya satu perangkat yang dapat menggunakannya dalam satu waktu. Untuk mengelola akses, perangkat harus memiliki tiga keadaan (tristate) agar dapat beroperasi pada bus data secara efisien.
