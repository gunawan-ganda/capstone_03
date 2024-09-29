# **Bike Sharing**

## **Business Problem Understanding**
### **Context**
Bike sharing adalah sebuah layanan yang menyediakan sepeda untuk disewa secara sementara oleh pengguna, biasanya dalam waktu yang singkat, seperti beberapa jam atau hari. Layanan ini bertujuan untuk memberikan alternatif transportasi yang ramah lingkungan, efisien, dan terjangkau bagi masyarakat.

Perusahaan bike sharing menghadapi tantangan untuk memenuhi permintaan pengguna yang dinamis di berbagai waktu. Pengguna sering kali kesulitan menemukan sepeda yang tersedia. Masalah ini dapat menyebabkan ketidakpuasan pelanggan dan inefisiensi operasional, seperti biaya logistik yang tinggi untuk meredistribusi sepeda. Mengelola ketersediaan sepeda dengan lebih akurat berdasarkan permintaan dapat membantu meningkatkan efisiensi dan pengalaman pelanggan.

### **Problem Statement**
Perusahaan perlu memprediksi jumlah pengguna sepeda pada waktu tertentu untuk mengoptimalkan penyediaan sepeda dan meningkatkan tingkat ketersediaan yang sesuai dengan kebutuhan. Gagalnya prediksi permintaan yang tepat dapat menyebabkan ketidakpuasan pelanggan karena kurangnya sepeda yang tersedia atau sebaliknya, terlalu banyak sepeda yang tidak digunakan.

### **Goals**
- Primary Goal: Memprediksi jumlah penyewaan sepeda pada waktu yang berbeda dengan akurasi tinggi, sehingga perusahaan dapat mendistribusikan sepeda dengan lebih efisien.
- Secondary Goal: Mengurangi biaya operasional yang terkait dengan redistribusi sepeda dan meningkatkan kepuasan pelanggan dengan memastikan ketersediaan sepeda sesuai permintaan.

### **Analytic Approach**
Untuk mencapai tujuan tersebut, pendekatan analitis berbasis machine learning akan digunakan:
- Data Collection & Preprocessing: Mengumpulkan data historis penyewaan sepeda, termasuk informasi waktu, data cuaca, dan variabel lain yang relevan; Membersihkan data dari anomali atau nilai yang hilang serta melakukan feature engineering seperti pengelompokan waktu.
- Model Selection: Menggunakan model prediksi regresi untuk memprediksi jumlah penyewaan sepeda.
- Training & Testing: Melatih model untuk menguji performa dan mencegah overfitting; Hyperparameter Tuning dilakukan untuk memilih model terbaik yang mampu menghasilkan prediksi paling akurat.

### **Metric Evaluation**
Untuk mengevaluasi keberhasilan model prediksi, beberapa metrik evaluasi dapat digunakan, antara lain:
- Root Mean Squared Error (RMSE): Akar dari MSE, metrik ini memberikan pandangan lebih intuitif tentang kesalahan prediksi dalam skala asli data.
- Mean Absolute Error (MAE): Mengukur rata-rata perbedaan absolut antara nilai sebenarnya dengan nilai prediksi. Metrik ini memberikan gambaran seberapa besar rata-rata kesalahan prediksi tanpa memedulikan arah (underestimate atau overestimate).
- Mean Absolute Percentage Error (MAPE): Rataan persentase error yang dihasilkan oleh model regresi.

Semakin kecil nilai RMSE, MAE, dan MAPE yang dihasilkan, berarti model semakin akurat dalam memprediksi jumlah penyewaan sepeda sesuai dengan limitasi fitur yang digunakan.