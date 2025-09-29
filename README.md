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
# contoh html
<!DOCTYPE html>
<html>
<head>
  <style>
    p { color: blue; }   /* internal */
  </style>
  <link rel="stylesheet" href="style.css"> <!-- eksternal -->
</head>
<body>
  <p style="color:red;">Contoh paragraf</p> <!-- inline -->
</body>
</html>
#Contoh CSS
p { color: green; }


# 4
Yang ditampilkan adalah deklrasi CSS dari ID, karena ID punya prioritas (specificity) lebih tinggi dibandingkan Class.
Urutan kekuatan CSS:
Inline CSS > ID > Class > Elemen > Default browser.
<!DOCTYPE html>
<html>
<head>
<style>
.text-paragraf { color: green; }
#paragraf-1 { color: blue; }
</style>
</head>
<body>
  <p id="paragraf-1" class="text-paragraf">
    Contoh paragraf
  </p>
</body>
</html>
