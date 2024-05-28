# AquaFeed

## Latar Belakang
Proyek "AquaFeed" adalah pengumpan ikan otomatis inovatif yang dirancang untuk menyederhanakan proses pemberian makan ikan secara teratur. Dilengkapi dengan tiga tombol, memungkinkan pengguna untuk memilih durasi makan 2, 3, atau 4 detik berdasarkan kebutuhan spesifik mereka. Setelah durasi pemberian makan dipilih, pengatur waktu memulai proses pemberian makan. Ketika pengatur waktu mencapai nol, motor servo diaktifkan untuk membuka wadah makanan, sementara LED dan buzzer memberikan indikator visual dan pendengaran untuk memberi sinyal proses pemberian makan. Selain itu, informasi rinci mengenai waktu pemberian makan yang dipilih dan status operasional pengumpan ditampilkan melalui antarmuka Serial Monitor, menawarkan umpan balik dan kontrol waktu nyata kepada pengguna. Setelah siklus pengumpanan selesai, motor servo kembali ke posisi semula, siap untuk siklus pengumpanan berikutnya. Penting untuk dicatat bahwa proyek ini beroperasi terus menerus, memastikan bahwa ikan diberi makan secara berkala, dengan durasi pemberian makan yang dipilih diulang setiap 10 detik.

## Solusi
Kami memanfaatkan fitur pemrograman Arduino IDE yang tangguh untuk memungkinkan pengguna menulis, menguji, dan mengunggah kode ke papan Arduino. Dengan bantuan perangkat lunak yang ditulis dengan baik, sistem dapat mengontrol motor servo, membaca input tombol, dan memberikan umpan balik secara real-time melalui buzzer dan LED terintegrasi. Selain itu, Serial Monitor Arduino IDE memberi pengguna akses mudah ke informasi penting tentang opsi waktu dan status operasional, memungkinkan mereka memantau dan mengonfirmasi operasi sistem yang sempurna. Sistem pemberian pakan ikan otomatis bekerja secara mulus bersama dengan perangkat keras mutakhir dan perangkat lunak yang dirancang dengan baik, sehingga pemilik tidak lagi bertanggung jawab dalam merawat ikannya.

## Implementasi pada Software
### Desain pada Proteus
...
### Bentuk Fisik Desain Hardware
...

## Fitur Perangkat dan Hardware Desain
### - Arduino Uno R3
![arduinor3](https://github.com/sharifmasyhur/AR_17_ProyekAkhirSSF/assets/144346489/50fe1485-dc71-4f9e-96b1-84ec7f0c52b1)

Semua perangkat keras dikendalikan oleh mikrokontroler Arduino UNO R3 yang akan mengeksekusi program dalam bahasa Assembly.
### - LED
![ledpinouts](https://github.com/sharifmasyhur/AR_17_ProyekAkhirSSF/assets/144346489/45afa83e-c5c5-48b2-8377-6cd961268969)

Isyarat visual yang menyala ketika wadah makanan digerakkan oleh motor servo. Sebuah resistor digunakan untuk membatasi arus yang mengalir melalui LED ketika dipasang ke salah satu pin digital Arduino.
### - Servo Motor
![servomotor](https://github.com/sharifmasyhur/AR_17_ProyekAkhirSSF/assets/144346489/7364d2cd-247a-459e-863a-7f8bdecb0f5a)

Wadah pakan ikan dibuka dan ditutup oleh suatu aktuator. Untuk kontrol posisi, motor servo dihubungkan ke salah satu pin PWM (Pulse Wide Modulation) Arduino.
### - Buzzer
![buzzer](https://github.com/sharifmasyhur/AR_17_ProyekAkhirSSF/assets/144346489/cec5a5de-f074-448f-b57f-0a1e0cae4e80)

Sinyal audio dihasilkan ketika wadah makanan digerakkan oleh motor servo. Pin digital Arduino memiliki bel yang terhubung dengannya
### - Resistor
![resistors](https://github.com/sharifmasyhur/AR_17_ProyekAkhirSSF/assets/144346489/47ffd94d-76b5-4e07-bef3-d0e2e26ea09c)

Resistansi yang terhubung langsung ke LED disediakan oleh resistor. Ketika arus yang disuplai ke LED lebih kecil dari arus awal, masalah kelistrikan dapat diminimalkan dengan menyertakan resistor.
### - Button
![button](https://github.com/sharifmasyhur/AR_17_ProyekAkhirSSF/assets/144346489/8e920319-e50b-44bb-b499-eda571b3a597)

Digunakan untuk memilih apakah akan memberi makan selama tiga, lima, atau sepuluh detik. Pin digital Arduino dihubungkan ke tiga tombol tekan. Untuk menjamin pembacaan yang konsisten, resistor pull-down dihubungkan ke setiap tombol.
### - Power Supply (Baterai)
![batteryarduino](https://github.com/sharifmasyhur/AR_17_ProyekAkhirSSF/assets/144346489/e07f1e48-e875-4087-9d02-a0c19ccd4894)

Sumber daya yang menjalankan komponen tambahan dan Arduino UNO. Melalui colokan listrik atau, untuk sumber daya yang lebih andal, pin Vin dan GND, Arduino UNO dapat diberi daya secara eksternal.

## Hasil Akhir dan Evaluasi Performa
Proyek AquaFeed telah berhasil dimulai dan memenuhi kriterianya. Selama pengembangan, ada kesulitan dalam mengimplementasikan interupsi dalam program Majelis. Interupsi perlu digunakan untuk mengelola fenomena asinkron, seperti penekanan tombol dan pembacaan sensor yang efisien. Silakan gunakan file bantuan. Ini memberikan solusi efektif untuk mengurangi kompleksitas dan meningkatkan efisiensi pembangunan. Sistem berfungsi dengan baik, memberikan pengguna pengalaman yang konsisten saat mereka makan ikan secara otomatis. Evaluasi ini menyoroti perlunya fleksibilitas dalam manajemen proyek dan manfaat menggunakan bahasa manajemen proyek yang selaras dengan persyaratan proyek. Hasil dari evaluasi ini menunjukkan pentingnya fleksibilitas dalam pendekatan pengembangan dan manfaat dari penggunaan bahasa pemrograman yang sesuai dengan kebutuhan proyek.

## Kesimpulan
Proyek AquaFeed telah berhasil diterapkan sebagai sistem penggantian tepung ikan otomatis, memungkinkan pengguna melakukan penggantian tepung dengan cara tersier dengan mudah. Sistem ini secara efektif mengoperasikan motor servo untuk memasak dan memanaskan kembali ikan sesuai durasi yang dipilih pengguna menggunakan tombol tekan. Pengguna dapat dengan mudah memilih durasi makan (2, 3, atau 4 hari), dan sistem akan meresponsnya. Integrasi komponen keras dengan komponen lunak yang tertulis di Majelis berhasil. Setiap komponen bekerja sama secara kohesif untuk memberikan pengalaman pengguna terbaikSecara keseluruhan, proyek AquaFeed telah menunjukkan peningkatan yang signifikan dalam otomatisasi budidaya ikan dan telah memberikan solusi yang efisien, efektif, dan menyenangkan bagi pengguna. Dengan kinerja yang kuat dari seluruh komponen dan integrasi yang kuat antara perangkat keras dan perangkat lunak, proyek ini telah mencapai semua tujuannya.
  
## Kontributor Proyek
- Yoel Dwi Miryano				      (2206059534)
- Sharif Fatih Asad Masyhur 		(2206063014)
- Sihombing Giovano Geraldo 	  (2206059566)
- Muhammad Lutfi Setiadi	      (2206059805)


