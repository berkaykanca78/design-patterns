![Design Patterns](https://sis.binus.ac.id/wp-content/uploads/2021/11/1-10.png)

---

[20 / 23] (Kalan : 3)

---

## Creational (Yaratımsal) ✔
Nesneleri yaratmakta kullanılır.

| #  | Desen          | Açıklama                                                                                                    | Örnek                                                             |
|----|-----------------|-------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------|
| 1  | Builder         | Kod maliyeti olarak biraz fazladır ama okunurluk açısından rahatlık sağlar. Her yapılacak işlem için ayrı metodlarla nesne döndürülür ve en son `Build()` metodunda işlem tamamlanır. | Ev inşasında gerekli her bir işlem ayrı metodlarda yapılıp en son build ile tamamlanır. |
| 2  | Singleton       | Sınıf içerisinde tek bir nesne üzerinden ilerlenmesini sağlar.                                             | Loglama işleminde tek bir instance üzerinden devam etmek mantıklıdır. |
| 3  | Abstract Factory| Benzer nesne üretimlerini gerçekleştirebilmek adına her nesne için ayrı bir fabrika sınıfı oluşturmamız gerekmektedir. Ayrıca bu desen, birden fazla interface kullanımı ile gerçekleştirilir. | Klasik ve modern mobilya ve masaları üretmek.                    |
| 4  | Prototype       | Aynı sınıftan üretilecek olan nesnelerin (birbirleri ile çok ufak farklılıkları olması durumunda) nasıl en verimli şekilde üretileceği problemidir. | Kitap satış uygulaması içerisinde kitapları satmadan önce son kullanıcıya kitaba ait ön tanıtım sağlamak. |
| 5  | Factory         | Bir nesne yaratma işlemi için bir üst sınıf kullanılarak alt sınıflardan uygun olanını seçmek.                | Birden fazla ödeme yöntemi olan bir sistemde ödeme işlemini gerçekleştirmek. |

---

## Structural (Yapısal) ✔
Nesneler arasındaki yapıları ifade eder.

| #  | Desen          | Açıklama                                                                                                    | Örnek                                                             |
|----|-----------------|-------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------|
| 1  | Proxy           | Web sitelerine giderken firewalla uğrayıp ondan sonra sunuculara ulaşılması gibi.                         | Dosya okuma işlemlerinde yetki kontrolü için yapılması.           |
| 2  | Adapter         | Farklı metodlar kullanan aynı işleri yapan işlemleri ortak birleştirici adaptör ile bağlamak.               | Farklı veritabanlarına bağlantı ve sorguları execute ederken kullanılması. (MySQL-MSSQL gibi.) |
| 3  | Decorator       | Nesnelerin farklı kombinasyonlar ile farklı özelliklere sahip olabilmesini (karmaşıklıktan uzak bir şekilde) sağlamak. | UI arayüz componentlerinin tasarlandığı bir uygulama. Butonlar, grafikler vs. içermesi. |
| 4  | Facade          | Karmaşık sistem veya alt sistemlerin daha basit ve anlaşılır arayüzle yönetilmesini sağlar.               | Alt sistemler için classlarımız olsun operasyon yönetsin. Facade ile kapsüllersek yönetmesi kullanması daha kolay olur. |
| 5  | Flyweight       | Çok sayıda benzer nesneye ihtiyaç duyulması problemine çözüm olarak getirilmiştir.                        | İkili oyunlarda ağaç yerleştirme için nesne üretmek zorundayız, flyweight ile bellek optimizasyonu sağlanabilir. Aynı ağaç, farklı noktalara nesne üretmeden kullanılabilir. Orman olacak ormana tek tek ağaç ekleme yapacağız bunun konum bilgilerini ve ağaç türünü vereceğiz. |
| 6  | Bridge          | Gerçekleştirimleri soyutlayarak birbirlerini iletişim kurabilecekleri bir köprü yapısı kurarak hiyerarşik karmaşıklığın önüne geçmeye çalışır. | TV Radyo gibi cihazlarda kumanda işlemleri için metotları yazıp kullanalım.
| 7  | Composite       | Nesneleri ağaç yapısına göre düzenleyerek ağaç yapısındaki alt üst ilişkisini kurmaya yarayan bir desendir. |  Şirklet çalışan hiyeraşiasi çalışan ve yöneitlr altında bşaka yönetici ve çalışanmlar çalışan hiyerarişisi modelleme işlemi için kullanalım. |
---

## Behavioral (Davranışsal)
Nesnelerin çalışma zamanına ait davranışlarını değiştirmek için oluşturulur.

| #  | Desen                  | Açıklama                                                                                                    | Örnek                                                             |
|----|------------------------|-------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------|
| 1  | Iterator               | Döngü içerisinde kullanılacak işlemlerde yardımcı olur.                                                    | Yeni bir collection oluşturulup kitap ekleme ve listeleme işlemi için kullanılması. |
| 2  | Command                | Direkt çağırmaktansa kapsülleyerek ana class yerine parametre ile başka classa erişimi sağlar.              | Merhaba ve hoşçakal için ayrı commandlar oluşturulup Invoker üzerinden kapsüllenip ilgili metodların kullanılması. |
| 3  | Visitor                | Farklı türleri aynı interface ile farklı metodlarla sağlar.                                               | Alışveriş sepetinde farklı ürünler için vergi hesaplamayı, ayrı classlarda sağlama. |
| 4  | Template               | Algoritma iskeleti tamamlamak, bazı adımları alt sınıfların uygulaması için algoritma yapısı değişmeden belli adımları özelleştirebilirsiniz. | İçeceği hazırlama adımları buna örnektir. Tek abstract class içinde işlemler sıraya dizilip sabit metodları yazıp classlar inherit edilerek override edilenler ile içecek hazırlanır. |
| 5  | Strategy               | Öncelikle bir interface oluşturulur, sonra stratejiler belirlenir, class içindeki yapı tasarlanır ve belirlenen stratejiye göre işlemler yapılır. | E-Ticaret sitesinde ödemede kredi kartı, PayPal, Bitcoin kullanımı için pattern kullanımı. |
| 6  | State                  | Nesnenin iş durumuna bağlı davranış değiştirmesine olanak sağlayan, farklı durumlarda farklı işlemler sağlar. | Lambanın düğmesinin açılması, kapanması, parlaklığının arttırılıp azaltılması ile ilgili durumlarının kontrolünün sağlanması. |
| 7  | Memento                | Bir nesnenin durumunu kaydedip geriye alma, ileri ve geri alma işlemlerinde kullanılabilir.                | Yapılan işlemin aktif/pasif olma durumu ve bunun geriye alınıp bir önceki duruma getirilmesi. |
| 8  | Chain of Responsibility| Sorumluluk Zinciri, bir isteği bir dizi işleyici (zinciri) boyunca iletmenize izin veren davranışsal bir tasarım desenidir. Karmaşık iş kurallarının olduğu ve iç içe geçmiş birçok if blokları yerine ara sınıflar kullanarak daha yönetilebilir ve okunaklı kodlar yazılmasını sağlar. | Çeşitli ürünlerde farklı iskontoların formülize edildiği bir sistemde kullanılması. |
| 9  | Observer               | Observer pattern, bir nesne kümesi arasındaki one-to-many ilişkiyi tanımlar. Bir nesnenin durumu değiştiğinde, bütün bağımlılarına bildirilir. | Hava istasyonu sıcaklık ve nem ölçsün, mobil bilgisayar uygulaması LCD ekranına isteyen bağlı kaldıkça alabilsin. Hangileri register edilmişse onları gösterir, unregister olanı çıkarır. |

---

## Kaynakça

| Yazar            | Kaynak                                |
|------------------|---------------------------------------|
| **Taner Saydam** | [Udemy](https://www.udemy.com/) - [YouTube](https://www.youtube.com/) |
| **Ahmet Babalı** | [Medium](https://medium.com/@ahmetbabali) |
| **Fatih İzgi**   | [Medium](https://medium.com/@fatihizgi) |
| **Ali Furkan Gökçe** | [Medium](https://medium.com/@alifurkangokce) |
| **Evren Bal**    | [Medium](https://medium.com/@evrenbal) |
| **Buse Tekin Ay** | [Medium](https://medium.com) |
| **Onur Dayıbaşı** | [Medium](https://medium.com) |
| **Veysel Mutlu** | [Medium](https://medium.com) |
