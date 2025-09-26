# Fruits and Vegetables Image Classification

## Projenin Özeti:
Bu projede, 36 farklı meyve ve sebze sınıfını Evrişimsel Sinir Ağları (CNN) kullanarak yüksek bir doğruluk oranıyla tahmin etmek amaçlanmıştır.

## Verisetinin Tanımı:
Veriseti 36 farklı meyve ve sebze türünün görüntülerini içermektedir.
Train, test, validation olmak üzere dağılmıştır.
Dengeli bir verisetidir.

## Uygulanan Yöntemler:

### Veri Ön İşleme:
Tüm görüntüler (128,128) boyutuna getirilmiştir.
Projede geliştirilen ilk modelin %77 doğruluk oranına sahip olduğu gözlemlenmiştir. %92 oranına sahip olan Validation Accuracy ile arasında %15 gibi büyük bir fark olması modelin overfitting ettiğini göstermiştir. Bunu engellemek amacıyla Data Augmentation uygulanmış ve doğruluk oranı %96'ya ulaşmıştır.

### Model Mimarisi: 
CNN mimarisi tercih edilmiştir.
Model, üç ardışık Evrişim (Conv2D) ve Pooling (MaxPooling2D) bloğundan oluşur.
'adam' optimizasyon algoritması kullanılmıştır.
İki farklı Dropout eklenerek overfitting engellenmeye çalışılmıştır.

### Görsel Analiz:
Doğruluk ve kayıp eğrileri görselleştirilmiştir.


#### Kaggle Linki:
https://www.kaggle.com/code/iremcibelek/fruit-vegetable-image-classification

* .ipynb dosya boyutum 10.3 mb olduğu için GitHub'a yüklemekte sıkıntı yaşadım. Dosya boyutunu küçültmek adına bazı output görsellerini çalıştırmadan yüklüyorum. Projenin son ve eksiksiz hali Kaggle'daki halidir.
