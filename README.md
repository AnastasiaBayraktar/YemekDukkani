# YemekDukkani

RESTAURANT SİTESİ





-Default admin girişi --> email:admin@gmail.com // şifre: Admin123.(sonunda nokta var)

Anastasia Bayraktar G141210105


Azure https://taste20191222092555.azurewebsites.net/Customer/Home 

 # Taste

-Dependencies--> Kullanılacak teknoloji,frameworkleri içerir.
-Taste proje dosyası genel olarak front-end kısmını oluşturuyor.
-wwwroot->css,javascript,boostrap ve resim dosyalarının bulunduğu yer.
-Areas-->Identity yani üyelik işlemlerinin yapıldığı yer. Üyelik işlemlerinde ya da giriş işlemlerinin front-end kısmı burada bulunur.
-Controller-> Üyelik işlemleri dışındaki sayfalardaki kontrol işlemlerini barındırır.
-Pages-->Her sayfanın front-end ve her sayfaya ait id işlemlerinin yapıldığı back-end kısmını oluşturur.
-Shared->Layout -->web sitesinin genel front-end kısmını yönetir. 
-Startup-->proje açılırken çalışacak servisleri başlatır.

# Taste.DataAccess

-Initializer-->Site için role'lerin(admin,üye...) işlemlerinin olduğu kısım.
-Repository-->Veritabanı sorgulama işlemlerinin bir merkezden yapılmasını sağlayan yapı.Tekrar bir yapıyı kullanmak yerine sistematik bir kalıp içerisinde çalışır.
-DBContext-->Veritabanına karşılık gelen obje yapısıdır. İçinde tablo yapısında karşılık gelen DbSet objelerini bulundurur.-CRUD(Create,Read,Update,Delete) işlemlerini gerçekleştirir.
-Migration-->CodeFirst ile yazılan bir projede, bilgilerin veri tabanında sık sık güncelleştirmesi durumu olduğunda; her defasında tüm veriler veri tabanında sıfırdan oluşturuluyor.

# Taste.Models

Genel olarak VeriTabanınında bulunun her özelliğin (Id,isim,numara...) nesne olarak oluşturup daha sonra Controller katmanında gerekli işlemleri yaparak kullanabilmemize olaran tanımaktadır.
Herbir sınıf ismi bir tabloyu belirtmektedir.(Category.cs-->Category tablosu)

# Taste.Utility

Statüye göre güvenli ödeme yapılmasını sağlayan katman.
EmailSender->ödeme esnasında e-mail sorgusu yapar.
SD--> Statüyü belirleyen sınıf.(Yönetici-üye ....)
StripeSetting-->>Güvenli ödeme için bulunan nesneler.

