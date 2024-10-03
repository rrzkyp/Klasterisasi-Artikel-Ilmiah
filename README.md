Dataset yang diambil adalah 100 abstrak artikel ilmiah yang disajikan dalam file berbentuk atau berformat csv. Isi dari dataset memiliki 4 kolom nomor, judul artikel, isi abstrak, dan truelabel. Seluruh artikel ilmiah ini yang dimuat file berkaitan dengan science.

Pada kode program setelah dilakukan import library dilakukan pembacaan data setdengan pembacaan data berisikan title, abstrak dan truelabel. pembacaan file dataset dilakukan untuk memastikan data yang dimasukan pada kodeprogram adalah sesuai.

Pada tahap preprocessing dilakukan pembersihan kata, seperti menghapus link, karakter khusus, nomor dan stopword selain itu juga dilakukan case folding. preprocessing dilakukan agar program dilakukan dapat lebih cepat dan menghasilkan hasil yang akurat.

LDA sendiri adalah sebuah model sebuah model generatif probabilistik yang digunakan untuk menganalisis topik dalam koleksi dokumen. LDA untuk menentukan jumlah topik yang sesuai menggunakan metode coherence score. Coherence score digunakan untuk menentukan hubungan kedekatan kata dalam topik .

TF-IDF dilakukan untuk menentukan pentingnya kata bergantung pada pengukuran skor TF-IDF. Kemudian setelah itu dilakukan inisialisasi model LDA dengan 9 topik . Untuk klasterisasi K-means menggunakan metode elbow. Tujuan utama dari elbow adalah menentukan jumlah optimal klaster yang harus digunakan dalam suatu dataset .metode elbow didapatkan jumlah cluster optimal yaitu k=4 sehingga inisialisasi cluster untuk model K-means berjumlah 4.

Selanjutnya dilakukan pembentukan jaringan dengan dengan library network. kata yang ingin ditampilkan dalam cluster adalah 8, kemudian dihitung jumlah frekuensi yang muncul tiap cluster, setelah didapatkan jumlah kemunculan dibuat jaringan yang mengaitkan hubungan tiap kata,

Hasil akurasi dengan menggunakan metode TF-IDF, LDA dan K-Means masih belum menunjukkan hasil yang terlalu tinggi, yaitu hanya 78 %. Sementara pada metode Word2Vec dan K-Means, akurasi menunjukkan hasil yang rendah yaitu 33%. Untuk penelitian selanjutnya dengan menggunakan metode yang sama diharapkan dapat menghasilkan akurasi yang lebih baik lagi dengan cara menambahkan dataset yang digunakan.

Dari 100 artikel ilmiah yang diproses, algoritma TF- IDF, LDA K-means dan graph mengindentifikasi kedalam 4 klaster, dalam pengerjaannya menggunakan bahasa python. dari hasil tersebut disimpulkan bahwa dengan menggunakan metode diatas dapat melakukan klasterisasi sesuai dengan topik yang terdapat dalam artikel ilmiah. Akurasi yang didapatkan berada pada 78 % dengan presisi 81 % dan recall 78% pada metode TF-IDF, LDA, K- means. Sedangkan pada metode Word2Vec dan K-Means mendapatkan hasil akurasi sebesar 33% presisi 39 % recall 33% dan F1 score 34%.


