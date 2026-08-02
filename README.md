# TDK ve Sözlükler

* **Yazar:** Çağrı Doğan
* **Uyumluluk:** NVDA 2022.1 ve sonrası

** Eklenti İşlev ve Özellikleri:**

* TDK, Dil Derneği ve Kubbealtı Lugatı'nda ayrı ayrı, ikili veya çoklu birleşik arama imkânı.
* **Çoklu Arama ve Çoklu Arama 2: kaynaklarını ayarlardan özelleştirebileceğiniz iki yapılandırılabilir birleşik arama modu.** *(Güncellendi)*
* **Çevrimdışı Eş/Zıt Anlamlı Sözlük — 42.000'den fazla kelime, internet bağlantısı gerekmez.** *(Yeni)*
* **Çevrimdışı Kafiye Sözlüğü — 81.000'den fazla kelime; zengin, tam ve yarım kafiye gruplarıyla.** *(Yeni)*
* TDK Bilim ve Sanat Terimleri Sözlüğü (70'ten fazla bilim dalı, çok dilli karşılıklar).
* Çevrimdışı Müzik Terimleri Sözlüğü (4700+ madde, madde adı ve tanım içi arama).
* **Çevrimdışı Argo Sözlüğü — Hulki Aktunç'un Büyük Argo Sözlüğü'nden 5.200'den fazla madde, internet bağlantısı gerekmez.** *(Yeni)*
* **TDK Batı Kökenli Sözcükler Sözlüğü — batı kökenli sözcüklerin Türkçe açıklamaları ve örnek cümleler.** *(Yeni)*
* TDK Kişi Adları Sözlüğü (ada göre ve anlama göre arama).
* Kelime listeleme (İle başlayan / İle biten) kaynak seçimiyle.
* Anagram çözücü kaynak seçimiyle.
* Sonuç pencerelerinden biçimli alıntı kopyalama (CF_HTML + düz metin).
* Akıllı Atasözü ve Deyim arama algoritması.
* Dahili Deyimler ve Atasözleri sözlükleri (çevrimdışı çalışır).
* Tureng (İngilizce-Türkçe / Türkçe-İngilizce) sözlük entegrasyonu.
* TDK Derleme Sözlüğü (Türkiye Türkçesi Ağızları — yöresel kelimeler ve yörelerine göre anlamları).
* İngilizceden İngilizceye sözlük, Metin Analizi, IP ve ISBN çözümleme.
* Vikisözlük ve Nişanyan Sözlük sonuçları NVDA penceresinde gösterilir; tarayıcı açılmaz.
* Arama geçmişi (son 100 arama oturum boyunca bellekte tutulur).
* Günün Kelimesi önbelleği (aynı gün içinde tekrar API çağrısı yapılmaz).
* Katman menüsünden etkileşimli tuş listesi.

---

## Eklentinin Felsefesi

Türkçe, binlerce yıllık kültürel birikimin taşıyıcısı olan bir dildir. Kelimelerin anlamını, kökenini ve kullanım bağlamını kavramak; sadece bir tanım öğrenmek değil, dilin iç dünyasıyla kurulan bir ilişkidir. Ancak bu ilişkiyi kurmak için gereken her araç — TDK, Dil Derneği, Kubbealtı, Nişanyan — günümüzde ya görsel arayüzlerle çevrilmiş, ya reklam katmanlarının arkasına gömülmüş ya da ekran okuyucuyla güçlükle gezilebilen web sayfaları hâline gelmiştir.

Ekran okuyucu kullanan biri için "hızlıca bir kelimeye bakmak", görme engeli olmayan bir okuyucuya kıyasla çok daha fazla adım gerektirir: tarayıcıyı açmak, adresi yazmak, sayfanın yüklenmesini beklemek, başlıklar ve bölümler arasında gezinerek asıl içeriğe ulaşmak, ardından tekrar okumakta olduğunuz yere dönmek. Okuma akışını bölen bu sürtünme, zaman içinde bir mikro yorgunluk birikimine dönüşür.

**TDK ve Sözlükler** bu sürtünmeyi ortadan kaldırmak için tasarlanmıştır.

### Damıtılmış bilgi, saf anlam

Web sözlükleri belirli bir kullanım biçimini ön varsayar: fare ile gezmek, gözle taramak, reklam alanlarını görmezden gelmek. Bu ön varsayım, söz konusu kaynakların ekran okuyucuyla kullanılmasını başından zorlaştırır.

Eklenti, bu kaynakların API'lerine ve veri akışlarına doğrudan erişerek yalnızca anlam bilgisini — tanımı, örnek cümleyi, köken notunu — alır ve NVDA'nın konuşma akışına en uygun biçimde sunar. Ortada reklam bloku yoktur, gezinilecek menü yoktur, yüklenecek resim yoktur. Yalnızca kelime vardır ve kelimenin anlamı.

Bu yaklaşımın somut karşılığı şudur: Bir Osmanlıca edebi metni okurken karşılaştığınız *müstağni* kelimesinin TDK'daki modern karşılığını, Kubbealtı'daki köklü tanımını ve Dil Derneği'nin sade açıklamasını **tek bir tuş kombinasyonuyla** ve **tarayıcınızı açmadan** yan yana görebilirsiniz.

### Birden fazla kurum, tek pencere

Türk dil kurumları birbirini tamamlar, birbirinin alternatifi değildir:

- **TDK Güncel Türkçe Sözlük** — Standart, geniş kapsamlı, çağdaş kullanıma odaklı.
- **Dil Derneği** — Öz Türkçe yaklaşımını benimseyen, yabancı kökenli kelimelere Türkçe karşılık arayan bir çizgide.
- **Kubbealtı Lugatı** — Klasik edebiyatta ve Osmanlı döneminde kullanılan kelimeleri, köken bilgisi ve edebi örneklerle derinlemesine ele alan paha biçilmez bir hazine.
- **Vikisözlük** — Topluluk tarafından derlenen; argo, bölgesel ağız ve neolojizmleri resmi kurumlardan önce kapsayan açık kaynak.
- **Nişanyan Sözlük** — Sevan Nişanyan'ın hazırladığı etimoloji sözlüğü; kelimenin köken dilini, ilk belgelendiği tarihi ve anlam değişiminin izini sürer.

Katman menüsündeki `F` tuşuyla **Çoklu Arama**, `"` tuşuyla **Çoklu Arama 2** başlatılır; seçili kaynakların yanıtları tek bir pencerede üst üste gelir. Her iki aramanın hangi kaynakları sorguladığı ayarlar panelinden özelleştirilebilir. Kaynaklar paralel sorgulandığından toplam bekleme süresi en yavaş API kadardır.

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

**Tüm tuş listesi için `<` (Küçüktür) tuşuna basın.**

---

## Hangi Kaynağı Ne Zaman Kullanmalıyım?

### `1` — Birleşik Arama (TDK + Dil Derneği)

**Ne işe yarar:** TDK ile Dil Derneği'ni eş zamanlı tarar; sonuçları tek pencerede alt alta gösterir.

**Ne zaman kullanılır:** Kelimenin hem yaygın hem de öz Türkçe karşılığını merak ettiğinizde. İki kurumun tanımları çoğu zaman birbirini tamamlar; kimi zaman ise ince anlam farklarını ortaya koyar.

---

### `"` — Çoklu Arama 2 *(Güncellendi)*

**Ne işe yarar:** Varsayılan olarak TDK + Dil Derneği + Kubbealtı Lugatı'nı paralel sorgular; sonuçları tek pencerede sunar. Hangi kaynakların sorgulanacağı **ayarlar panelinden** özelleştirilebilir.

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

### `F` — Çoklu Arama *(Güncellendi)*

**Ne işe yarar:** Varsayılan olarak TDK, Dil Derneği, Vikisözlük, Nişanyan ve Kubbealtı'nı aynı anda paralel sorgular; sonuçları tek bir NVDA penceresinde üst üste gösterir. Hangi kaynakların dahil edileceği **ayarlar panelinden** özelleştirilebilir — listeye Eş/Zıt Anlamlılar, TDK Bilim Sözlüğü ve TDK Derleme Sözlüğü de eklenebilir.

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

### `J` — Argo Sözlüğü *(çevrimdışı)* *(Yeni)*

**Ne işe yarar:** Hulki Aktunç'un *Türkçenin Büyük Argo Sözlüğü*'nden derlenen 5.200'den fazla maddeyi barındıran çevrimdışı sözlükte **madde adına göre** arama yapar. Birden fazla eşleşme varsa seçilebilir bir liste açılır.

**Ne zaman kullanılır:** Bir argo sözcüğün tanımını, etimolojisini veya örnek kullanımını merak ettiğinizde. Sokak dili, tarihi Türkçe argo ve toplumsal jargon açısından kapsamlı bir kaynak.

**Örnek:** *Palavra* yazıp `J` ile arattığınızda kelimenin İspanyolca kökenini, tanımını ve Yahya Kemal'den alınan örnek cümleyi görürsünüz.

---

### `K` — Argo Sözlüğü (Tanım İçi Arama) *(çevrimdışı)* *(Yeni)*

**Ne işe yarar:** Aynı argo sözlüğünde bu sefer **tanımların içinde** arama yapar. `S` tuşunun atasözleri sözlüğüne yaptığını, `N` tuşunun müzik sözlüğüne yaptığını `K` argo sözlüğüne yapar.

**Ne zaman kullanılır:** Kavramı biliyorsunuz ama onu karşılayan argo sözcüğü bulamıyorsunuz. Örneğin *rezil* yazıp arattığınızda tanımında bu kavram geçen madde başlıkları listelenir.

---

### `Z` — Eş/Zıt Anlamlı Sözlük *(çevrimdışı)* *(Yeni)*

**Ne işe yarar:** 42.000'den fazla kelimeyi kapsayan çevrimdışı eş/zıt anlamlı sözlükte arama yapar. Kaynak, Boğaziçi Üniversitesi bünyesinde derlenen ve akademisyenler tarafından elle doğrulanmış **KeNet Türkçe WordNet** veritabanıdır. İnternet bağlantısı gerekmez.

**Ne zaman kullanılır:** Bir kelimenin yerine geçebilecek başka kelimeler ararken, yazarken eş anlamlı seçenek değerlendirirken ya da zıt anlamlıları öğrenmek istediğinizde.

**Örnek:** *Güzel* yazıp arattığınızda eş anlamlı olarak *hoş*, *latif*, *tatlı*, *şirin* gibi seçenekler; zıt anlamlı olarak *çirkin* listelenir. *Büyük* için eş anlamlılar arasında *iri*, *koca*, *kocaman*; zıt anlamlılar arasında *küçük*, *ufak* görünür.

**Not:** Sözlük kelime köklerine göre çalışır; arama küçük harfe dönüştürülerek yapılır.

---

### `Y` — Kafiye Sözlüğü *(çevrimdışı)* *(Yeni)*

**Ne işe yarar:** 81.000'den fazla kelimeyi kapsayan çevrimdışı kafiye sözlüğünde arama yapar. Kaynak, **KeNet Türkçe WordNet** veritabanının kelime listesidir. Aranan kelimeyle sondan itibaren kaç harf ortaksa sonuçlar o kadar güçlü kafiye sayılır ve üç grupta listelenir: **Zengin Kafiye** (3 veya daha fazla ortak harf), **Tam Kafiye** (2 ortak harf) ve **Yarım Kafiye** (1 ortak harf). İnternet bağlantısı gerekmez; yanıt anlık gelir.

**Ne zaman kullanılır:** Şiir veya şarkı sözü yazarken, tekerleme ararken ya da bir kelimeyle sesteş biten seçenekleri hızlıca görmek istediğinizde.

**Örnek:** *Güzel* yazıp `Y` ile arattığınızda Zengin Kafiye grubunda *gazel*, *dizel*, *ezel*, *tüzel* gibi sonuçlar; *Mutlu* için ise *umutlu*, *kutlu*, *bulutlu* gibi sonuçlar görürsünüz.

**Not:** Yarım Kafiye grubu kısa kelimelerde binlerce sonuç içerebileceğinden varsayılan olarak gösterilmez. Ayarlar panelinden "Sınırlı (İlk 100)" veya "Hepsini Göster" seçilerek etkinleştirilebilir.

---

### `X` — TDK Batı Kökenli Sözcükler *(Yeni)*

**Ne işe yarar:** TDK'nın Batı Kökenli Sözcükler Sözlüğü'nü sorgular (`sozluk.gov.tr/bati`). Avrupa dillerinden Türkçeye geçmiş sözcükler için açıklamaları, sözcük türünü ve  örnek cümleler gösterir.

**Ne zaman kullanılır:** Metinde karşılaştığınız batı  kökenli bir sözcüğün anlamını öğrenmek ve örnek cümleler istediğinizde. Öz Türkçe yazım hedeflerken veya çeviri yaparken pratik bir başvuru noktasıdır.

**Örnek:** *Organizasyon* yazıp `X` ile arattığınızda örgütlenme* ya da *düzenleme* gibi Türkçe karşılıkları ve çeşitli eserlerden alıntılanan çok sayıda örnek cümle görürsünüz.

---

### `D` — TDK Derleme Sözlüğü *(Türkiye Türkçesi Ağızları)*

**Ne işe yarar:** TDK'nın Derleme Sözlüğü'nü sorgular. Standart Türkçede bulunmayan ya da farklı anlamlar kazanmış yöresel kelimeleri; anlamları, kullanıldıkları il ve ilçeler ile kaynak künyesiyle birlikte sunar.

**Ne zaman kullanılır:** Yöresel bir kelimeyle karşılaştığınızda, bir kelimenin Anadolu'nun farklı bölgelerindeki kullanımını merak ettiğinizde ya da sözlü edebiyat ve folklor metinleri üzerine çalışırken.

**Örnek:** *Kötek* yazıp `D` ile arattığınızda kelimenin hangi illerde hangi anlamlarda kullanıldığını ve hangi derleme kaynaklarında belgelendiğini görürsünüz.

---

### Kelime Avcısı (Liste Modu) *(Güncellendi)*

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

### Metin Analizi ve Bilgi Sistemi

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

### Anagram Çözücü *(Güncellendi)*

Katman komutundan sonra `0` (Sıfır) tuşuna basın.

Elinizdeki harfleri girin (örn: *k r a a l*). Eklenti, bu harflerle yazılabilecek Türkçe kelimeleri uzundan kısaya sıralayarak listeler.

**Kaynak seçimi:** Sonuç listesinin üst kısmındaki açılır menüden farklı bir sözlük kaynağı seçip bulunan kelimelere o kaynakta bakabilirsiniz — listeyi kapatmadan kaynak değiştirebilirsiniz.

---

### TDK Günün İçeriği

* **Elle erişim:** Katman komutundan sonra `G` tuşuna basın.
* **Otomatik bildirim:** Ayarlar panelinden etkinleştirirseniz NVDA her açıldığında günün içeriği otomatik seslendirilir.
* **Önbellek:** Aynı gün içinde `G`'ye birden fazla kez basıldığında içerik önbellekten anında gelir.

---

### Arama Geçmişi

* **Erişim:** Katman komutundan sonra `H` tuşuna basın.
* **İşlevi:** Son 100 aramayı en yeniden eskiye doğru listeler. Seçtiğiniz arama aynı sözlükte yenilenir.
* **Not:** Geçmiş, oturumlar arasında diske kaydedilir; NVDA kapatılıp açıldıktan sonra da korunur.

---

### Alıntı Olarak Kopyalama *(Yeni)*

Bir sorgu yaptıktan sonra katman komutunu açın (`NVDA+Shift+,`) ve **`C`** tuşuna basın.

Sonuç, biçimlendirmesi korunarak panoya kopyalanır. Word, LibreOffice Writer veya modern bir metin düzenleyiciye yapıştırdığınızda içerik girintili bir alıntı bloğu olarak görünür; başlıklar, kalın metin ve madde işaretleri biçimleriyle birlikte aktarılır.

Bu özellik özellikle akademik veya gazetecilik bağlamında değerlidir: Bir tanımı veya açıklamayı kaynak göstererek bir belgeye aktarırken biçimlendirmeyi sıfırdan kurmak zorunda kalmazsınız.

**Not:** Henüz bir sorgu yapılmamışsa NVDA "Kopyalanacak sonuç yok." der. Daha önce yapılmış bir sorgu varsa "Son sonuç panoya kopyalandı." der.

---

### Katman Tuş Listesi

Tüm tuşları ve işlevlerini tek pencerede görmek için katman komutundan sonra `<` (Küçüktür) tuşuna basın.

**Tam liste:**

| Tuş | İşlev |
|-----|-------|
| `1` | TDK + Dil Derneği (Birleşik) |
| `"` | Çoklu Arama 2 (Yapılandırılabilir — varsayılan: TDK + Dil Derneği + Kubbealtı) |
| `F` | Çoklu Arama (Yapılandırılabilir — varsayılan: TDK + DD + Vikisözlük + Nişanyan + Kubbealtı) |
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
| `J` | Argo Sözlüğü (madde adı) |
| `K` | Argo Sözlüğü (tanım içi arama) |
| `Z` | Eş/Zıt Anlamlı Sözlük (çevrimdışı) |
| `Y` | Kafiye Sözlüğü (çevrimdışı) |
| `X` | TDK Batı Kökenli Sözcüklere Türkçe Karşılıklar |
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

## Ayarlar ve Özelleştirme

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
| **Kafiye Sözlüğünde Yarım Kafiye Gösterimi** *(Yeni)* | Yarım kafiye sonuçlarının (1 ortak harf) gösterilip gösterilmeyeceğini belirler: Gösterme (varsayılan), Sınırlı Göster (İlk 100) veya Hepsini Göster. |
| **Çoklu Arama Kaynakları** *(Güncellendi)* | Çoklu Arama'nın (`F` tuşu) hangi sözlükleri sorgulayacağını belirler. Ok tuşlarıyla gezilip Boşluk ile işaretlenebilen listeden TDK, Dil Derneği, Kubbealtı, Vikisözlük, Nişanyan, Eş/Zıt Anlamlılar, TDK Bilim Sözlüğü ve TDK Derleme Sözlüğü arasından seçim yapılır. Varsayılan: TDK + Dil Derneği + Vikisözlük + Nişanyan + Kubbealtı. |
| **Çoklu Arama 2 Kaynakları** *(Güncellendi)* | Çoklu Arama 2'nin (`"` tuşu) hangi sözlükleri sorgulayacağını belirler. Aynı kaynak listesinden seçim yapılır. Varsayılan: TDK + Dil Derneği + Kubbealtı. |

---

## İpuçları

* **Pencereyi kapatmak:** Sonuç pencereleri NVDA'nın sanal görüntüleme penceresinde açılır. `Esc` ile kapatılır.
* **Alıntı kopyalama:** Sorgu sonrası katman komutunu açıp `C` tuşuna basın; biçimli alıntı panoya alınır ve Word ile LibreOffice'e yapıştırınca biçimlendirme korunur.
* **Tuşları özelleştirmek:** *NVDA Menüsü → Tercihler → Girdi Hareketleri → TDK ve Sözlükler* yolundan tüm komutlara istediğiniz kısayolu atayabilirsiniz.
* **Katman kuralı:** Katman komutundan sonra basılan tuş, yalnızca o an geçerlidir; ardından katman kapanır. Birden fazla işlem yapmak için her seferinde katmanı yeniden açmanız ya da `<` listesini kullanmanız gerekir.

---

## Teşekkür ve Katkıda Bulunanlar

Bu eklentinin satır satır işlenmesinde ve kodlanmasında emeği geçen şahsım **Çağrı Doğan** olarak; ortaya yalnızca bilgiye erişimi hızlandıran değil, aynı zamanda kullanırken keyif veren bir araç çıkmasından mutluluk duyuyorum.

Bu projenin asıl kıvılcımı **Tuba Vural** sayesinde çakıldı. Fikrin NVDA_TR grubunda filizlenmesinden bugünkü haline gelmesine kadar; test süreçleri, geri bildirimler, kaynak önerileri ve içerik derleme konularındaki titiz çabası ve yol arkadaşlığı için kendisine en içten teşekkürlerimi sunuyorum.

Kodlama sürecindeki desteği için yapay zeka asistanlarımız **Google Gemini** ve **Claude**'a; bilgi hazinelerinden faydalandığımız **TDK**, **Dil Derneği**, **Kubbealtı** ve **Tureng** gibi köklü kurumlara; eserlerini eklentimize dahil ederek değer kattığımız **Ülkü & Hüseyin Kuşçu**, **Ömer Asım Aksoy**, **Vural Sözer** ve **Hulki Aktunç** gibi kıymetli isimlere saygılarımızla...