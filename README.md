Digit Classification Using Convolutional Neural Network With MNIST Dataset

Input Layer:

Convolutional Layer dengan 32 filter, masing-masing berukuran 3x3, menggunakan fungsi aktivasi ReLU.
Input Shape: (28, 28, 1) karena gambar MNIST berukuran 28x28 piksel dengan satu saluran warna (grayscale).
Hidden Layers:

MaxPooling Layer setelah setiap Convolutional Layer dengan ukuran pooling 2x2 untuk mereduksi dimensi spasial.
Convolutional Layer dengan 64 filter, masing-masing berukuran 3x3, menggunakan fungsi aktivasi ReLU.
MaxPooling Layer lagi dengan ukuran pooling 2x2.
Convolutional Layer lagi dengan 64 filter, masing-masing berukuran 3x3, menggunakan fungsi aktivasi ReLU.
Flatten Layer untuk meratakan output dari Convolutional Layers menjadi vektor satu dimensi.
Dense Layer dengan 64 neuron, menggunakan fungsi aktivasi ReLU.
Dense Layer output dengan 10 neuron (sesuai dengan jumlah kelas digit), menggunakan fungsi aktivasi softmax untuk output klasifikasi multikelas.
Optimizer dan Loss Function:

Optimizer: Adam optimizer.
Loss Function: Sparse Categorical Crossentropy, cocok untuk kasus klasifikasi dengan label integer.
Metrik Evaluasi:

Metrik yang digunakan untuk evaluasi adalah akurasi (accuracy), yang mengukur seberapa akurat model dalam memprediksi kelas dari gambar-gambar MNIST.
Model ini kemudian dilatih dengan 5 epoch pada data pelatihan (ds_train) dan divisualisasikan performanya pada data pengujian (ds_test). Setelah pelatihan selesai, dilakukan evaluasi model pada data pengujian untuk mendapatkan nilai loss dan akurasi.

Dari summary model dan hasil training, model memiliki arsitektur yang cukup standar untuk klasifikasi gambar menggunakan CNN dengan dataset MNIST.
