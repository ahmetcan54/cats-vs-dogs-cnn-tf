
# 🐶🐱 CNN ile Kedi ve Köpek Sınıflandırması (TensorFlow + Keras)

Bu proje, TensorFlow ve Keras kullanılarak oluşturulmuş bir Evrişimli Sinir Ağı (CNN) ile kedi ve köpek resimlerini sınıflandırmaya yönelik bir uygulamadır.

Model, Kaggle üzerinden indirilebilen **Dogs vs Cats** veri kümesi ile eğitilmiş olup Google Colab üzerinde çalışacak şekilde yapılandırılmıştır.

---

## 📁 Proje Dosyaları

- `cats_vs_dogs_cnn.ipynb`  
  Veri yükleme, ön işleme, model eğitimi ve değerlendirme gibi tüm adımları içeren Jupyter defteri.

---

## 🔧 Özellikler

- `ImageDataGenerator` ile veri yükleme ve artırma
- Keras Sequential API ile özel CNN mimarisi
- Eğitim süreci görselleştirme (Matplotlib ile)
- Doğrulama sonuçlarının grafikle gösterimi
- Modelin kaydedilmesi

---

## 🚀 Nasıl Çalıştırılır?

1. Google Colab’de dosyayı açın.
2. Gerekirse Google Drive’ı bağlayın.
3. Veri kümesini yükleyin ve çıkarın (veya Kaggle’dan bağlanın).
4. Hücreleri sırasıyla çalıştırın.

---

## 📦 Veri Kümesi

**Dogs vs Cats** veri kümesini Kaggle üzerinden indirebilirsiniz:  
🔗 [https://www.kaggle.com/c/dogs-vs-cats/data](https://www.kaggle.com/c/dogs-vs-cats/data)

Veri klasörü şu şekilde yapılandırılmalıdır:

```
/dataset/
  /train/
    cat.0.jpg
    dog.0.jpg
    ...
```

---

## 🧠 Model Yapısı

- Giriş boyutu: 150x150 RGB görüntüler
- Conv2D + MaxPooling katmanları
- Aşırı öğrenmeyi önlemek için Dropout
- Çıkış: 2 sınıflı sınıflandırma (sigmoid aktivasyon)

---

## 📝 Gereksinimler

Colab ortamında çalışır. Yerel çalıştırmak isterseniz:

```bash
pip install tensorflow matplotlib
```

---

## 📊 Örnek Sonuçlar

Eğitim doğruluğu %90'ın üzerine çıkarken, doğrulama doğruluğu genellikle %85–88 civarında seyretmiştir (veri artırma ve epoch sayısına bağlı olarak).

---

## 📃 Lisans

Bu proje eğitim amaçlıdır. Kaynak göstererek serbestçe kullanılabilir veya değiştirilebilir.

---

## 🙌 Katkı ve Teşekkür

TensorFlow ve Keras dökümantasyonundaki örneklerden ilham alınarak geliştirilmiştir. Derin öğrenmeye giriş amaçlıdır.
