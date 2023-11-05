
# Meningkatkan Kecerahan, Meregangkan Kontras & Membalik Citra

- Peningkatan Kecerahan: Peningkatan kecerahan dilakukan dengan tujuan untuk membuat gambar menjadi lebih terang.
- Peregangan Kontras: Peregangan kontras dilakukan untuk memperjelas perbedaan antara intensitas piksel pada citra.
- Pembalikan Citra: Pembalikan citra dilakukan untuk membalik nilai intensitas piksel pada citra.

Library yang digunakan:

- cv2: cv2 adalah library OpenCV untuk pemrosesan gambar. Ini digunakan untuk memuat, memanipulasi, dan menyimpan gambar dalam berbagai format.
- numpy: numpy adalah library untuk komputasi numerik dalam Python. Ini digunakan untuk melakukan operasi matematika pada array dan matriks.
- matplotlib.pyplot: matplotlib.pyplot adalah library plotting untuk Python. Ini digunakan untuk membuat visualisasi data, termasuk gambar.
- skimage: skimage adalah library scikit-image untuk pemrosesan gambar. Skimage menyediakan kumpulan algoritma untuk pemrosesan gambar, termasuk penyaringan, segmentasi, dan ekstraksi fitur.

Penjelasan penyelesaian Meningkatkan Kecerahan, Meregangkan Kontras & Membalik Citra yang digunakan di skrip:

- cv2: Skrip mengimpor library OpenCV untuk pemrosesan gambar.
- numpy: Skrip mengimpor library numpy untuk komputasi numerik dalam Python.
- skimage: Skrip mengimpor library skikit-image untuk pemrosesan gambar.
- citra: Skrip memuat gambar bernama '1.jpg' menggunakan fungsi cv2.imread() dan menyimpannya dalam variabel 'citra'.
- cv.imshow(): Skrip menampilkan gambar asli menggunakan fungsi cv.imshow().
- print(): Skrip mencetak bentuk dan tipe data gambar menggunakan fungsi print().
- citra_gray: Skrip membuat versi grayscale dari gambar dengan menerapkan jumlah tertimbang dari saluran merah, hijau, dan biru ke setiap piksel.
- cv.imshow(): Skrip menampilkan gambar grayscale menggunakan fungsi cv.imshow().
- citra_biner: Skrip membuat versi biner dari gambar grayscale dengan mengatur semua piksel dengan intensitas lebih besar atau sama dengan nilai ambang batas ke 0 dan semua piksel lainnya ke 1.
- cv.imshow(): Skrip menampilkan gambar biner menggunakan fungsi cv.imshow().
- cv.imwrite(): Skrip menyimpan citra grayscale ke sebuah berkas bernama "Hasil-grayscale-citra.png" menggunakan fungsi cv.imwrite().
- plt.imshow(): Skrip menampilkan citra biner menggunakan fungsi plt.imshow() dari library matplotlib.
- kernel: Skrip membuat kernel untuk pemfilteran gambar.
- cv2.filter2D(): Skrip menerapkan kernel ke citra biner menggunakan fungsi cv2.filter2D() dan menyimpan hasilnya dalam variabel 'citraOutput'.
- plt.imshow(): Skrip menampilkan gambar asli dan gambar yang telah difilter secara berdampingan menggunakan fungsi plt.imshow().
- img: Skrip memuat gambar asli menggunakan fungsi cv2.imread() dan menyimpannya dalam variabel 'img'.
- cv2.imshow(): Skrip menampilkan gambar asli menggunakan fungsi cv2.imshow().
- cv2.calcHist(): Skrip menghitung histogram gambar asli menggunakan fungsi cv2.calcHist() dan menyimpannya dalam variabel 'hist'.
- plt.plot(): Skrip menampilkan histogram menggunakan fungsi plt.plot().
- cv2.cvtColor(): Skrip mengubah gambar asli dari BGR ke ruang warna RGB menggunakan fungsi cv2.cvtColor().
- plt.imshow(): Skrip menampilkan gambar asli menggunakan fungsi plt.imshow().
- plt.plot(): Skrip menampilkan histogram menggunakan fungsi plt.plot().
- plt.subplots(): Skrip menampilkan gambar asli dan histogram secara berdampingan menggunakan fungsi plt.subplots().
- cv2.imread(): Skrip memuat gambar asli menggunakan fungsi cv2.imread() dan menyimpannya dalam variabel 'abu'.
- cv2.equalizeHist(): Skrip menerapkan penyetaraan histogram ke gambar grayscale menggunakan fungsi cv2.equalizeHist() dan menyimpan hasilnya dalam variabel 'hist2'.
- plt.imshow(): Skrip menampilkan gambar grayscale dan histogramnya secara berdampingan menggunakan fungsi plt.imshow() dan plt.hist().
- citra_cerah: Skrip membuat versi yang lebih cerah dari gambar asli dengan menambahkan nilai konstan ke setiap piksel.
- plt.subplot(): Skrip menampilkan gambar asli dan gambar yang lebih terang secara berdampingan bersama dengan histogramnya menggunakan fungsi plt.subplots().
- citra_kontras: Skrip ini membuat versi kontras yang lebih tinggi dari gambar asli dengan mengalikan setiap piksel dengan nilai konstan.
- plt.subplots(): Skrip menampilkan gambar asli dan gambar dengan kontras yang lebih tinggi secara berdampingan bersama dengan histogramnya menggunakan fungsi plt.subplots().

Berikut alur penjelasan skrip tersebut:

- Skrip mengimpor library yang diperlukan untuk pemrosesan gambar.
- Skrip memuat gambar '1.jpg' menggunakan fungsi cv2.imread() dan menyimpannya dalam variabel 'citra'.
- Skrip menampilkan gambar asli menggunakan fungsi cv.imshow().
- Skrip mencetak bentuk dan tipe data gambar menggunakan fungsi print().
- Skrip mengekstrak saluran merah, hijau, dan biru dari gambar dan menyimpannya dalam variabel terpisah.
- Skrip membuat versi grayscale dari gambar dengan menerapkan jumlah tertimbang dari saluran merah, hijau, dan biru ke setiap piksel.
- Skrip menampilkan gambar grayscale menggunakan fungsi cv.imshow().
- Skrip membuat versi biner dari gambar grayscale dengan mengatur semua piksel dengan intensitas lebih besar atau sama dengan nilai ambang batas ke 0 dan semua piksel lainnya ke 1.
- Skrip menampilkan gambar biner menggunakan fungsi cv.imshow().
- Skrip menyimpan citra grayscale ke sebuah file bernama "Hasil-gray-citra.png" menggunakan fungsi cv.imwrite().
- Skrip memuat gambar grayscale dari file yang disimpan menggunakan fungsi imread() dari library scikit-image dan menyimpannya dalam variabel 'citra_biner'.
- Skrip menampilkan gambar grayscale menggunakan fungsi plt.imshow().
- Skrip membuat kernel untuk penyaringan gambar.
- Skrip menerapkan kernel ke citra biner menggunakan fungsi cv2.filter2D() dan menyimpan hasilnya dalam variabel 'citraOutput'.
- Skrip menampilkan gambar asli dan gambar yang telah difilter secara berdampingan menggunakan fungsi plt.subplots().
- Skrip memuat gambar asli menggunakan fungsi cv2.imread() dan menampilkannya menggunakan fungsi cv2.imshow().
- Skrip menghitung histogram gambar asli menggunakan fungsi cv2.calcHist() dan menampilkannya menggunakan fungsi plt.plot().
- Skrip mengkonversi gambar asli dari BGR ke ruang warna RGB menggunakan fungsi cv2.cvtColor() dan menampilkannya menggunakan fungsi plt.imshow().
- Skrip menampilkan gambar asli dan histogramnya secara berdampingan menggunakan fungsi plt.subplots().
- Skrip memuat gambar asli dalam skala abu-abu menggunakan fungsi cv2.imread() dan menerapkan penyetaraan histogram menggunakan fungsi cv2.equalizeHist().
- Skrip menampilkan gambar skala abu-abu dan histogramnya secara berdampingan menggunakan fungsi plt.imshow() dan plt.hist().
- Skrip ini membuat versi yang lebih cerah dari gambar asli dengan menambahkan nilai konstan ke setiap piksel.
- Skrip menampilkan gambar asli dan gambar yang lebih terang secara berdampingan bersama dengan histogramnya menggunakan fungsi plt.subplots().
- Skrip membuat versi kontras yang lebih tinggi dari gambar asli dengan mengalikan setiap piksel dengan nilai konstan.
- Skrip menampilkan gambar asli dan gambar dengan kontras yang lebih tinggi secara berdampingan bersama dengan histogramnya menggunakan fungsi plt.subplots().

Sitasi:
- [1] https://rizafennisya.files.wordpress.com/2017/01/pcd-3.pdf
- [2] https://id.scribd.com/doc/225959903/Pengolahan-citra-digital-Pertemuan-3
- [3] https://id.scribd.com/document/390721316/MKB3383-Teknik-Pengolahan-Citra-2-Operasi-Piksel-dan-Histogram-1-pdf
- [4] https://lib.unika.ac.id/index.php?bid=50633&fid=2029&p=fstream-pdf
- [5] https://discuss.ray.io/t/change-opencv-dependency-to-scikit-image/1695
- [6] https://stackoverflow.com/questions/66360041/how-to-convert-cv2-image-to-skimage
- [7] https://scikit-image.org/docs/stable/user_guide/data_types.html
- [8] https://github.com/opencv/opencv/issues/15179
- [9] https://github.com/scikit-image/scikit-image/issues/2293
- [10] https://lindevs.com/convert-opencv-image-to-scikit-image-using-python
- [11] https://discuss.ray.io/t/change-opencv-dependency-to-scikit-image/1695
- [12] https://github.com/scikit-image/scikit-image/issues/2293
- [13] https://github.com/opencv/opencv/issues/15179
- [14] https://scikit-image.org
- [15] https://www.geeksforgeeks.org/image-processing-in-python/
- [16] https://lindevs.com/convert-opencv-image-to-scikit-image-using-python
- [17] https://discuss.ray.io/t/change-opencv-dependency-to-scikit-image/1695
- [18] https://github.com/scikit-image/scikit-image/issues/2293
- [19] https://github.com/opencv/opencv/issues/15179
- [20] https://stackoverflow.com/questions/66360041/how-to-convert-cv2-image-to-skimage
- [21] https://lindevs.com/convert-opencv-image-to-scikit-image-using-python
- [22] https://scikit-image.org/docs/stable/user_guide/data_types.html
- [23] https://www.perplexity.ai/search/Meningkatkan-Kecerahan-Meregangkan-rIA8mlLsSKqOvIMu61L3Mg?s=c 
## 🔗 Link Data Diri
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/anugrahak)

## Authors

- Anugrah AK. [@aanggaanugrahhakk](https://www.github.com/aanggaanugrahhakk)


## Identitas Authors

Nama: Anugrah AK.

NIM: 202131037

Kelas: B