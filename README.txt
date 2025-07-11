# Sahte İnceleme Tespiti (Fake Review Detection)

Bu repoda, iki farklı veri seti üzerinde sahte inceleme tespiti için eğitilen modellerin kodları, eğitim ve test çıktıları ile tüm modeller (.pkl) ve vektörizer dosyaları bulunmaktadır.

## Dosya Açıklamaları

- **train_model_FINAL_FIXED.ipynb**  
  1. veri seti ile eğitim yapılan ana Jupyter Notebook dosyasıdır.  
  - Naive Bayes, SVM, LightGBM, MLP modellerinin eğitim kodları ve çıktılarını içerir.
  - Eğitim sonunda modeller ve TF-IDF vektörizer `.pkl` formatında `models` klasörüne kaydedilir.

- **test_model_FINAL_FIXED.ipynb**  
  1. veri seti ile eğitilen modellerin test ve karşılaştırma sonuçlarını içerir.
  - Modelleri ve vektörizeri yükleyip, test skorlarını ve confusion matrix sonuçlarını üretir.

- **train_model_dataset2_FIXED_FINAL.ipynb**  
  2. veri seti ile eğitim yapılan notebook dosyasıdır.
  - Aynı modeller ve yöntemler 2. veri seti için tekrarlanmıştır.

- **test_model_dataset2_FIXED_FINAL.ipynb**  
  2. veri setiyle eğitilen modellerin test skorları ve confusion matrixlerini içerir.

- **models/**  
  Tüm eğitilmiş model ve vektörizer dosyaları (`.pkl`).

- **data/**  
  Kullanılan veri setlerinin orijinal/küçültülmüş halleri (dosya boyutunu düşürmek için küçük alt kümeler).

## Kullanım

1. Gerekli kütüphaneleri yüklemek için `requirements.txt` dosyasını kullanın.
2. Notebookları sırasıyla açıp, çalıştırın veya mevcut çıktıları inceleyin.  
3. Eğitim tamamlandıktan sonra modeller `models/` klasöründe kayıtlı olacak, test notebookları ile performans analizlerini görebilirsiniz.

## Notlar

- Her model ve notebookun çıktıları kayıtlı şekilde bırakılmıştır.
- Eğitim/test kodlarında kullanılan kod bloklarında, dışarıdan alınan kodlar/parametreler için yorum satırı ile referans eklenmiştir.
- Proje, tamamen yerel olarak tekrar edilebilir yapıdadır.

## Referanslar
- scikit-learn ve LightGBM dökümantasyonları:  
  https://scikit-learn.org/stable/, https://lightgbm.readthedocs.io/en/latest/
- Kısa kod adaptasyonu için:  
  https://www.kaggle.com/code/andreshg/naive-bayes-svm-mlp-lightgbm-text-classification

  BERŞAN KAYRA KORKMAZ
  211101062