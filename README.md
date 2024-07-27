# Design Patterns

![Design Patterns](https://sis.binus.ac.id/wp-content/uploads/2021/11/1-10.png)

---

## Creational (Yaratımsal)
Nesneleri yaratmakta kullanılır.

<table>
  <thead>
    <tr>
      <th>#</th>
      <th>Desen</th>
      <th>Açıklama</th>
      <th>Örnek</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Builder</td>
      <td>Kod maliyeti olarak biraz fazladır ama okunurluk açısından rahatlık sağlar. Her yapılacak işlem için ayrı metodlarla nesne döndürülür ve en son `Build()` metodunda işlem tamamlanır.</td>
      <td>Ev inşasında gerekli her bir işlem ayrı metodlarda yapılıp en son build ile tamamlanır.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Singleton</td>
      <td>Sınıf içerisinde tek bir nesne üzerinden ilerlenmesini sağlar.</td>
      <td>Loglama işleminde tek bir instance üzerinden devam etmek mantıklıdır.</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Abstract Factory</td>
      <td>Benzer nesne üretimlerini gerçekleştirebilmek adına her nesne için ayrı bir fabrika sınıfı oluşturmamız gerekmektedir. Ayrıca bu desen, birden fazla Interface kullanımı ile gerçekleştirilir.</td>
      <td>Klasik ve modern mobilya ve masaları üretmek.</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Prototype</td>
      <td>Aynı sınıftan üretilecek olan nesnelerin (birbirleri ile çok ufak farklılıkları olması durumunda) nasıl en verimli şekilde üretileceği problemidir.</td>
      <td>Kitap satış uygulaması içerisinde kitapları satmadan önce son kullanıcıya kitaba ait ön tanıtım sağlamak.</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Factory</td>
      <td>Bir nesne yaratma işlemi için bir üst sınıf kullanılarak alt sınıflardan uygun olanını seçmek.</td>
      <td>Birden fazla ödeme yöntemi olan bir sistemde ödeme işlemini gerçekleştirmek.</td>
    </tr>
  </tbody>
</table>

---

## Structural (Yapısal)
Nesneler arasındaki yapıları ifade eder.

<table>
  <thead>
    <tr>
      <th>#</th>
      <th>Desen</th>
      <th>Açıklama</th>
      <th>Örnek</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Proxy</td>
      <td>Web sitelerine giderken firewalla uğrayıp ondan sonra sunuculara ulaşılması gibi.</td>
      <td>Dosya okuma işlemlerinde yetki kontrolü için yapılması.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Adapter</td>
      <td>Farklı metodlar kullanan aynı işleri yapan işlemleri ortak birleştirici adaptör ile bağlamak.</td>
      <td>Farklı veritabanlarına bağlantı ve sorguları execute ederken kullanılması. (MySQL-MSSQL gibi.)</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Decorator</td>
      <td>Nesnelerin farklı kombinasyonlar ile farklı özelliklere sahip olabilmesini (karmaşıklıktan uzak bir şekilde) sağlamak.</td>
      <td>UI arayüz componentlerinin tasarlandığı bir uygulama. Butonlar, grafikler vs. içermesi.</td>
    </tr>
  </tbody>
</table>

---

## Behavioral (Davranışsal)
Nesnelerin çalışma zamanına ait davranışlarını değiştirmek için oluşturulur.

<table>
  <thead>
    <tr>
      <th>#</th>
      <th>Desen</th>
      <th>Açıklama</th>
      <th>Örnek</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Iterator</td>
      <td>Döngü içerisinde kullanılacak işlemlerde yardımcı olur.</td>
      <td>Yeni bir collection oluşturulup kitap ekleme ve listeleme işlemi için kullanılması.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Command</td>
      <td>Direk çağırmaktansa kapsülleyerek ana class yerine parametre ile başka classa erişimi sağlar.</td>
      <td>Merhaba ve hoşçakal için ayrı commandlar oluşturulup Invoker üzerinden kapsüllenip ilgili metodların kullanılması.</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Visitor</td>
      <td>Farklı türleri aynı interface ile farklı metodlarla sağlar.</td>
      <td>Alışveriş sepeti farklı ürünler için vergi hesaplama, ayrı classlarda sağlama.</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Template</td>
      <td>Algoritma iskeleti tamamlamak, bazı adımları alt sınıfların uygulaması için algoritma yapısı değişmeden belli adımları özelleştirebilirsiniz.</td>
      <td>İçeceği hazırlama adımları buna örnektir. Tek abstract class içinde işlemler sıraya düzeltilip sabit metodları yazıp classlar inherit edip override edilenleri override edip mevcut class nesne üreterek içecek hazırlar.</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Strategy</td>
      <td>Öncelikle bir interface oluşturulur sonra stratejiler belirlenir, class içindeki yapı tasarlanır ve belirlenen stratejiye göre işlemler yapılır.</td>
      <td>E-Ticaret sitesi ödemede kredi kartı, PayPal, Bitcoin kullanımı için pattern kullanımı.</td>
    </tr>
    <tr>
      <td>6</td>
      <td>State</td>
      <td>Nesnenin iş durumuna bağlı davranış değiştirmesine olanak sağlayan, farklı durumlarda farklı işlemler sağlar.</td>
      <td>Lambanın düğmesinin açılması, kapanması, parlaklığının arttırılıp azaltılması ile ilgili durumlarının kontrolünün sağlanması.</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Memento</td>
      <td>Bir nesnenin durumunu kaydedip geriye alma, geriye ve ileri alma işlemlerinde kullanılabilir.</td>
      <td>Yapılan işlemin aktif/pasif olma durumu ve bunun geriye alınıp bir önceki duruma getirilmesi.</td>
    </tr>
    <tr>
      <td>8</td>
      <td>Chain of Responsibility</td>
      <td>Sorumluluk Zinciri, bir isteği bir dizi işleyici (zinciri) boyunca iletmenize izin veren davranışsal bir tasarım desenidir. Karmaşık iş kurallarının olduğu ve iç içe geçmiş birçok if blokları yerine ara sınıflar kullanarak daha yönetilebilir ve okunaklı kodlar yazılmasını sağlar.</td>
      <td>Çeşitli ürünlerde farklı iskontoların formülize edildiği bir sistemde kullanılması.</td>
    </tr>
  </tbody>
</table>

---

## Kaynakça

- **Taner Saydam** - [Udemy](https://www.udemy.com/) - [YouTube](https://www.youtube.com/)
- **Ahmet Babalı** - [Medium](https://medium.com/@ahmetbabali)
- **Fatih İzgi** - [Medium](https://medium.com/@fatihizgi)
- **Ali Furkan Gökçe** - [Medium](https://medium.com/@alifurkangokce)
- **Evren Bal** - [Medium](https://medium.com/@evrenbal)
