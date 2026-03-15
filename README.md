# TDK ve Sözlükler (Sürüm 2026.6.0)

* **Yazar:** NVDA_TR
* **Uyumluluk:** NVDA 2022.1 ve sonrası

**🔔 Eklenti İşlev ve Özellikleri:**

* TDK, Dil Derneği ve Kubbealtı Lugatı'nda ayrı ayrı, ikili veya üçlü birleşik arama imkânı.
* **Beşli Arama: TDK + Dil Derneği + Vikisözlük + Nişanyan + Kubbealtı tek pencerede.** *(Yeni)*
* TDK Bilim ve Sanat Terimleri Sözlüğü entegrasyonu (70'ten fazla bilim dalı, çok dilli karşılıklar).
* **Çevrimdışı Müzik Terimleri Sözlüğü (4700+ madde, hem madde adı hem tanım içi arama).**
* **TDK Kişi Adları Sözlüğü entegrasyonu (ada göre ve anlama göre arama).**
* **Kelime listeleme (İle başlayan / İle biten) artık kaynak seçimine sahip.** *(Güncellendi)*
* **Anagram çözücüde kaynak seçimi.** *(Güncellendi)*
* **Sonuç pencerelerinde NVDA+Alt+C ile alıntı olarak kopyalama (CF_HTML + düz metin).** *(Yeni)*
* Akıllı Atasözü ve Deyim arama algoritması.
* Dahili Deyimler ve Atasözleri sözlükleri (çevrimdışı çalışır).
* Tureng (İngilizce-Türkçe / Türkçe-İngilizce) sözlük entegrasyonu.
* **TDK Derleme Sözlüğü (Türkiye Türkçesi Ağızları — yöresel kelimeler ve yörelerine göre anlamları).**
* İngilizceden İngilizceye sözlük, Metin Analizi, IP ve ISBN çözümleme.
* **Vikisözlük ve Nişanyan Sözlük sonuçları artık NVDA penceresinde gösterilir; tarayıcı açılmaz.** *(Güncellendi)*
* Arama geçmişi (son 100 arama oturum boyunca bellekte tutulur).
* Günün Kelimesi önbelleği (aynı gün içinde tekrar API çağrısı yapılmaz).
* Katman menüsünden etkileşimli tuş listesi.

---

## 🎯 Eklentinin Felsefesi

Türkçe, binlerce yıllık kültürel birikimin taşıyıcısı olan bir dildir. Kelimelerin anlamını, kökenini ve kullanım bağlamını kavramak; sadece bir tanım öğrenmek değil, dilin iç dünyasıyla kurulan bir ilişkidir. Ancak bu ilişkiyi kurmak için gereken her araç — TDK, Dil Derneği, Kubbealtı, Nişanyan — günümüzde ya görsel arayüzlerle çevrilmiş, ya reklam katmanlarının arkasına gömülmüş ya da ekran okuyucuyla güçlükle gezilebilen web sayfaları hâline gelmiştir.

Ekran okuyucu kullanan biri için "hızlıca bir kelimeye bakmak", görme engeli olmayan bir okuyucuya kıyasla çok daha fazla adım gerektirir: tarayıcıyı açmak, adresi yazmak, sayfanın yüklenmesini beklemek, başlıklar ve bölümler arasında gezinerek asıl içeriğe ulaşmak, ardından tekrar okumakta olduğunuz yere dönmek. Okuma akışını bölen bu sürtünme, zaman içinde bir mikro yorgunluk birikimine dönüşür.

**TDK ve Sözlükler** bu sürtünmeyi ortadan kaldırmak için tasarlanmıştır.

### Damıtılmış bilgi, saf anlam

Web sözlükleri belirli bir kullanım biçimini ön varsayar: fare ile gezmek, gözle taramak, reklam alanlarını görmezden gelmek. Bu ön varsayım, söz konusu kaynakların ekran okuyucuyla kullanılmasını başından zorlaştırır.

Eklenti, bu kaynakların API'lerine ve veri akışlarına doğrudan erişerek yalnızca anlam bilgisini — tanımı, örnek cümleyi, köken notunu — alır ve NVDA'nın konuşma akışına en uygun biçimde sunar. Ortada reklam bloku yoktur, gezinilecek menü yoktur, yüklenecek resim yoktur. Yalnızca kelime vardır ve kelimenin anlamı.

Bu yaklaşımın somut karşılığı şudur: Bir Osmanlıca edebi metni okurken karşılaştığınız *müstağni* kelimesinin TDK'daki modern karşılığını, Kubbealtı'daki köklü tanımını ve Dil Derneği'nin sade açıklamasını **tek bir tuş kombinasyonuyla** ve **tarayıcınızı açmadan** yan yana görebilirsiniz.

### Beş kurum, tek pencere

Türk dil kurumları birbirini tamamlar, birbirinin alternatifi değildir:

- **TDK Güncel Türkçe Sözlük** — Standart, geniş kapsamlı, çağdaş kullanıma odaklı.
- **Dil Derneği** — Öz Türkçe yaklaşımını benimseyen, yabancı kökenli kelimelere Türkçe karşılık arayan bir çizgide.
- **Kubbealtı Lugatı** — Klasik edebiyatta ve Osmanlı döneminde kullanılan kelimeleri, köken bilgisi ve edebi örneklerle derinlemesine ele alan paha biçilmez bir hazine.
- **Vikisözlük** — Topluluk tarafından derlenen; argo, bölgesel ağız ve neolojizmleri resmi kurumlardan önce kapsayan açık kaynak.
- **Nişanyan Sözlük** — Sevan Nişanyan'ın hazırladığı etimoloji sözlüğü; kelimenin köken dilini, ilk belgelendiği tarihi ve anlam değişiminin izini sürer.

Katman menüsündeki `F` tuşuyla bu beş kaynağın yanıtı **tek bir pencerede** üst üste gelir. Kaynaklar aynı anda paralel olarak sorgulanır; toplam bekleme süresi en yavaş API kadardır.

### Az tuş, çok işlev

Eklentinin katman mimarisi, her işlemi mümkün olduğu kadar az adıma indirgemek üzere tasarlanmıştır. İki tuşla katmanı açarsınız, tek tuşla kaynağı seçersiniz. Zamanla bu kısayollar alışkanlığa dönüşür; kelimeyle kurulan anlık bağlantı, düşünce akışını kesmez hâle gelir.

Arama geçmişi (`H`), günün kelimesi (`G`), tersine arama (`S`) ve anagram çözücü (`0`) gibi özellikler bu anlayışın uzantısıdır: Bilgiye ulaşma yolunu sürekli kısaltmak, her aşamayı mümkün olduğu kadar az tuş vuruşuna indirgemek.

---

## Nasıl Kullanılır?

Eklenti iki ana komut yapısı üzerinden çalışır:

### 1. Hızlı Arama (Anlık Bilgi)

Kısayol: `NVDA` + `,` (Virgül)

İmlecin üzerindeki kelimeyi veya o an seçili metni, **en son kullandığınız sözlükte** (varsayılan: Birleşik Arama) anında sorgular.

* **Metin seçiliyse:** Seçili metni sorgular.
* **Metin seçili değilse:** İmlecin üzerindeki kelimeyi otomatik algılar.
* **Hiçbir şey yoksa:** Kelimeyi elle yazabileceğiniz bir giriş kutusu açılır.

**Örnek:** Bir gazete makalesini okurken *müseccel* kelimesine geldiniz. `NVDA`+`,` tuşlarına basmanız yeterli; okuma akışınız kesilmeden anlamı duyarsınız.

### 2. Kaynak Seçim Katmanı (Detaylı Araştırma)

Kısayol: `NVDA` + `Shift` + `,` (Virgül)

Bu kombinasyona bastığınızda "Sözlük Katmanı" etkinleşir. NVDA kısa bir özet seslendirir; ardından yalnızca bir tuşa basarak istediğiniz kaynağı seçersiniz.

**Tüm tuş listesi için `<` (Küçüktür) tuşuna basın.** Açılan listeden bir seçenek seçtiğinizde o işlem başlar; liste kapanmadan başka işlemler de yapabilirsiniz.

---

## Hangi Kaynağı Ne Zaman Kullanmalıyım?

### `1` — Birleşik Arama (TDK + Dil Derneği)

**Ne işe yarar:** TDK ile Dil Derneği'ni eş zamanlı tarar; sonuçları tek pencerede alt alta gösterir.

**Ne zaman kullanılır:** Kelimenin hem yaygın hem de öz Türkçe karşılığını merak ettiğinizde. İki kurumun tanımları çoğu zaman birbirini tamamlar; kimi zaman ise ince anlam farklarını ortaya koyar.

---

### `"` — Üçlü Arama (TDK + Dil Derneği + Kubbealtı Lugatı)

**Ne işe yarar:** Birleşik arama `1`'in genişletilmiş halidir. Üç kaynağı paralel sorgular ve tek pencerede sunar.

**Ne zaman kullanılır:** Özellikle Osmanlıca kökenli, arkaik veya edebi kelimelerle karşılaştığınızda bu mod çok değer katar. Kubbealtı, kelimenin dildeki tarihsel serüvenini, edebi örneklerde nasıl kullanıldığını ve Arapça ya da Farsça kökenini belgeler.

---

### `2` — TDK Atasözleri ve Deyimler (Akıllı Liste)

**Ne işe yarar:** Yazdığınız kelimenin geçtiği tüm atasözü ve deyimleri listeler.

* Tek sonuç varsa doğrudan gösterir.
* Birden fazla sonuç varsa seçilebilir bir liste açar; listeden seçtiğinizde anlamı TDK'da aranır.

**Örnek:** *Taş* yazıp arattığınızda *"taş çatlasa"*, *"taşı gediğine koymak"*, *"taş kesmek"* gibi onlarca deyim listelenir; hepsinin anlamına tek tek ulaşabilirsiniz.

---

### `3` — Vikisözlük *(NVDA penceresinde gösterilir)*

**Ne zaman kullanılır:** Türkçe olmayan bir sözcük, dilbilgisel çözümleme ya da çok dilli karşılaştırma istediğinizde. Vikisözlük topluluğu tarafından derlenir; resmi kurumların kapsamamayabileceği argo, bölgesel ağız veya neolojizmler burada bulunabilir. Sonuçların altındaki bağlantıyla doğrudan sayfaya da gidebilirsiniz.

---

### `4` — Nişanyan Sözlük *(NVDA penceresinde gösterilir)*

**Ne zaman kullanılır:** "Bu kelime Türkçeye nasıl girdi?" sorusu aklınızı kurcaladığında. Sevan Nişanyan'ın derlediği bu etimoloji sözlüğü; köken dilini, ilk belgelendiği tarihi ve anlam değişiminin izini sürer. Sonuçların altındaki bağlantıyla tam sayfaya da geçebilirsiniz.

**Örnek:** *Bütçe* kelimesini arattığınızda kelimenin Fransızca kökenli olduğunu, Osmanlıcaya hangi dönemde ve hangi biçimle girdiğini, hatta kavramın İngiltere ve Fransa'daki siyasi tarihini öğrenirsiniz. Dil meraklıları için bitimsiz bir kaynak.

---

### `F` — Beşli Arama *(TDK + Dil Derneği + Vikisözlük + Nişanyan + Kubbealtı)*

**Ne işe yarar:** Beş kaynağı aynı anda paralel olarak sorgular ve sonuçları tek bir NVDA penceresinde üst üste gösterir.

**Ne zaman kullanılır:** Bir kelimeyi en kapsamlı biçimde araştırmak istediğinizde. Tek sorguda hem çağdaş Türkçe karşılığını (TDK, Dil Derneği), hem kökenini (Nişanyan), hem topluluk tanımını (Vikisözlük), hem de tarihsel ve edebi bağlamını (Kubbealtı) yan yana görebilirsiniz.

**Not:** Kaynaklardan biri sonuç döndürmezse yalnızca o kaynak için "bulunamadı" notu çıkar; diğerleri yine gösterilir.

---

### `5` — Kubbealtı Lugatı *(doğrudan API, tarayıcı açılmaz)*

**Ne işe yarar:** `eski.lugatim.com` API'sini sorgular; tarayıcı açmadan sonucu NVDA penceresinde gösterir.

**Ne zaman kullanılır:** Osmanlıca metin okurken, klasik şiir incelerken ya da kelimenin tarihsel ve edebi bağlamını merak ettiğinizde. Kubbealtı; tanımın yanı sıra Yahyâ Kemal, Tanpınar, Necip Fazıl gibi ustalardan alınmış örnek cümlelerle kelimenin gerçek dildeki yaşamını belgeler.

**Örnek:** *Seyyah* kelimesini `5` ile arattığınızda:
> *(Ar. siyāḥat "yeryüzünde gezmek"ten seyyāḥ)* Seyâhat eden, uzak ülkeleri gezip dolaşan kimse, gezgin.
> *İstanbul bütün şehirler arasında birinci derecede göründü ve Avrupa'nın en yüksek şâirlerinin gözlerini kamaştırdı ve en güzîde ruhlu seyyahlarının muhayyilesine yerleşti* (Yahyâ Kemal).

---

### `6` — Sadece TDK Güncel Türkçe Sözlük

**Ne işe yarar:** Birleşik aramadan (`1`) farklı olarak yalnızca TDK Güncel Türkçe Sözlük'ü sorgular; Dil Derneği sorgusu yapılmaz.

**Ne zaman kullanılır:** Yalnızca TDK'nın resmî tanımını görmek istediğinizde veya Dil Derneği'nin sonuç döndürmediği durumlarda daha hızlı yanıt almak için.

---

### `7` — Sadece Dil Derneği

**Ne işe yarar:** Yalnızca Dil Derneği API'sini sorgular.

**Ne zaman kullanılır:** Bir kelimenin öz Türkçe karşılığını veya Dil Derneği'nin özgün yorumunu doğrudan görmek istediğinizde.

---

### `B` — TDK Bilim ve Sanat Terimleri Sözlüğü *(doğrudan API, tarayıcı açılmaz)*

**Ne işe yarar:** TDK'nın Bilim ve Sanat Terimleri Sözlüğü'nü sorgular. Matematik, Fizik, Tıp, Dil Bilimi, Müzik ve daha pek çok bilim dalına ait teknik terimleri Türkçe karşılıkları ve çok dilli eşdeğerleriyle (İngilizce, Fransızca, Almanca, Latince) birlikte sunar. Sonuçlar sözlük adı ve yayın yılına göre gruplandırılır.

**Ne zaman kullanılır:** Akademik metin okurken ya da yazarken teknik bir terimin Türkçe karşılığını veya yabancı dil eşdeğerini bulmak istediğinizde.

---

### `Ö` — TDK Kişi Adları Sözlüğü (Ada Göre Arama)

**Ne işe yarar:** TDK'nın Kişi Adları Sözlüğü'nü ada göre sorgular (`sozluk.gov.tr`). Aranan adın anlamını, kökenini ve cinsiyetini gösterir.

* Tek sonuç varsa doğrudan gösterir.
* Birden fazla sonuç varsa seçilebilir bir liste açılır.

**Ne zaman kullanılır:** Bir ismin anlamını ya da kökenini merak ettiğinizde. Doğum tescili için uygun isim araştırırken veya edebi bir metinde geçen karakter adının ardındaki anlam katmanını keşfetmek istediğinizde.

**Örnek:** *Deniz* yazıp `Ö` ile arattığınızda adın Türkçe kökenli olduğunu, hem kız hem erkek adı olarak kullanıldığını ve "büyük su kütlesi" anlamını taşıdığını görürsünüz.

---

### `Ç` — TDK Kişi Adları Sözlüğü (Anlama Göre Arama)

**Ne işe yarar:** Aynı TDK Kişi Adları Sözlüğü'nü bu sefer **anlam içinde** arama yaparak sorgular. Girdiğiniz kavramı tanımında barındıran tüm adları listeler.

**Ne zaman kullanılır:** Belirli bir anlam veya kavramı taşıyan isimler bulmak istediğinizde.

**Örnek:** *Işık* yazıp `Ç` ile arattığınızda tanımında ışık, aydınlık veya parlaklık kavramı geçen tüm adlar listelenir: Aydın, Nûr, Ziya, Işıl ve diğerleri.

---

### `Q` – `T` — Arama Motorları *(tarayıcıda açılır)*

| Tuş | Motor | En iyi kullanım |
|-----|-------|-----------------|
| `Q` | Google | Genel, kapsamlı, haber ve akademik |
| `W` | DuckDuckGo | Gizlilik odaklı, reklamsız sonuçlar |
| `E` | Bing | Microsoft ekosistemi, görsel arama |
| `R` | Yahoo | Haber ve finans haberleri |
| `T` | Yandex | Türkiye lokasyonlu, Rusça içerik |

---

### `A` — Yerel (Çevrimdışı) Sözlük

**Ne işe yarar:** Eklentiyle birlikte gelen dahili veritabanında arama yapar. Aranan kelimenin geçtiği tüm deyim ve atasözlerini anında listeler. API çağrısı yapmadığı için yanıt anlık gelir.

---

### `S` — Tersine Arama (Kavramdan Deyime)

**Ne işe yarar:** Yerel sözlükteki **tanımların içinde** arama yapar; başlığa değil, açıklamaya bakar.

**Ne zaman kullanılır:** Kavramı biliyorsunuz ama onu en iyi ifade eden deyimi unuttuğunuzda.

**Örnek:** *Sabır* yazıp arattığınızda, başlığında "sabır" geçmeyen ancak tanımında bu kavrama değinen deyimler de listelenir.

---

### `M` — Müzik Terimleri Sözlüğü *(çevrimdışı)*

**Ne işe yarar:** 4700'ü aşkın müzik terimini barındıran çevrimdışı sözlükte **madde adına göre** arama yapar. Birden fazla eşleşme varsa seçilebilir bir liste açılır.

---

### `N` — Müzik Terimleri (Tanım İçi Arama) *(çevrimdışı)*

**Ne işe yarar:** Aynı müzik sözlüğünde bu sefer **tanımların içinde** arama yapar. `S` tuşunun atasözleri sözlüğüne yaptığını `N` müzik sözlüğüne yapar.

---

### `D` — TDK Derleme Sözlüğü *(Türkiye Türkçesi Ağızları)*

**Ne işe yarar:** TDK'nın Derleme Sözlüğü'nü sorgular. Standart Türkçede bulunmayan ya da farklı anlamlar kazanmış yöresel kelimeleri; anlamları, kullanıldıkları il ve ilçeler ile kaynak künyesiyle birlikte sunar.

**Ne zaman kullanılır:** Yöresel bir kelimeyle karşılaştığınızda, bir kelimenin Anadolu'nun farklı bölgelerindeki kullanımını merak ettiğinizde ya da sözlü edebiyat ve folklor metinleri üzerine çalışırken.

**Örnek:** *Kötek* yazıp `D` ile arattığınızda kelimenin hangi illerde hangi anlamlarda kullanıldığını ve hangi derleme kaynaklarında belgelendiğini görürsünüz.

---

### 🧩 Kelime Avcısı (Liste Modu) *(Güncellendi)*

Bulmaca çözerken, şiir yazarken ya da bir kalıba uyan kelimeleri ararken kullanabileceğiniz listeleme özelliği.

Katman komutunu (`NVDA`+`Shift`+`,`) uyguladıktan sonra:

* **`*` (Yıldız):** Seçili veya yazılan ifadeyle **BAŞLAYAN** kelimeleri listeler.
* **`-` (Tire):** Seçili veya yazılan ifadeyle **BİTEN** kelimeleri listeler.

**Kaynak seçimi:** Sonuç listesinin üst kısmında bir açılır menü bulunur. Buradan TDK GTS, Birleşik Arama, Dil Derneği veya Kubbealtı gibi farklı kaynaklardan birini seçip listeyi kapatmadan aynı kelimeyi farklı sözlüklerde sorgulayabilirsiniz.

**Örnek:** *Çiçek* yazıp `*` tuşuna basarsanız: çiçek, çiçekli, çiçekçi, çiçekalma, çiçeklenmek… gibi onlarca sonuç listelenir. `-` tuşuyla *lik* yazıp ararsanız "lik" ile biten tüm kelimeleri bulursunuz.

---

### `I` — Tureng Sözlük (İngilizce ↔ Türkçe)

**Ne işe yarar:** Tureng.com veritabanını doğrudan sorgular. Tarayıcı açmadan, kelimenin farklı bağlamlardaki karşılıklarını (genel, teknik, argo, tıbbi vb.) listeler.

---

### 📊 Metin Analizi ve Bilgi Sistemi

Katman komutundan sonra `.` (Nokta) tuşuna basın.

#### Çoklu kelime seçiliyse — Metin İstatistikleri

* **Okuma süresi:** Ortalama okuma hızına göre dakika cinsinden tahmin.
* **Kelime sayısı:** Noktalama işaretleri ayrıştırılarak doğru sayım.
* **Yapısal analiz:** Paragraf ve cümle sayısı.
* **Frekans analizi:** Metindeki en sık kullanılan kelimeler.
* **İçerik türü:** Harf/rakam yoğunluğuna göre metin türü tahmini.

#### Tek kelime veya özel veri seçiliyse — Akıllı Tanıma

* **Standart İngilizce kelime:** İngilizce-İngilizce tanımı getirir; bulunamazsa Tureng'e yönlenir.
* **IP adresi (`192.168.1.1` formatı):** Konum, ISS ve ülke bilgisini sorgular.
* **ISBN numarası (10 veya 13 hane):** Kitabın adını, yazarını ve yayıncısını getirir.

---

### 🔠 Anagram Çözücü *(Güncellendi)*

Katman komutundan sonra `0` (Sıfır) tuşuna basın.

Elinizdeki harfleri girin (örn: *k r a a l*). Eklenti, bu harflerle yazılabilecek Türkçe kelimeleri uzundan kısaya sıralayarak listeler.

**Kaynak seçimi:** Sonuç listesinin üst kısmındaki açılır menüden farklı bir sözlük kaynağı seçip bulunan kelimelere o kaynakta bakabilirsiniz — listeyi kapatmadan kaynak değiştirebilirsiniz.

---

### 📅 TDK Günün İçeriği

* **Elle erişim:** Katman komutundan sonra `G` tuşuna basın.
* **Otomatik bildirim:** Ayarlar panelinden etkinleştirirseniz NVDA her açıldığında günün içeriği otomatik seslendirilir.
* **Önbellek:** Aynı gün içinde `G`'ye birden fazla kez basıldığında içerik önbellekten anında gelir.

---

### 🕓 Arama Geçmişi

* **Erişim:** Katman komutundan sonra `H` tuşuna basın.
* **İşlevi:** Son 100 aramayı en yeniden eskiye doğru listeler. Seçtiğiniz arama aynı sözlükte yenilenir.
* **Not:** Geçmiş yalnızca oturum süresince bellekte tutulur; NVDA kapatılınca sıfırlanır.

---

### 📋 Alıntı Olarak Kopyalama *(Yeni)*

Bir sorgu yaptıktan sonra katman komutunu açın (`NVDA+Shift+,`) ve **`C`** tuşuna basın.

Sonuç, biçimlendirmesi korunarak panoya kopyalanır. Word, LibreOffice Writer veya modern bir metin düzenleyiciye yapıştırdığınızda içerik girintili bir alıntı bloğu olarak görünür; başlıklar, kalın metin ve madde işaretleri biçimleriyle birlikte aktarılır.

Bu özellik özellikle akademik veya gazetecilik bağlamında değerlidir: Bir tanımı veya açıklamayı kaynak göstererek bir belgeye aktarırken biçimlendirmeyi sıfırdan kurmak zorunda kalmazsınız.

**Not:** Henüz bir sorgu yapılmamışsa NVDA "Kopyalanacak sonuç yok." der. Daha önce yapılmış bir sorgu varsa "Son sonuç panoya kopyalandı." der.

---

### 🗂️ Katman Tuş Listesi

Tüm tuşları ve işlevlerini tek pencerede görmek için katman komutundan sonra `<` (Küçüktür) tuşuna basın.

**Tam liste:**

| Tuş | İşlev |
|-----|-------|
| `1` | TDK + Dil Derneği (Birleşik) |
| `"` | Üçlü Arama (TDK + Dil Derneği + Kubbealtı) |
| `F` | Beşli Arama (TDK + DD + Vikisözlük + Nişanyan + Kubbealtı) |
| `2` | TDK Atasözleri ve Deyimler |
| `3` | Vikisözlük (NVDA penceresinde) |
| `4` | Nişanyan Sözlük (NVDA penceresinde) |
| `5` | Kubbealtı Lugatı (API) |
| `6` | Sadece TDK Güncel Türkçe Sözlük |
| `7` | Sadece Dil Derneği |
| `B` | TDK Bilim ve Sanat Terimleri |
| `Q` | Google |
| `W` | DuckDuckGo |
| `E` | Bing |
| `R` | Yahoo |
| `T` | Yandex |
| `A` | Çevrimdışı Atasözleri Sözlüğü |
| `S` | Tersine Arama (Kavramdan Deyime) |
| `M` | Müzik Terimleri Sözlüğü (madde adı) |
| `N` | Müzik Terimleri (tanım içi arama) |
| `D` | TDK Derleme Sözlüğü (Türkiye Türkçesi Ağızları) |
| `I` | Tureng (İngilizce ↔ Türkçe) |
| `Ö` | TDK Kişi Adları Sözlüğü (ada göre) |
| `Ç` | TDK Kişi Adları Sözlüğü (anlama göre) |
| `*` | İle Başlayan Kelimeler (kaynak seçimli) |
| `-` | İle Biten Kelimeler (kaynak seçimli) |
| `0` | Anagram Çözücü (kaynak seçimli) |
| `C` | Son Sonucu Alıntı Olarak Kopyala |
| `G` | Günün Kelimesi (TDK) |
| `H` | Arama Geçmişi |
| `.` | Metin Analizi / Akıllı Bilgi |
| `<` | Bu Tuş Listesi |
| `Esc` | Katmandan Çık |

---

## ⚙️ Ayarlar ve Özelleştirme

**NVDA Menüsü → Tercihler → Ayarlar → TDK ve Sözlükler**

| Ayar | Açıklama |
|------|----------|
| **Varsayılan Kaynak** | `NVDA`+`,` tuşuna basıldığında doğrudan hangi sözlüğün çalışacağını belirler. |
| **Tureng Limiti** | Tureng sonuç sayısı. `0` veya boş bırakılırsa tamamı gösterilir. Varsayılan: 30. |
| **DD Okunuş Notasyonu** | Dil Derneği'nin `(-.)` hece uzunluğu notasyonunu sözel forma dönüştürür: `(-.)` → `(-.) uzun-kısa heceli`. Notasyonun kendisi silinmez, yanına açıklama eklenir. |
| **TDK Örnek Cümleleri** | TDK sonuçlarında örnek cümlelerin gösterilip gösterilmeyeceği. |
| **Otomatik Kopyalama** | Bulunan sonucun otomatik olarak panoya kopyalanması. |
| **Sesli Geri Bildirim** | Arama başladığında bip sesi. |
| **Sonuç Bildirim Türü** | Sonucun pencerede mi gösterileceği yoksa yalnızca mı sesletileceği. |
| **Başlangıç Bildirimi** | NVDA açılışında Günün Kelimesi'nin otomatik okunması. |

---

## 💡 İpuçları

* **Pencereyi kapatmak:** Sonuç pencereleri NVDA'nın sanal görüntüleme penceresinde açılır. `Esc` ile kapatılır.
* **Alıntı kopyalama:** Sorgu sonrası katman komutunu açıp `C` tuşuna basın; biçimli alıntı panoya alınır ve Word ile LibreOffice'e yapıştırınca biçimlendirme korunur.
* **Tuşları özelleştirmek:** *NVDA Menüsü → Tercihler → Girdi Hareketleri → TDK ve Sözlükler* yolundan tüm komutlara istediğiniz kısayolu atayabilirsiniz.
* **Katman kuralı:** Katman komutundan sonra basılan tuş, yalnızca o an geçerlidir; ardından katman kapanır. Birden fazla işlem yapmak için her seferinde katmanı yeniden açmanız ya da `<` listesini kullanmanız gerekir.

---

## 💖 Teşekkür ve Katkıda Bulunanlar

Bu eklentinin satır satır işlenmesinde ve kodlanmasında emeği geçen şahsım **Çağrı Doğan** olarak; ortaya yalnızca bilgiye erişimi hızlandıran değil, aynı zamanda kullanırken keyif veren bir araç çıkmasından mutluluk duyuyorum.

Bu projenin asıl kıvılcımı **Tuba Vural** sayesinde çakıldı. Fikrin NVDA_TR grubunda filizlenmesinden bugünkü haline gelmesine kadar; test süreçleri, geri bildirimler, kaynak önerileri ve içerik derleme konularındaki titiz çabası ve yol arkadaşlığı için kendisine en içten teşekkürlerimi sunuyorum.

Kodlama sürecindeki desteği için yapay zeka asistanlarımız **Google Gemini** ve **Claude**'a; bilgi hazinelerinden faydalandığımız **TDK**, **Dil Derneği**, **Kubbealtı** ve **Tureng** gibi köklü kurumlara; eserlerini eklentimize dahil ederek değer kattığımız **Ülkü & Hüseyin Kuşçu**, **Ömer Asım Aksoy** ve **Vural Sözer** gibi kıymetli isimlere saygılarımızla...
