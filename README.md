# TDKSozluk
NVDA için geliştirilen TDK ve Sözlükler adlı bu eklenti TDK Güncel Türkçe Sözlük, Dil Derneği, Vikisözlük, Nişanyan, Kubbealtı Lugatı, dahili deyim ve atasözleri sözlükleri, web motorları ve Tureng sözlük'te hızlı arama yapmanızı sağlar.
# TDK ve Sözlükler (Sürüm 2026.3.5)

* **Yazar:** NVDA_TR
* **Uyumluluk:** NVDA 2022.1 ve sonrası

**🔔 Eklenti İşlev ve Özellikleri:**

* TDK ve Dil Derneği sözlüklerinde ayrı ayrı veya birleşik arama imkânı.
* Kelime listeleme özelliği (İle başlayan ve İle biten kelimeler).
* Akıllı Atasözü ve Deyim arama algoritması.
* Dahili Deyimler ve Atasözleri Sözlükleri.
* Tureng (İngilizce-Türkçe / Türkçe-İngilizce) sözlük entegrasyonu.
* İngilizceden İngilizceye sözlük, Metin Analizi, IP ve ISBN çözümleme.
* Wikisözlük, Nişanyan Sözlük, Kubbealtı Lugatı gibi sözlüklerde ve Google, Duckduckgo, Yandex, Bing, Yahoo gibi arama motorlarında tarayıcı üzerinden otomatik arama başlatma olanağı.

---

### 🎯 Eklentinin Felsefesi

Bilgiye erişim, bir tarayıcı sekmesi açıp reklam yığınları arasında boğuşmaktan çok daha zahmetsiz olmalıdır. Özellikle bir metni okurken karşılaştığınız ve aşina olmadığınız bir kelime, deyim veya ifade, okuma akışınızı bölmemelidir.

**TDK ve Sözlükler** eklentisi; Türkiye'nin en köklü dil kurumlarının (TDK ve Dil Derneği) hazinesini, ekran okuyucu kullanıcıları için **"damıtılmış"** bir şekilde sunar. Karmaşık web arayüzlerini, görsel kalabalığı ve erişilemez butonları aradan çıkararak, sizi doğrudan kelimenin saf anlamıyla buluşturur.

Amacımız sadece bir sözlük sunmak değil; bilgisayar başındaki dil deneyiminizi hızlandırmak ve zenginleştirmektir.

---

## Nasıl Kullanılır?

Eklenti, iki ana komut yapısı üzerinden çalışır:

### 1. Hızlı Arama (Anlık Bilgi)

Kısayol: `NVDA` + `,` (Virgül)

İmlecin üzerindeki kelimeyi veya o an seçili olan metni, **en son kullandığınız** sözlükte (Varsayılan: Birleşik Arama) anında arar.

* **Metin seçiliyse:** Seçili metni sorgular.
* **Metin seçili değilse:** İmlecin üzerinde durduğu kelimeyi otomatik algılar ve sorgular.
* **Hiçbir şey yoksa:** Ekrana bir yazı kutusu gelir, kelimeyi manuel yazıp `Enter`'a basarak arama yapabilirsiniz.

### 2. Kaynak Seçim Katmanı (Detaylı Araştırma)

Kısayol: `NVDA` + `Shift` + `,` (Virgül)

Bu tuş kombinasyonuna bastığınızda "Sözlük Katmanı" devreye girer ve NVDA size kaynakları sesli olarak sayar. Ardından, elinizi diğer tuşlardan çekip sadece aşağıdaki karakter tuşlarına basarak ilgili kaynağı seçebilirsiniz:

---

## Hangi Kaynağı Ne Zaman Kullanmalıyım?

Her sözlük farklı bir ihtiyaca çözüm sunar. İşte kullanım senaryoları:

### `1` Birleşik Arama (TDK + Dil Derneği)

**Senaryo:** Bir kelimenin anlamını tam olarak kavramak istiyorsunuz, ancak tek bir kuruma bağlı kalmak istemiyorsunuz.

**İşlevi:** TDK ve Dil Derneği veritabanlarını eş zamanlı tarar. Sonuç penceresinde üstte TDK'nin, altta Dil Derneği'nin tanımını sunar. Böylece iki kurum arasındaki anlam nüanslarını (örneğin "Olasılık" ya da "İtikat" kelimeleri için sundukları tanımların farklarını) tek pencere içinde karşılaştırabilirsiniz.

### `2` TDK Atasözleri ve Deyimler (Akıllı Liste)

**Senaryo:** Aklınıza bir deyim takıldı ama tamamını hatırlayamıyorsunuz. "Damla damla göl olur" mu yoksa "Damlaya damlaya" mı emin değilsiniz?

**İşlevi:** Yazdığınız kelimenin geçtiği tüm atasözlerini ve deyimleri tarar.

* Eğer **tek bir sonuç** varsa, doğrudan o sözün anlamını ekrana getirir.
* Eğer **birden fazla sonuç** varsa (Örn: "El" kelimesi geçen yüzlerce deyim), size seçilebilir bir liste penceresi sunar. Listeden seçtiğiniz deyimin anlamı TDK Güncel Sözlük'te aranır.

### `3` - `5` Web Sözlükleri (Tarayıcıda Açılır)

| Tuş | Sözlük | Açıklama |
| --- | --- | --- |
| **`3`** | **Vikisözlük** | Daha sivil, çok dilli ve katılımcı tanımlar için idealdir. |
| **`4`** | **Nişanyan Sözlük** | **"Bu kelime nereden geliyor?"** diyorsanız adresiniz burasıdır. Kelimelerin kökenini (etimoloji), tarihçesini ve hangi dilden geçtiğini öğrenmek için kullanılır. |
| **`5`** | **Kubbealtı Lugatı** | Özellikle Osmanlıca metinler okurken veya "Lügat", "Müşkülpesent" gibi eski/edebi kelimelerin derin manalarını ararken en iyi kaynaktır. |

### `Q` - `T` Arama Motorları

Sözlüklerde bulamadığınız özel isimler, teknik terimler, hata kodları veya genel kültür aramaları için metni doğrudan varsayılan tarayıcınızda açar:

* **`Q` Google:** En kapsamlı genel arama.
* **`W` DuckDuckGo:** Gizlilik odaklı arama.
* **`E` Bing:** Microsoft'un arama motoru.
* **`R` Yahoo:** Haber ve finans ağırlıklı sonuçlar.
* **`T` Yandex:** Özellikle görsel ve Türkiye lokasyonlu aramalarda güçlü bir alternatif.

### `A` Yerel (Çevrimdışı) Sözlük

**Senaryo:** İnternet bağlantınızın olmadığı durumlarda veya çok hızlı başvuru yapmak istediğinizde.

**İşlevi:** Eklentiyle birlikte gelen dâhili veritabanında arama yapar. İçinde aradığınız kelimenin geçtiği tüm deyim ve atasözlerini listeler. Örneğin "Göz" için arama yaptığınızda, içinde "göz" geçen (Göz atmak, Gözden düşmek, İki gözü iki çeşme vb.) yüzlerce başlığı anında önünüze getirir.

### `S` Tersine Arama (Kavram Arama)

**Senaryo:** Aklınıza bir durum veya kavram geldi (örneğin "sinirlenmek" veya "çaresizlik") ancak bunu en iyi anlatan deyimi, atasözünü veya kelimeyi hatırlayamıyorsunuz.

**İşlevi:** Yerel (Çevrimdışı) sözlükteki **açıklamaların ve tanımların** içinde arama yapar. Örneğin "öfke" yazıp arattığınızda; başlığında "öfke" geçmese bile, açıklamasında "öfke" kelimesi geçen (Örn: *Küplere binmek, Tepesi atmak, Kan beynine sıçramak*) tüm deyim ve atasözlerini önünüze serer. Duruma cuk oturacak deyim / sözü bulmak için kullanabilirsiniz.

### 🧩 3. Kelime Avcısı (Liste Modu)

Bulmaca çözerken, şiir yazarken ya da sadece "sonu şu heceyle biten kelimeler neydi?" diye düşünürken kullanabileceğiniz güçlü bir listeleme özelliğidir.

Katman komutunu (`NVDA`+`Shift`+`,`) uyguladıktan sonra:

* **`*` (Yıldız):** Seçili (veya yazılan) ifade ile **BAŞLAYAN** kelimeleri listeler.
*Örnek: Yıldız tuşuna basıp "Kal" yazdıktan sonra enter tuşuna basarsanız; "Kalem", "Kalp", "Kaldırım" gibi kelimelerin listesi gelir.*
* **`-` (Tire):** Seçili (veya yazılan) ifade ile **BİTEN** kelimeleri listeler.
*Örnek: Tire tuşuna basıp "mak" yazarsanız; "Koşmak", "Yapmak", "Ekmek" gibi kelimelerin listesi gelir.*

**Önemli:** Açılan listeden bir kelime seçip `Enter`'a bastığınızda, eklenti o kelimeyi otomatik olarak **"Birleşik Arama" (TDK + Dil Derneği)** modunda sorgular.

### `I` Tureng Sözlük (İngilizce - Türkçe & Türkçe-İngilizce)

**Senaryo:** İngilizce bir metin okurken bilmediğiniz bir kelimeye denk geldiniz veya Türkçe bir kelimenin İngilizce karşılığını (teknik, tıbbi, hukuki vb. kategoriler dahil) öğrenmek istiyorsunuz.

**İşlevi:** Tureng.com veritabanını tarar. Kelimenin farklı kategorilerdeki (Genel, Teknik, Hukuk vb.) karşılıklarını temiz bir liste halinde, örnek cümlelerle birlikte sunar. Tarayıcı açmanıza gerek kalmaz.

### 📊 4. Metin Analizi ve Bilgi Sistemi

Sözlük eklentisi, kelime anlamlarını sorgulamanın ötesine geçerek; editörler, öğrenciler ve yazılımcılar için gelişmiş bir analiz aracı sunar. Bu özellik, seçili metnin veya imlecin üzerindeki kelimenin türüne göre akıllıca davranarak size en doğru bilgiyi vermeyi amaçlar.

**Nasıl Kullanılır?**
Kaynak seçim katmanını açın (`NVDA` + `Shift` + `,`), ardından `.` (Nokta) tuşuna basın.

#### A. Çoklu Kelime Seçimi ve Detaylı İstatistikler

Eğer bir metin bloğu (birden fazla kelime) seçtiyseniz, eklenti bu metni inceler ve şu raporu sunar:

* **Okuma Süresi:** Metnin ortalama bir hızla ne kadar sürede okunabileceğini hesaplar.
* **Doğru Kelime Sayımı:** Noktalama işaretlerini kelimelerden ayırarak , sayım yapar.
* **Yapısal Analiz:** Metindeki paragraf ve cümle sayılarını tespit eder.
* **Frekans Analizi:** Metnin ana fikrini anlamanızı kolaylaştırmak için, metin içinde en sık kullanılan 20 kelimeyi listeler.
* **İçerik Türü:** Metnin harf veya rakam yoğunluğuna bakarak türü hakkında (düz yazı mı, kod/veri mi) ipucu verir.

#### B. Tek Kelime ve Özel Veri Tespiti

Seçim yoksa veya tek kelime seçiliyse, modül verinin türünü algılar:

* **Sözlük Tanımı:** Standart bir İngilizce kelime ise, kelimenin tanımını İngilizce olarak getirir. Kelimeyle ilgili sonuç bulunamazsa arama Tureng Sözlük'e yönlendirilir.
* **IP Adresi Sorgusu:** Veri bir IP adresi formatındaysa (Örn: 192.168.1.1), konum ve sağlayıcı bilgisini sorgular.
* **ISBN Kitap Sorgusu:** Veri 10 veya 13 haneli bir ISBN numarasıysa, kitabın adını ve yazarını getirir.

#### C. Çalışma Mantığı ve Öncelik Sırası

Eklenti en doğru sonucu vermek için şu sırayı takip eder:

1. **Yazı Alanı Seçimi:** Önce aktif yazı kutusundaki seçime bakar.
2. **Sanal Tampon:** Yoksa, web sayfasındaki/belgedeki seçime bakar.
3. **Sistem İmleci:** Seçim yoksa, imlecin üzerindeki kelimeyi yakalar.
4. **Yazı Alanı:** Hiçbiri yoksa aranacak ifadenin girilebileceği bir yazı alanı açar.

### 🔠 5. Anagram Çözücü (Kelime Türetmece)

Scrabble oynarken veya "elimdeki harflerle neler yazabilirim?" diye düşünürken kullanabileceğiniz, bulmaca severler için tasarlanmış bir araçtır.

Katman komutunu (`NVDA`+`Shift`+`,`) uyguladıktan sonra `0` (Sıfır) tuşuna basın.

Açılan kutuya elinizdeki harfleri (Örn: *k a l e m*) girdiğinizde, eklenti bu harflerle yazılabilecek anlamlı Türkçe kelimeleri, uzunluklarına göre sıralayarak listeler.

### 📅 6. TDK Günün İçeriği

TDK'nin her gün yayınladığı "Günün Kelimesi" ve "Günün Atasözü/Deyimi" içeriğine anında ulaşabilirsiniz.

* **Manuel Erişim:** Katman komutunu uyguladıktan sonra `G` tuşuna basarak günün içeriğini anında görüntüleyebilirsiniz.
* **Otomatik Bildirim:** Ayarlar panelinden ilgili seçeneği aktif ederseniz, NVDA her açıldığında günün kelimesi ve anlamı size otomatik olarak seslendirilir.

### ⚙️ Ayarlar ve Özelleştirme

Eklentiyi kendi çalışma alışkanlıklarınıza göre kişiselleştirebilirsiniz. Ayarlar paneline ulaşmak için **NVDA Menüsü** -> **Tercihler** -> **Ayarlar** yolunu izleyin ve açılan listeden **"TDK ve Sözlükler"** kategorisini bulun.

Bu panelden şu yapılandırmaları yapabilirsiniz:

* **Varsayılan Kaynak:** `NVDA`+`,` kısayoluna bastığınızda, katman açılmadan doğrudan hangi sözlükte arama yapılacağını (Örn: Sadece TDK, Tureng vb.) seçebilirsiniz.
* **Tureng limiti:** Tureng sonuç listesinin uzunluğunu belirleyebilirsiniz. Varsayılan değer 30'dur. Sonuçların tamamının gösterilmesini istiyorsanız bu alan boş bırakılmalıdır.
* **TDK sonuçlarından örnek cümleleri çıkarma:** Onay kutusunu TDK sonuçlarına örnek cümlelerin dahil edilip edilmeyeceğini belirlemek için kullanabilirsiniz.
* **Otomatik kopyalama:** Bu onay kutusunu bulunan sonuçların otomatik olarak panoya kopyalanması için kullanabilirsiniz.
* **Sesli Geri Bildirim:** Arama işleminin başladığını bildiren bip sesini açıp kapatabilirsiniz.
* **Sonuç Bildirim türü:** Arama sonuçların bir pencredede mi gösterilsin yoksa sadece seslendirilsin mi tercihini yapabilirsiniz.
* **Başlangıç Bildirimi:** NVDA açıldığında TDK Günün Kelimesi'nin otomatik olarak okunup okunmayacağını belirleyebilirsiniz.

### 💡 İpuçları ve Kişiselleştirme

* **Pencereyi Kapatma:** TDK, Dil Derneği, Atasözleri, Yerel sözlük, Tureng ve metin analiz sonuçları NVDA'nın "Sanal Görüntüleme" penceresinde açılır. Okuma işiniz bittiğinde `ESC` tuşuna basarak pencereyi kapatabilir ve işinize kaldığınız yerden devam edebilirsiniz.
* **Tuşları Değiştirme:** Eğer "Ben Kelime Listeleme özelliğini çok sık kullanıyorum, ona özel tek bir tuş atamak istiyorum" derseniz; *NVDA Menüsü -> Tercihler -> Girdi Hareketleri -> TDK ve Sözlükler* yolunu izleyebilirsiniz. Burada tüm komutlara istediğiniz klavye kısayolunu atayabilirsiniz.

### 💖 Teşekkür ve Katkıda Bulunanlar

Bu eklentinin satır satır işlenmesinde ve kodlanmasında emeği geçen şahsım **Çağrı Doğan** olarak; ortaya sadece bilgiye erişimi hızlandıran değil, aynı zamanda kullanırken keyif veren bir araç çıkmasından mutluluk duyuyorum.

Bu projenin asıl kıvılcımı ise **Tuba Vural** sayesinde çakıldı. Fikrin NVDA_TR grubunda filizlenmesinden bugünkü haline gelmesine kadar; test süreçleri, geri bildirimler, kaynak önerileri ve içerik derleme konularındaki titiz çabası ve yol arkadaşlığı için kendisine en içten teşekkürlerimi sunuyorum.

Kodlama sürecindeki desteği için yapay zeka asistanımız **Google Gemini**'ye; bilgi hazinelerinden faydalandığımız **TDK**, **Dil Derneği** ve **Tureng** gibi köklü kurumlara; eserlerini eklentimize dahil ederek değer kattığımız **Ülkü & Hüseyin Kuşçu** ve **Ömer Asım Aksoy** gibi kıymetli isimlere saygılarımızla...
