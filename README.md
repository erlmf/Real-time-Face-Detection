# Real-time-Face-Detection

Real-Time Face Recognition using Eigenfaces and SVM
This project performs face recognition using PCA (Eigenfaces) and SVM classifier. It also includes real-time detection via webcam.

# Requirements
Python 3.x

pip (Python package installer)

Install Required Libraries
bash
Copy
Edit
pip install opencv-python numpy matplotlib scikit-learn gdown joblib
Pastikan juga webcam di laptop/PC kamu berfungsi dengan baik.

How to Run
Download the code:

Simpan file handson2.py di direktori kerja kamu.

Run the Python script:

bash
Copy
Edit
python handson2.py
Program Flow:

Secara otomatis, script akan download dataset dari Google Drive (face_recognition.zip) dan ekstrak file-nya.

Preprocessing dataset:

Load gambar-gambar wajah.

Deteksi wajah menggunakan Haar Cascade.

Crop, resize, dan flatten wajah.

Training:

Data akan dibagi menjadi train/test set.

Pipeline dengan Mean Centering, PCA, dan SVM akan dilatih.

Evaluation:

Menampilkan classification report.

Menampilkan plot cumulative explained variance PCA.

Menampilkan eigenfaces (principal components).

Saving Model:

Pipeline model akan disimpan sebagai eigenface_pipeline.pkl.

Real-time Recognition:

Webcam akan aktif.

Wajah yang terdeteksi akan diidentifikasi secara real-time.

Confidence score dan label akan ditampilkan di layar.

Exit:

Tekan q pada keyboard untuk keluar dari webcam mode.
