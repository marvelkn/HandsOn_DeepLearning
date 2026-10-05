# Deep Learning Weekly Task

Marvel Kevin Nathanael

NIM: 00000108042

Pengerjaan hands-on berdasarkan TLM Week 1–6 dan contoh kode dari [Packt, Deep Learning with TensorFlow and Keras 3rd edition](https://github.com/PacktPublishing/Deep-Learning-with-TensorFlow-and-Keras-3rd-edition). Struktur dan pola nama mengikuti folder Weekly_Task yang diberikan di kelas. Kode notebook ditulis ulang untuk pengerjaan ini.

| Week | Materi | File |
| --- | --- | --- |
| 1 | MNIST: baseline, MLP, dropout | 1 notebook |
| 2 | Regresi sederhana, regresi multipel, klasifikasi | 4 notebook |
| 3 | CNN untuk MNIST | 1 notebook |
| 4 | Word embedding dan SMS spam | 1 notebook |
| 5 | GRU untuk prediksi karakter | 1 notebook |
| 6 | Transformer encoder-decoder | 1 notebook |

## Menjalankan

Gunakan Python 3.12. Instal dependensi dengan pip install -r requirements.txt, lalu buka notebook dari direktori Week yang sesuai. Week 4 memakai dataset lokal. Week 1, 2, 3, dan 5 mengunduh dataset saat pertama dijalankan. Week 6 memakai data sintetis.

Notebook disimpan tanpa output agar angka hasil berasal dari run sendiri. Jalankan sel berurutan, lalu simpan notebook jika output akan dikumpulkan. Lingkungan pembuat repo tidak menyediakan TensorFlow, sehingga eksperimen belum dieksekusi di sini.

## Sumber data

- MNIST lewat tf.keras.datasets.mnist.
- [Auto MPG, UCI](https://archive.ics.uci.edu/dataset/9/auto+mpg).
- [SMS Spam Collection, UCI](https://archive.ics.uci.edu/dataset/228/sms+spam+collection), disalin dari materi contoh lokal. Kredit: Almeida, Hidalgo, dan Yamakami (2011).
- [Alice's Adventures in Wonderland, Project Gutenberg](https://www.gutenberg.org/ebooks/11) untuk Week 5.

## Batasan

Week 4 memakai embedding yang dilatih dari awal. Week 5 melatih GRU kecil selama lima epoch. Week 6 memakai pasangan kalimat sintetis, sehingga evaluasinya hanya memeriksa alur Transformer, bukan kemampuan terjemahan umum.
