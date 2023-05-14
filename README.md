# Gender Classification menggunakan VGG, ResNet and GoogleNet
Dalam Repository ini kelompok kami yakni Al Khwarizmi melakukan implementasi model beberapa model deep learning untuk klasifikasi jenis kelamin (gender) dengan datasets CelebA. Model Deep Learning yang kami coba implementasikan yakni:
- [VGG16](https://github.com/mohammadfikrinursyahbani/FaceClassificationByGender/blob/main/fix_face_classification.ipynb).
- [ResNet-18](https://github.com/mohammadfikrinursyahbani/FaceClassificationByGender/blob/main/ResNet.ipynb)
- [Google Net Inception v1](https://github.com/mohammadfikrinursyahbani/FaceClassificationByGender/blob/main/GoogleNet_Gender_Recognition_.ipynb).

## Strategi Implementasi Model
Dalam implementasi model di atas kami menggunakan beberapa kriteria untuk uji coba yakni:
1. Menguji scope Learning rate yakni 0.001, 0.01 dan 0.1
2. Menguji scope Batch size yakni 16, 32 dan 64 dengan menggunakan hasil learning rate terbaik
3. Menguji scope  Split data yakni 80:20, 70:30 dan 60:40 menggunakan hasil learning rate terbaik.

## Kesimpulan
- Learning rate : Semakin kecil learning rate, loss functionya semakin kecil, namun untuk proses waktu training semakin lama
- Batch_size : Semakin besar, semakin cepat proses training, namun loss function semakin besar
- epoch : Semakin banyak semakin bisa untuk belajar atau training, namun ketika tidak ada perubahan pada akurasi tiap epoch nya, maka besar epoch tidak terlalu berimbas pada model
- split training test 80:20; 70:30; dan 60:40; : Tidak memberikan pengaruh yang signifikan pada akurasi model
- Arsitektur Model : Dalam hal ini model VGG16 dengan learning rate 0.001, 80:20, batch size: 16 dan epoch 20 mendapatkan akurasi paling tinggi sebesar 93.4%.
