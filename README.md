# praktikum 2
Jawaban
# 2
Kalau kita pakai h1 { ... }, maka semua elemen <h1> di dalam halaman akan kena aturan CSS itu. Jadi sifatnya umum, berlaku untuk semua judul <h1> tanpa melihat posisinya.
Sedangkan kalau kita pakai #intro h1 { ... }, maka CSS hanya berlaku untuk <h1> yang ada di dalam elemen dengan id intro. Jadi lebih spesifik, hanya judul <h1> yang ada di bagian tertentu saja yang akan berubah.

# 3
Yang akan ditampilkan oleh browser adalah inline CSS.
Karena urutan prioritas CSS (specificity) adalah:
Inline CSS → paling kuat.
Internal CSS (di dalam <style>).
Eksternal CSS (file .css).
Aturan bawaan browser.
Jadi kalau satu elemen diatur oleh ketiganya, maka inline CSS yang dipakai.
<img width="720" height="842" alt="Cuplikan layar 2025-09-29 143912" src="https://github.com/user-attachments/assets/b936fcf3-86bc-4a5a-8898-3f2a8b759658" />
