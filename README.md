# GDP Analizi
Bu proje, ülkelerin Gayri Safi Yurt İçi Hasıla (GDP) değerleri hakkında derinlemesine bir analiz yapmayı amaçlamaktadır.

## İçerik
Veri manipülasyonu için kullanılan kütüphaneler: numpy ve pandas
Görselleştirme için kullanılan kütüphaneler: seaborn ve matplotlib
Makine öğrenimi için kullanılan kütüphane: sklearn

## Veri İçeriği
Projede, bir CSV dosyasından bir veri çerçevesi data olarak yüklenmiştir.
### Veri İncelemesi
isnull().sum() kullanarak her sütundaki eksik değerlerin sayısını kontrol ediyoruz.
describe() kullanarak veri kümesi hakkında temel istatistikleri görüntülüyoruz.
Dataframenin başlangıcını görmek için başlangıç satırlarını yazdırıyoruz.
### Veri Gruplama
'Region' sütununa göre veriyi gruplayarak 'GDP ($ per capita)', 'Literacy (%)' ve 'Agriculture' için ortanca değerleri buluyoruz.
### Veri İmputasyonu
Eksik değerleri ilgili 'Region'larına göre dolduruyoruz. 'Climate' sütunu için modu, diğerleri için ortancayı kullanıyoruz.
## Görselleştirmeler
GDP per capita'ya göre ilk 20 ülkeyi gösteren bir çubuk grafiği.
![image](https://github.com/mami94/GDP-Analysis/assets/61093189/4fe12fdc-b828-4bea-816d-24f3cedb0497)

Çeşitli sayısal sütunlar arasındaki korelasyonu görselleştiren bir ısı haritası.
![image](https://github.com/mami94/GDP-Analysis/assets/61093189/349f838d-bce9-49db-af6e-97d115880f93)


'GDP ($ per capita)' ile onunla en yüksek mutlak korelasyona sahip diğer altı değişken arasındaki ilişkiyi gösteren dağılım grafikleri.
![image](https://github.com/mami94/GDP-Analysis/assets/61093189/09a2ab7e-6c1f-41e3-b0a1-e3791555a902)

## Özellik Mühendisliği
'Region' ve 'Climate' sütunları etiket kodlanmıştır ve bu kodlanmış değerler 'Region_label' ve 'Climate_label' adında yeni sütunlarda saklanmıştır.
