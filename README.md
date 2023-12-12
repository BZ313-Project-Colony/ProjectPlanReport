# Proje planı

## Proje Tanımı

QR Pass büyük çaplı organizasyonları planlamayı, katılımcıları takip etmeyi ve kitlelere ulaşmayı kolaylaştıran bir projedir. Web arayüzü üzerinden etkinlikleri görüntüleme ve etkinlik daveti gönderme imkanı sunarken, mobil uygulaması üzerinden etkinlik başlangıçlarında QR kod ile giriş çıkış ve katılım kontrolü sağlama imkanı sunar. Yöneticilerin büyük organizasyonlarda her şeyi bir arada tutabileceği bir platform olarak karşımıza çıkıyor.

## Proje Kapsamı

-   Web ve mobil tabanlı uygulama geliştirilecek.
    
-   Web geliştirme: Etkinlik oluşturma, katılımcı kaydı, QR kod oluşturma, yönetici arayüzü.
    
-   Mobil geliştirme: QR kod okuma, katılımcı bilgilerini görüntüleme.
    

## Kullanılacak Teknolojiler

  

Projemizin mobil tarafında yapılacak olan QR scanner için Dart dili tabanlı Flutter kullanılacaktır. Frontend kısmında yönetici ve kullanıcı arayüzlerini oluştururken JS kütüphanesi olan React kullanılacaktır. Backend kısmında Spring Boot Java kullanılacak olup projemizde veritabanı servisi olarak Postgre tercih edilecektir.

  

## Proje Süresi ve Zaman Çizelgesi

### Gereksinim Analizi Raporu (13 Kasım - 16 Kasım)

Projenin başlangıç aşamasında projenin genel amacını, kapsamını ve müşteri gereksinimlerini belirleyen bu raporun amacı, projenin temel gereksinimlerini anlamak, belirlemek ve belgelemektir. Projenin hedeflerini ve işlevselliğini netleştirerek projenin başarılı bir şekilde planlanmasına temel oluşturur. Müşteri ile bir anlaşma noktası oluşturarak, projenin yönetimi ve geliştirilmesi sürecini yönlendirmek amacıyla yazılmıştır.

### Yazılım Mimarisi ve Tasarımı Raporu (17 Kasım - 19 Kasım)

Yazılım Mimarisi ve Tasarımı Raporu, projenin mimari yapısını, bileşenlerini ve tasarım prensiplerini belirleyen bu raporun amacı, projenin teknik yönünü tasarlamak ve bu tasarımın projenin gereksinimlerini nasıl karşılayacağını anlatmaktır. Yazılım mimarisi ve tasarımı raporu, geliştirme ekibine yönergeler sağlar ve projenin bütünlüğünü, genişletilebilirliğini, bakımını ve performansını güvence altına almayı ve geliştiriciler arasında ortak bir anlayış oluşturarak kodlama sürecini daha etkili hale getirmeyi hedeflemiştir.

### Sprint - 1 - Login (20 Kasım - 26 Kasım)

**Mobil:** QR Pass mobil uygulamasında yönetici giriş ekranı yapılmıştır.

**Frontend:** QR Pass web arayüzünde kullanıcı ve yönetici giriş ekranları yapılmıştır.

**Backend:** Giriş ekranlarından kullanıcı adı ve şifre bilgisini alır ve response döndürür.

  

### Sprint - 2 - Event Creation (27 Kasım - 3 Aralık)

**Mobil:** Etkinlik ekranında oluşturulan etkinlikler ve bilgileri liste şeklinde görüntülenir.

**Frontend:** Yönetici ekranında etkinlik oluşturma penceresinde etkinliğe dair etkinlik adı, tarihi ve saati, yeri ve kişi sayısının belirlenerek etkinlik oluşturulur.

Oluşturulan etkinlikler ve bilgileri liste şeklinde görüntülenir.

**Backend:** Etkinlik bilgileri alınır ve etkinlik id’si belirlenir.

  

### Sprint - 3 - Event Detail (4 Aralık - 10 Aralık)

**Mobil:** Etkinlik detayları görüntüleme ekranında etkinlik id, etkinlik adı, yeri, tarih ve saatinin görüntülenmesi.

**Frontend:** Etkinlik detayları görüntüleme ekranında etkinlik id, etkinlik adı, yeri, tarih ve saatinin görüntülenmesi. Etkinlik için alarm kurulması ve etkinlik linkinin kopyalanması özellikleri eklenmiştir. Bu ekranda etkinlik katılımcılarından kaç tanesinin biletinin okunduğu görüntülenebilmektedir.

**Backend:** Etkinlik id’sine göre etkinlik bilgilerini gösteriyor.

### Sprint - 4 - Register Participants (11 Aralık- 17 Aralık)

**Mobil:** Etkinliğin bilgileri ve etkinliğe kayıt olan katılımcıların listesi görüntülenebilmektedir.

**Frontend:** Bu ekranda katılımcılar etkinlik seçerek isim soyisim ve mail bilgileriyle katılımcı olma talebi gönderiyorlar. Etkinliğe kayıt olma talebi gönderen katılımcılar yöneticinin ekranında görüntülenebilmektedir. Etkinliği silme seçeneği de bulunmaktadır.

**Backend:** Etkinliğe kayıt olan kullanıcının bilgileri alınıyor ve QR kod içeren bileti kullanıcıya gönderiliyor. Etkinlik silme durumunda katılımcıların bilgileri de silinmektedir.

  

### Sprint - 5 - Confirm Tickets (18 Aralık - 24 Aralık)

**Mobil:** Katılımcının QR kodu okunarak bileti görüntülenmektedir. Onaylama veya silme seçenekleri bulunmaktadır.

**Backend:** Okunan biletten katılımcının bilgilerine ulaşılmaktadır, yönetici katılımcıyı onaylayabilir veya silebilir.



### Test Etme, Hata Ayıklama ve Entegrasyon (25 Aralık - 29 Aralık)

**Test Senaryolarının Hazırlanması**
    
-   Uygulamanın temel fonksiyonları için kapsamlı test senaryoları oluşturulacak.


-   QR kod tarama, veri çıkarma ve arayüz işlevselliği test edilecek.
    

  **Manuel ve Otomatik Testlerin Yürütülmesi**
    

-   Hazırlanan test senaryoları doğrultusunda manuel testler gerçekleştirilecek.
    
-   Otomatik test senaryoları, uygulamanın temel işlevselliğini ve performansını kontrol etmek için kullanılacak.
    

  **Hata Ayıklama ve İyileştirme**
    

-   Test sırasında ortaya çıkan hatalar belirlenip kayıt altına alınacak.
    
-   Hata ayıklama süreci, geliştirme ekibi tarafından hataların çözümüne odaklanacak.
    
-   İyileştirmeler ve güncellemeler, hata düzeltme süreci içinde uygulanacak.
    

  

### Projenin Müşteriye Teslimi (30 Aralık - 31 Aralık)

**Son Kontroller ve Onaylar**
    

-   Test ve hata düzeltme aşamalarının ardından, uygulama tekrar test edilecek.
    
-   Müşteri gereksinimlerine uygunluğu kontrol edilecek ve onay alınacak.
    

  **Belgelerin ve Kılavuzların Teslim Edilmesi**
    

-   Kullanıcı kılavuzları, teknik belgeler ve gerektiğinde eğitim materyalleri müşteriye sağlanacak.
    
-   Uygulama ile ilgili önemli bilgiler içeren bir dokümantasyon müşteriye teslim edilecek.
    

  **Müşteri Geri Bildirimi ve Son Değerlendirme**
    

-   Müşteriye uygulama sunulacak ve geri bildirimleri alınacak.
    
-   Son değerlendirme toplantısı düzenlenecek ve projenin başarıyla tamamlandığı onaylanacak.
    

## ![](https://lh7-us.googleusercontent.com/-hmaKGy-h-Ya7bIsEmDl1cRGA8Rt8j9aZal2reX8Xae_p87QIiMcLj8UYmjV5qIit1vHzIzp2MLBLcrMX_MP9zro90G-p48NNMkypLuMQgCgJVpAybS8tW9NtJTvAWuupXMUjRBo_YUKLWT6y7H_CXs)

![](https://lh7-us.googleusercontent.com/FzUINZW0cEMlw2XNl3Avi2YesXD4Tm3ITX6z7kpR0CzovPUMlk3DjUncvaMLz2qzJHBu5NpmbCgPrTOeftn826EpFV_jlIxIMwHvAuCgfB90DNvZTVWC-i4RrgU_p75T9niMvSuPT5BlVw-srh8xIA0)
## Risk Analizi ve Yönetimi

**Olası Riskler ve çözümleri:**
    

-   Geliştirme sürecinde teknik zorluklar.
    
-   Değişen müşteri gereksinimleri.
    
-   Ekip üyelerinin beklenmedik ayrılıkları.
    
-   Zaman kayıpları
    
-   Güvenlik zafiyetleri
    

   **Risk Yönetimi Stratejileri:**
    

-   Düzenli risk incelemeleri ve sürekli güncellenen bir risk yönetim planı.
    
-   Müşteri ile sık sık iletişim kurarak gereksinim değişikliklerini hızla ele alma.
    
-   Ekip üyeleri arasında bilgi paylaşımını teşvik etme.
    
-   Sürekli olarak projenin ilerleyişini izleme ve takip etme.
    

## İletişim Planı

-   Haftalık durum toplantıları: Cumartesi günleri
    
-   Acil durumlar için anlık iletişim kanalları(Discord,Whatsapp)
    

## Maliyet Tahminleri ve Bütçe

-   Geliştirme araçları ve yazılımları maliyeti
    
-   İnsan kaynakları maliyeti
    
-   Altyapı ve hosting maliyeti
    

## Kalite ve Test Planı

-   Sürekli entegrasyon ve otomatik test süreçleri
    
-   İlerleme raporları ve test sonuçları düzenli olarak paylaşılacak
    

## Proje İlerleme İzleme ve Raporlama

-   Gantt şeması kullanılacak.
    
-   Github’da görev panoları güncellenecek.
    
-   Haftalık ilerleme raporları oluşturulacak.
    

## Değişiklik Yönetimi

-   Ekipte ortak karar ile yapılması gereken değişiklikler belirlenir.
    
-   Değişiklik değerlendirilecek ve onay süreci belirlenir.
    
-   Değişiklik tamamlanıp sisteme entegre edilir.
    

  

## Eğitim ve Dokümantasyon

-   Ekip içi eğitimler
    
-   Kullanıcı kılavuzları ve yardım belgeleri
    

## Proje Sonlandırma ve Teslimat

-   Proje tamamlandığında kullanıcıya kullanım eğitimi verilir.
    
-   Proje dokümantasyonu müşteriye teslim edilecektir.
    

Proje ekibi tarafından yazılan bu rapor, QR Pass isimli projemizin proje planı olmakla beraber projenin gerçekleştirilmesi için yukarıda belirtilen detaylar dikkate alınarak yazılmıştır. Projemizin belirlenen aşamalarında görevlendirmeler ekip içerisinde paylaşılmış olup proje ilerlemesi belirtilen detaylarla titizlikle takip edilecektir.
