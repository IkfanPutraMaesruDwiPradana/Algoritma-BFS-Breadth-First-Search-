Algoritma BFS

suatu metode pencarian yang digunakan untuk menjelajahi semua simpul (node) pada sebuah graf (graph) secara berurutan, dimulai dari simpul awal dan menyebar ke simpul tetangga sebelum melanjutkan ke simpul yang lebih jauh. Algoritma ini sering disebut juga dengan pencarian melebar.
Prinsip Kerja BFS:

1. Mulai dari node awal: BFS memulai pencarian dari node sumber (root) atau simpul awal.
Kunjungi semua tetangga: Semua tetangga langsung dari simpul tersebut diperiksa terlebih dahulu, lalu dilanjutkan ke simpul tetangga-tetangga mereka.
2. Gunakan antrian (queue): BFS menggunakan struktur data antrian (queue) untuk memastikan bahwa simpul yang diperiksa adalah berdasarkan urutan tingkat kedalaman, yaitu pertama simpul yang lebih dekat ke sumber, kemudian yang lebih jauh.
3. Marking untuk menghindari kunjungan ulang: Agar tidak mengunjungi simpul yang sama lebih dari sekali, simpul yang sudah dikunjungi akan ditandai.

Implementasi pada Permainan 8-Puzzle:

Tujuan: Mengatur kembali potongan-potongan puzzle agar membentuk urutan yang benar, yaitu angka 1 hingga 8, dengan posisi kosong (0) di sudut kanan bawah.

Pencarian Jalur: Dalam permainan ini, BFS digunakan untuk menemukan urutan langkah-langkah yang diperlukan untuk mencapai konfigurasi akhir (solusi) dari konfigurasi awal.

Langkah Implementasi BFS pada Puzzle:

1. Mula-mula kita memiliki puzzle awal (misalnya, konfigurasi acak) dan puzzle tujuan yang berisi urutan yang benar (1 hingga 8 dengan posisi kosong di akhir).
2. BFS mulai dari puzzle awal, mengeksplorasi langkah-langkah yang mungkin (misalnya, memindahkan angka yang berdekatan dengan posisi kosong), dan mencari jalur yang mengarah ke puzzle tujuan.
3. Setiap langkah atau perubahan posisi akan dihitung dan dieksplorasi level demi level menggunakan antrian.


