# SIG_Animating-Time-Series-Data

*Tutorial Animating Time Series Data

1. Download terlebih dahulufile ASAM_shp.zip dan ne_10m_land.zip 

2. Pada panel PEramban QGIS, temukan direktori tempat kita menyimpan data unduhan. Luaskan ne_!0m_land.zip dan pilih layer ne_10m_land.shp seret layer ke kanvas. Selanjutnya cari file ASAM_shp.zip dan pilih layer asam_data_download/ASAM_events.shp layer dan seret ke kanvas (*Gambar 1*)

3. Setelah lapisan dimuat. kita dapat melohat masing-masing titik yang mewakili insiden lokasi pembajakan. Ada ribuan insiden dan sulit ditentukan dengan lebih banyak pembajakan. Daripada poin individual, cara yang lebih baik memvisualisasikan data ini adalah melalui heatmap. Pilih layer ASAM_events dan klik tombol Open the layer Sty;ling panel. Klik Single symbok drop=down (*Gambar 2*)

4. Di drop-down pemilihan perender, pilih perender heatmap. Selanjutnya, pilih color ramp warna Viridis (*Gambar 3*)

5. Sesuaikan nilai Radius 5,0. Di bagian bawah, luaskan bagian Layer Rendering dan sesuaikan Opacity menjadi 75%. Ini memberikan efek visual yang bagus dari hotspot dengan lapisan tanah di bawahnya (*Gambar 4*)

6. Sekarang mari kita animasikan data ini untuk menunjukkan eta insiden pembajakan tahunan. Klik kanan pada layer ASAM_event, dan pilih Properties (*Gambar 5*) 

7. Pada Layer Properties, pilih tab Temporal dan aktifkan dengan klik kotak centang (*Gambar 6*)

8. Data sumber berisi atribut dateofocc - mewakili tanggal terjadinya insiden. Ini adalah bidang yang akan digunakan untuk menentukan poin yang diberikan untuk setiap periode waktu. Pilih Single Field with Data/Time di menu Configuration drop-down, dateofocc sebagai Field (*Gambar 7*)

9. Sekarang simbol jam akan muncul di sebelah nama layer. Klik pada Temporal Control Panel dari bilah Toolbar (*Gambar 8*)

10. Klik pada Animated Temporal Navigation untuk mengaktifkan kontrol animasi. Klik the Set to Full Range di sebelah Range to automatically untuk mengatur rentang waktu agar cocok dengan kumpulan data (*Gambar 9*)

11. Sekarang kita siap untuk melihat animasi. Tetapkan langkah sebagai 1 tahun lalu klik tombol Play untuk memulai animasi (*Gambar 10*)

12. Akan sangat membantu juga untuk menampilkan label yang menunjukkan kerangka waktu saat ini di peta. Kita dapat melakuknnya dengan menggunakan Title decoration. pilih View klik Decoration lalu pilih Title laberl (*Gambar 11*)

13. Klik kotak centang untuk mengaktifkannya dan klik tombol Insert an Expression untuk menampilkan tahun. Di sini variabel @map_start_time berisi stempel waktu potongan waktu saat ini yang ditampilkan. JAdi kita bisa menggunakan stempel waktu itu dan memformatnya untuk menampilkan tahun kejadian. Lihat Dokumentasi QGIS untuk detail tentang berbagai opsi pemformatan yang didukung untuk stempel waktu (*Gambar 12*)

14. PIlih ukuran font sebagai 25, atur warna bilah latar belakang dan atur tranpasaransi menjadi 50%. Di penempatan pilih Bottom Right. Lalu klik OK (*Gambar 13*)

15. Setelah parameter diatur sesuai, tahun akan ditampilan di kanan bawah. Untuk mengekspor ini sebagai gambar dan mengonversinya sebagai GIF pilih Export Animation di Temporal control (*Gambar 14*)

16. Klik pada ... Direktori keluaran untuk memilih direktori tempat gambar akan disimpan (*Gambar 15*)

17. Di bawah Extent pilih Calculate from layer lalu pilih ne_10_land layer lalu klik Save (*Gambar 16*)

18. Setelah ekspor selesai, kita akan melihat gambar PNG untuk setiap tahun di direktori keluaran (*Gambar 17*)


