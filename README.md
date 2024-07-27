# Design Patterns
<img src="https://sis.binus.ac.id/wp-content/uploads/2021/11/1-10.png"/>

---
## Creational -  (Yaratımsal) Nesneleri yaratmakta kullanılır.
### 1) Builder: Kod maliyeti olarak biraz fazladır ama okunurluk açısından rahatlık sağlar. Her yapılacak işlem için ayrı metodlarla nesne döndürülür ve en son Build() metodunda işlem tamamlanır. 
- Ev inşasında gerekli her bir işlem ayrı metodlarda yapılıp en son build ile tamamlanması buna bir örnektir.
### 2) Singleton: Sınıf içerisinde tek bir nesne üzerinden ilerlenmesini sağlar. 
- Loglama işleminde tek bir instance üzerinden devam etmek mantıklıdır. İçerisine dizin bilgisi verilip ilgili loglar oraya kaydedilir.
### 3) Abstract Factory: Benzer nesne üretimlerini gerçekleştirebilmek adına her nesne için ayrı bir fabrika sınıfı oluşturmamız gerekmektedir. Ayrıca bu desen, birden fazla Interface kullanımı ile gerçekleştirilir.  
- Klasik ve modern mobilya ve masaları üretmek için bir örnek yapabiliriz.
---
## Structural - (Yapısal) Nesneler arasındaki yapıları ifade eder.
### 1) Proxy: Web sitelerine giderken firewalla uğrayıp ondan sonra sunuculara ulaşılması gibi. 
- Dosya okuma işlemlerinde yetki kontrolü için yapılması buna örnektir.
### 2) Adapter: Telefonlardan adaptöre hangisi bağlıysa o çalışır gibi düşünelim.  Farklı metodlar kullanan aynı işleri yapan işlemleri ortak birleştirici adaptör ile bunları bağlayabiliriz.
- Farklı veritabanlarına bağlantı ve sorguları execute ederken kullanabiliriz. MySql- MsSql gibi..
### 3) Decorator: Decorator Design Pattern, nesnelerin farklı kombinasyonlar ile farklı özelliklere sahip olabilmesini (karmaşıklıktan uzak bir şekilde) sağlamak amacı ile kullanılır. 
- UI Arayüz componentlerinin tasarlandığı bir uygulama. Butonlar, grafikler vs içermesi.
---
## Behavioral -  (Davranışsal) Nesnelerin çalışma zamanına ait davranışlarını değiştirmek için oluşturulur.
### 1) Iterator: Döngü içerisinde kullanılacak işlemlerde yardımcı olur.
- Yeni bir collection oluşturulup kitap ekleme ve listeleme işlemi için kullanılması buna örnektir.
### 2) Command: Direk çağırmaktansa kapsülleyerek ana class yerine paramtere ile başka classa erişimi.
- Merhaba ve hoşçakal için ayrı commandlar oluşturulup Invoker üzerinden kapsüllenip bundan türetilip iligli metodların kullanılması.
### 3) Visitor: Farklı türleri aynı interface ile farklı metodlarla sağlar.
- Alışveriş sepeti farklı ürünler için vergi hesaplama, ayrı classlarda sağlama.
### 4) Template: Algoritma iskeleti tamamlamak bazı adımları alt sınıfların uygulaması için algoritma yapısı değişmeden belli adımları özelleştirebilirsiniz.
- İçeceği hazırlama adımları buna örnektir. Tek abstract class içinde işlemler sıraya düzeltilip sabit meotdları yazıp classlar inherit edip override edilenleri override edip içerisinde mevcut class nesne ürete içecek hazırlar,classa göre hazırlama.
### 5) Strategy: Öncelikle bir interfece oluşturulur sonra strajeiler berlierlenir class içindeki yapı tasaralanır ve belirlenen stratejiye göre işlemler yapılır.
- E-Ticaret sitesi ödemede: ister kredi kartı ister paypal ister bitcoin kullanımı için pattern kullanımı
### 6) State: Nesne iş durumuna bağlı davarnış değiştirmesien olanak sağlayan, farklı durumlarada farklı işlemler sağlar. İhtiyaca göre durumların kolayca dönüştürlmesini sağlayan bir tasarım desenidir.
- Lambanın düğmesinin açılması kapanması parlaklığının arttırılıp azaltılması ile ilgili durumlarının kontorlünün sağlanması buna örnektir.
### 7) Memento: Bir nesnenin durmunu kaydedip geriye gelme, geriye ve ileri al işlemlerinde kullanılabilir.
- Yapılan işlemin aktif/pasif olma durumu ve bunun geriye alınıp bir önceki duruma getirlmesi örnek olabilir.
### 8) Chain Of Responsibility: Sorumluluk Zinciri, bir isteği bir dizi işleyici (zinciri) boyunca iletmenize izin veren davranışsal bir tasarım desenidir .Karmaşık iş kurallarının olduğu ve iç içe ve birsürü if blokları ile yapacağımız işler yerine ara sınıflar kullanarak daha yönetilebilir ve okunaklı kodlar yazılmasını sağlar.
- Çeşitli ürünlerde farklı iskontoların formülize edildiği bir sistemde kullanılabilir.
---
#### Kaynakça:
- Taner Saydam - Udemy - YouTube
- Ahmet Babalı - Medium
- Fatih İzgi - Medium
- Ali Furkan Gökçe - Medium
- Evren Bal - Medium
