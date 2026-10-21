# Deteksi Jumlah Jari (3 Jari vs 5 Jari)

Aplikasi web sederhana untuk mengenali apakah tangan yang ditunjukkan ke kamera menampilkan **3 jari** atau **5 jari**. Model klasifikasi gambar dilatih dengan [Teachable Machine](https://teachablemachine.withgoogle.com/) dan dijalankan langsung di browser memakai TensorFlow.js, tanpa server tambahan.
## Link Demo
https://rafhwal.github.io/My-Model-3-Finger-or-5-Finger/

## Fitur

- Prediksi real-time dari kamera (webcam).
- Prediksi dari gambar yang diunggah.
- Menampilkan persentase keyakinan untuk setiap kelas.

## Tentang Model

| Item | Keterangan |
|---|---|
| Platform | Teachable Machine (Image Project) |
| Kelas | `3 Jari/3 Finger`, `5 Jari/5 Finger` |
| Jumlah sampel | Lebih dari 3.000 gambar per kelas |
| Ukuran input | 224 x 224 piksel |
| Format ekspor | TensorFlow.js |

Alur pembuatannya: mengumpulkan sampel gambar untuk tiap kelas lewat webcam, melatih model di Teachable Machine, lalu mengekspornya sebagai model TensorFlow.js.

## Struktur Proyek

```
.
├── index.html   # halaman web, sudah berisi model yang tertanam
└── README.md
```

File `index.html` memuat model (`model.json`, `metadata.json`, dan `weights.bin`) langsung di dalam kodenya, sehingga cukup satu file untuk menjalankan aplikasi.

## Teknologi

- HTML, CSS, JavaScript
- [TensorFlow.js](https://www.tensorflow.org/js) 1.3.1
- [@teachablemachine/image](https://github.com/googlecreativelab/teachablemachine-community) 0.8

## Tips Agar Prediksi Akurat

- Gunakan pencahayaan yang cukup.
- Posisikan tangan di tengah kamera dengan jarak yang mirip saat pengambilan sampel.
- Gunakan latar belakang yang tidak terlalu ramai.

## Pembuat

- Nama: *(La Ode Ihwal Rafael)*
- NIM: *(F1G125037)*
- Mata kuliah: *(Ilmu Komputer)*
- Universitas: *(Universitas HaluOleo)*
