Apple (AAPL) Hisse Senedi Fiyat Tahmin Projesi
Bu proje, Apple Inc. (AAPL) şirketinin geçmiş hisse senedi kapanış fiyatlarını kullanarak gelecekteki fiyat trendlerini tahmin etmek amacıyla geliştirilmiştir. Proje kapsamında geleneksel Makine Öğrenmesi (Linear Regression) ve modern Derin Öğrenme (LSTM & GRU) modelleri karşılaştırmalı olarak analiz edilmiştir.
Kurulum ve Çalıştırma Talimatları
Projeyi yerel bilgisayarınızda çalıştırmak için aşağıdaki adımları takip edebilirsiniz:
Bu depoyu bilgisayarınıza indirin:
git clone https://github.com/Mhytafaburukk/stock-prediction-project.git
Gerekli kütüphaneleri yükleyin:
pip install yfinance pandas matplotlib scikit-learn tensorflow
Jupyter Notebook uygulamasını başlatın ve Apple_Stock_Prediction.ipynb.ipynb dosyasını çalıştırın.
Kullanılan Veri Seti
Kaynak: Yahoo Finance (yfinance kütüphanesi)
Hisse Senedi: Apple (AAPL)
Zaman Aralığı: 2021 - Günümüz (Günlük Kapanış ve İşlem Hacmi Verileri)
Model Performans Karşılaştırmaları (Metrics)
Modellerin test veri seti üzerindeki başarı oranları aşağıdaki hata payı kriterlerine (MSE ve RMSE) göre ölçülmüştür:
Linear Regression: (Notebook çıktındaki MSE ve RMSE değerlerini buraya yazabilirsin)
LSTM: MSE: 133.86, RMSE: 11.57
GRU (Şampiyon): MSE: 57.00, RMSE: 7.55
Proje Bulguları ve Özet Analiz
Linear Regression: Borsa gibi yüksek dalgalanma içeren zaman serilerinde yetersiz kalmıştır. Günlük iniş çıkışları yakalayamayıp sadece genel yükseliş trendini düz bir hat olarak çizebilmiştir.
LSTM vs GRU: Her iki derin öğrenme modeli de zaman serilerindeki geçmiş verileri hafızasında tutma yeteneği sayesinde fiyat hareketlerini son derece başarılı takip etmiştir.
Sonuç: GRU modeli, ani fiyat değişimlerine daha hızlı adapte olan sade mimarisi sayesinde 7.55 RMSE skoru elde ederek projenin en başarılı ve kararlı modeli olmuştur.
Bunu düzenleme ekranına yapıştırıp sağ üstteki yeşil "Commit changes..." butonuna bastığında her şey tamamlanmış olacak!
