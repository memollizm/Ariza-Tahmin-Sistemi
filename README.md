# <p align="center">Arıza Tahmin Sistemi</p>

Bu proje, makine verilerini analiz ederek arıza tahmin sisteminin geliştirilmesine yönelik bir çalışmadır. Proje, endüstriyel makinelerde oluşabilecek arızaları tahmin etmek için makine öğrenmesi ve veri görselleştirme tekniklerini kullanmaktadır. Veriler, AI4I 2020 endüstriyel IoT veri kümesinden alınmış ve çeşitli özellikler (hava sıcaklığı, işlem sıcaklığı, dönme hızı, tork vb.) üzerinden analiz edilmiştir.

<br>
<br>

## Proje Özeti

Proje, makine verilerinin analizini ve arıza tahminini gerçekleştirmek için aşağıdaki adımları izler:

1. **Veri Yükleme ve İşleme:** Veri kümesi `ai4i2020.csv` dosyasından yüklenmiştir. Veriler, Türkçeye çevrilmiş sütun adlarıyla yeniden adlandırılmıştır.
2. **Veri Keşfi ve Görselleştirme:** Veriler üzerinde çeşitli korelasyon analizleri ve dağılım grafikleri oluşturulmuştur. Bu grafikler, değişkenler arasındaki ilişkileri ve anormallikleri analiz etmek için kullanılmıştır.
3. **Makine Öğrenmesi Modelleri:** Projede çeşitli makine öğrenmesi modelleri (Rastgele Ormanlar, Naive Bayes) kullanılarak makine arızası tahmini gerçekleştirilmiştir.
4. **Model Karşılaştırması:** Modellerin doğruluk oranları karşılaştırılmış ve grafikte gösterilmiştir.

<br>

## Kullanılan Teknolojiler

- **Python:** Projenin temel programlama dili.
- **Pandas:** Veri yükleme ve işleme.
- **Seaborn & Matplotlib:** Veri görselleştirme.
- **Scikit-Learn:** Makine öğrenmesi modelleri ve metrik hesaplamaları.
- **t-SNE:** Yüksek boyutlu verilerin iki boyutlu görselleştirilmesi.

<br>

## Veri Kümesi

Veri kümesi, makine sensörlerinden elde edilen çeşitli özellikleri içermektedir:

- **Hava Sıcaklığı [K]**
- **İşlem Sıcaklığı [K]**
- **Dönme Hızı [rpm]**
- **Tork [Nm]**
- **Takım Aşınması [dk]**
- **Makine Arızası Türleri:** 
  - Takım Aşınması Arızası (TWF)
  - Yüksek Hızlı Mil Arızası (HDF)
  - Güç Arızası (PWF)
  - Soğutucu Akışkan Arızası (OSF)
  - Sensör Arızası (RNF)

<br>

## Veri Görselleştirme

Verilerin keşifsel analizi, aşağıdaki grafikler ile gerçekleştirilmiştir:

- **Korelasyon Matrisi:** Veriler arasındaki korelasyonların incelenmesi.
- **Scatter Plot:** Dönme hızı ve tork arasındaki ilişkinin görselleştirilmesi.
- **Box Plot:** Ürün tipine göre hava sıcaklığı dağılımı.
- **Violin Plot:** Ürün tipine göre takım aşınmasının görselleştirilmesi.
- **Bar Plot:** İşlem sıcaklığının güç arızasına etkisi.
- **t-SNE:** Yüksek boyutlu verilerin iki boyutta görselleştirilmesi.

<br>

## Makine Öğrenmesi Modelleri

### 1. Rastgele Ormanlar (Random Forest)

- **Model:** 100 ağaçlı Rastgele Ormanlar modeli kullanılmıştır.
- **Doğruluk Skoru:** Eğitim ve test verileri ile eğitilen modelin doğruluk skoru hesaplanmıştır.
- **Karışıklık Matrisi ve Sınıflandırma Raporu:** Modelin sınıflandırma performansı ölçülmüştür.

### 2. Naive Bayes

- **Model:** Gaussian Naive Bayes modeli.
- **Doğruluk Skoru:** Test verileri ile doğruluk skoru hesaplanmıştır.

<br>

## Sonuçlar ve Model Karşılaştırması

Modellerin doğruluk oranları karşılaştırılmış ve aşağıdaki şekilde görselleştirilmiştir:

- **Rastgele Ormanlar:** %99 doğruluk oranı.
- **Naive Bayes:** %99 doğruluk oranı.

<br>

## Sonuç

Bu proje, makine sensör verileri kullanılarak arıza tahmin sisteminin nasıl geliştirileceğini göstermektedir. Farklı makine öğrenmesi modelleri ile yapılan analizler sonucunda, Rastgele Ormanlar modeli en iyi performansı göstermiştir. Verilerin görselleştirilmesi, arıza tahminini etkileyen faktörlerin daha iyi anlaşılmasını sağlamıştır.
