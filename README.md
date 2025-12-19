# ANALISIS HALVING RANDOM SEARCH CROSS VALIDATION PADA OPTIMASI MODEL MACHINE LEARNING

## Abstrak
Penelitian ini bertujuan menganalisis efektivitas metode Halving Random Search Cross Validation sebagai alternatif optimasi hyperparameter pada model machine learning dibandingkan Grid Search Cross Validation dan Random Search Cross Validation. Dataset yang digunakan adalah Internet Service Churn dengan empat algoritma: KNN, Decision Tree, SVM, dan Gaussian Naive Bayes. Proses pengujian melibatkan 10-fold cross validation dan pengulangan tiga kali untuk memastikan validitas hasil.

Hasil eksperimen menunjukkan bahwa Halving Random Search Cross Validation mampu mencapai performa akurasi, presisi, dan recall yang kompetitif (selisih < 0,5%) dibandingkan Grid Search pada sebagian besar model, dengan penghematan waktu komputasi hingga 62–74% pada KNN, Decision Tree, dan SVM. Namun, pada Gaussian Naive Bayes dengan ruang hyperparameter kecil, metode ini lebih lambat karena overhead successive halving. Random Search menunjukkan kecepatan tinggi tetapi kurang stabil pada SVM dan Gaussian Naive Bayes.

Kesimpulan penelitian menyatakan bahwa Halving Random Search Cross Validation adalah metode paling seimbang untuk kasus bisnis seperti prediksi churn, dengan rekomendasi penerapan pada model kompleks dan pengembangan lanjutan menggunakan Hyperband atau Bayesian Optimization.

## Kata Kunci
Halving Random Search Cross-Validation; Hyperparameter Optimization; Machine Learning

## Rincian Singkat
- Dataset: Internet Service Churn  
- Algoritma: K-Nearest Neighbors (KNN), Decision Tree, Support Vector Machine (SVM), Gaussian Naive Bayes  
- Evaluasi: 10-fold cross validation, 3 pengulangan  
- Pembanding: Grid Search CV, Random Search CV

## Rekomendasi
Untuk penggunaan pada model yang memiliki ruang hyperparameter besar dan kompleksitas tinggi disarankan menerapkan Halving Random Search CV; untuk eksplorasi cepat tetap gunakan Random Search; untuk optimasi lebih lanjut pertimbangkan Hyperband atau Bayesian Optimization.