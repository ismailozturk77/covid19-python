İsmayil Öztürk Ögr No: 132130122 Bursa Uludağ Üniversitesi

**COVID-19 Hastaneye Yatış Tahmini - Python**

Bu proje, COVID-19 hastalarına ait verileri kullanarak bir kişinin hastaneye yatıp yatmayacağını tahmin etmeyi amaçlar. Modelleme süreci Python programlama dili ve scikit-learn kütüphanesi kullanılarak gerçekleştirilmiştir.

🧾 Kullanılan Veri Seti:
- Dosya adı: covid_related_disease_data.csv
- Satır sayısı: 3000
- Önemli sütunlar: Age, Symptoms, Severity, Smoking_Status, BMI
- Hedef değişken: Hospitalized (0 = Yatmadı, 1 = Yattı)

🛠️ Kodun İşleyişi (main.py):
1. Veri yüklenir (`covid_related_disease_data.csv`).
2. Eksik değerler kontrol edilir ve kullanıcıya hangi sütunlarda eksiklik olduğu yazdırılır.
3. Kategorik değişkenler sayısal forma çevrilir (label encoding).
4. Tahmin için kullanılacak sütunlar seçilir: Age, Symptoms, Severity, Smoking_Status, BMI
5. Hedef değişken: Hospitalized
6. Veri eğitim (%80) ve test (%20) olarak ikiye ayrılır.
7. Random Forest sınıflandırıcı modeli oluşturulur ve 10 katlı çapraz doğrulama yapılır.
8. Model test verisiyle değerlendirilir ve doğruluk oranı hesaplanır.
9. Tahmin sonuçları `yes` ve `no` olarak dönüştürülüp `predictions.csv` adlı dosyaya yazılır.

📂 Üretilen Dosyalar:
- predictions.csv: Modelin tahmin ettiği ve gerçek değerleri içeren çıktı dosyası

🔧 Kullanılan Kütüphaneler:
- pandas
- scikit-learn (RandomForestClassifier, accuracy_score, train_test_split, cross_val_score)

🧪 Başlatmak için:
```bash
pip install pandas scikit-learn
python main.py
```

Detaylı açıklama için rapor dosyasına başvurabilirsiniz: https://docs.google.com/document/d/1vkd0lh7qb8zlBHswxsR9Kmu4Oe5tok9i/edit?usp=sharing&ouid=111731595050658472244&rtpof=true&sd=true

