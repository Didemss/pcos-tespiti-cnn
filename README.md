# 🏥 PCOS Tespiti - CNN ile Derin Öğrenme Projesi

## 📋 Proje Amacı
Polikistik Over Sendromu (PCOS) teşhisi için ultrason görüntülerinden otomatik tespit yapabilen bir derin öğrenme modeli geliştirmek. 
Kadın sağlığı alanında yapay zeka destekli tanı sistemlerine olan ilgim, bu proje konusunu seçmemde en büyük motivasyon kaynağı oldu. Kendi hayatımda da bu alandaki ihtiyaçları ve zorlukları bizzat deneyimlediğim için, bu projeye daha fazla anlam yükleyebiliyorum.
## 📊 Veri Seti Hakkında Bilgi
- *Kaynak:* [PCOS Detection using Ultrasound Images](https://www.kaggle.com/datasets/anaghachoudhari/pcos-detection-using-ultrasound-images)
- *Görsel Sayısı:* 3,856 adet (1,540 eğitim / 1,932 test)
- *Sınıflar:* Sağlıklı vs PCOS'lu (infected/notinfected)
- *Çözünürlük:* 224×224 piksel, RGB
- *Veri Seti Özelliği:* Yumurtalık ultrason görüntüleri üzerinden PCOS tespiti için hazırlanmıştır.

## 🛠️ Kullanılan Yöntemler
- *Veri Ön İşleme:* Normalizasyon, boyut standartizasyonu
- *Data Augmentation:* Döndürme, çevirme, yakınlaştırma, kaydırma
- *CNN Mimarisi:* Konvolüsyonel katmanlar, pooling, dropout
- *Regularization:* L2 regularization, dropout katmanları
- *Hiperparametre Optimizasyonu:* Learning rate, dropout oranı, katman sayısı
- *Görselleştirme:* Grad-CAM ile model interpretability
- *Değerlendirme:* Accuracy, Precision, Recall, F1-Score, Confusion Matrix

## 📈 Elde Edilen Sonuçlar
- *En Yüksek Doğruluk:* %87 test accuracy
- *Recall İyileştirme:* %69 → %87 (PCOS'lu vakaların kaçırılma oranı düşürüldü)
- *Overfitting Kontrolü:* Validation accuracy %100 → %87 (overfitting çözüldü)
- *Grad-CAM Başarısı:* Modelin ultrason görüntülerinde odaklandığı bölgeler görselleştirildi

## 👩‍💻 Proje Hakkında
Akbank Derin Öğrenme Bootcamp kapsamında geliştirilmiştir. Kadın sağlığı ve yapay zeka kesişiminde anlamlı bir proje olması hedeflenmiştir.

https://www.kaggle.com/code/didemsezgin/didem-sezgin-proje
