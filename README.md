Fail graphics.hpengepala menyediakan akses kepada perpustakaan fungsi untuk melaksanakan operasi grafik asas, terutamanya dalam konteks pengkompil C dan C++ yang lebih lama seperti Turbo C++. Fungsi ini membolehkan untuk melukis pelbagai bentuk, memanipulasi warna, dan memaparkan teks dalam tetingkap grafik.

Berikut adalah beberapa fungsi utama yang terdapat dalam graphics.h:

Fungsi Lukisan:
• line(int x1, int y1, int x2, int y2): Melukis garisan antara dua titik yang ditentukan.
• circle(int x, int y, int radius): Melukis bulatan dengan pusat dan jejari tertentu.
• rectangle(int x1, int y1, int x2, int y2): Melukis segi empat tepat yang tidak diisi menggunakan koordinat penjuru kiri atas dan kanan bawahnya.
• bar(int x1, int y1, int x2, int y2): Melukis segi empat tepat yang diisi.
• arc(int x, int y, int stangle, int endangle, int radius): Melukis lengkok bulat. 
• ellipse(int x, int y, int stangle, int endangle, int xradius, int yradius): Melukis lengkok elips.
• drawpoly(int numpoints, int *polypoints): Melukis poligon.

Fungsi Warna dan Gaya:
• setcolor(int color): Menetapkan warna lukisan untuk operasi seterusnya.
• setbkcolor(int color): Menetapkan warna latar belakang.
• setfillstyle(int pattern, int color): Menetapkan corak isian dan warna untuk bentuk isian.
• setlinestyle(int style, unsigned pattern, int thickness): Menetapkan gaya garisan (pepejal, bertitik, putus-putus) dan ketebalan.

Fungsi Teks:
• outtext(char *textstring): Memaparkan rentetan teks pada kedudukan kursor semasa.
• outtextxy(int x, int y, char *textstring): Memaparkan rentetan teks pada koordinat yang ditentukan.
• settextjustify(int horiz, int vert): Menetapkan justifikasi mendatar dan menegak untuk teks.
• settextstyle(int font, int direction, int charsize): Menetapkan fon, arah penulisan dan saiz aksara untuk teks.

Fungsi Permulaan dan Pengurusan:
• initgraph(int *graphdriver, int *graphmode, char *pathtodriver): Memulakan sistem grafik.
• closegraph(): Mematikan sistem grafik.
• detectgraph(int *graphdriver, int *graphmode): Mengesan pemacu dan mod grafik yang tersedia.
• getch(): Menunggu input aksara daripada papan kekunci (sering digunakan untuk menjeda tetingkap grafik).
• delay(unsigned milliseconds): Menjeda pelaksanaan program untuk tempoh tertentu.

Fungsi ini membolehkan pembangun mencipta atur cara grafik, animasi dan visualisasi yang ringkas dalam persekitaran khusus yang graphics.h disokong.
