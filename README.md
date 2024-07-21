# Design Patterns
---
## Creational -  (Yaratımsal) Nesneleri yaratmakta kullanılır.
### 1) Builder: Kod maliyeti olarak biraz fazladır ama okunurluk açısından rahatlık sağlar. Her yapılacak işlem için ayrı metodlarla nesne döndürülür ve en son Build() metodunda işlem tamamlanır. 
- Ev inşasında gerekli her bir işlem ayrı metodlarda yapılıp en son build ile tamamlanması buna bir örnektir.
### 2) Singleton: Sınıf içerisinde tek bir nesne üzerinden ilerlenmesini sağlar. 
- Loglama işleminde tek bir instance üzerinden devam etmek mantıklıdır. İçerisine dizin bilgisi verilip ilgili loglar oraya kaydedilir.
---
## Structural - (Yapısal) Nesneler arasındaki yapıları ifade eder.
### 1) Proxy: Web sitelerine giderken firewalla uğrayıp ondan sonra sunuculara ulaşılması gibi. 
- Dosya okuma işlemlerinde yetki kontrolü için yapılması buna örnektir.
---
## Behavioral -  (Davranışsal) Nesnelerin çalışma zamanına ait davranışlarını değiştirmek için oluşturulur.
### 1) Iterator: Döngü içerisinde kullanılacak işlemlerde yardımcı olur.
- Yeni bir collection oluşturulup kitap ekleme ve listeleme işlemi için kullanılması buna örnektir.
---
#### Kaynakça:
- Taner Saydam - Udemy - YouTube
- Ahmet Babalı - Medium
