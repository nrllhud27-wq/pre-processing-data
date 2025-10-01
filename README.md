# pre-processing-data
## Konteks

Data mining merupakan salah satu tahapan penting dalam analisis data, dimana kualitas data sangat menentukan hasil analisis. Sebelum dilakukan proses analisis lebih lanjut, data perlu melalui tahap preprocessing agar lebih bersih, konsisten, dan siap digunakan. Pada tugas ini, preprocessing dilakukan terhadap dataset film yang memuat informasi seperti nama sutradara, durasi, pendapatan, genre, dan atribut lainnya.

## Problem Statement

Data mentah sering kali mengandung nilai yang hilang, tidak konsisten, atau tidak standar. Jika data tersebut langsung digunakan untuk analisis, maka hasil yang diperoleh bisa bias atau tidak akurat. Oleh karena itu, diperlukan proses preprocessing untuk:
- Menghapus nilai hilang pada kolom penting (misalnya budget dan gross).
- Menstandarkan nilai yang tidak konsisten (misalnya perbedaan penulisan "Color" dan "color").
- Mengatasi nilai tidak valid seperti "?" atau "N/A".
- Melakukan transformasi data agar lebih terstruktur (contohnya genre yang dipisahkan menjadi beberapa kolom).

## Tujuan

Tujuan dari tugas ini adalah:
- Melatih keterampilan dalam melakukan preprocessing data menggunakan Python dan Pandas.
- Membersihkan data sehingga dapat digunakan untuk analisis lebih lanjut.
- Menyimpan dataset yang sudah bersih dengan format baru sebagai output akhir.

## Dataset

Dataset yang digunakan adalah movie_sample_dataset.csv, berisi data film dengan beberapa atribut penting, di antaranya:

- color
- Nama sutradara (director_name)
- Durasi film (duration)
- Pendapatan (gross)
- Genre (genres)
- Judul Film (Movie Tittle)
- Tahun (Tittle year)
- Bahasa (Language)
- Negara (Country)
- Budget
- imdb_score
- actors
- movie_facebook_likes


## Hasil 

Tahapan preprocessing yang dilakukan meliputi:
- Memuat Data – Mengimpor dataset menggunakan Pandas ke dalam DataFrame.
- Memeriksa Data – Melihat struktur data, tipe data, dan mengecek jumlah nilai yang hilang pada setiap kolom.
- Membersihkan Data
- Menghapus baris dengan nilai kosong pada kolom budget dan gross.
- Menghapus nilai tidak standar seperti "?" dan "N/A".
- Menstandarkan format teks, misalnya "Color" menjadi "color".
- Transformasi Data
- Membuat dummy variables untuk genre menggunakan teknik one-hot encoding.
- Melakukan normalisasi teks agar konsisten (diubah menjadi huruf kecil dan di-strip).
- Menyimpan Data – Dataset hasil preprocessing disimpan sebagai csv

## Kesimpulan

Hasil preprocessing menunjukkan bahwa dataset yang awalnya berisi nilai hilang dan inkonsistensi berhasil dibersihkan. Data menjadi lebih rapi, tidak ada nilai kosong pada kolom penting, dan sudah siap digunakan untuk analisis data mining selanjutnya.

## Rekomendasi

Tahapan preprocessing sebaiknya selalu dilakukan sebelum analisis agar hasil yang diperoleh akurat. Untuk dataset yang lebih besar, dapat ditambahkan teknik scaling atau normalization numerik agar model analisis lebih optimal. Ke depan, proses cleaning bisa dikembangkan dengan automasi sehingga lebih efisien untuk dataset berskala besar.
