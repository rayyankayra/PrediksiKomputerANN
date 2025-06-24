# PrediksiKomputerANN

## ⚙️ Teknologi dan Library
- Python 3.x
- PyTorch
- NumPy
- Matplotlib / Seaborn
- scikit-learn

## 🔢 Proses Utama
1. **Data Sintesis**  
   Data sebesar 10.000 baris dibuat menggunakan rumus berbasis arus, tegangan, dan daya. Nilai acak dibuat menggunakan `numpy.random`, dan diatur dengan `np.random.seed(42)` serta `torch.manual_seed(42)` untuk memastikan hasil yang konsisten.

2. **Normalisasi dan Split**  
   Data dinormalisasi menggunakan Min-Max Scaling dan dibagi menjadi 80% data pelatihan dan 20% data uji.

3. **Pelatihan Model**  
   Tiga model dilatih menggunakan optimizer Adam selama 50 epoch. Fungsi loss yang digunakan adalah **Mean Squared Error (MSE)**.

4. **Evaluasi**  
   Model dievaluasi berdasarkan dua metrik:
   - **Mean Absolute Error (MAE)**
   - **Koefisien Determinasi (R²)**

5. **Visualisasi**  
   Hasil training-loss dan MAE antar model divisualisasikan dalam bentuk grafik untuk menunjukkan perbandingan performa.

## 📊 Hasil Singkat
| Model    | MAE YouTube | R² YouTube | MAE Idle | R² Idle |
|----------|-------------|------------|----------|---------|
| SimpleNN | 0.48        | 0.8891     | 0.34     | 0.7135  |
| DeepNN   | 0.55        | 0.8558     | 0.41     | 0.6902  |
| LSTM     | 0.48        | 0.8904     | 0.37     | 0.7001  |

## 💡 Catatan
- Untuk menjalankan kode dengan hasil konsisten, pastikan seed ditetapkan sebelum sintesis data.
- Dataset hasil sintesis akan sama setiap kali kode dijalankan (deterministik).

## ✍️ Penulis
Rayyan Kaira Paraditra  
Universitas Brawijaya — Tugas Akhir 2025

