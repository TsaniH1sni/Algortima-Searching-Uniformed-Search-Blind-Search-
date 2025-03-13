# Algortima-Searching-Uniformed-Search-Blind-Search-
1. Depth First Search (DFS)
Fungsionalitas:
Kode pertama mengimplementasikan algoritma Depth First Search (DFS) menggunakan rekursi pada struktur graf berarah. DFS adalah metode pencarian yang menjelajahi graf dengan menyelam lebih dalam ke setiap cabang sebelum kembali ke simpul sebelumnya.

Cara kerja:

Menggunakan kelas Graph untuk merepresentasikan graf dalam bentuk daftar adjacency.
Memiliki metode addEdge(u, v) untuk menambahkan sisi (edge) ke dalam graf.
Metode DFSUtil(v, visited) digunakan untuk menelusuri graf secara rekursif.
Metode DFS(v) adalah fungsi utama yang memulai DFS dari simpul yang ditentukan.

2. Breadth First Search (BFS)
Fungsionalitas:
Kode kedua mengimplementasikan Breadth First Search (BFS) menggunakan struktur antrean (queue). BFS menelusuri graf secara lebar terlebih dahulu, yaitu menjelajahi semua simpul di satu level sebelum berpindah ke level berikutnya.

Cara kerja:

Menggunakan struktur data deque dari collections untuk menyimpan simpul yang akan dieksplorasi.
Fungsi bfs(graph, root) menelusuri graf menggunakan antrian FIFO.
Set visited digunakan untuk memastikan simpul tidak dikunjungi lebih dari sekali.
Node pertama diambil dari antrian, diproses, dan semua tetangga yang belum dikunjungi ditambahkan ke antrian.

3. Uniform Cost Search (UCS)
Fungsionalitas:
Kode ketiga mengimplementasikan Uniform Cost Search (UCS), sebuah algoritma pencarian optimal berbasis biaya terendah. UCS berguna dalam pencarian jalur terpendek pada graf berbobot.

Cara kerja:

Menggunakan struktur data priority queue untuk mengevaluasi node dengan biaya terendah terlebih dahulu.
uniform_cost_search(goal, start) mencari jalur terpendek dari start ke simpul tujuan (goal).
Graf direpresentasikan sebagai dictionary, dengan daftar adjacency dan biaya antar node disimpan dalam dictionary cost.
Algoritma terus mengevaluasi jalur yang memiliki biaya lebih rendah hingga mencapai simpul tujuan.
