## Percobaan 2 : Lab - Build a Switch and Router Network

### Link Youtube:
https://youtu.be/thgEDhoFZOw?si=r9OdFf5Js4os6TLQ

### Ping Gagal
![RTO](https://github.com/user-attachments/assets/c208a8e8-a68c-4ade-8c33-eac91657971d)
#### Ping PC-B melalui command prompt di PC-A
<p align="justify">
Ping belum berhasil karena interface router atau default gateway belum dikonfigurasi atau belum diaktifkan (shutdown), sehingga paket data yang dikirim dari PC tidak dapat diteruskan ke perangkat tujuan. Router belum memiliki alamat IP aktif pada interface nya yang berfungsi sebagai default gateway, sehingga lalu lintas pada Layer 3 belum dapat diteruskan antar subnet. Akibatnya, ketika perangkat dari satu subnet mencoba mengirimkan paket ke subnet lain, router belum memiliki arah atau jalur yang jelas untuk meneruskan paket tersebut karena proses routing belum berjalan. Kondisi ini menyebabkan komunikasi antar subnet terhenti karena tidak ada jalur yang dapat dilalui oleh paket ICMP. Selain itu, kemungkinan lain adalah pengaturan alamat IP pada PC atau router belum sesuai dengan jaringan yang digunakan, atau kabel jaringan belum tersambung dengan benar ke port yang seharusnya. Selama interface router masih nonaktif dan belum ada konfigurasi gateway yang valid, perangkat tidak dapat saling berkomunikasi, sehingga setiap permintaan ping akan gagal dan muncul pesan Request timed out karena tidak ada balasan dari alamat tujuan.
</p>

### Ping Berhasil
<img width="1379" height="565" alt="Konfigurasi" src="https://github.com/user-attachments/assets/6548cf19-bb62-4155-aa9c-13af11488288" />

#### Ping PC-B melalui command prompt di PC-A
<p align="justify">
Ping berhasil karena router sudah dikonfigurasi dengan benar dan mampu meneruskan lalu lintas data antar dua subnet tanpa kendala. Interface pada router sudah diaktifkan dan setiap perangkat memiliki alamat IP yang sesuai dengan subnetnya masing-masing. Dengan begitu, jalur komunikasi antar PC menjadi terbuka sehingga paket ICMP dapat dikirim dan diterima dengan sukses. Selain itu, switch Cisco 2960 secara default juga mengaktifkan port yang terhubung ke perangkat, sehingga tidak memerlukan konfigurasi tambahan agar koneksi berfungsi. Hasil Reply from yang muncul menunjukkan bahwa semua paket ping berhasil dikirim dan diterima tanpa kehilangan data (0% loss), menandakan bahwa jaringan sudah berfungsi dengan baik dan koneksi antar perangkat berjalan lancar.
</p>

### Topology
![IMG_6762](https://github.com/user-attachments/assets/60754999-9608-4f2c-82d5-d26a50a97b86)







