# graphics.h — Pengenalan & Fungsi

`graphics.h` ialah fail pengepala yang menyediakan akses kepada perpustakaan fungsi untuk melaksanakan operasi grafik asas, terutamanya dalam konteks pengkompil C dan C++ yang lebih lama seperti **Turbo C++**.

Fungsi-fungsi dalam `graphics.h` membolehkan pembangun:
- Melukis pelbagai bentuk 2D seperti garis, bulatan, segi empat, dan poligon
- Memanipulasi warna dan corak lukisan
- Memaparkan teks dalam tetingkap grafik
- Menguruskan permulaan dan penutupan sistem grafik

---

## Fungsi Utama

### Fungsi Lukisan
- `line(int x1, int y1, int x2, int y2)`  
  Melukis garisan antara dua titik yang ditentukan.

- `circle(int x, int y, int radius)`  
  Melukis bulatan dengan pusat dan jejari tertentu.

- `rectangle(int x1, int y1, int x2, int y2)`  
  Melukis segi empat tepat (tidak diisi) menggunakan koordinat penjuru atas kiri dan bawah kanan.

- `bar(int x1, int y1, int x2, int y2)`  
  Melukis segi empat tepat yang diisi.

- `arc(int x, int y, int stangle, int endangle, int radius)`  
  Melukis lengkok bulatan.

- `ellipse(int x, int y, int stangle, int endangle, int xradius, int yradius)`  
  Melukis lengkok elips.

- `drawpoly(int numpoints, int *polypoints)`  
  Melukis bentuk poligon berdasarkan bilangan titik dan koordinatnya.

---

### Fungsi Warna dan Gaya
- `setcolor(int color)`  
  Menetapkan warna lukisan.

- `setbkcolor(int color)`  
  Menetapkan warna latar belakang.

- `setfillstyle(int pattern, int color)`  
  Menetapkan corak dan warna isian untuk bentuk berisi.

- `setlinestyle(int style, unsigned pattern, int thickness)`  
  Menetapkan gaya dan ketebalan garisan (pepejal, bertitik, putus-putus).

---

### Fungsi Teks
- `outtext(char *textstring)`  
  Memaparkan teks pada kedudukan kursor semasa.

- `outtextxy(int x, int y, char *textstring)`  
  Memaparkan teks pada koordinat yang ditentukan.

- `settextjustify(int horiz, int vert)`  
  Menetapkan penjajaran mendatar dan menegak bagi teks.

- `settextstyle(int font, int direction, int charsize)`  
  Menetapkan fon, arah tulisan dan saiz aksara.

---

### Fungsi Permulaan dan Pengurusan
- `initgraph(int *graphdriver, int *graphmode, char *pathtodriver)`  
  Memulakan mod grafik.

- `closegraph()`  
  Menutup sistem grafik dan kembali ke mod teks.

- `detectgraph(int *graphdriver, int *graphmode)`  
  Mengesan pemacu dan mod grafik yang tersedia.

- `getch()`  
  Menunggu input papan kekunci (digunakan untuk menjeda paparan grafik).

- `delay(unsigned milliseconds)`  
  Menjeda pelaksanaan program untuk masa tertentu.

---

## Kegunaan

Dengan `graphics.h`, pembangun boleh membina:
- Aplikasi pembelajaran grafik asas
- Projek visualisasi dalam C/C++
- Animasi ringkas atau simulasi 2D
- Permainan 2D berasaskan piksel untuk projek pendidikan

---

## Nota

`graphics.h` tidak tersedia dalam banyak pengkompil moden secara lalai. Ia lebih sesuai digunakan dalam persekitaran **DOSBox** atau **Turbo C++ IDE**. Untuk alternatif moden, pertimbangkan perpustakaan seperti **SDL**, **SFML**, atau **OpenGL**.

---
