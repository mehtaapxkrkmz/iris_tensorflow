# Iris Flower Classification with TensorFlow

## Yararlanılan Proje
https://thecleverprogrammer.com/2021/10/17/iris-flower-classification-with-machine-learning/

## Proje Açıklaması
Bu projede, Iris çiçeği türlerini sınıflandırmak için bir yapay sinir ağı (ANN) modeli kullanılmıştır. Veri seti, çiçeklerin yaprak boyutu, genişliği ve petal uzunluğu gibi özelliklere dayalı olarak üç farklı türde sınıflandırılmıştır: *Iris-setosa*, *Iris-versicolor*, ve *Iris-virginica*. Model, TensorFlow ve Keras kullanılarak oluşturulmuştur.

## Kullanılan Kütüphaneler
- `tensorflow`
- `numpy`
- `pandas`
- `matplotlib`
- `plotly`

## Veri Seti
Veri seti, [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/iris)'nden alınmıştır ve her bir çiçeğin 4 özelliğiyle (SepalLength, SepalWidth, PetalLength, PetalWidth) birlikte türünü içerir.

## Model Yapısı
Model, şu iki katmandan oluşan bir yapay sinir ağıdır:
1. **Dense Layer** (8 nöron, `ReLU` aktivasyonu)
2. **Output Layer** (3 nöron, `Softmax` aktivasyonu)

Modelin eğitiminde `sparse_categorical_crossentropy` kayıp fonksiyonu ve `Adam` optimizasyon algoritması kullanılmıştır.

## Eğitim
Model, 50 epoch boyunca eğitilmiştir ve eğitim sırasında doğruluk metriği izlenmiştir.

## Kullanım
Modeli eğitmek ve tahmin yapmak için aşağıdaki adımları izleyebilirsiniz:

1. Gerekli kütüphaneleri yükleyin.
2. Veri setini yükleyin ve eğitime uygun hale getirin.
3. Modeli tanımlayıp derleyin.
4. Modeli eğitin ve doğruluğu izleyin.
5. Yeni verilerle tahmin yapın.

## Sonuç
Model, verilen çiçek özelliklerine göre doğru tür tahmininde bulunur.

## Lisans
Bu proje MIT lisansı ile lisanslanmıştır.
