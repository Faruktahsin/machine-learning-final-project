# Breast Cancer Classification

Türkiye Yapay Zeka Akademisi Makine Öğrenmesi Final Ödevi kapsamında hazırlanmış uçtan uca makine öğrenmesi projesidir.

## Projenin Amacı

Bu projede Breast Cancer Wisconsin veri setindeki tümör özellikleri kullanılarak tümörlerin iyi huylu (benign) veya kötü huylu (malignant) olarak sınıflandırılması amaçlanmıştır.

## Veri Seti

Scikit-learn içerisinde bulunan Breast Cancer Wisconsin veri seti kullanılmıştır.

Veri seti 569 gözlemden oluşmaktadır.

Hedef değişken:

- `0`: Malignant
- `1`: Benign

Veri seti doğrudan scikit-learn üzerinden yüklendiği için projeyi çalıştırmak için harici bir veri dosyasına ihtiyaç yoktur.

## Uygulanan Adımlar

- Veri inceleme
- Eksik değer kontrolü
- Aykırı değer analizi
- Öznitelik mühendisliği
- One-Hot Encoding
- StandardScaler ile ölçekleme
- SelectKBest ile öznitelik seçimi
- Train / Validation / Test ayrımı
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Validation performanslarının karşılaştırılması
- 5-Fold Cross Validation
- GridSearchCV ile hiperparametre optimizasyonu
- Final test değerlendirmesi
- Confusion Matrix
- Permutation Feature Importance

## Model Değerlendirmesi

Modeller Accuracy, Precision, Recall ve F1 Score metrikleri kullanılarak karşılaştırılmıştır.

Validation sonuçlarına göre en başarılı model seçilmiş, ardından 5-Fold Cross Validation ve GridSearchCV ile modelin performansı değerlendirilmiştir.

Son aşamada seçilen model daha önce kullanılmamış test verisi üzerinde değerlendirilmiştir.

Detaylı model sonuçları ve grafikler notebook dosyasında bulunmaktadır.

## Çalıştırma

Projeyi çalıştırmak için gerekli temel kütüphaneler:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
