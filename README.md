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

Gunakan Python 3.12. Instal dependensi:

```powershell
python -m pip install -r requirements.txt
```

Buka notebook dari direktori Week yang sesuai dan jalankan sel berurutan. Week 4 memakai dataset lokal. Week 1, 2, 3, dan 5 mengunduh dataset saat pertama dijalankan. Week 6 memakai data sintetis.

## Hasil run lokal

Semua notebook dijalankan dari awal sampai akhir dengan Python 3.12 dan TensorFlow 2.20 di CPU. Output yang tersimpan berasal dari run tersebut.

| Week | Eksperimen | Hasil |
| --- | --- | --- |
| 1 | MNIST, model dropout terpilih | Test accuracy 97,59% |
| 2 | Regresi sederhana NumPy (data sintetis) | Test MAE 6,779 |
| 2 | Regresi sederhana TensorFlow (data sintetis) | Test MAE 8,855 |
| 2 | Auto MPG | Test MAE 1,776 mpg |
| 2 | MNIST softmax | Test accuracy 92,62% |
| 3 | CNN MNIST | Test accuracy 99,13% |
| 4 | SMS spam | Test accuracy 97,8%; PR-AUC 0,9721 |
| 5 | GRU prediksi karakter | Validation loss 2,915 |
| 6 | Transformer pada 12 pasangan sintetis | Exact match 12/12 |

## Sumber data

- MNIST lewat tf.keras.datasets.mnist.
- [Auto MPG, UCI](https://archive.ics.uci.edu/dataset/9/auto+mpg).
- [SMS Spam Collection, UCI](https://archive.ics.uci.edu/dataset/228/sms+spam+collection), disalin dari materi contoh lokal. Kredit: Almeida, Hidalgo, dan Yamakami (2011).
- [Alice's Adventures in Wonderland, Project Gutenberg](https://www.gutenberg.org/ebooks/11) untuk Week 5.

## Batasan

Week 4 membuang 403 teks SMS duplikat sebelum split, tetapi kemiripan pesan yang tidak identik masih bisa memengaruhi evaluasi. Embedding dilatih dari awal. Week 5 memakai korpus terbatas dan tiga epoch; contoh teks keluarannya belum koheren. Week 6 memakai pasangan kalimat sintetis dengan kosakata yang sama di train dan test, sehingga exact match 12/12 belum menunjukkan kemampuan terjemahan umum.
