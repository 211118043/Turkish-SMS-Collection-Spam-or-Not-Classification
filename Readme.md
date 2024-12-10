# Turkish SMS Collection: Spam or Not Classification

Bu proje, Türkçe SMS mesajlarını spam ya da normal olarak sınıflandırmayı amaçlar. Bu çalışmada veri işleme, özellik mühendisliği ve makine öğrenmesi yöntemleri kullanılmıştır. Amaç, metin tabanlı veriler üzerinde bir sınıflandırma modeli geliştirmek ve performansını ölçmektir.

## Proje İçeriği

### 1. Veri İşleme
- SMS mesajları `Message` ve etiket bilgileri `Group` şeklinde sütunlara ayrılmıştır.
- Eğitim ve test veri setleri, %80-%20 oranında ayrılmıştır.

### 2. Özellik Mühendisliği
- Metin verileri, **TF-IDF (Term Frequency-Inverse Document Frequency)** yöntemi ile sayısal hale getirilmiştir.
- En sık geçen 5000 kelime seçilerek özellikler oluşturulmuştur.

### 3. Model Eğitimi
- **Logistic Regression** algoritması ile sınıflandırma modeli oluşturulmuştur.
- Modelin performansı şu metriklerle değerlendirilmiştir:
  - Accuracy
  - Confusion Matrix
  - Classification Report

### 4. Testler
- Test veri seti üzerindeki tahminlerin yanı sıra, modelin yeni cümleler üzerindeki performansı da değerlendirilmiştir.

## Sonuçlar

### Başarı Skorları
- Modelin doğruluk oranı: **%98.1**
- Confusion Matrix:


### Gözlemler
- Model, "indirim" gibi spam mesajlarda sıkça geçen kelimelere fazla ağırlık verebilir.
- Daha karmaşık modeller (ör. transformers) bağlamı daha iyi yakalayabilir.

**Notebook'u Çalıştırma**
 - Projeyi çalıştırmak için dosyayı bir Jupyter Notebook ortamında açın ve adım adım çalıştırın.

## Öneriler
- Daha yüksek başarı için daha fazla veriyle eğitmek veya bağlamı yakalamak için transformers tabanlı modelleri denemek.
- Eğitim verilerindeki örneklerin çeşitliliğini artırmak.

## İletişim
Bu proje hakkında geri bildirim vermek veya geliştirmelere katkıda bulunmak için iletişime geçebilirsiniz.