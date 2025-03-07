# ECommerceAngular

🏗️ Mimari Özellikler:

Microservices mimarisi ve API Gateway (Ocelot) ile modüler yapı
Carter ile Minimal API kullanımı
Domain Events ile modüler tasarım
.NET 9 backend, Entity Framework, MediatR ve CQS pattern
Angular + Capacitor (Ionic) ile hem web hem mobil uyumlu ön yüz
Grid, Selectbox gibi özel UI bileşenleri
Google Cloud üzerinde NGINX ile deployment

💪 Teknik Özellikler:

Kafka ve Debezium ile Outbox Pattern kullanarak veri tutarlılığı
SignalR ile gerçek zamanlı bildirim ve veri güncelleme sistemi
RabbitMQ, MassTransit ve gRPC ile servisler arası iletişim
Şu an MSSQL kullanıyor yakında PostgreSQL'e geçiş sağlıyıcam
Elasticsearch ile güçlü arama özellikleri
Consul ile Service Discovery
Redis ile Cache stratejileri
Polly ile hata toleransı
Hangfire ile arka plan görev planlaması
Jenkins ile CI/CD
Serilog ile Centralized Log yönetimi
Docker ile Containerization ve Mikroservis dağıtımı
OpenTelemetry ve Zipkin ile Tracing and Monitoring
Prometheus ve Grafana ile Metrik toplama ve Görselleştirme

🛒 E-Ticaret Özellikleri:

UI Bileşenleri
Grid: Kullanıcı istediği gridde istediği sütunların gözükmesini sağlıyabiliyor.İstediği sütunda orderby atabilir, Her row için detay kısmı eklenebiliyor,Grid'in kod içinde kullanımı aktif kullanılan grid kütüphanelere göre çok daha kolay
ve özelleştirilebilir durumda. Xml ve Excell Export alabiliyor
Textbox:Type bilgisine göre otomatik oluşmakda örneğin number type için number dışında veri eklenebilmesi gibi durumlar engellenmekte
Segment Language:Site içinde aktif kullanılan dilleri bir segment olarak sunar
TextEditör: Quill Js kullandım
Checkbox,Selectbox,Spinner,Texteditör,Textarea ve diğerleri


Admin Panel

Ana Sayfa:
UI üzerinde günlük sipariş sayısı, bekleyen sipariş sayısı, günlük sipariş tutarı, toplam sipariş sayısı ve toplam satış tutarı gösterildi. Bu veriler grafik üzerinde de görselleştirildi. Order veritabanına gereksiz yük binmemesi adına istatistikler farklı bir tabloda tutuldu.

Ürün:
   Ürün Bilgisi:Kullanıcı burada ürün ismi marka kategori gibi verileri girer ve ürünün tipini belirtir Normal yada varyasyon ürün
   Ürün Kargo Bilgisi:Admin ürüne ait kargo bilgilerini girer otomatik olarak desi hesaplanır 
   Ürün Resmi:Admin ürünlere ait resimleri buraya ekleyebilir silebilir
   Varyasyon:Admin eğerki ürün varyasyon ürünüyse burada varyasyon bilgisi ekleyebilir varyasyonlara ait kombinasyonların tamamını generate ettirebilir
   Ürün Özellikleri:Admin ürünlere ait özellik ekleyebilir silebilir
   Ürün Storuğu:Admin stok kalem olarak ürünlere ait stok ekliyebilir stok ekleme sırasında ürünlere ürün indirimi % ve - indirimi uygulayabilir varyasyon ürünler için varyasyona ait stok eklenmesi sağlanmıştır


Ürün Özellikleri:
Admin Ürünlere eklenebilecek ürün özelliklerini burada ekler

Ürün Soruları:
Admin Ürünlere yöneltilen soruları burada bakar grid üzerinden cevap verebilir cevap verilen ürünler otomatik olarak onaylandı olarak gösterilir dilerse soruları silebilir

Ürün Yorumları:
Admin Ürünlere yöneltilen yorumlara burada bakar grid üzerinden cevap verebilir cevap verilen ürünler otomatik olarak onaylandı olarak gösterilir dilerse soruları silebilir

İndirim:
Kullanıcı Ürünlere ait indirim uygulayabilir burada Uygulayabileceği indirimler Kategori - % indirimleri Marka - % indirimleri buradaki indirimler ürün indirimleri uygulandıktan sonra uygulanmaktadır

Varyasyon:
Admin Ürünlere eklebilecek varyasyon bilgilerini burada ekler Örneğin renk kırmızı vb.

Marka:
Marka ekleme, silme, güncelleme işlemleri yapıldı. Grid üzerinden marka güncelleme sağlandı.

Slider:
Slider ekleme, silme ve güncelleme işlemleri tamamlandı.

Kategori:
Kategorilere ekleme, silme ve güncelleme işlemleri yapıldı. Kategorilere ait filtrelerin eklenmesi sağlandı.

Sayfa:
Sayfa ekleme, silme ve güncelleme işlemleri tamamlandı. Web için GrapesJS kullanılarak bir web page builder entegrasyonu sağlandı.

Vitrin:
Vitrin ekleme, silme ve güncelleme işlemleri tamamlandı. Şu an için üç çeşit vitrin mevcut:

8x8 Showcase
Swiper Showcase
Text Showcase
Bu vitrinlerin sayısı artırılabilir. Nihai amaç, kullanıcının ana sayfayı aktif bir şekilde yönetebilmesini sağlamaktır.

Depo:
Depo ekleme, silme ve güncelleme işlemleri tamamlandı. Grid üzerinde güncelleme yapılabilmesi sağlandı.

Para Birimi:
Kullanıcı her dil için istediği para birimlerini ekleyebilir. Hangfire kullanılarak para birimi eklenirken ve gece saat 02:00’de aktif kur güncellemesi otomatik olarak gerçekleştirildi.

Siparişler:
Kullanıcı, siparişlerin detayını görüntüleyebilir, fatura oluşturabilir, faturayı onaylayabilir, kargoya gönderebilir ve faturayı görüntüleyebilir.

Sepet İndirimleri:
Kullanıcı, sepeti belirli bir tutara ulaşan müşterilere yüzdesel (%) veya sabit miktarlı (-) indirimler uygulayabilir.

Aktiviteler:
Kullanıcı, ürünlerle ilgili yapılan işlemleri "Aktiviteler" penceresinden görüntüleyebilir. Kim tarafından güncellendiği, silindiği vb. durumlar burada gösterilir.

Admin Kullanıcıları:
Kullanıcı, sisteme yeni admin kullanıcıları ekleyebilir ve onlara yetkiler atayabilir.

Kullanıcı Grupları:
Kullanıcı, sisteme kullanıcı grupları ekleyebilir.

Çeviri:
Kullanıcı, sistemde bulunan dillerin çevirilerini değiştirebilir, yeni çeviriler ekleyebilir ve silebilir.

Dil Kodu:
Kullanıcı, sistemde dil kodu ekleyebilir, silebilir ve güncelleyebilir. Ancak yeni diller eklenirken firma bilgilendirilmeli ve mobil tarafta statik olarak dil kodu tanımlanmalıdır.

(Bu işlem, gereksiz dosya okuma/yazma yükünden ve sistem başlatılırken projeyi daha hızlı açabilmek için yapılmıştır.)

LLM Bilgisi:
Kullanıcı, OpenAI kütüphanelerinden hangisini kullanıyorsa onun bilgilerini kaydedebilir.

Web Site Bilgisi:
Kullanıcı, web sitesi bilgilerini (örneğin logo, site ismi vb.) buraya girebilir. Şu an için dinamik olarak tutulsa da, bu bilgiler yalnızca projenin başında değiştirildiği için ilerleyen süreçte statik hale getirilmelidir. (Gereksiz veritabanı isteklerinden kaçınmak için.)

Mail Tasarımı:
Kullanıcı, sistemde aktif olarak kullanılan mail şablonlarını güncelleyebilir. Örneğin:

Şifre değiştirme mesajları
Kullanıcıya özel bildirimler
Mail içeriklerinde kullanılacak dinamik keywordler (örneğin "şifremi unuttum" kodu, kullanıcı e-posta adresi vb.) UI üzerinde gösterilmiş ve mesaj içinde kullanılabilir hale getirilmiştir.

Mail Bilgisi:
Kullanıcı, sistemde mail bilgilerini girebilir.

SMS Şablonları:
Mail tasarımında olduğu gibi kullanıcı, sistemde SMS şablonlarını düzenleyebilir.

E-Arşiv Bilgisi:
Kullanıcı, e-arşivle ilgili bilgileri girebilir. E-arşiv bilgileri girilirken doğrulama mekanizması uygulanmıştır.

Ödeme Sağlayıcıları:
Projeye entegre ödeme sağlayıcıları listelenebilir. Kullanıcı, aktif ödeme sağlayıcısını değiştirebilir ve sağlayıcıya ait bilgileri güncelleyebilir.

Kargo Sağlayıcıları:
Projeye entegre kargo sağlayıcıları listelenebilir. Kullanıcı, aktif kargo sağlayıcısını değiştirebilir ve sağlayıcıya ait bilgileri güncelleyebilir.

Diller:
Kullanıcı, sidebar üzerinden diller arasında geçiş yapabilir. Her dilin kendine ait verileri vardır.

Bazı veriler global olarak tanımlıdır (örneğin admin kullanıcıları gibi), ancak geri kalan veriler dil bazlı olarak sunulmaktadır.

(Bu, projedeki dil sayısına ve trafiğe bağlı olarak, ileride dil bazlı multi-tenant DB yapısına geçişe uygun olacak şekilde tasarlanmıştır.)


User Inteface

Nots:
User tarafında veritabanı üzerinden çekilen maksimum sayfa limiti 10'dur. Bu, bütün listeler için geçerlidir ve sayfa scroll oldukça yeni isteğin atılması sağlanmıştır (Örnek: Vitrin listesindeki ürünler 10'lu 10'lu gelmektedir; mobilde ise 6-8-10 gibi değişebilmektedir).
Aynı şekilde, her bir listedeki ürünler ya da diğerleri için fade-in efekti uygulanıp, sanki tek tek geliyormuş hissi yaratılmıştır.

Anasayfa:
Anasayfa üzerinde kategori sayfası ve vitrin slider listeleri gösterilmektedir. Vitrin üzerinde 8 adet ürün gösterilmiş olup, diğer vitrindeki ürünlere vitrin detay üzerinden ulaşılabilir.

Katalog:
Kategori ve açıklama hakkında bilgiler burada yer almaktadır. Dinamik olarak kategoriye ait filtreler, filtre butonuna tıklandığında sidebar'da gösterilmektedir. Sidebar üzerinde eklenen filtreler, filtre butonu üzerinde gösterilerek kaldırılabilmesi sağlanmıştır. Bu sayede, kullanıcının odak noktasını kaybetmeden ürünler arasında rahat dolaşabilmesi amaçlanmıştır.

Ürün Detay:
Ürün detay sayfasında kullanıcı, ürünün özelliklerine ulaşabilir; resim galerisi üzerinde resimleri tek tek görüntüleyebilir; ürünlere soru sorabilir. Soru sorulan ürünler cevaplanmadan, tekrar soru sorulması engellenmiştir. Bu sayede bot yazılımlar gibi durumların önüne geçilmesi hedeflenmiştir.
Yorumlar kısmında, admin tarafından onaylanan yorumlar listelenmektedir. Kullanıcı, ürünü satın almadan yorum yapamamaktadır.

Kullanıcı Bilgileri:
Kullanıcı ad-soyad bilgilerini güncelleyebilir. "Hesabı Onayla" butonu ile kendi mailine aktivasyon kodu gönderebilir. Bot yazılımlarını engellemek adına, aktivasyon maili gönderilmiş kişilere tekrar mail gönderilmez; tarih aralığı aktif olan kişilere ise yalnızca "İşlem Başarılı" ibaresi gösterilir. Bu sayede, firmanın maillerinin spam klasörüne düşmemesi sağlanmıştır.

Favorilerim:
Kullanıcı beğendiği ürünleri favorileyebilir ve bu sayfada görüntüleyebilir.

Adreslerim:
Kullanıcı adres bilgilerini burada görüntüleyebilir.

Siparişlerim:
Kullanıcı siparişlerini burada görüntüleyebilir. İstenirse fatura buradan indirilebilir. Kullanıcı, eline ulaşan ürünler için yorum ekleyebilir.

Question:
Kullanıcı, göndermiş olduğu sorguları ve cevaplarını burada görüntüleyebilir.

Yorumlar:
Kullanıcı, daha önce yapmış olduğu yorumların onaylanıp onaylanmadığını görüntüleyebilir ya da silebilir.

Auth İşlemleri:
Kullanıcı giriş yapabilir, kayıt olabilir, "Şifremi Unuttum" maili gönderebilir.
