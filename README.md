## Percobaan 2 : Lab - Build a Switch and Router Network

### Link Youtube:
https://youtu.be/thgEDhoFZOw?si=r9OdFf5Js4os6TLQ

### Ping Gagal
![RTO](https://github.com/user-attachments/assets/c208a8e8-a68c-4ade-8c33-eac91657971d)
Ping belum berhasil karena interface router atau default gateway belum dikonfigurasi atau belum diaktifkan (shutdown), sehingga paket data yang dikirim dari PC tidak dapat diteruskan ke perangkat tujuan. 
Router belum memiliki alamat IP aktif pada interface-nya yang berfungsi sebagai default gateway, sehingga lalu lintas pada Layer 3 belum dapat diteruskan antar subnet. Akibatnya, ketika perangkat dari 
satu subnet mencoba mengirimkan paket ke subnet lain, router belum memiliki arah atau jalur yang jelas untuk meneruskan paket tersebut karena proses routing belum berjalan. Kondisi ini menyebabkan komunikasi 
antar subnet terhenti karena tidak ada jalur yang dapat dilalui oleh paket ICMP. Selain itu, kemungkinan lain adalah pengaturan alamat IP pada PC atau router belum sesuai dengan jaringan yang digunakan, atau 
kabel jaringan belum tersambung dengan benar ke port yang seharusnya. Selama interface router masih nonaktif dan belum ada konfigurasi gateway yang valid, perangkat tidak dapat saling berkomunikasi, sehingga 
setiap permintaan ping akan gagal dan muncul pesan Request timed out karena tidak ada balasan dari alamat tujuan.




