# TDK ve Sözlükler (Sürüm 2026.5.4)

* **Yazar:** NVDA_TR
* **Uyumluluk:** NVDA 2022.1 ve sonrası

**🔔 Eklenti İşlev ve Özellikleri:**

* TDK, Dil Derneği ve Kubbealtı Lugatı'nda ayrı ayrı, ikili veya üçlü birleşik arama imkânı.
* TDK Bilim ve Sanat Terimleri Sözlüğü entegrasyonu (70'ten fazla bilim dalı, çok dilli karşılıklar).
* **TDK Derleme Sözlüğü entegrasyonu (yöresel ağız kelimeleri, bölge ve künye bilgisiyle).** *(Yeni)*
* Çevrimdışı Müzik Terimleri Sözlüğü (4700+ madde, hem madde adı hem tanım içi arama).
* TDK Kişi Adları Sözlüğü entegrasyonu (ada göre ve anlama göre arama).
* Kelime listeleme özelliği (İle başlayan / İle biten kelimeler).
* **Anagram ve kelime listesi sonuçları artık varsayılan veya geçici seçili kaynakta aranır.** *(Güncellendi)*
* Akıllı Atasözü ve Deyim arama algoritması.
* Dahili Deyimler ve Atasözleri sözlükleri (çevrimdışı çalışır).
* Tureng (İngilizce-Türkçe / Türkçe-İngilizce) sözlük entegrasyonu.
* İngilizceden İngilizceye sözlük, Metin Analizi, IP ve ISBN çözümleme.
* Vikisözlük, Nişanyan Sözlük ve arama motorlarında tarayıcı üzerinden otomatik arama başlatma.
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

### Üç kurum, tek pencere

Türk dil kurumları birbirini tamamlar, birbirinin alternatifi değildir:

- **TDK Güncel Türkçe Sözlük** — Standart, geniş kapsamlı, çağdaş kullanıma odaklı.
- **Dil Derneği** — Öz Türkçe yaklaşımını benimseyen, yabancı kökenli kelimelere Türkçe karşılık arayan bir çizgide.
- **Kubbealtı Lugatı** — Klasik edebiyatta ve Osmanlı döneminde kullanılan kelimeleri, köken bilgisi ve edebi örneklerle derinlemesine ele alan paha biçilmez bir hazine.

Katman menüsündeki `"` (çift tırnak) tuşuyla bu üç kaynağın yanıtı **tek bir pencerede** üst üste gelir. Kaynaklar aynı anda paralel olarak sorgulanır; toplam bekleme süresi en yavaş API kadardır.

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

**Ne zaman kullanılır:** Aklınıza yarım bir deyim takıldığında, ya da belirli bir kavramı içeren bütün kalıpları bulmak istediğinizde.

**Örnek:** *Taş* yazıp arattığınızda *"taş çatlasa"*, *"taşı gediğine koymak"*, *"taş kesmek"* gibi onlarca deyim listelenir; hepsinin anlamına tek tek ulaşabilirsiniz.

---

### `3` — Vikisözlük *(tarayıcıda açılır)*

**Ne zaman kullanılır:** Türkçe olmayan bir sözcük, dilbilgisel çözümleme ya da çok dilli karşılaştırma istediğinizde. Vikisözlük topluluğu tarafından derlenir; resmi kurumların kapsamamayabileceği argo, bölgesel ağız veya neolojizmler burada bulunabilir.

---

### `4` — Nişanyan Sözlük *(tarayıcıda açılır)*

**Ne zaman kullanılır:** "Bu kelime Türkçeye nasıl girdi?" sorusu aklınızı kurcaladığında. Sevan Nişanyan'ın derlediği bu etimoloji sözlüğü; köken dilini, ilk belgelendiği tarihi ve anlam değişiminin izini sürer.

**Örnek:** *Bütçe* kelimesini arattığınızda kelimenin Fransızca kökenli olduğunu, Osmanlıcaya hangi dönemde ve hangi biçimle girdiğini, hatta kavramın İngiltere ve Fransa'daki siyasi tarihini öğrenirsiniz. Dil meraklıları için bitimsiz bir kaynak.

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

**Örnek:** *Enlem* kelimesini `B` ile arattığınızda Gökbilim, Coğrafya ve Matematik terimleri sözlüklerinden ayrı ayrı sonuçlar gelir:
- **Gökbilim Terimleri Sözlüğü (1969):** Türkçe: *arz derecesi* | İngilizce: *latitude* | Fransızca: *latitude* | Almanca: *Breite* — Bir küre üzerindeki herhangi bir noktanın temel düzlemden açısal uzaklığı…
- **Coğrafya Terimleri Sözlüğü (1980):** Türkçe: *coğrafi arz* | İngilizce: *latitude* — Yeryuvarı üzerinde herhangi bir noktadan geçen koşut çemberin eşlekle arasındaki yay parçasının açısal değeri.

---

### `D` — TDK Derleme Sözlüğü *(doğrudan API, tarayıcı açılmaz)* *(Yeni)*

**Ne işe yarar:** TDK'nın Türkiye Türkçesi Ağızları Sözlüğü'nü sorgular. Anadolu'nun dört bir yanından derlenen yöresel ağız kelimelerini, anlamlarını, kullanıldıkları bölgeleri ve kaynak künye bilgilerini (eser adı, yazar, yayın yılı) tam olarak gösterir. Aynı kelimenin farklı illerdeki anlam değişimleri madde başlıklarıyla ayrıştırılmış şekilde sunulur; künye bilgileri gereksiz tekrar yapılmadan gruplandırılır.

**Ne zaman kullanılır:** Standart sözlüklerde bulunmayan yöresel bir kelimeyle karşılaştığınızda; bir kelimenin farklı illerdeki anlam değişimlerini merak ettiğinizde; tarihî veya lehçe araştırmalarında kaynak künye bilgisine ihtiyaç duyduğunuzda.

**Örnek:** *hor* kelimesini `D` ile arattığınızda kelimenin Trabzon'da "yumurta sarısı", Gaziantep'te "gösterişsiz, çelimsiz", Sivas'ta "bereketsiz" gibi birbirinden farklı anlamlarda kullanıldığı; her anlamın hangi eserde, hangi yazar tarafından derlendiği künye bilgisiyle birlikte gösterilir.

---

### `Ö` — TDK Kişi Adları Sözlüğü (Ada Göre Arama)

**Ne işe yarar:** TDK'nın Kişi Adları Sözlüğü'nü ada göre sorgular (`sozluk.gov.tr`). Aranan adın anlamını, kökenini ve cinsiyetini gösterir.

* Tek sonuç varsa doğrudan gösterir.
* Birden fazla sonuç varsa seçilebilir bir liste açılır.

**Ne zaman kullanılır:** Bir ismin anlamını ya da kökenini merak ettiğinizde. Doğum tescili için uygun isim araştırırken, edebi bir metinde geçen karakter adının ardındaki anlam katmanını keşfetmek istediğinizde.

**Örnek:** *Deniz* yazıp `Ö` ile arattığınızda adın Türkçe kökenli olduğunu, hem kız hem erkek adı olarak kullanıldığını ve "büyük su kütlesi" anlamını taşıdığını görürsünüz.

---

### `Ç` — TDK Kişi Adları Sözlüğü (Anlama Göre Arama)

**Ne işe yarar:** Aynı TDK Kişi Adları Sözlüğü'nü bu sefer **anlam içinde** arama yaparak sorgular. Girdiğiniz kavramı tanımında barındıran tüm adları listeler.

**Ne zaman kullanılır:** Belirli bir anlam veya kavramı taşıyan isimler bulmak istediğinizde. `Ö` tuşunun ada göre aradığını `Ç` anlama göre arar.

**Örnek:** *Işık* yazıp `Ç` ile arattığınızda tanımında ışık, aydınlık veya parlaklık kavramı geçen tüm adlar listelenir: Aydın, Nûr, Ziya, Işıl ve diğerleri.


### `Q` – `T` — Arama Motorları *(tarayıcıda açılır)*

Sözlüklerde karşılık bulamadığınız özel isimler, teknik terimler, kısaltmalar veya güncel olaylar için seçili metni doğrudan tarayıcıda arar:

| Tuş | Motor | En iyi kullanım |
|-----|-------|-----------------|
| `Q` | Google | Genel, kapsamlı, haber ve akademik |
| `W` | DuckDuckGo | Gizlilik odaklı, reklamsız sonuçlar |
| `E` | Bing | Microsoft ekosistemi, görsel arama |
| `R` | Yahoo | Haber ve finans haberleri |
| `T` | Yandex | Türkiye lokasyonlu, Rusça içerik |

---

### `A` — Yerel (Çevrimdışı) Sözlük

**Ne işe yarar:** Eklentiyle birlikte gelen dahili veritabanında arama yapar. Aranan kelimenin geçtiği tüm deyim ve atasözlerini anında listeler.

**Ne zaman kullanılır:** İnternet bağlantısı olmadığında veya çok hızlı bir başvuruya ihtiyaç duyduğunuzda. API çağrısı yapmadığı için yanıt anlık gelir.

---

### `S` — Tersine Arama (Kavramdan Deyime)

**Ne işe yarar:** Yerel sözlükteki **tanımların içinde** arama yapar; başlığa değil, açıklamaya bakar.

**Ne zaman kullanılır:** Kavramı biliyorsunuz ama onu en iyi ifade eden deyimi unuttuğunuzda. Klasik sözlüklerin yapamadığı "anlam odaklı" aramayı gerçekleştirir.

**Örnek:** *Sabır* yazıp arattığınızda, başlığında "sabır" geçmeyen ancak tanımında bu kavrama değinen deyimler de listelenir; kavramı farklı biçimlerde dile getiren kalıpları bir arada görürsünüz.

---

### `M` — Müzik Terimleri Sözlüğü *(çevrimdışı)*

**Ne işe yarar:** 4700'ü aşkın müzik terimini barındıran çevrimdışı sözlükte **madde adına göre** arama yapar. Türk müziği makamları, çalgı adları, Batı müziği terimleri ve icra yönergeleri aynı veritabanında bir arada yer alır.

Sözlük üç ana kaynaktan oluşur: Turkish Music Portal, Evin İlyasoğlu'nun Müzik Terimleri Sözlüğü ve Vural Sözer'in Müzik Terimleri Sözlüğü. Bu üç kaynağın ortak maddeleri tekilleştirilerek birleştirilmiştir.

**Ne zaman kullanılır:** Müzik metni okurken ya da yazarken karşılaştığınız bir terimin tanımına hızlıca ulaşmak istediğinizde. Birden fazla eşleşme varsa seçilebilir bir liste açılır.

**Örnek:** *Makam* yazıp `M` ile arattığınızda makam, makam geçişi, makam taşıması gibi başlıklar listelenir; birini seçince tam tanıma ulaşırsınız.

---

### `N` — Müzik Terimleri (Tanım İçi Arama) *(çevrimdışı)*

**Ne işe yarar:** Aynı müzik sözlüğünde bu sefer **tanımların içinde** arama yapar. Aranan kavramın madde başlığında değil, açıklamasında geçtiği tüm maddeler listelenir.

**Ne zaman kullanılır:** Bir kavramı içeren ama o kavramı başlığa taşımamış maddeleri bulmak istediğinizde. `S` tuşunun atasözleri sözlüğüne yaptığını `N` müzik sözlüğüne yapar.

**Örnek:** *Perde* yazıp `N` ile arattığınızda, başlığında "perde" geçmeyen ancak tanımında bu terimi kullanan tüm maddeler listelenir.

---

### 🧩 Kelime Avcısı (Liste Modu)

Bulmaca çözerken, şiir yazarken ya da bir kalıba uyan kelimeleri ararken kullanabileceğiniz listeleme özelliği.

Katman komutunu (`NVDA`+`Shift`+`,`) uyguladıktan sonra:

* **`*` (Yıldız):** Seçili veya yazılan ifadeyle **BAŞLAYAN** kelimeleri listeler.
* **`-` (Tire):** Seçili veya yazılan ifadeyle **BİTEN** kelimeleri listeler.

Listeden bir kelime seçip `Enter`'a basınca eklenti o kelimeyi **o an etkin olan kaynakta** sorgular. Katman menüsünden geçici bir kaynak seçilmişse o kaynak, seçilmemişse ayarlardaki varsayılan kaynak kullanılır.

**Örnek:** *Çiçek* yazıp `*` tuşuna basarsanız: çiçek, çiçekli, çiçekçi, çiçekalma, çiçeklenmek… gibi onlarca sonuç listelenir. `-` tuşuyla *lik* yazıp ararsanız "lik" ile biten tüm kelimeleri bulursunuz.

---

### `I` — Tureng Sözlük (İngilizce ↔ Türkçe)

**Ne işe yarar:** Tureng.com veritabanını doğrudan sorgular. Tarayıcı açmadan, kelimenin farklı bağlamlardaki karşılıklarını (genel, teknik, argo, tıbbi vb.) ve örnek cümleleri listeler.

**Ne zaman kullanılır:** İngilizce bir metin okurken bilmediğiniz bir kelimeye denk geldiğinizde veya Türkçe bir ifadenin İngilizce karşılığını aradığınızda.

**Örnek:** *Leverage* kelimesini `I` ile arattığınızda; finans, mühendislik ve günlük kullanımdaki Türkçe karşılıkları ayrı kategorilerde listelenir.

---

### 📊 Metin Analizi ve Bilgi Sistemi

Katman komutundan sonra `.` (Nokta) tuşuna basın.

#### Çoklu kelime seçiliyse — Metin İstatistikleri

Uzunca bir metin bloğu seçip `.` tuşuna bastığınızda:

* **Okuma süresi:** Ortalama okuma hızına göre dakika cinsinden tahmin.
* **Kelime sayısı:** Noktalama işaretleri ayrıştırılarak doğru sayım.
* **Yapısal analiz:** Paragraf ve cümle sayısı.
* **Frekans analizi:** Metindeki en sık kullanılan kelimeler.
* **İçerik türü:** Harf/rakam yoğunluğuna göre metin türü tahmini.

**Örnek kullanım:** Yazdığınız bir dilekçenin kaç kelime içerdiğini, ortalama cümle uzunluğunu ve hangi kelimeleri tekrar ettiğinizi öğrenmek için son derece kullanışlıdır.

#### Tek kelime veya özel veri seçiliyse — Akıllı Tanıma

Modül, seçilen verinin türüne göre otomatik karar verir:

* **Standart İngilizce kelime:** İngilizce-İngilizce tanımı getirir; bulunamazsa Tureng'e yönlenir.
* **IP adresi (`192.168.1.1` formatı):** Konum, ISS ve ülke bilgisini sorgular.
* **ISBN numarası (10 veya 13 hane):** Kitabın adını, yazarını ve yayıncısını getirir.

**Örnek:** Bir akademik kaynak listesinde `9789754583038` gibi bir ISBN görüp `.` tuşuna basarsanız; kitabın adına ve yazarına anında ulaşırsınız.

---

### 🔠 Anagram Çözücü

Katman komutundan sonra `0` (Sıfır) tuşuna basın.

Elinizdeki harfleri girin (örn: *k r a a l*). Eklenti, bu harflerle yazılabilecek Türkçe kelimeleri uzundan kısaya sıralayarak listeler. Listeden bir kelime seçtiğinizde **o an etkin olan kaynakta** aranır; katman menüsünden geçici kaynak seçilmişse o kaynak, seçilmemişse varsayılan kaynak kullanılır.

**Örnek:** *a l a k* harflerini girerseniz *kala* ve *laka* gibi geçerli Türkçe kelimeler listelenir. Bulmaca ve kelime oyunları için güçlü bir araç.

---

### 📅 TDK Günün İçeriği

TDK'nin her gün yayınladığı "Günün Kelimesi" ve "Günün Atasözü/Deyimi"ne ulaşmanın iki yolu:

* **Elle erişim:** Katman komutundan sonra `G` tuşuna basın.
* **Otomatik bildirim:** Ayarlar panelinden etkinleştirirseniz NVDA her açıldığında günün içeriği otomatik seslendirilir.
* **Önbellek:** Aynı gün içinde `G`'ye birden fazla kez basıldığında içerik önbellekten anında gelir; gereksiz API çağrısı yapılmaz.

---

### 🕓 Arama Geçmişi

* **Erişim:** Katman komutundan sonra `H` tuşuna basın.
* **İşlevi:** Son 100 aramayı en yeniden eskiye doğru listeler. Seçtiğiniz aramanın aynı sözlükte yenilenir.
* **Not:** Geçmiş yalnızca oturum süresince bellekte tutulur; NVDA kapatılınca sıfırlanır.

---

### 🗂️ Katman Tuş Listesi

Tüm tuşları ve işlevlerini tek pencerede görmek için katman komutundan sonra `<` (Küçüktür) tuşuna basın.

Açılan listeden bir öğeyi seçince o işlem doğrudan başlatılır; liste `Esc` ile kapatılana kadar açık kalır, birden fazla işlem yapabilirsiniz.

**Tam liste:**

| Tuş | İşlev |
|-----|-------|
| `1` | TDK + Dil Derneği (Birleşik) |
| `"` | Üçlü Arama (TDK + Dil Derneği + Kubbealtı) |
| `2` | TDK Atasözleri ve Deyimler |
| `3` | Vikisözlük (tarayıcı) |
| `4` | Nişanyan Sözlük (tarayıcı) |
| `5` | Kubbealtı Lugatı (API) |
| `6` | Sadece TDK Güncel Türkçe Sözlük |
| `7` | Sadece Dil Derneği |
| `B` | TDK Bilim ve Sanat Terimleri |
| `D` | TDK Derleme Sözlüğü *(Yeni)* |
| `Q` | Google |
| `W` | DuckDuckGo |
| `E` | Bing |
| `R` | Yahoo |
| `T` | Yandex |
| `A` | Çevrimdışı Atasözleri Sözlüğü |
| `S` | Tersine Arama (Kavramdan Deyime) |
| `M` | Müzik Terimleri Sözlüğü (madde adı) |
| `N` | Müzik Terimleri (tanım içi arama) |
| `I` | Tureng (İngilizce ↔ Türkçe) |
| `Ö` | TDK Kişi Adları Sözlüğü (ada göre) |
| `Ç` | TDK Kişi Adları Sözlüğü (anlama göre) |
| `*` | İle Başlayan Kelimeler |
| `-` | İle Biten Kelimeler |
| `0` | Anagram Çözücü |
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
| **Varsayılan Kaynak** | `NVDA`+`,` hızlı araması ile kelime listesi ve anagram sonuçlarından yapılan aramalar bu kaynağı kullanır. |
| **Tureng Limiti** | Tureng sonuç sayısı. `0` veya boş bırakılırsa tamamı gösterilir. Varsayılan: 30. |
| **TDK Örnek Cümleleri** | TDK sonuçlarında örnek cümlelerin gösterilip gösterilmeyeceği. |
| **Otomatik Kopyalama** | Bulunan sonucun otomatik olarak panoya kopyalanması. |
| **Sesli Geri Bildirim** | Arama başladığında bip sesi. |
| **Sonuç Bildirim Türü** | Sonucun pencerede mi gösterileceği yoksa yalnızca mı sesletileceği. |
| **Başlangıç Bildirimi** | NVDA açılışında Günün Kelimesi'nin otomatik okunması. |

---

## 💡 İpuçları

* **Pencereyi kapatmak:** Sonuç pencereleri NVDA'nın sanal görüntüleme penceresinde açılır. `Esc` ile kapatılır.
* **Tuşları özelleştirmek:** *NVDA Menüsü → Tercihler → Girdi Hareketleri → TDK ve Sözlükler* yolundan tüm komutlara istediğiniz kısayolu atayabilirsiniz.
* **Katman kuralı:** Katman komutundan sonra basılan tuş, yalnızca o an geçerlidir; ardından katman kapanır. Birden fazla işlem yapmak için her seferinde katmanı yeniden açmanız ya da `<` listesini kullanmanız gerekir.
* **Geçici kaynak seçimi:** Katman menüsünden seçtiğiniz kaynak o oturum için geçici olarak etkinleşir. Kelime listesi, anagram ve `NVDA`+`,` hızlı araması bu geçici seçimi dikkate alır.

---

## 💖 Teşekkür ve Katkıda Bulunanlar

Bu eklentinin satır satır işlenmesinde ve kodlanmasında emeği geçen şahsım **Çağrı Doğan** olarak; ortaya yalnızca bilgiye erişimi hızlandıran değil, aynı zamanda kullanırken keyif veren bir araç çıkmasından mutluluk duyuyorum.

Bu projenin asıl kıvılcımı **Tuba Vural** sayesinde çakıldı. Fikrin NVDA_TR grubunda filizlenmesinden bugünkü haline gelmesine kadar; test süreçleri, geri bildirimler, kaynak önerileri ve içerik derleme konularındaki titiz çabası ve yol arkadaşlığı için kendisine en içten teşekkürlerimi sunuyorum.

Kodlama sürecindeki desteği için yapay zeka asistanlarımız **Google Gemini** ve **Claude**'a; bilgi hazinelerinden faydalandığımız **TDK**, **Dil Derneği**, **Kubbealtı** ve **Tureng** gibi köklü kurumlara; eserlerini eklentimize dahil ederek değer kattığımız **Ülkü & Hüseyin Kuşçu**, **Ömer Asım Aksoy** ve **Vural Sözer** gibi kıymetli isimlere saygılarımızla...
