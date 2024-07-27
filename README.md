# Design Patterns

![Design Patterns](https://sis.binus.ac.id/wp-content/uploads/2021/11/1-10.png)

---

## Creational (Yaratımsal)
Nesneleri yaratmakta kullanılır.

| Desen      | Açıklama                                                                                                                                             | Örnek                                                                                       |
|------------|------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| Builder ✔  | Kod maliyeti olarak biraz fazladır ama okunurluk açısından rahatlık sağlar. Her yapılacak işlem için ayrı metodlarla nesne döndürülür ve en son `Build()` metodunda işlem tamamlanır. | Ev inşasında gerekli her bir işlem ayrı metodlarda yapılıp en son build ile tamamlanır.     |
| Singleton ✔| Sınıf içerisinde tek bir nesne üzerinden ilerlenmesini sağlar.                                                                                       | Loglama işleminde tek bir instance üzerinden devam etmek mantıklıdır.                       |
| Abstract Factory ✔ | Benzer nesne üretimlerini gerçekleştirebilmek adına her nesne için ayrı bir fabrika sınıfı oluşturmamız gerekmektedir. Ayrıca bu desen, birden fazla Interface kullanımı ile gerçekleştirilir. | Klasik ve modern mobilya ve masaları üretmek.                                                |
| Prototype ✔| Aynı sınıftan üretilecek olan nesnelerin (birbirleri ile çok ufak farklılıkları olması durumunda) nasıl en verimli şekilde üretileceği problemidir. | Kitap satış uygulaması içerisinde kitapları satmadan önce son kullanıcıya kitaba ait ön tanıtım sağlamak. |
| Factory ✔  | Bir nesne yaratma işlemi için bir üst sınıf kullanılarak alt sınıflardan uygun olanını seçmek.                                                       | Birden fazla ödeme yöntemi olan bir sistemde ödeme işlemini gerçekleştirmek.                 |

---

## Structural (Yapısal)
Nesneler arasındaki yapıları ifade eder.

| Desen      | Açıklama                                                                                                                                             | Örnek                                                                                       |
|------------|------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| Proxy ✔    | Web sitelerine giderken firewalla uğrayıp ondan sonra sunuculara ulaşılması gibi.                                                                    | Dosya okuma işlemlerinde yetki kontrolü için yapılması.                                     |
| Adapter ✔  | Farklı metodlar kullanan aynı işleri yapan işlemleri ortak birleştirici adaptör ile bağlamak.                                                        | Farklı veritabanlarına bağlantı ve sorguları execute ederken kullanılması. (MySQL-MSSQL gibi.)|
| Decorator ✔| Nesnelerin farklı kombinasyonlar ile farklı özelliklere sahip olabilmesini (karmaşıklıktan uzak bir şekilde) sağlamak.                               | UI arayüz componentlerinin tasarlandığı bir uygulama. Butonlar, grafikler vs. içermesi.     |

---

## Behavioral (Davranışsal)
Nesnelerin çalışma zamanına ait davranışlarını değiştirmek için oluşturulur.

| Desen                | Açıklama                                                                                                                                             | Örnek                                                                                       |
|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| Iterator ✔           | Döngü içerisinde kullanılacak işlemlerde yardımcı olur.                                                                                              | Yeni bir collection oluşturulup kitap ekleme ve listeleme işlemi için kullanılması.         |
| Command ✔            | Direk çağırmaktansa kapsülleyerek ana class yerine parametre ile başka classa erişimi sağlar.                                                        | Merhaba ve hoşçakal için ayrı commandlar oluşturulup Invoker üzerinden kapsüllenip ilgili metodların kullanılması.|
| Visitor ✔            | Farklı türleri aynı interface ile farklı metodlarla sağlar.                                                                                          | Alışveriş sepeti farklı ürünler için vergi hesaplama, ayrı classlarda sağlama.              |
| Template ✔           | Algoritma iskeleti tamamlamak, bazı adımları alt sınıfların uygulaması için algoritma yapısı değişmeden belli adımları özelleştirebilirsiniz.          | İçeceği hazırlama adımları buna örnektir. Tek abstract class içinde işlemler sıraya düzeltilip sabit metodları yazıp classlar inherit edip override edilenleri override edip mevcut class nesne üreterek içecek hazırlar.|
| Strategy ✔           | Öncelikle bir interface oluşturulur sonra stratejiler belirlenir, class içindeki yapı tasarlanır ve belirlenen stratejiye göre işlemler yapılır.      | E-Ticaret sitesi ödemede kredi kartı, PayPal, Bitcoin kullanımı için pattern kullanımı.     |
| State ✔              | Nesnenin iş durumuna bağlı davranış değiştirmesine olanak sağlayan, farklı durumlarda farklı işlemler sağlar.                                         | Lambanın düğmesinin açılması, kapanması, parlaklığının arttırılıp azaltılması ile ilgili durumlarının kontrolünün sağlanması.|
| Memento ✔            | Bir nesnenin durumunu kaydedip geriye alma, geriye ve ileri alma işlemlerinde kullanılabilir.                                                          | Yapılan işlemin aktif/pasif olma durumu ve bunun geriye alınıp bir önceki duruma getirilmesi.|
| Chain of Responsibility ✔ | Sorumluluk Zinciri, bir isteği bir dizi işleyici (zinciri) boyunca iletmenize izin veren davranışsal bir tasarım desenidir. Karmaşık iş kurallarının olduğu ve iç içe geçmiş birçok if blokları yerine ara sınıflar kullanarak daha yönetilebilir ve okunaklı kodlar yazılmasını sağlar. | Çeşitli ürünlerde farklı iskontoların formülize edildiği bir sistemde kullanılması.         |

---

## Kaynakça
- Taner Saydam - Udemy - YouTube
- Ahmet Babalı - Medium
- Fatih İzgi - Medium
- Ali Furkan Gökçe - Medium
- Evren Bal - Medium
