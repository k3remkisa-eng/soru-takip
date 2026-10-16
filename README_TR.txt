SORU TAKİP - ANDROID KURULUM REHBERİ
====================================

Uygulama özellikleri:
- TYT ve AYT ayrı ders listeleri
- Günlük soru hedefi, toplam soru, doğru, yanlış ve net
- Net hesabı: doğru - yanlış / 4
- Gün bazlı geçmiş ve haftalık toplamlar
- Telefonda yerel kayıt (localStorage)
- Çevrimdışı açılma (ilk kez çevrimiçi açıldıktan sonra)
- Yedek dışa aktarma ve yedekten geri yükleme
- Ücretsiz; reklam yok, hesap gerekmiyor

ÖNEMLİ:
Ana ekrana gerçek uygulama gibi eklemek ve çevrimdışı çalıştırmak için dosyaların HTTPS üzerinden yayınlanması gerekir. En kolay ücretsiz yöntem GitHub Pages.

GITHUB PAGES İLE ÜCRETSİZ YAYINLAMA:
1. Chrome'da https://github.com adresini açıp giriş yap veya ücretsiz hesap oluştur.
2. Sağ üstte + işaretine basıp "New repository" seç.
3. Repository name alanına soru-takip yaz.
4. Public seç; "Add a README file" işaretli olabilir. "Create repository" de.
5. Repository sayfasında "Add file" > "Upload files" seç.
6. Bu ZIP dosyasını bilgisayarında aç. İçindeki index.html, manifest.json, sw.js, icon-192.png ve icon-512.png dosyalarını GitHub'a yükle. Dosyaları bir klasörün içine değil, repository ana sayfasına yükle.
7. "Commit changes" düğmesine bas.
8. Repository içinde Settings > Pages bölümünü aç.
9. "Build and deployment" altında Source: "Deploy from a branch" seç.
10. Branch: main, folder: /(root) seç ve Save'e bas.
11. 1-3 dakika bekle. Pages ekranında verilen https://KULLANICIADI.github.io/soru-takip/ adresini aç.
12. Sitede TYT/AYT soru alanlarını görüyorsan yayın başarılı.

ANDROID ANA EKRANA EKLEME:
1. Telefonda Chrome ile GitHub Pages adresini aç.
2. Sayfanın yüklenmesini bekle ve bir kez çevrimiçi açık tut.
3. Chrome sağ üstte ⋮ menüsüne bas.
4. "Ana ekrana ekle" veya "Uygulamayı yükle" seçeneğine bas.
5. "Yükle" ya da "Ekle" de.
6. Ana ekrandaki Soru Takip simgesine basarak aç.
7. Çevrimdışı çalışma için ilk açılışta dosyaların önbelleğe alınması gerekir.

KAYITLAR VE YEDEK:
- Kayıtlar sunucuya gönderilmez; uygulamanın açıldığı tarayıcıda/cihazda tutulur.
- Tarayıcı verisini temizlemek veya uygulamayı kullandığın tarayıcı verilerini silmek kayıtları kaldırabilir.
- Düzenli olarak "Verileri dışa aktar" ile JSON yedeği indir.
- Telefon değiştirince yeni telefonda uygulamayı açıp "Yedekten içe aktar" ile bu JSON dosyasını seç.
- Yerel kayıtlar otomatik olarak başka telefona eşitlenmez.
- İlk kurulum ve ilk açılış için internet gerekir. Sonrasında çevrimdışı açılabilir.

DOSYA DÜZENİ:
index.html    Uygulamanın ekranı ve işlevleri
manifest.json Android ana ekran uygulaması ayarları
sw.js         Çevrimdışı önbellek
icon-192.png  Uygulama simgesi (küçük)
icon-512.png  Uygulama simgesi (büyük)
