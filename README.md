# 🚢 Titanic Survival Prediction – EDA & Logistic Regression

Bu proje, Titanic yolcularının hayatta kalma durumunu etkileyen faktörleri analiz etmek ve bir makine öğrenmesi modeli yardımıyla bu durumu tahmin etmeyi amaçlamaktadır.

## Proje Aşamaları

### 1. Veri Seti
- Kullanılan veri: [Seaborn Titanic dataset](https://github.com/mwaskom/seaborn-data/blob/master/titanic.csv)
- Toplam 891 satır, 15+ sütun
- Hedef değişken: `survived` (0 = öldü, 1 = hayatta)

### 2. EDA (Exploratory Data Analysis)
- Eksik veriler tespit edildi (`age`, `deck`, `embarked`)
- Cinsiyet, sınıf ve hayatta kalma ilişkileri analiz edildi
- Boxplot'larla `fare` ve `age` değişkenlerinde aykırı değerler gözlemlendi

### 3. Özellik Mühendisliği
- Kategorik veriler (`sex`, `embarked`) etiketlendi
- Kullanılan özellikler:
  - `pclass`, `sex`, `age`, `fare`, `sibsp`, `parch`
- Hedef: `survived`

### 4. Modelleme
- Model: **Logistic Regression**
- Eğitim/Test ayrımı: %80 / %20
- Model Başarısı:
  - Accuracy: **%82**
  - F1-Score: 0.83 (ölü) / 0.79 (hayatta)

### 5. Değerlendirme
- Confusion matrix ile tahmin performansı görselleştirildi
- Özellik önem katsayıları bar grafiği ile yorumlandı

---

## 📈 Sonuçlar

| Metric      | Değer |
|-------------|-------|
| Accuracy    | 82.5% |
| Precision   | 85% (hayatta olmayan) |
| Recall      | 85% (hayatta olmayan) |
| F1-Score    | 83% (ortalama) |

---

## 🔧 Kullanılan Kütüphaneler
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`

---


