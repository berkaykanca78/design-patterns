# Design Patterns

![Design Patterns](https://sis.binus.ac.id/wp-content/uploads/2021/11/1-10.png)

---

## Creational (Yaratımsal) 
#### 5 Çeşit:
Nesneleri yaratmakta kullanılır.

### 1. Builder
Kod maliyeti olarak biraz fazladır ama okunurluk açısından rahatlık sağlar. Her yapılacak işlem için ayrı metodlarla nesne döndürülür ve en son `Build()` metodunda işlem tamamlanır.

- **Örnek:** Ev inşasında gerekli her bir işlem ayrı metodlarda yapılıp en son build ile tamamlanır.

### 2. Singleton
Sınıf içerisinde tek bir nesne üzerinden ilerlenmesini sağlar.

- **Örnek:** Loglama işleminde tek bir instance üzerinden devam etmek mantıklıdır. İçerisine dizin bilgisi verilip ilgili loglar oraya kaydedilir.

### 3. Abstract Factory
Benzer nesne üretimlerini gerçekleştirebilmek adına her nesne için ayrı bir fabrika sınıfı oluşturmamız gerekmektedir. Ayrıca bu desen, birden fazla Interface kullanımı ile gerçekleştirilir.

- **Örnek:** Klasik ve modern mobilya ve masaları üretmek.

### 4. Prototype
Aynı sınıftan üretilecek olan nesnelerin (birbirleri ile çok ufak farklılıkları olması durumunda) nasıl en verimli şekilde üretileceği problemidir.

- **Örnek:** Kitap satış uygulaması içerisinde kitapları satmadan önce son kullanıcıya kitaba ait ön tanıtım sağlamak.

### 5. Factory
Bir nesne yaratma işlemi için bir üst sınıf kullanılarak alt sınıflardan uygun olanını seçmek.

- **Örnek:** Birden fazla ödeme yöntemi olan bir sistemde ödeme işlemini gerçekleştirmek. Restoran otomasyonunda sipariş verme işleminde yiyecek ve içeceklerin factory design pattern ile nesnelerinin oluşturularak kullanılması.

---

## Structural (Yapısal)
Nesneler arasındaki yapıları ifade eder.

### 1. Proxy
Web sitelerine giderken firewalla uğrayıp ondan sonra sunuculara ulaşılması gibi.

- **Örnek:** Dosya okuma işlemlerinde yetki kontrolü için yapılması.

### 2. Adapter
Farklı metodlar kullanan aynı işleri yapan işlemleri ortak birleştirici adaptör ile bağlamak.

- **Örnek:** Farklı veritabanlarına bağlantı ve sorguları execute ederken kullanılması. (MySQL-MSSQL gibi.)

### 3. Decorator
Nesnelerin farklı kombinasyonlar ile farklı özelliklere sahip olabilmesini (karmaşıklıktan uzak bir şekilde) sağlamak.

- **Örnek:** UI arayüz componentlerinin tasarlandığı bir uygulama. Butonlar, grafikler vs. içermesi.

---

## Behavioral (Davranışsal)
Nesnelerin çalışma zamanına ait davranışlarını değiştirmek için oluşturulur.

### 1. Iterator
Döngü içerisinde kullanılacak işlemlerde yardımcı olur.

- **Örnek:** Yeni bir collection oluşturulup kitap ekleme ve listeleme işlemi için kullanılması.

### 2. Command
Direk çağırmaktansa kapsülleyerek ana class yerine parametre ile başka classa erişimi sağlar.

- **Örnek:** Merhaba ve hoşçakal için ayrı commandlar oluşturulup Invoker üzerinden kapsüllenip ilgili metodların kullanılması.

### 3. Visitor
Farklı türleri aynı interface ile farklı metodlarla sağlar.

- **Örnek:** Alışveriş sepeti farklı ürünler için vergi hesaplama, ayrı classlarda sağlama.

### 4. Template
Algoritma iskeleti tamamlamak, bazı adımları alt sınıfların uygulaması için algoritma yapısı değişmeden belli adımları özelleştirebilirsiniz.

- **Örnek:** İçeceği hazırlama adımları buna örnektir. Tek abstract class içinde işlemler sıraya düzeltilip sabit metodları yazıp classlar inherit edip override edilenleri override edip mevcut class nesne üreterek içecek hazırlar.

### 5. Strategy
Öncelikle bir interface oluşturulur sonra stratejiler belirlenir, class içindeki yapı tasarlanır ve belirlenen stratejiye göre işlemler yapılır.

- **Örnek:** E-Ticaret sitesi ödemede kredi kartı, PayPal, Bitcoin kullanımı için pattern kullanımı.

### 6. State
Nesnenin iş durumuna bağlı davranış değiştirmesine olanak sağlayan, farklı durumlarda farklı işlemler sağlar.

- **Örnek:** Lambanın düğmesinin açılması, kapanması, parlaklığının arttırılıp azaltılması ile ilgili durumlarının kontrolünün sağlanması.

### 7. Memento
Bir nesnenin durumunu kaydedip geriye alma, geriye ve ileri alma işlemlerinde kullanılabilir.

- **Örnek:** Yapılan işlemin aktif/pasif olma durumu ve bunun geriye alınıp bir önceki duruma getirilmesi.

### 8. Chain of Responsibility
Sorumluluk Zinciri, bir isteği bir dizi işleyici (zinciri) boyunca iletmenize izin veren davranışsal bir tasarım desenidir. Karmaşık iş kurallarının olduğu ve iç içe geçmiş birçok if blokları yerine ara sınıflar kullanarak daha yönetilebilir ve okunaklı kodlar yazılmasını sağlar.

- **Örnek:** Çeşitli ürünlerde farklı iskontoların formülize edildiği bir sistemde kullanılması.

---

## Kaynakça
- Taner Saydam - Udemy - YouTube
- Ahmet Babalı - Medium
- Fatih İzgi - Medium
- Ali Furkan Gökçe - Medium
- Evren Bal - Medium
