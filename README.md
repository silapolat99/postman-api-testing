API Automation Suite (Postman)

Bu repo, **JSONPlaceholder** uç noktaları (endpoints) üzerinde gerçekleştirdiğim API test otomasyon süreçlerini içerir. Proje kapsamında manuel test senaryoları JavaScript ile otomatize edilmiş ve veri bütünlüğü (data integrity) doğrulanmıştır.

Test Senaryoları ve Kapsam
Koleksiyon içerisinde iki ana iş akışı (workflow) test edilmiştir:

GET - Data Retrieval:
Belirli bir kaynağın çekilmesi sırasında HTTP 200 durum kodu, yanıt süresi (performance latency < 500ms) ve dönen verinin ID doğruluğu kontrol edilmiştir.
POST - Resource Creation: Yeni bir kayıt oluşturma isteği gönderilerek sistemin HTTP 201 (Created) dönüp dönmediği ve gönderilen 'title' verisinin yanıt ile eşleşip eşleşmediği (assertion) doğrulanmıştır.

Teknik Altyapı
Aracı:Postman (v10+)
Scripting: JavaScript (Postman Sandbox)
Validasyonlar: Status code verification, JSON body matching, Response time performance tests.

Çalıştırma Talimatı
Testleri kendi Postman ortamınızda simüle etmek için:
1. Depodaki `.json` uzantılı koleksiyon dosyasını bilgisayarınıza indirin.
2. Postman uygulamasında **Import** butonunu kullanarak dosyayı içeri aktarın.
3. Koleksiyonun üzerindeki **Run Collection** butonuna basarak tüm senaryoları otomatik olarak koşturun.

İletişim: www.linkedin.com/in/sıla-polat

