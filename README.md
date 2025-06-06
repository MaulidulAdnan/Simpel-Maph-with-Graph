# 🚗 Peta Jalur Multimoda Jawa Timur (Dijkstra & TSP)

Repositori ini berisi implementasi struktur data graf berbasis Python untuk memodelkan **peta jalur antar kota di Jawa Timur**. Program ini mendukung pemilihan rute tercepat berdasarkan moda transportasi (_mobil_, _motor_, _jalan kaki_) menggunakan algoritma **Dijkstra**, serta pencarian **rute optimal TSP** (Traveling Salesman Problem) dengan pendekatan _brute-force_.

## ✨ Fitur Utama

- Struktur graf berbasis kelas `MultiModeGraph`.
- Pemodelan bobot waktu dan jarak untuk setiap moda transportasi.
- Visualisasi graf dan rute menggunakan `matplotlib`.
- Algoritma:
  - 🔺 **Dijkstra**: Menemukan rute tercepat dari satu kota ke kota lainnya.
  - 🔄 **TSP Brute Force**: Menemukan rute optimal melewati semua kota sekali.
  
## 🛠️ Teknologi yang Digunakan

- Python 3.x
- `matplotlib` untuk visualisasi graf
- `heapq` untuk implementasi Dijkstra
- `itertools` untuk permutasi TSP

## 🗺️ Daftar Kota

Program ini mencakup 10 kota di Jawa Timur, antara lain:

- Surabaya
- Sidoarjo
- Gresik
- Lamongan
- Mojokerto
- Jombang
- Malang
- Blitar
- Kediri
- Pasuruan

## ▶️ Cara Menjalankan Program

1. Pastikan Python 3 dan `matplotlib` telah terinstal:
   ```bash
   pip install matplotlib
   ```

2. Jalankan program:
   ```bash
   python map\ strukdat.py
   ```

3. Masukkan input sesuai instruksi di terminal:
   - Moda transportasi (`mobil`, `motor`, `jalan`)
   - Kota asal dan tujuan

4. Program akan menampilkan:
   - Rute tercepat dari kota asal ke kota tujuan
   - Rute terbaik untuk mengunjungi semua kota (TSP)
   - Visualisasi graf dan rute yang dilalui

## 📌 Contoh Output

```
=== RUTE TERCEPAT MENGGUNAKAN DIJKSTRA ===
Pilih transportasi (mobil/motor/jalan): mobil
Masukkan kota asal anda: Surabaya
Masukkan kota tujuan anda: Malang

✅ Rute tercepat dari Surabaya ke Malang dengan mobil:
Surabaya -> Sidoarjo -> Malang
Total waktu: 2.00 jam
Total jarak: 95.00 km

=== RUTE TSP TERBAIK (Semua kota dikunjungi sekali) ===
📍 Rute TSP: Surabaya -> ... -> Kediri
Total waktu: 17.80 jam
Total jarak: 720.00 km
```

## 📁 Struktur File

- `map strukdat.py` – Program utama, termasuk:
  - Struktur graf
  - Fungsi Dijkstra dan TSP
  - Visualisasi graf
  - Data kota dan koneksi antar kota

## 🧠 Catatan Teknis

- Algoritma TSP menggunakan pendekatan brute-force sehingga kompleksitas waktu sangat tinggi untuk kota lebih dari 10.
- Visualisasi dapat ditingkatkan dengan penambahan peta interaktif atau GUI.

## 📜 Lisensi

Proyek ini bebas digunakan untuk keperluan akademik dan pembelajaran. Harap cantumkan atribusi jika digunakan untuk publikasi atau proyek komersial.
