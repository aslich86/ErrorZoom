# ErrorZoom

## Mengatasi Error Zoom Penting Ga Penting di Ubuntu

Jadi, ketika pertama kali membuka Zoom muncul peringatan seperti ini


Wayland screen sharing is not yet enabled. Please restart Zoom for it to automatically enable, or manually change the value of "enableWaylandShare" to "true" in "/home/username/.var/app/us.zoom.Zoom/config/zoomus.conf".

Error tersebut terkait dengan penggunaan Wayland untuk screen sharing di Zoom di lingkungan desktop Linux seperti Ubuntu atau Zorin OS. Wayland adalah server display yang digunakan oleh beberapa lingkungan desktop Linux modern.

Berikut adalah langkah-langkah untuk mengatasi error tersebut:

Langkah 1: Ganti Nilai enableWaylandShare
Buka terminal.

Ketik perintah berikut untuk membuka file konfigurasi Zoom:

```
nano ~/.var/app/us.zoom.Zoom/config/zoomus.conf
```

Cari baris yang menyatakan enableWaylandShare dan ganti nilainya menjadi true. Jika baris tersebut tidak ada, tambahkan baris berikut ke file tersebut:

```
enableWaylandShare=true
```

Simpan perubahan dengan menekan Ctrl + X, lalu tekan Y untuk mengonfirmasi penyimpanan, dan terakhir tekan Enter untuk keluar.

Langkah 2: Restart Zoom
Tutup Zoom jika sudah terbuka.

Buka Zoom lagi dan lihat apakah masalahnya sudah teratasi.
