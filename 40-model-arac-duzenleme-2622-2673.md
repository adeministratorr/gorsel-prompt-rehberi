> [← Genel İçindekiler](gorsel-prompt-rehberi.md) · [Süleyman’a Umut Ol — Dayanışma Çağrısı](gorsel-prompt-rehberi.md#suleymana-umut-ol)

<a id="sec-2622"></a>
# 2622. Aynı etiket, farklı model — davranış farkları neden önemli?

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Rehberdeki açılım promptları bilinçli olarak model-agnostiktir: aynı Türkçe prompt Gemini'de de ChatGPT'te de anlaşılır. Fakat anlaşılması ile aynı sonucu vermesi aynı şey değildir.

Aynı `/lego` etiketi:

- bir modelde minifigür oranlarına daha hızlı yatkınlaşır,
- diğerinde yüzeysel blok dokusu kaplaması riskine daha yakındır,
- metin yazarken biri kutu üstündeki yazıyı doğru basabilir, diğeri bozuk harf üretebilir.

Kısayolu kullanmak serbesttir; sonucu **kontrol etmek** zorunludur. Bu ailenin amacı, kontrolü hangi farklara bakarak yapacağınızı göstermektir.

## Neye dikkat edilmeli?

Bir etiketin "çalışması" ile "doğru çalışması" aynı şey değildir. Bu aileyi okuduktan sonra §45'teki kontrol listesini hangi modelde üretirseniz üretin, aynı şekilde uygulayın.

---

# 2623. Gemini'de Nano Banana ile fotoğraf + etiket akışı

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Gemini'nin görsel üretim katmanı Nano Banana ailesidir (Nano Banana 2 ve Nano Banana Pro). Fotoğraf dönüştürme akışı:

1. Gemini'de yeni sohbet açın, dönüştürmek istediğiniz fotoğrafı sohbete ekleyin.
2. Etiketi mesaj olarak yazın. Tek başına (`/lego`) ya da kontrollü açılımıyla (`/lego — kimlik ve kıyafet renkleri korunsun`).
3. Sonucu §45 kontrol listesiyle değerlendirin.
4. İnce ayar için tek değişiklik içeren takip mesajı yazın (2661).

## Neye dikkat edilmeli?

Gemini, Nano Banana Pro'da birden çok referans görseli tek üretimde birleştirebilir; uygulama yüzeyine göre 6–14 görsel (2638). Birden fazla kişi fotoğrafı yüklerken kimlik karışmasını önlemek için hangi görselin kimlik referansı, hangisinin stil referansı olduğunu promptta adıyla belirtin.

---

# 2624. Nano Banana Pro'nun resmî prompt formülü — Özne + Eylem + Bağlam + Kompozisyon + Stil

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Google'ın kendi prompting rehberi (Google Cloud, Mart 2026), referans görsel olmadan üretimde anahtar kelime listesi yerine **anlatımlı sahne** tarifi önerir:

> [Özne] + [Eylem] + [Yer/bağlam] + [Kompozisyon] + [Stil]

### Türkçe prompt (örnek)

> [Özne] Kovan çerçevesini inceleyen bir arıcı. [Eylem] Çerçeveyi iki elle kavramış, hafif öne eğilmiş. [Bağlam] Yaban çiçekli tarlanın kenarı, geç sabah ışığı. [Kompozisyon] Göz hizası, 50 mm, yüzeysel odak. [Stil] Belgesel fotoğraf, doğal ten dokusu.

### English prompt

> [Subject] A beekeeper inspecting a frame of honeycomb. [Action] Leaning slightly, holding the frame with both hands. [Location] Edge of a wildflower field, late morning. [Composition] Eye-level, 50 mm, shallow focus. [Style] Documentary photography, natural skin texture.

## Neye dikkat edilmeli?

Bu formül §38'deki şablonla aynı işi yapar; fark, Google'ın bunu Nano Banana ailesi için resmîleştirmiş olmasıdır. Slash-style etiketin yanına açılım yazarken bu beş slota da değinmek, etiketin bıraktığı boşluğu doldurur.

---

# 2625. Referans görsel formülü — [Referanslar] + [İlişki talimatı] + [Yeni senaryo]

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Nano Banana Pro'nun en güçlü yanı birden çok referans görseli yönetebilmektir. Google'ın formülü:

> [Referans görseller] + [İlişki talimatı] + [Yeni senaryo]

### Türkçe prompt (örnek)

> Eklenen eskiz görseli yapı referansı, eklenen kumaş örneği doku referansı olsun. Bu ikisini birleştirerek yüksek detaylı bir koltuk görseli üret ve güneş alan minimalist bir salona yerleştir.

### English prompt

> Use the attached sketch as the structure reference and the attached fabric swatch as the texture reference. Combine them into a high-fidelity armchair render and place it in a sun-lit minimalist living room.

## Neye dikkat edilmeli?

- 5 kişiye kadar kimlik tutarlılığı taşınabilir; grup kompozisyonunda her kişiyi ayrı referans görselde verin.
- Nano Banana Pro'nun bilgi kesim tarihi Ocak 2025'tir; sonrasında ortaya çıkan nesne ve üniformalları doğru almak için referans görselle verin (2638).

---

# 2626. Nano Banana'da metin yazdırma — tırnak, font, metin-önce tekniği

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Nano Banana ailesi metin yazmada güçlüdür. Google'ın önerileri dört maddeye indirgenebilir:

1. **Tırnak:** Yazılacak metni tırnak içine alın: `"Mutlu Yıllar"`.
2. **Font:** Yazı karakterini tanımlayın: "kalın beyaz sans-serif" ya da adıyla bir font.
3. **Yerelleştirme:** Prompt tek dilde yazılıp görseldeki metnin dili ayrıca istenebilir (Türkçe dahil 10'dan fazla dil).
4. **Metin-önce tekniği:** Uzun metinli görselde önce metni sohbette kararlaştırın, ardından görseli isteyin.

### Türkçe prompt (örnek)

> Bir bilim fuarı afişi üret. Yalnızca "Foton Fuarı 2026" yazsın: kalın, beyaz, sans-serif font, koyu lacivert zemin. Başka hiçbir metin ekleme.

### English prompt

> Generate a science fair poster. Render only the text "Foton Fuarı 2026" in a bold white sans-serif font on a deep navy background. Do not add any other text.

## Neye dikkat edilmeli?

Metinli görselde her harfi tek tek kontrol edin (§18). "Neredeyse doğru" yazı, eğitim materyalinde tamamen yanlış yazı kadar zararlıdır.

---

# 2627. ChatGPT'te fotoğraf + etiket akışı

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

ChatGPT'nin görsel modeli GPT Image ailesidir. Akış Gemini ile aynı mantıktadır:

1. Yeni sohbet açın, dönüştürmek istediğiniz fotoğrafı sohbete ekleyin.
2. Etiketi mesaj olarak yazın. Tek başına (`/lego`) ya da kontrollü açılımıyla.
3. Sonucu §45 kontrol listesiyle değerlendirin.
4. İnce ayarı konuşarak sürdürün; ChatGPT aynı görsel üzerinde konuşmalı düzenlemeye yatkındır.

Slash (`/`) bazı ChatGPT arayüzlerinde uygulama komutlarını çağırmak için kullanılır; fakat `/lego` gibi stil etiketleri bu komut sisteminin parçası değildir (§891). Etiket, prompt metni olarak modele gider.

## Neye dikkat edilmeli?

ChatGPT görsellerde uzun ve doğal dil talimatlarına dayanır. Etiket tek başına bırakıldığında model açılımı kendisi tahmin eder; kritik kısıtlarınız varsa (kimlik, ölçü, yazı) açılımı siz yazın (2629).

---

# 2628. Aynı `/lego` etiketi iki modelde — beklenen fark tablosu

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Açılım promptu §892'dedir. Aynı kaynak fotoğraf, aynı etiket, iki model:

| Bakılacak nokta | ChatGPT (GPT Image) | Gemini (Nano Banana Pro) |
|---|---|---|
| Kimlik korunumu | Genellikle güçlü; yüz benzerliğini korumaya eğilimli | Referans görselle verildiğinde güçlü; 5 kişiye kadar tutarlılık (2625) |
| Blok dokusu | Yüzey kaplaması riski biraz daha yüksek; açılım şart | Gerçek blok geometrisine yönelimi belirgin |
| Varsayılan estetik | Nötr-temiz ürün çekimi havası | Stüdyo kontrolü istenmediğinde sıcak, parlak ton |
| Metin (kutu üstü yazı) | Genellikle doğru; uzun metinde bozulur | Kısa metinde güçlü; font belirtince iyileşir (2626) |
| Görsel boyutu | Kısa kenar ~1024 px civarı | 1K / 2K / 4K seçenekli (2638) |

Tablodaki satırlar gözlem kılavuzudur; sürüm güncellemeleriyle değişebilir. Bu yüzden kendi A/B kaydınızı tutun (2637).

## Neye dikkat edilmeli?

Tablo bir "hangisi daha iyi" sıralaması değildir. Soru şudur: bu iş için hangi fark kritik? Kimlik kritikse referans görsel akışını, metin kritikse tırnak + font kuralını devreye alın.

---

# 2629. Kısayol yetmediğinde: etikete açılım ekleme kuralı

Slash-style etiket, §893'te tanımlanan preset çağrısıdır. Etiket tek başına bırakıldığında model boşlukları varsayılanla doldurur. Aşağıdaki dört durumda varsayılana güvenmeyin, açılımı yazın:

1. **Kimlik:** Yüz, kıyafet, vücut ölçüsü korunacaksa.
2. **Yazı:** Görselde belirli bir metin basılacaksa (tırnakla birlikte, 2626).
3. **Ölçü ve oran:** Baskı boyutu, platform oranı ya da nesne ölçüsü kritikse (2650).
4. **Yasaklar:** Belirli bir öğenin kesinlikle görünmemesi gerekiyorsa — ama olumlu çerçeveleyerek (2639).

### Kısa kullanım

> `/lego`

### Kontrollü açılım

> `/lego — kimlik referansı olarak yüklenen fotoğrafı kullan; poz ve kıyafet renkleri korunsun; masa üstü koleksiyon figürü ölçeği`

### English

> `/lego — use the uploaded photo as identity reference; preserve pose and clothing colors; desk-scale collectible figurine`

## Neye dikkat edilmeli?

Açılım yazmak "uzun prompta dönüş" demek değildir; tek cümlelik açılım çoğu zaman yeterlidir. Kural basittir: **kritik olan her kısıt etiketin dışında açıkça yazılır.**

---

# 2630. Kontrollü düzenleme formülü — Lock + Change + Amount + Constraint

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Nano Banana'da ve ChatGPT'te mevcut bir görseli düzenlerken kullanılabilecek dört parçalı yapı:

1. **Lock (sabit):** Değişmemesi gerekenleri adıyla listeleyin — yüz, düzen, yazı, renk tonu.
2. **Change (değişiklik):** Tek bir şey değiştirin.
3. **Amount (miktar):** Değişikliğin dozunu belirtin — "hafif", "yarı", "tamamen".
4. **Constraint (sınır):** Değişikliğin neyi bozmaması gerektiğini yazın.

### Türkçe prompt (örnek)

> Yüklenen fotoğrafta yüz, saç ve arka plan tamamen aynı kalsın [Lock]. Yalnızca ceketin rengini değiştir [Change], lacivert yap [Amount]. Kumaş dokusu ve ışık yönü bozulmasın [Constraint].

### English prompt

> In the uploaded photo keep the face, hair, and background exactly the same [Lock]. Change only the jacket color [Change] to navy [Amount]. Do not break the fabric texture or the lighting direction [Constraint].

## Neye dikkat edilmeli?

Mesaj başına tek değişiklik ilkesi iki modelde de işleri kontrol edilebilir kılar. Beş değişiklik tek cümleye sıkıştırıldığında hangisinin uygulanmadığını ayırt etmek imkânsızlaşır.

---

<a id="sec-2631"></a>
# 2631. Çalışılmış örnek: `/lego` — iki modelde A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı kaynak fotoğrafı iki modelde `/lego` ile dönüştürüp farkları kaydetmek. Açılım promptu §892'dedir.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/lego — use the uploaded photo as identity reference, preserve pose and clothing`

### Nano Banana varyantı

> Yüklenen fotoğrafı kimlik referansı olarak kullan. Özneyi birbirine geçen oyuncak yapı bloklarından kurulmuş fiziksel bir modele dönüştür; ana siluet, renk dağılımı ve tanınabilir özellikler korunsun. Minifigür benzeri sadeleştirilmiş oranlar kullanılabilir ancak yüz benzerliği korunmalı. Masa üstü koleksiyon figürü ölçeğinde, sade stüdyo zemininde göster.

## Beklenen fark

- Nano Banana gerçek blok geometrisine daha belirgin yönelir; ChatGPT bazen yüzeye blok dokusu kaplar.
- Kimlik: ChatGPT yüz benzerliğini tek hamlede koruma eğilimindedir; Nano Banana'da kimlik referansı cümlesi açıkça yazılmalıdır (2625).

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: siluet aynı mı, bloklar gerçekten birleşik mi, yüz tanınır mı? Biri başarısızsa hatayı açılıma ekleyin; etiketi suçlamayın.

### Sonuç görseli

`images/ab-01-lego-chatgpt.png`  
`images/ab-01-lego-nanobanana.png`

---

# 2632. Çalışılmış örnek: `/figurine` — koleksiyon figürü A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Kutu ve kaide gibi ikincil nesneler içeren koleksiyon figürü dönüşümünde iki modelin kompozisyon davranışını görmek.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/figurine — desk-scale collectible figure on a round base, product box behind it, studio lighting`

### Nano Banana varyantı

> Yüklenen fotoğrafı kimlik referansı olarak kullan. Özneyi masa üstü koleksiyon figürüne dönüştür: yuvarlak kaide üzerinde, arkasında resmi olmayan sade ürün kutusu. Stüdyo aydınlatması, sade zemin. Kutu üstünde yalnızca "FIGURINE" yazsın; başka metin ekleme.

## Beklenen fark

- Kutu ve yazı gerektiren kompozisyonlarda Nano Banana'nın metin kontrolü (tırnak + font) avantaj sağlar (2626).
- ChatGPT kompozisyonu tek cümleden tahmin eder; kaide biçimi tekrar denemede değişebilir.

## Neye dikkat edilmeli?

Kutu üstü yazı her harften kontrol edilmelidir (§18). Marka adı geçen kutu istemek telif riskini de beraberinde getirir (2656); jenerik kutu kullanın.

### Sonuç görseli

`images/ab-02-figurine-chatgpt.png`  
`images/ab-02-figurine-nanobanana.png`

---

# 2633. Çalışılmış örnek: `/cutaway` — kesit görünüm A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Eğitim amaçlı kesit görünümde (§5) iki modelin teknik doğruluk davranışını görmek.

### ChatGPT varyantı

> (nesne fotoğrafını ekleyin) `/cutaway — reveal the internal structure, keep the outer shell and proportions, label parts in Turkish`

### Nano Banana varyantı

> Yüklenen nesne fotoğrafının dış kabuğunu koru; iç yapıyı kesit görünümünde göster. Kesilen yüzeyin düzlemsel ve temiz olmasına, parçaların gerçek konumlarında kalmasına dikkat et. Ana parçaları Türkçe adlandır. Dekoratif ışıklandırma ve arka plan ekleme.

## Beklenen fark

- Etiket iç yapıyı modelin tahminiyle doldurur: gerçek nesne değilse iki model de uydurabilir. Rehber §90'daki uyarı burada da geçerlidir: aynı prompt aynı doğruluğu vermez.
- Türkçe etiket yazımında Nano Banana'nın metin kontrolü avantajlıdır; ChatGPT uzun etiket listesinde harf hatası yapabilir.

## Neye dikkat edilmeli?

Kesit görünümünde doğruluk, estetikten önce gelir: parça adları ders kitabıyla eşleşiyor mu, iç yapı makul mü? Şüphede konu uzmanına göstermeden kullanmayın (§18).

### Sonuç görseli

`images/ab-03-cutaway-chatgpt.png`  
`images/ab-03-cutaway-nanobanana.png`

---

# 2634. Çalışılmış örnek: `/postcard` — vintage seyahat kartpostalı A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Metin + grafik + fotoğrafın tek karede birleştiği kartpostal formatında iki modelin yazı ve period-look davranışını görmek.

### ChatGPT varyantı

> (şehir fotoğrafını ekleyin) `/postcard — 1960s travel postcard, "SELANİK" in vintage serif lettering, linen texture, muted colors`

### Nano Banana varyantı

> Yüklenen şehir fotoğrafını 1960'lar seyahat kartpostalına dönüştür. Üstte yalnızca "SELANİK" yazsın: vintage serif harfyle, krem rengi şerit içinde. Ketan bez doku ve yıpranmamış hafif soluk renk paleti. Alt köşeye metin ekleme.

## Beklenen fark

- Türkçe karakterli büyük başlık (İ, Ş) Nano Banana'da tırnak + font kuralıyla daha güvenilir sonuç verir (2626).
- Period dokusu (ketan bez, soluk renk) iki modelde de etiketin dışına yazılınca belirginleşir; tek `/postcard` genellikle jenerik vintage verir.

## Neye dikkat edilmeli?

Kartpostal metni başlıktan ibaret kalmalı; modelin "Hoş geldiniz…" gibi ek cümle ekleme isteğini sınırlayın. Şehir adının dönemi doğru olsun: tarihsel ad ile bugünkü ad farklıysa hangisini istediğinizi bilin (§89'da bilgi kaynağı olmadığı uyarısı).

### Sonuç görseli

`images/ab-04-postcard-chatgpt.png`  
`images/ab-04-postcard-nanobanana.png`

---

# 2635. Çalışılmış örnek: `/hologram-object` — hologram nesne A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Işık yayması gereken bir efektte (§1660 civarı aile) iki modelin yarı saydamlık ve ışık kontrolünü görmek.

### ChatGPT varyantı

> (nesne fotoğrafını ekleyin) `/hologram-object — translucent projected line-object, dark background, restrained glow, keep the silhouette`

### Nano Banana varyantı

> Yüklenen nesne fotoğrafını koyu zemin üzerinde yarı saydam bir hologram izdüşümüne dönüştür. Çizgisel iskelet yapısı korunmalı; parlama tek renk ve sınırı açık olsun. Işığın zemine bıraktığı hafif yansıma eklenebilir; ama gerçek ışık kaynağı veya duman efekti ekleme.

## Beklenen fark

- Hologram, "parlaklık dozunu" belirtmeyi gerektirir; belirtmediğinde iki model de parlaklığı şişirir. Amount parçası (2630) burada işe yarar: "sınırlı parlama".
- Siluet korunumu: nesnenin orijinal oranı iki modelde de kayma eğilimindedir; açılımda "siluet korunmalı" yazın.

## Neye dikkat edilmeli?

Hologram görsel, bir nesnenin gerçek durumu değildir; ders materyalinde "temsilî" olarak etiketlenmelidir. Sahte ürün tanıtımı ya da var olmayan cihaz fotoğrafı gibi sunulmamalıdır.

### Sonuç görseli

`images/ab-05-hologram-chatgpt.png`  
`images/ab-05-hologram-nanobanana.png`

---

# 2636. Çalışılmış örnek: `/film-noir-portrait` — noir portre A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Işık ve atmosfer ağırlıklı bir portre formatında iki modelin monokrom ve gölge kontrolünü görmek.

### ChatGPT varyantı

> (portre fotoğrafını ekleyin) `/film-noir-portrait — controlled monochrome noir, venetian blind shadow on the wall, restrained contrast, keep identity`

### Nano Banana varyantı

> Yüklenen portreyi monokrom film-noir estetiğine çevir. Duvara düşen jaluzi gölgesi belirgin ama abartısız; kontrast kontrollü, siyahlar kapansın ama yüz detayı kaybolmasın. Kimlik referansı olarak fotoğrafı kullan; yüz benzerliği korunmalı.

## Beklenen fark

- Noir'in ana kontrolü ışık dozudur: "siyahlar kapansın ama yüz detayı kaybolmasın" cümlesi iki modelde de gereklidir (2624 Kompozisyon slotu).
- Nano Banana'da ışık yönü "jaluzi gölgesi soldan" gibi belirtilirse tekrarlanabilirlik artar (2640).

## Neye dikkat edilmeli?

Monokrom dönüşümde ten değerleri değişir; portre kişisel veridir ve rıza dışında dönüştürülmemelidir (2655). Ders materyalinde ışık tipini anlatan örnekse, kaynak fotoğrafın serbest lisanslı olması tercih edilir.

### Sonuç görseli

`images/ab-06-noir-chatgpt.png`  
`images/ab-06-noir-nanobanana.png`

---

<a id="sec-2637"></a>
# 2637. A/B test protokolü ve kayıt şablonu

Model farklarını kendi gözünüzle belgelemek için kısa bir protokol yeterlidir:

1. **Aynı kaynak:** Tek bir kaynak görsel seçin; iki modelde aynı dosyayı kullanın.
2. **Aynı etiket:** Etiketi aynı biçimde yazın; açılım cümlesi kelimesi kelimesine aynı olsun.
3. **Aynı kriterler:** Aşağıdaki beş kritere tabloda puan verin (1–5).
4. **Aynı gün:** Sürümler hızla değiştiği için karşılaştırmayı tek oturumda yapın.

## Kayıt şablonu

| Tarih | Etiket | Model | Kimlik | Doku/yapı | Metin | Oran/ölçü | Genel | Not |
|---|---|---|---|---|---|---|---|---|
| 2026-09-03 | `/lego` | ChatGPT | 4 | 3 | — | 4 | 4 | yüzey kaplaması hafif |
| 2026-09-03 | `/lego` | Nano Banana | 4 | 4 | — | 4 | 4 | blok geometrisi iyi |

## Neye dikkat edilmeli?

Bu kayıt rehberdir, yarışma değil. Amaç, "hangi işte hangi model" sorusuna kendi işlerinizden cevap toplamaktır (2649).

---

<a id="sec-2638"></a>
# 2638. Nano Banana Pro teknik sınırları — hızlı tablo

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Google'ın model belgelerinde paylaşılan sınırlar (Eylül 2026 itibarıyla):

| Özellik | Nano Banana 2 (Gemini 3.1 Flash Image) | Nano Banana Pro (Gemini 3 Pro Image) |
|---|---|---|
| Çözünürlük | 512 px, 1K, 2K, 4K | 1K, 2K, 4K |
| En-boy oranı | 1:1, 3:2, 2:3, 3:4, 4:3, 4:5, 5:4, 9:16, 16:9, 21:9 + 1:4, 4:1, 1:8, 8:1 | 1:1, 3:2, 2:3, 3:4, 4:3, 4:5, 5:4, 9:16, 16:9, 21:9 |
| Referans görsel | 14'e kadar | 14'e kadar (uygulama yüzeyine göre 6–14) |
| Kişi tutarlılığı | 5 kişiye kadar | 5 kişiye kadar |
| Bilgi kesim tarihi | Ocak 2025 + canlı arama desteği | Ocak 2025 + canlı arama desteği |
| İzlenebilirlik | SynthID + C2PA içerik kanıtı | SynthID + C2PA içerik kanıtı |

## Neye dikkat edilmeli?

Bilgi kesim tarihi Ocak 2025 demek, sonrasında çıkan bir cihazı, üniformayı, logoyu modelin "hatırlamadığı" demektir; bunları referans görselle verin. Filigranları kaldırmaya çalışmak hem teknik olarak gereksiz hem etik olarak yanlıştır (2657).

---

# 2639. Olumlu çerçeveleme — "arabasız sokak" değil "boş sokak"

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Google'ın prompting en iyi uygulamalarından biri: **istediğinizi tarif edin, istemediğinizi değil.**

> Arabasız sokak ❌ → Boş sokak ✔
> Metin ekleme ❌ → Yalnızca şu yazı görünsün: "…" ✔

Neden? Model "araba" ve "metin" kavramlarının görsel temsilini bilir; "yasak" ile uyarıldığında o kavramı promptta görünür kılmak yine de mümkündür.

## Rehber bağlamı

Bu kural rehberin genel yaklaşımıyla aynıdır: `# 165`'te "premium, cinematic" gibi boş süslerin neden çıkarılması gerektiği anlatılmıştı. Olumsuz komutlar da aynı gereksiz gürültüdür; onun yerine olumlu tarifi yazın.

## Neye dikkat edilmeli?

Tek istisna güvenlik sınırlarıdır: "gerçek kişi yüzü ekleme" gibi etik sınırlar olumlu çerçeveyle karşılanamaz; bunlar açıkça yazılır (2655).

---

# 2640. Işık ve kamera yönetimi — creative director yaklaşımı

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Google, Nano Banana'da sonuç kalitesini yükselten iki kontrol katmanı önerir:

## Işık tasarımı

- **Stüdyo kurulumu:** "üç nokta softbox kurulumu" — ürün ve nesne çekiminde dengeli ışık.
- **Dramatik:** "chiaroscuro aydınlatma, sert yüksek kontrast", "altın saat arkadan ışık, uzun gölgeler".

## Kamera, lens ve odak

- **Gövde:** GoPro (geniş açı, aksiyon), Fujifilm (renk karakteri), tek kullanımlık kamera (dürüst, nostaljik flaş).
- **Lens:** "düşük açı, yüzeysel derinlik" gibi fotoğraf terimleriyle perspektif dayatılabiliyor.

Bu terimler rehberde zaten sistematik işlenmiş durumda: `Kamera, Lens, Işık ve "Capture Source" Prompt Dili` ailesi aynı kelime dağarcığını Türkçe–İngilizce eşleştirmelerle verir. Buradaki fark şudur: Nano Banana ve GPT Image bu terimleri doğal dilin içinde bekler; Midjourney ise parametre sözdizimini (`--ar`, `--sref`) ayrıca kullanır (2643).

## Neye dikkat edilmeli?

Işık ve kamera terimleri gerçek bir fotoğrafçılık anlamı taşır; hobi mükemmelliği kelimeleri gibi boş süse dönüşmemeli (§165). "Cinematic 8K ultra detailed" fotoğrafçılık bilgisi değil, gürültüdür.

---

## Bu turdaki güncel kaynak sinyalleri (ek — 2622+)

- Google Blog — **7 tips to get the most out of Nano Banana Pro** (20 Kasım 2025)  
  Metin yazdırma, stüdyo kalitesinde kontrol düzenlemeleri, oran/çözünürlük ve karakter tutarlılığı konularının resmî önerileri.  
  https://blog.google/products-and-platforms/products/gemini/prompting-tips-nano-banana-pro/

- Google Cloud — **The ultimate Nano Banana prompting guide** (6 Mart 2026)  
  Özne+Eylem+Bağlam+Kompozisyon+Stil ve Referanslar+İlişki+Senaryo formülleri; düzenleme ve creative-director teknikleri; model teknik özellikleri.  
  https://cloud.google.com/blog/products/ai-machine-learning/ultimate-prompting-guide-for-nano-banana

- fal.ai — **Nano Banana Pro Prompting Guide & Examples** (Haziran 2026)  
  Lock + Change + Amount + Constraints yapısı, mesaj başına tek değişiklik, 5 kişi / 14 referans sınırları.  
  https://fal.ai/learn/tools/nano-banana-pro-prompting-guide

- Zapier — **The 8 best AI image generators in 2026**  
  Araç seçimi karşılaştırması (2642'deki tablonun temel kaynağı).  
  https://zapier.com/blog/best-ai-image-generator/

- Albato — **Best AI Image Generators in 2026: 7 Tools Compared**  
  Kullanım senaryosuna göre araç seçimi.  
  https://albato.com/blog/publications/best-ai-image-generators

---

# Araç ve Model Rehberi — Hangi Araç Hangi İş İçin?

Bu aile, rehberin model-agnostik prompt dilini hangi araca taşıyacağınıza karar vermenize yardımcı olur. Araçlar hızla güncellendiği için buradaki tablo **Eylül 2026 itibarıyla** bir fotoğraftır; kararın kendisi ("hangi iş için hangi özellik kritik") tablodan daha kalıcıdır.

---

# 2641. Araç seçimi neden prompt dilinden sonra gelir?

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Rehberin ana dili — anlatım biçimi (kesit, patlatılmış görünüm, flat lay …) — tüm araçlarda çalışır. Araç seçimi bu dili taşıyacağınız taşıttır; seçim şu sorularla yapılır:

- İş **düzenleme ağırlıklı mı**, üretim ağırlıklı mı?
- **Metin** basılacak mı?
- **Kimlik** korunacak mı?
- Çıktı **ticari mi**? (lisans ve güvence sorusu — 2654)
- **Parametre dili** mi (Midjourney), doğal dil mi gerekiyor?

Prompt önce yazılır; araç, o promptun en az bozulacağı taşıyıcı olarak seçilir.

---

<a id="sec-2642"></a>
# 2642. Hızlı karşılaştırma tablosu — Eylül 2026

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

| Araç | En güçlü yön | Metin yazma | Kimlik/düzenleme | Parametre dili | Eylül 2026 itibarıyla başlangıç ücreti |
|---|---|---|---|---|---|
| Midjourney (v8.2) | Estetik, editoryal ve sinematik görüntü | Orta–iyi | Ayrı edit modeli (--sref ile stil tutarlılığı) | Var (`--ar`, `--sref`, `--sw`, `--stylize`) | Ücretli planla başlar (temel ~10 $/ay) |
| ChatGPT (GPT Image) | Prompt sadakati, konuşmalı düzenleme | İyi | Güçlü; fotoğraf + talimat akışı | Yok; doğal dil | Ücretsiz katman sınırlı; Plus ~20 $/ay |
| Gemini (Nano Banana Pro) | Referanslı düzenleme, 14 görsel birleştirme, 2K/4K | İyi (tırnak + font) | Çok güçlü; 5 kişiye kadar tutarlılık | Oran/çözünürlük menüden | Ücretsiz katman sınırlı; ücretli katmanlar var |
| Ideogram | Görsel içinde metin | Çok iyi | Orta | Yok; doğal dil | Ücretsiz katman var |
| Adobe Firefly | Ticari güvence (endemnifikasyon), Adobe ekosistemi | İyi | İyi | Yok; doğal dil | Ücretsiz katman; Standard ~10 $/ay |
| Flux (2 Pro) | Fotorealizm, açık ağırlıklar, yerel çalışma | Orta | Kontrol odaklı; LoRA ile özelleştirme | Sınırlı | Open weight ücretsiz; API ücretli |
| Stable Diffusion | Tam kontrol, self-hosting, topluluk araçları | Orta | ControlNet/LoRA ile zengin | Yok; çalışma zamanı araçları | Open source ücretsiz |
| Reve | Yinelemeli tasarım işleri | Orta | İyi | Yok | Ücretsiz katman; Lite ~8 $/ay |

Ücretler sık değişir; karar vermeden önce güncel fiyat sayfasına bakın. Tablo karar rehberidir, fiyat garantisi değildir.

---

# 2643. Midjourney — parametre dili olan araç

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Midjourney, rehberde parametre sözdizimini belgeleyen tek araca laık: promptun sonuna eklenen kısa anahtarlar davranışı değiştirir.

- `--ar 16:9` — en-boy oranı (2650)
- `--sref <görsel>` — stil referansı; stil tutarlılığı için (§2011 civarı aile)
- `--sw <0–1000>` — stil referansının dozu
- `--stylize <değer>` — modelin estetik yorum özgürlüğü

### Türkçe prompt + parametre

> Bir lise kimya laboratuvarının kesit görünümü, ders kitabı illüstrasyonu, sade renk paleti `--ar 3:2 --stylize 50`

## Neye dikkat edilmeli?

Parametreler doğal dil talimatı değildir; model versiyonuna göre değişir ve eğitim promptlarının çoğuna gerekmez. Estetik dozunu (`--stylize`) düşük tutmak, anlatım biçiminin ön planda kalmasını sağlar.

---

# 2644. GPT Image (ChatGPT) — doğal dil ve konuşmalı düzenleme

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

ChatGPT'nin gücü üç yerde toplanır:

1. **Prompt sadakati:** Uzun doğal dil talimatlarını izleme konusunda güçlü; rehberdeki açılım promptları az bozulur.
2. **Konuşmalı düzenleme:** Aynı görsel üzerinde sıralı ince ayar (2661).
3. **Metin:** Kısa ve orta uzunlukta metni güvenilir basar.

## Neye dikkat edilmeli?

Prompt sadakati, yanlış tarifin de sadakatle uygulandığı anlamına gelir: §17'deki zayıf/ kontrollü prompt farkı burada net görülür. Modelin tahmine bıraktığınız boşluk, sizin kontrolünüzden çıkmıştır.

---

# 2645. Gemini (Nano Banana Pro) — referanslı düzenleme ve seri tutarlılık

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Nano Banana Pro'nun ayırt edici özellikleri bu rehberde şöyle karşılık bulur:

- **Referans formülü** (2625) → seri tutarlılık işleri (2662)
- **Metin kuralları** (2626) → afiş, kart, diyagram etiketi
- **Lock + Change + Amount + Constraint** (2630) → kontrollü düzenleme (2659–2660)
- **2K/4K çıkış** → baskıya yakın işler (2663)

### Google Pics — Docs/Slides içinde üretim (Eylül 2026)

Google'ın Eylül 2026'da Workspace'e açtığı Pics aracı, Nano Banana modelini Docs ve Slides içine taşır: sunum ve dokümandan çıkmadan görsel üretme, nesne bazında ayırıp tek öğeyi değiştirme (object segmentation), görseldeki yazıyı fontu koruyarak düzeltme/çevirme ve tek prompttan çoklu varyant. Öğretmen için pratik karşılığı: ders slaytındaki kavram görseli, aynı dosyada üretilip aynı dosyada düzeltilir; indir-yükle döngüsü kalkar. Erişim (Pro/Ultra ve kurumsal Workspace) ve ücretsiz katman sınırları sık değişir; ders öncesi güncel sayfadan doğrulanır.

## Neye dikkat edilmeli?

Ücretsiz katmanda günlük üretim sınırı vardır ve sınırlar sık değişir; ders hazırlığı gibi zamanı kritik işlerde sınırı önceden hesaplayın.

---

# 2646. Ideogram ve metin-ağırlıklı araçlar

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Görselin kendisi metinden oluşuyorsa (afiş, kart, alt yazılı şema), metin doğruluğu birinci kriterdir. Ideogram bu iş için tasarlanmış araçlardan biridir; Nano Banana Pro ve GPT Image da metinde iyidir.

## Karar kuralı

- Metin ≤ 5 kelime: her üçü de yeterli; alışkanlığınıza göre seçin.
- Metin uzun ya da çok satırlı: Ideogram veya tırnak + font kuralıyla Nano Banana (2626).
- Çok dilli metin (Türkçe karakterler dahil): Nano Banana'nın yerelleştirme özelliği belirgin avantaj (2626).

---

# 2647. Adobe Firefly — ticari güvence gereken işler

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Firefly'in farkı teknik değil, hukukidir: çıktılar ticari kullanım için tazmin güvencesiyle (endemnifikasyon) gelir ve eğitim verisi lisanslı içerikle sınırlandırılmıştır.

## Karar kuralı

- Okul içi deneme, kişisel kullanım: güvence kritik değil.
- Kitap, kurum sitesi, ticari ürün: güvence bir kriterdir; bütçeye göre Firefly ya da hukuki görüş devreye girer.

## Neye dikkat edilmeli?

"Endemnifikasyon var" demek "telif ihlali yapılamaz" demek değildir. Üretilen görselde üçüncü kişinin yüzü, marka logosu, telifli karakter varsa sorun lisansla çözülmez, promptla önlenir (2656).

---

# 2648. Flux ve Stable Diffusion — açık ağırlıklar ve tam kontrol

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Açık ağırlıklı modeller (Flux, Stable Diffusion) kendi bilgisayarınızda ya da kendi sunucunuzda çalışabilir:

- **Avantaj:** Veri dışarı çıkmaz; sınıf fotoğrafları gibi hassas materyal için önemli. ControlNet/LoRA ile çok ince kontrol.
- **Maliyet:** Teknik kurulum ve iyi bir GPU gerekir; zaman maliyeti yüksek.

## Karar kuralı

Teknik ekip ve gizlilik gereği olan okul/kurum senaryoları için değerlendirin; bireysel kullanıcı için Gemini/ChatGPT/Ideogram akışları çoğu eğitim işini daha kısa sürede bitirir.

---

# 2649. Eğitim işi için araç seçim akışı

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Aşağıdaki tablo "hangi iş, hangi araçla başlar" sorusunun kısa cevabıdır:

| İş | İlk seçenek | Yedek |
|---|---|---|
| Ders diyagramı, kesit, şema | Nano Banana (metin + etiket) | GPT Image |
| Afiş, kart, yazılı materyal | Ideogram ya da Nano Banana (2626) | GPT Image |
| Fotoğraf düzenleme, seri tutarlılık | Nano Banana Pro (2625, 2630) | GPT Image konuşmalı düzenleme |
| Editoryal, sinematik görsel | Midjourney | GPT Image |
| Ticari yayın, güvence gereği | Firefly | Hukuki görüşle diğerleri |
| Gizlilik kritik, kendi sunucu | Flux / Stable Diffusion | — |

## Neye dikkat edilmeli?

Tablo akışı sabitlemez: aynı iş iki araçta denenebilir ve A/B kaydınızla (2637) kendi kurumunuz için doğrulanmış seçim yapılır. Araç seçimi, §90'daki kuralın bir uzantısıdır: aynı prompt her araçta aynı sonucu vermez.

---

# En-Boy Oranı ve Boyut Rehberi

Oran, promptun en başında değil ama **üretim tuşuna basmadan önce** düşünülmelidir. Yanlış oranda üretilen iyi görsel, doğru oranda yeniden üretilmek zorunda kalır.

---

# 2650. Oran neden prompttan önce düşünülmeli?

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Oran, kompozisyonun çerçevesidir. Kesit görünümü (§5) yatay senaryoda anlaşılırken dik karede sıkışır; flat lay (§ civarı aile) karede güçlüdür, dik formatta kenarlarda boşluk bırakır.

Oran sonradan kırpılarak düzeltilebilir; fakat kırpma, modelin kompozisyon kararını keser: etiketler dışarıda kalabilir, denge bozulur. Metin içeren görselde kırpma yazıyı kesebilir; bu durumda yeniden üretim tek çözümdür.

## Neye dikkat edilmeli?

Üretmeden önce tek soru: bu görsel nerede gösterilecek? Cevap tablodaki satırı verir (2651). Görsel birden çok yerde kullanılacaksa en geniş kullanım oranında üretilip kırpılabilir; ama metinli görselde bu yol güvenli değildir.

---

<a id="sec-2651"></a>
# 2651. Senaryo bazlı oran tablosu

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

| Kullanım yeri | Önerilen oran | Not |
|---|---|---|
| Sunum slaytı (16:9 ekran) | 16:9 | Tam ekran kullanılacaksa slaytla aynı |
| Çıktı/A4 el ilanı | 3:4 ya da 21:29,7 (yazıcı ayarına göre) | Baskıda 300 DPI hedefleyin (2663) |
| Instagram kare gönderi | 1:1 | |
| Instagram dikey gönderi | 4:5 | Akışta 1:1'den büyük görünür |
| Story / Reels / Shorts | 9:16 | Metin üst ve alt kenardan uzak dursun |
| YouTube küçük resmi | 16:9 | |
| Blog başlık görseli | 16:9 ya da 3:2 | |
| Okul panosu / poster | 2:3 | |

Nano Banana ailesinin desteklediği oranlar (2638) bu tabloyu doğrudan karşılar: 1:1, 3:2, 2:3, 3:4, 4:3, 4:5, 5:4, 9:16, 16:9, 21:9.

---

# 2652. Araçlarda oranı ayarlama

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Oran ayarı araçtan araca farklı üç yolla yapılır:

| Araç | Yol | Örnek |
|---|---|---|
| Midjourney | Parametre | `--ar 16:9` |
| Gemini (Nano Banana) | Menüden oran seçimi ya da promptta belirtme | "16:9 oranıyla üret" |
| ChatGPT (GPT Image) | Promptta söyleme | "yatay 16:9 kompozisyonda üret" |
| Ideogram | Arayüzden oran seçimi | — |

## Türkçe prompt (örnek)

> Bu diyagramı 16:9 yatay oranda yeniden üret; etiketlerin tamamı çerçeve içinde kalsın.

### English prompt

> Regenerate this diagram in a 16:9 landscape ratio; keep all labels inside the frame.

## Neye dikkat etilmeli?

Oran değişikliği "kırp" değil "yeniden kompozisyon" istemektir. Modelden kırpma değil, orana uygun yeniden yerleşim istemek etiket kaybını önler.

---

# Telif, Etik ve Güvenli Kullanım

Rehberde bu konular şimdiye kadar bölümlerin içinde (sahte kimlik belgesi uyarıları, gerçeğe dayanmayan veri kuralı) ele alınmıştı. Bu aile onları tek yerde toplar; eğitim bağlamı önceliklidir.

---

# 2653. Neden ayrı bir bölüm gerekiyor?

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Eğitim materyali çoğunlukla paylaşılır: okul sitesi, e-öğrenme platformu, basılı kitap. Görsel bir kez üretilince, onu üreten promptun mürekkebi kurumaya gider; görsel yıllarca dolaşır. Bu yüzden üç soru üretime değil, **paylaşım kararı anında** sorulmalıdır:

1. Bu görseli paylaşmaya hakkım var mı? (kaynak görseller ve kişiler)
2. Bu görselde sahte bir gerçeklik var mı? (belge, kişi, kurum)
3. Bu görselin üretiminde kullanılan aracın koşulları paylaşım türüme uyuyor mu?

---

# 2654. Üretilen görselin hakları — araçlar arası fark

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Araçların kullanım koşulları ürettiğiniz görselin kullanım haklarını belirler:

- Adobe Firefly: ticari kullanım için tazmin güvencesi sunan araçtır (2647).
- Gemini ve ChatGPT: ücretli katmanlarında ticari kullanıma geniş izin verir; koşullar sürüme göre değişebilir.
- Açık ağırlıklı modeller (Flux, SD): model lisansına ek olarak kullandığınız arayüzün koşulları da bakılır.

## Neye dikkat edilmeli?

Araç ücreti, "bu görsel benim malım" garantisi değildir. Üçüncü kişinin yüzü, markası, telifli karakteri görselde varsa sorun hak ihlalidir ve araç ücretiyle çözülmez (2656).

---

# 2655. Gerçek kişiler ve öğrenci fotoğrafları

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Eğitim bağlamının en hassas alanı budur:

- **Öğrenci fotoğrafı** üzerinde düzenleme yapılacaksa veli/öğrenci rızası ve kurumun veri politikası önce gelir. Bulut tabanlı araçlara hassas kişisel fotoğraf göndermek, o veriyi üçüncü tarafa iletme kararıdır.
- **Rızasız kişi** dönüştürülemez: `/film-noir-portrait` gibi formatlar kişisel/portre fotoğraflarda yalnızca rızalı ya da serbest lisanslı görsellerle çalışılmalıdır (2636).
- **Ünlü ve kamu personeli:** "X'in yargıç olarak fotoğrafı" istemi, hem kişilik hakları hem §18'deki doğrulama kuralı bakımından sorunludur; kurgusal karakterle çalışın.

## Sınıf içi kısa kural

Gerçek yüz gerekiyorsa rıza + kurum politikası + en az veri ilkesi. Gerçek yüz gerekmiyorsa kurgusal model ya da illüstrasyon.

---

# 2656. Markalar, logolar ve telifli karakterler

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

`/lego` gibi formatlar marka estetiğini andırdığı için bu soru sık gelir. Üç katman ayırt edilir:

1. **Jenerik tarife çevirme:** `interlocking toy bricks` (§892'nin notu) marka adı geçmeden aynı görsel dili verir; eğitim materyalinde tercih edilen yoldur.
2. **Marka adı promptta:** Marka estetiği istekleri genellikle çalışır ama çıktının ticari kullanımı marka haklarıyla sınırlıdır.
3. **Telifli karakter:** Pikachu, Mickey gibi karakterler teliflidir; eğitim diyagramında "telifli karakter" gerekiyorsa lisanslı görsel kullanmak tek güvenli yoldur.

## Neye dikkat edilmeli?

Rehberdeki dönüşüm formatlarının (minifigür, koleksiyon figürü, kutu) çoğu jenerik tarifeye çevrilebilir durumdadır; §892'deki gibi `interlocking toy bricks` yerine marka adı kullanmak zorunlu değildir.

---

# 2657. Filigran ve izlenebilirlik — SynthID ve C2PA

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Nano Banana ailesi her çıktıya görünmez SynthID filigranı ekler ve C2PA içerik kanıtı taşır; diğer büyük araçlar da benzer iz taşıma yönüne gitmektedir.

Bu iki nedenden önemlidir:

1. **Şeffaflık:** Görselin AI ile üretildiği doğrulanabilir; eğitim materyalinde bu bir sorun değil, özellik.
2. **Kanıt değeri:** AI görseli belge yerine geçmez (§89). C2PA bilgisi "üretim geçmişi" kanıtlar, gerçeklik kanıtlamaz.

## Neye dikkat etilmeli?

Filigranı kaldırma araçları kullanmak, hem koşulların ihlali hem de izlenebilirliğin silinmesidir. Eğitim bağlamında yapılacak doğru iş, görselin kaynağını ve üretim aracını metinde belirtmektir.

---

<a id="sec-2658"></a>
# 2658. Sınıfta kullanım için kısa kontrol listesi

Görsel üretim öncesi ve sonrası tek bakışta geçilecek liste:

- [ ] Kaynak fotoğraf varsa: rızası ve lisansı uygun mu?
- [ ] Görselde tanınabilir gerçek kişi var mı? Varsa gerekçesi yazılı mı?
- [ ] Marka, logo, telifli karakter var mı? Jenerik tarifeye çevrilebilir mi?
- [ ] Metinler harf harf doğru mu? (§18)
- [ ] Görsel "gerçek" sunuluyor mu? Temsilî olduğu belli mi?
- [ ] Paylaşım yeri (site, kitap, platform) araç koşullarıyla uyumlu mu? (2654)
- [ ] Üretim aracı ve tarih kaydedildi mi? (A/B kaydı, 2637)
- [ ] Dinî ve millî hassasiyet var mı? Peygamber tasviri, ibadetle alay, kutsala saygısızlık, bayrak/şehitlik istismarı ve kültür karikatürü yok mu? (§1563, aile-147)

## Neye dikkat edilmeli?

Bu liste §45'in görsel doğrulama listesiyle birlikte kullanılır: biri görselin teknik doğruluğunu, bu liste görselin etik ve hukuki konumunu kontrol eder.

---

# Düzenleme Akışları — Üretmekten Düzenlemeye

Eğitim ve içerik işinin büyük bölümü sıfırdan üretim değil, düzenlemedir. Bu aile üretimden düzenlemeye geçişte alınan kararları ve iki modelde çalışan teknikleri toplar.

---

<a id="sec-2659"></a>
# 2659. Yeni üret mi, düzenle mi? Karar rehberi

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Bir görsel istendiği gibi değilse iki yol vardır:

| Durum | Yol | Neden |
|---|---|---|
| Kompozisyon temelden yanlış | Yeni üretim | Düzeltme, yanlış yapıyı kopyalar |
| Kompozisyon doğru, bir öğe yanlış | Düzenleme (2630) | Üretim, doğru kısımları da riske atar |
| Metin bozuk | Metni düzelterek düzenleme | Üretimde metin tekrar bozulabilir |
| Kimlik kaymış | Referanslı yeniden üretim (2625) | Düzenleme kimliği geri getirmez |
| Dozu aşmış efekt | Düzenleme + Amount (2630) | Tek değişken döndürülür |

## Neye dikkat edilmeli?

Üçüncü denemeden sonra sonuç hâlâ uzaksa sorun prompttadır: etiketin açılımını yazmadan (2629) denemeye devam etmek, aynı boşluğun tekrar doldurulmasını beklemektir.

---

# 2660. Seçerek düzenleme — metinle maske (semantic masking)

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Nano Banana ailesinde maske, görsel editördeki fırçayla değil **metinle** çizilir: düzenlenecek bölge adıyla anılır, kalan kısmın sabit kalacağı yazılır (§ Google'ın resmî önerisi).

### Türkçe prompt (örnek)

> Yüklenen sınıf fotoğrafında yalnızca sağ duvardaki panoyu değiştir: panoyu güneş sistemi diyagramı yap. Duvar rengi, sıralar, ışık ve diğer her şey aynı kalsın.

### English prompt

> In the uploaded classroom photo change only the board on the right wall: turn it into a solar system diagram. Keep the wall color, desks, lighting, and everything else the same.

## Neye dikkat edilmeli?

Maske bölgesini "sağ duvardaki pano" gibi konum + nesne ile tanımlayın. "Pano" tek başına yazıldığında model benzer öğeyi yanlış seçebilir. Gerçek öğrenci yüzü içeren sınıf fotoğrafları için 2655'teki kural önce gelir.

---

# 2661. İteratif iyileştirme — mesaj başına tek değişiklik

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Konuşmalı düzenlemede kontrol, dozu ayarlamaktan geçer:

1. Tek değişiklik isteyin: "arka planı gece yap."
2. Sonucu değerlendirin (§45).
3. Yeni değişikliği yeni mesajda isteyin.

Beş değişiklik tek cümlede birleştirilirse hangisinin uygulanmadığı ayrıştırılamaz; her adımda geri dönüş noktası kaybolur.

## Neye dikkat edilmeli?

İterasyonda "görsel şunu da yapsın" birikimi, başlangıç kompozisyonunu bozar. Üç–dört adımdan sonra hâlâ uzaksa, 2659 tablosuna dönüp "yeni üretim" kararı verin.

---

# 2662. Seri tutarlılığı — aynı karakter, aynı stil, çok görsel

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Ders kitabı sayfası, hikâye dizisi ve sosyal medya serisi birden çok görselin aynı karakter/stil ile üretilmesini gerektirir:

1. **Karakter sayfası:** Karakteri bir kez referans görselle sabitleyin; sonraki görsellerde aynı referansı kullanın (2625).
2. **Stil kilitli prompt:** Stil tarifini kelimesi kelimesine aynı yazın: "sıcak pastel palet, sınırlı gölge, yuvarlak hat çizimi".
3. **Aynı oturum:** Konuşmalı araçlarda aynı sohbette devam etmek tutarlılığı artırır.

### Türkçe prompt (örnek)

> Bu referans görseldeki öğretmen karakteri, sonraki her görselde aynı kıyafet, aynı saç ve aynı yüzle görünsün. İlk görsel: öğretmen güneş sistemi panosunu gösteriyor.

### English prompt

> Keep the teacher character from this reference image in every following image: same clothes, same hair, same face. First image: the teacher pointing at a solar system board.

## Neye dikkat edilmeli?

Tutarlılık %100 değildir; karakter detayları sahne değiştikçe kayabilir. Kritik projede her görseli yan yana koyup §45 listesiyle ayrı ayrı kontrol edin; kayma varsa referans görseli yeniden yükleyin.

---

# 2663. Oran değiştirme, çözünürlük yükseltme ve baskıya hazırlık

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

- **Oran değiştirme:** Nano Banana'da yeni oran isteyip yeniden kompozisyon istemek; kırpma değil (2652).
- **Çözünürlük:** Nano Banana 1K/2K/4K çıkış destekler; baskı işlerinde 2K ve üstü hedefleyin (2638).
- **Baskı kuralı:** A4 çıktıda ~300 DPI hedeflenir; 4K görsel A4 baskı için yeterli yakınlıktadır, sunum için 2K çoğu zaman yeterlidir.
- **Büyütme (upscale):** Ayrı upscale araçları da mevcuttur; ama önce yüksek çözünürlüklü üretim, sonradan büyütmeden daha temizdir.

## Neye dikkat edilmeli?

Yeniden boyutlandırılmış görselde metin yeniden kontrol edilir: ölçek değişimi kenar yazılarını bozabilir.

---

<a id="sec-2664"></a>
# 2664. Düzenleme slop filtresi

Düzenleme akışı kendi slop risklerini taşır; §163'teki genel belirtiler burada şöyle somutlaşır:

- **Aşırı parlama:** Her düzenlemede ışık biraz daha şişer; Amount'ı düşürün (2630).
- **Doku kayması:** Düzenlenen bölge kalan görselden daha pürüzsüz olur; "doku aynı kalsın" kısıtını ekleyin (2630).
- **Kenar kaynaşması:** Değişen öğe ile arka plan arası geçiş bulanık olur; bölgeyi konum + nesne olarak net tanımlayın (2660).
- **Aşırı temizlik:** Gerçek fotoğraf hissi kaybolur; "rahatsız etmeyen gerçekçi kusurlar kalsın" istenebilir.

## Neye dikkat edilmeli?

Her düzenleme adımından sonra görseli bir öncekiyle yan yana koyun: fark istediğiniz tek değişiklikse devam edin; birden çok fark belirdiyse bir adım geri dönün.

---

<a id="aile-134"></a>
# İndeks Kelimesinden Tam Preset'e — En Sık Geçen Dokuz Kısayol

Rehber taramasında bazı kısayolların tur indekslerinde ve aile metinlerinde ikişer üçer kez geçtiği, ama bağımsız bölümü olmadığı görüldü (§891'deki üç statüden “indeks kelimesi” grubundakiler). Aşağıdaki dokuz bölüm bu boşluğu kapatır; her biri daha önce atıf yapılan adın ilk tam preset karşılığıdır.

---

# 2665. `/continuity-lock` — Seri Süreklilik Kilidi

## Türkçe prompt

> Seri boyunca değişmemesi gereken kimlik, kıyafet, nesne geometrisi, ortam, zaman, ışık ve renk özelliklerini sabitle. Her kareyi aynı dünyanın devamı gibi üret; değişen yalnız promptta açıkça yazan öğe olsun.

## English

> Lock identity, clothing, object geometry, environment, time, lighting, and color properties that should remain unchanged across the series. Render each frame as a continuation of the same world; change only what the prompt explicitly names.

## Neye dikkat edilmeli?

Kilit cümlesi serinin her promptuna aynen kopyalanır; kısaltılmış veya mealen yazılmış kilit çalışmaz. Sapan kare bulununca kilit değil, değişen öğenin cümlesi düzeltilir.

---

# 2666. `/material-swap` — Malzeme Değiştir, Formu Koru

## Türkçe prompt

> [NESNE]'nin biçimini, oranlarını ve tanınabilir özelliklerini aynen koru; yalnız malzemesini [YENİ MALZEME] ile değiştir. Yeni malzemenin fiziksel davranışı (yansıma, doku, kenar kalınlığı) görünsün; forma yalnızca doku kaplama.

## English

> Preserve the shape, proportions, and recognizable features of [OBJECT] exactly; change only its material to [NEW MATERIAL]. Show the physical behavior of the new material (reflection, texture, edge thickness) instead of merely wrapping the form in texture.

## Neye dikkat edilmeli?

Malzeme değişince ışık da değişir; gölge ve yansıma yeni malzemeye uymuyorsa sonuç fotomontaj gibi durur. Önce formun korunduğunu, sonra malzemenin inandırdığını ayrı ayrı denetleyin.

---

# 2667. `/material-grid` — Aynı Nesnenin Malzeme Karşılaştırması

## Türkçe prompt

> Aynı [NESNE]'yi 2×3 grid içinde altı farklı malzemeyle göster. Kamera açısı, ışık ve kadraj bütün hücrelerde aynı olsun; değişen yalnız malzeme olsun. Her hücrenin altına malzeme adını Türkçe yaz.

## English

> Show the same [OBJECT] in six different materials inside a 2×3 grid. Keep camera angle, lighting, and framing identical across cells; vary only the material. Label each cell with the material name in Turkish.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin (§1971); model fazladan hücre eklemeye eğilimlidir. Malzeme adlarındaki yazı harf harf denetlenir.

---

# 2668. `/tunnel-book` — Katmanlı Kâğıt Derinlik

## Türkçe prompt

> [SAHNE]'yi önden arkaya 4–5 paralel kâğıt katmanla kurulan tunnel book olarak göster. Her katman lazer kesim hissi versin; katman aralıkları önden bakınca gerçek derinlik üretsin. Kitap sırtı ve kapak çerçevesi görünsün; sahne tek düz illüstrasyona dönmesin.

## English

> Build [SCENE] as a tunnel book made of 4–5 parallel paper layers from front to back. Give each layer a laser-cut character so the gaps produce real depth when viewed head-on. Show the book spine and cover frame; do not flatten the scene into a single illustration.

## Neye dikkat edilmeli?

Derinlik gerçekten katman aralığından gelsin; bulanık arka planla taklit edilen derinlik tunnel book değildir. Katman sayısı üçe düşerse teknik okunmaz.

---

# 2669. `/mid-bite` — Isırılmış An

## Türkçe prompt

> [YEMEK]'i ilk ısırık alınmış, masada yarım kalmış hâliyle göster: ısırık izi, dağılmış kırıntı ve doğal el konumu. “İştah açıcı katalog” parlaklığına çekme; yaşanmışlık izleri sınırlı ve gerçekçi kalsın.

## English

> Show [FOOD] mid-bite and left on the table: visible bite mark, scattered crumbs, and a natural hand position. Do not polish it into appetizing catalog gloss; keep the lived-in traces limited and realistic.

## Neye dikkat edilmeli?

Dağınıklık bilinçli sınırlansın: tek ısırık izi, birkaç kırıntı; fazlası iştahı değil tiksintiyi çağırır. El ve ısırık izi aynı ısırığı anlatsın.

---

# 2670. `/tufted` — Püsküllü Halı Dönüşümü

## Türkçe prompt

> [ÖZNE]'yi püsküllü halı (tufted rug) tekniğiyle kurulmuş fiziksel nesneye dönüştür. Hav yüksekliği ve iplik yönü formu takip etsin; renk geçişleri halı dokumasının çözünürlüğünde sadeleşsin. Yalnızca yüzeye halı dokusu kaplama.

## English

> Transform [SUBJECT] into a physical object built with tufted-rug technique. Let pile height and yarn direction follow the form; simplify color transitions to the resolution of rug weaving. Do not merely wrap the surface in carpet texture.

## Neye dikkat edilmeli?

Yüz ve yazı gibi ince detaylar halı çözünürlüğünde okunmaz; bu öğeler ya büyütülsün ya tasarımdan çıkarılsın. Arka plan da aynı teknikte olsun, kolaj hissi vermesin.

---

# 2671. `/whittled` — Yontulmuş Ahşap Nesne

## Türkçe prompt

> [NESNE]'yi el oymasıyla yontulmuş ahşap heykelciğe dönüştür. Bıçak izleri ve ahşap damarı görünsün; keskin mühendislik kenarları yumuşasın. Tek parça ağaçtan oyulmuş hissi versin; yapıştırılmış parçalar belli olmasın.

## English

> Turn [OBJECT] into a hand-whittled wooden carving. Show knife marks and wood grain; soften sharp engineered edges. Make it feel carved from a single piece of wood without visible glued joints.

## Neye dikkat edilmeli?

Ahşap damarı formla birlikte aksın; damara ters yontulmuş gibi duran keskin köşeler tekniği ele verir. Minik parçalar (parmak, anten) kaba kalırsa ölçek büyütülsün.

---

# 2672. `/plushie` — Peluş Oyuncak Dönüşümü

## Türkçe prompt

> [KARAKTER]'i dikiş izleri ve kumaş dokusu görünen peluş oyuncağa dönüştür. Gözler düğme ya da nakış olsun; oranlar sevimlilik için hafif büyütülmüş başla sadeleşsin ama karakter tanınır kalsın.

## English

> Turn [CHARACTER] into a plush toy with visible seams and fabric texture. Use button or embroidered eyes; simplify proportions with a slightly enlarged head for cuteness while keeping the character recognizable.

## Neye dikkat edilmeli?

Sevimlilik anatomiyi yutmasın: uzuv sayısı ve yönü doğru kalsın. Kumaş deseni karakterin ayırt edici işaretlerini kapatıyorsa desen seyreltilir.

---

# 2673. `/embroidery` — El Nakışı İllüstrasyon

## Türkçe prompt

> [SAHNE]'yi kasnakta duran el nakışı illüstrasyona dönüştür. Dikiş yönleri formu takip etsin (Fransız düğümü, sap işi, balık sırtı ihtiyaca göre); iplik parlaklığı ve kumaş dokusu görünsün. Baskı değil, gerçek dikiş hissi versin.

## English

> Render [SCENE] as a hand-embroidered illustration in its hoop. Let stitch directions follow the form (French knots, stem stitch, fishbone as needed); show thread sheen and fabric weave. It should feel like real stitching, not print.

## Neye dikkat edilmeli?

Yazı nakışla yazılmaz; metin gerekiyorsa kumaşa iliştirilmiş küçük etiket olarak gösterilsin. Renk sayısı sınırlı tutulsun, her renk gerçek iplik karşılığı gibi dursun.

---

<a id="aile-135"></a>
# Kartpostal Dönemleri ve Seyahat Efemerası — İndeks Kelimelerinin Tam Preset Karşılıkları

§667'deki kartpostal kısayolları ile §722'deki ephemera kısayolları tur indekslerinde ad olarak geçiyor, bağımsız bölümleri yoktu. Aşağıdaki bölümler bu boşluğu kapatır. İki ailenin ortak kuralları burada da geçerlidir: kartpostalda önce dönem ve üretim biçimi seçilir, kusurlar o baskı sürecinden türetilir (§667); efemerada nesnenin gerçek işlevi, dönemi, baskı tekniği, gerekli bilgisi ve doğal kullanım izi sırayla kurulur (§722). Bilet, biniş kartı ve pul türü öğeler açıkça kurmaca ve illüstrasyon olarak üretilir; gerçek kurum adı, logo ve sahte resmiyet izlenimi verilmez.

---

# 2674. `/large-letter` — Büyük Harfli Kartpostal

## Türkçe prompt

> [ŞEHİR]'i 1930–50 arası large-letter kartpostal olarak göster: şehrin adı dev harflerle önde, her harfin içi şehrin farklı manzarasıyla dolsun. Litografi baskı hissi, sınırlı renk paleti ve ince beyaz çerçeve olsun.

## English

> Show [CITY] as a 1930s–50s large-letter postcard: the city name in giant letters in front, each letter filled with a different city view. Use a lithographic print feel, a limited color palette, and a thin white border.

## Neye dikkat edilmeli?

Harf içindeki manzaralar aynı şehre ait olsun; model başka şehirlerin simgelerini karıştırmaya eğilimlidir. Şehir adındaki yazı harf harf denetlenir.

---

# 2675. `/linen-card` — Keten Dokulu Kartpostal

## Türkçe prompt

> [ŞEHİR] manzarasını keten (linen) dönem kartpostal olarak göster: yüksek doygunluklu renkler, belirgin kumaş dokusu ve hafif abartılı gökyüzü. Baskı dokusu tüm yüzeyde eşit olsun.

## English

> Show a [CITY] view as a linen-era postcard: highly saturated colors, visible fabric texture, and a slightly exaggerated sky. Keep the print texture even across the surface.

## Neye dikkat edilmeli?

Doku kâğıttan gelsin, grenden değil; gren eklemek linen hissi vermez. Renk abartısı döneme uysun, neon tonlara kaymasın.

---

# 2676. `/rppc` — Gerçek Fotoğraf Kartpostalı

## Türkçe prompt

> [SAHNE]'yi gerçek fotoğraf kartpostalı (RPPC) olarak göster: siyah-beyaz fotoğraf, kartpostal sırtı formatı ve döneme uygun (1907–1930) sade tipografi. Fotoğraf stüdyo değil, sahada çekilmiş gibi dursun.

## English

> Show [SCENE] as a real photo postcard (RPPC): black-and-white photograph, postcard-back format, and plain period-appropriate (1907–1930) typography. Make the photo feel taken in the field, not in a studio.

## Neye dikkat edilmeli?

Dönemle uyuşmayan araç, giysi ve bina detayı en sık hatadır; her öğe tarihe karşı denetlenir. Arka yüzdeki posta çizgileri dönemin formatına uysun.

---

# 2677. `/hand-tinted` — El Boyaması Fotoğraf Kartı

## Türkçe prompt

> Siyah-beyaz [SAHNE] fotoğrafını el boyaması (hand-tinted) kartpostal olarak göster: renklendirme kısmi ve düzensiz olsun, bazı alanlar boyasız kalsın. Fırça izleri yakından sezilsin.

## English

> Show a black-and-white [SCENE] photograph as a hand-tinted postcard: keep the coloring partial and uneven, leaving some areas unpainted. Let brush marks be faintly visible up close.

## Neye dikkat edilmeli?

Tam ve pürüzsüz renklendirme el işi değil modern renklendirmedir; eksik bırakılan alan tekniğin kanıtıdır. Ten renkleri lekesiz ve tek tonda olmasın.

---

# 2678. `/photochrom` — Photochrom Esintili Seyahat Kartı

## Türkçe prompt

> [ŞEHİR] manzarasını photochrom baskı esintili seyahat kartı olarak göster: litografik renk katmanları, yumuşak gökyüzü geçişleri ve 1890–1910 dönemi kompozisyonu. Renkler doğal ama hafif teatral olsun.

## English

> Show a [CITY] view as a photochrom-inspired travel card: lithographic color layers, soft sky transitions, and an 1890–1910 composition. Keep colors natural but slightly theatrical.

## Neye dikkat edilmeli?

Dönem mimarisi ve ulaşım araçları doğrulanır; modern detay photochrom yanılsamasını anında bozar. Gökyüzü abartılırsa kartpostal değil fantezi olur.

---

# 2679. `/midcentury-card` — Yüzyıl Ortası Litografi Kart

## Türkçe prompt

> [ŞEHİR]'i yüzyıl ortası (1945–1965) litografi seyahat kartı olarak göster: düz renk alanları, stilize çizim dili ve dönemin tipografisi. Otomobil ve tabela gibi dönem işaretleri tutarlı olsun.

## English

> Show [CITY] as a mid-century (1945–1965) lithographic travel card: flat color fields, a stylized illustration language, and period typography. Keep period markers like cars and signs consistent.

## Neye dikkat edilmeli?

Tipografi dönemin karakterini taşısın; modern font tüm illüzyonu bozar. Araç modelleri tek onyıla ait olsun, karışmasın.

---

# 2680. `/roadside-card` — Yol Kenarı Americana Kartı

## Türkçe prompt

> [MOTEL / LOKANTA / BENZİNLİK]'i yol kenarı Americana kartpostalı olarak göster: gece neon tabelası, park etmiş dönem otomobilleri ve abartılı davetkâr kompozisyon. Tabela yazısı harf harf doğru olsun.

## English

> Show [MOTEL / DINER / GAS STATION] as a roadside Americana postcard: night neon signage, parked period cars, and an exaggerated welcoming composition. Render the sign text letter by letter correctly.

## Neye dikkat edilmeli?

Neon yazı en sık bozulan öğedir; kısa tutulur ve denetlenir. Tabela, bina ve araçlar aynı onyıla ait olsun.

---

# 2681. `/motel-card` — Vintage Motel Kartpostalı

## Türkçe prompt

> [MOTEL]'i vintage motel kartpostalı olarak göster: havuz, avlu ve oda kapıları aynı karede; “vacancy” tabelası ve dönem otomobili. Gün ışığı, temiz ve davetkâr düzen.

## English

> Show [MOTEL] as a vintage motel postcard: pool, courtyard, and room doors in one frame, with a vacancy sign and a period car. Use daylight and a clean, inviting layout.

## Neye dikkat edilmeli?

Havuz ve bina perspektifi tutarlı olsun; model suyu eğri çizmeye eğilimlidir. Tabela ve plaka gibi yazılar denetlenir.

---

# 2682. `/park-card` — Milli Park Kartı

## Türkçe prompt

> [MİLLİ PARK]'ı vintage milli park kartı olarak göster: simgesel manzara önde, yaban hayatı küçük ve doğal ölçeğinde, park amblemi köşede. Doğa abartılı renklere boğulmasın.

## English

> Show [NATIONAL PARK] as a vintage national-park card: the iconic landscape in front, wildlife small and at natural scale, the park emblem in a corner. Do not drown nature in exaggerated colors.

## Neye dikkat edilmeli?

Hayvan türü parka ait olsun; yanlış tür bilen izleyicide güveni bitirir. Amblem gerçek kurum logosunun kopyası olmasın, sadeleştirilmiş olsun.

---

# 2683. `/tourist-map-card` — Resimli Turist Haritası Kartı

## Türkçe prompt

> [ŞEHİR]'i resimli turist haritası kartpostalı olarak göster: şematik sokaklar, numaralı simgeler ve küçük efsane (lejant). Harita yön oku ve ölçek çubuğu içersin; coğrafi ilişkiler kabaca doğru olsun.

## English

> Show [CITY] as an illustrated tourist-map postcard: schematic streets, numbered landmarks, and a small legend. Include a north arrow and scale bar; keep geographic relationships roughly correct.

## Neye dikkat edilmeli?

Simge konumları gerçek şehre aykırı olmasın; şematik olması yanlış olması demek değildir. Lejant numaralarıyla harita numaraları birebir eşleşsin.

---

# 2684. `/panorama-card` — Açılır Panoramik Kart

## Türkçe prompt

> [MANZARA]'yı üç panelli açılır (fold-out) panoramik kartpostal olarak göster: paneller arası süreklilik kusursuz olsun, katlama çizgileri belli olsun. Ufuk çizgisi üç panelde tek çizgide birleşsin.

## English

> Show [VIEW] as a three-panel fold-out panorama postcard: keep continuity across panels seamless while showing the fold lines. Align the horizon into a single line across all three panels.

## Neye dikkat edilmeli?

Ufuk ve perspektif panel sınırlarında kırılmasın; model her paneli ayrı sahne gibi üretmeye eğilimlidir. Kat izi görünür ama yırtık gibi durmasın.

---

# 2685. `/then-now-card` — Önce / Şimdi Kartı

## Türkçe prompt

> Aynı [MEKÂN]'ı önce/sonra kartı olarak göster: sol yarı tarihsel fotoğraf diliyle, sağ yarı bugünkü hâliyle; bakış açısı ve kadraj iki tarafta aynı olsun. Ortada ince ayraç çizgisi olsun.

## English

> Show the same [PLACE] as a then-and-now card: the left half in historical photographic language, the right half as it looks today, with identical viewpoint and framing on both sides. Use a thin divider line in the middle.

## Neye dikkat edilmeli?

Değişen yalnız zaman olsun (§23 mantığı): açı, ölçek ve ışık yönü sabit kalsın. Tarihsel yarıdaki dönem detayları ayrıca doğrulanır.

---

# 2686. `/postcard-journal` — Kartpostal + Seyahat Günlüğü

## Türkçe prompt

> [ŞEHİR] kartpostalını seyahat günlüğü sayfasıyla birlikte göster: kartpostal üstte, altında el yazısı tarih, kısa not ve yapıştırılmış bilet parçası. El yazısı okunabilir, Türkçe karakterler doğru olsun.

## English

> Present a [CITY] postcard together with a travel-journal page: the postcard on top, with a handwritten date, a short note, and a pasted ticket stub below. Keep the handwriting legible with correct Turkish characters.

## Neye dikkat edilmeli?

El yazısı harf harf denetlenir; model tarih ve isimlerde harf uydurur. Bilet parçası kartpostalla aynı şehre ve döneme ait olsun.

---

# 2687. `/luggage-label` — Bavul Etiketi

## Türkçe prompt

> [OTEL / ŞEHİR] için vintage bavul etiketi (luggage label) tasarla: kalıpla kesilmiş (die-cut) etiket formu, kalın renk alanları, kısa şehir adı ve küçük simge. Kenarları hafif yıpranmış, baskı tekniği döneme uygun olsun.

## English

> Design a vintage luggage label for [HOTEL / CITY]: a die-cut label shape, bold color fields, a short city name, and a small icon. Show slightly worn edges and period-appropriate printing.

## Neye dikkat edilmeli?

Etiket gerçek işlevindeymiş gibi dursun: yapışma izi ve bavul köşesi bağlamı güçlendirir. Yazı kısa ve harf harf doğru olsun.

---

# 2688. `/hotel-label` — Otel Bavul Etiketi

## Türkçe prompt

> [OTEL ADI] için otel bavul etiketi tasarla: otelin cephesi veya amblemi küçük illüstrasyonla, otel adı döneme uygun tipografiyle. Gerçek bir otelin birebir logosu kopyalanmasın.

## English

> Design a hotel luggage label for [HOTEL NAME]: the hotel facade or emblem as a small illustration, with the hotel name in period typography. Do not copy a real hotel's exact logo.

## Neye dikkat edilmeli?

Logo benzerliği telif riski taşır; amblem sadeleştirilmiş ve özgün olsun. Tipografi ve baskı tekniği aynı döneme ait olsun.

---

# 2689. `/airline-label` — Havayolu Bavul Etiketi

## Türkçe prompt

> Kurmaca [HAVAYOLU] için havayolu bavul etiketi tasarla: stilize kanat/küre motifi, kısa marka adı ve dönem renkleri. Gerçek havayolu adı ve logosu kullanılmasın.

## English

> Design an airline luggage label for a fictional [AIRLINE]: a stylized wing or globe motif, a short brand name, and period colors. Do not use any real airline name or logo.

## Neye dikkat edilmeli?

Kurmaca olduğu belli olsun; gerçek marka izlenimi verecek yazı ve amblemden kaçınılır. Etiket formu dönemin havayolu etiket ölçülerine uysun.

---

# 2690. `/airport-tag` — Havalimanı Bagaj Etiketi

## Türkçe prompt

> [ŞEHİR] havalimanı koduyla ([KOD]) tarihsel bagaj etiketi tasarla: kod büyük ve okunabilir, havalimanı adı küçük yazıyla, dönem baskı renkleri. Modern barkod ve QR kullanılmasın.

## English

> Design a historical baggage tag with the [CITY] airport code ([CODE]): a large readable code, the airport name in small type, and period print colors. Do not use modern barcodes or QR codes.

## Neye dikkat edilmeli?

Kod ve şehir eşleşsin; uydurma kod güveni bitirir. Modern takip simgeleri dönem yanılsamasını bozar.

---

# 2691. `/tag-poster` — Etiket Anı Posteri

## Türkçe prompt

> Seyahat anılarını bavul etiketleri kolajı posteri olarak düzenle: 5–7 etiket farklı boyut ve açıda, ortada tek hero etiket, arka plan sade kraft tonunda. Etiketler aynı geziye ait olsun.

## English

> Arrange travel memories as a luggage-tag collage poster: 5–7 tags at varied sizes and angles, one hero tag in the center, on a plain kraft background. Keep all tags from the same trip.

## Neye dikkat edilmeli?

Etiketler aynı dönem ve baskı dilinde olsun; karışık dönem kolajı dağınık durur. Hero etiket dışındakiler sade tutulsun, yazı kalabalığı olmasın.

---

# 2692. `/matchbook` — Vintage Kibritlik

## Türkçe prompt

> [MEKÂN] reklamlı vintage kibritlik (matchbook) göster: ön yüzde illüstrasyon ve mekân adı, içte kibrit çöpleri, arkada kısa adres satırı. Kibritlik hafif açık dursun.

## English

> Show a vintage matchbook advertising [VENUE]: an illustration and venue name on the front, matchsticks inside, and a short address line on the back. Keep the matchbook slightly open.

## Neye dikkat edilmeli?

Mekân adı ve adres harf harf denetlenir. Kibrit çöpleri sayılabilir ve düzgün dizili olsun; model uydurma çöp ekler.

---

# 2693. `/matchbook-wall` — Kibritlik Koleksiyon Posteri

## Türkçe prompt

> Farklı [ŞEHİR] mekânlarına ait 9–12 kibritliği grid poster olarak diz: her kibritlik farklı tasarımda ama aynı fotoğraf diliyle çekilmiş olsun. Izgara hizası kusursuz olsun.

## English

> Arrange 9–12 matchbooks from different [CITY] venues as a grid poster: each matchbook with a different design but photographed in the same visual language. Keep the grid alignment perfect.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin; model eksik ya da fazla hücre üretmeye eğilimlidir. Her kibritlikteki yazı ayrı ayrı denetlenir.

---

# 2694. `/motel-key` — Retro Motel Anahtarı

## Türkçe prompt

> Retro motel oda anahtarını büyük plastik anahtarlıkla göster: anahtarlıkta motel adı ve oda numarası, metal anahtar sade. Anahtarlık rengi döneme uygun (örn. bakır-turuncu) olsun.

## English

> Show a retro motel room key with an oversized plastic fob: the motel name and room number on the fob, a plain metal key. Use a period-appropriate fob color (e.g., copper orange).

## Neye dikkat edilmeli?

Oda numarası ve motel adı yazı denetiminden geçsin. Anahtar dişleri abartılı ya da imkânsız olmasın; sade ve inandırıcı kalsın.

---

# 2695. `/airline-poster` — Jet Çağı Havayolu Posteri

## Türkçe prompt

> Kurmaca [HAVAYOLU]'nun [DESTİNASYON] posterini jet çağı (1955–1970) diliyle tasarla: stilize uçak ve destinasyon illüstrasyonu, kısa slogan, dönemin tipografisi. Gerçek havayolu adı kullanılmasın.

## English

> Design a jet-age (1955–1970) poster for fictional [AIRLINE] to [DESTINATION]: a stylized plane and destination illustration, a short slogan, and period typography. Do not use any real airline name.

## Neye dikkat edilmeli?

Uçak modeli döneme ait olsun; modern jet silueti anakronizmdir. Slogan kısa tutulsun ve harf harf denetlensin.

---

# 2696. `/rail-poster` — Demiryolu Seyahat Posteri

## Türkçe prompt

> [GÜZERGÂH] için demiryolu seyahat posteri tasarla: buharlı ya da erken dizel lokomotif, abartılı manzara perspektifi ve kısa destinasyon yazısı. 1920–1950 poster dilinde olsun.

## English

> Design a railway travel poster for [ROUTE]: a steam or early diesel locomotive, an exaggerated landscape perspective, and a short destination line. Keep it in 1920–1950 poster language.

## Neye dikkat edilmeli?

Lokomotif tipi güzergâhın dönemine uysun; ray ve vagon sayısı tutarlı olsun. Yazı posteri domine etmesin.

---

# 2697. `/airline-brochure` — Vintage Havayolu Broşürü

## Türkçe prompt

> Kurmaca [HAVAYOLU] için üç panelli vintage havayolu broşürü kapağı ve iç sayfa düzeni göster: koltuk düzeni şeması, menü kartı ve destinasyon listesi. Sayfa numaraları ve hizalama tutarlı olsun.

## English

> Show the cover and inside spread of a tri-fold vintage airline brochure for fictional [AIRLINE]: a seating chart, a menu card, and a destination list. Keep page numbers and alignment consistent.

## Neye dikkat edilmeli?

Şema ile liste çelişmesin (koltuk sayısı iki yerde aynı olsun). Gerçek marka ve güncel fiyat bilgisi kullanılmasın.

---

# 2698. `/tourist-brochure` — Turizm Ofisi Broşürü

## Türkçe prompt

> [ŞEHİR] turizm ofisi için vintage broşür kapağı tasarla: simgesel manzara, “resmî” hissi veren arma benzeri amblem ve üç dilde kısa karşılama satırı. Amblem gerçek kurum arması kopyası olmasın.

## English

> Design a vintage tourist-office brochure cover for [CITY]: an iconic view, an official-feeling crest-like emblem, and a short welcome line in three languages. Do not copy any real institutional crest.

## Neye dikkat edilmeli?

Üç dildeki satırlar ayrı ayrı denetlenir; model bilmediği dilde harf uydurur. Amblem özgün ve sade olsun.

---

# 2699. `/motel-brochure` — Vintage Motel Broşürü

## Türkçe prompt

> [MOTEL] için vintage motel broşürü göster: dış cephe fotoğraf dili, oda içi küçük kare, fiyat listesi ve yol tarifi şeması. Bilgiler birbiriyle tutarlı olsun.

## English

> Show a vintage motel brochure for [MOTEL]: exterior photo language, a small room inset, a price list, and a directions diagram. Keep all information mutually consistent.

## Neye dikkat edilmeli?

Fiyat, adres ve telefon formatı aynı döneme ait olsun. Oda karesi dış cepheyle aynı tesise aitmiş gibi dursun.

---

# 2700. `/foldout-map` — Açılır Turist Haritası

## Türkçe prompt

> [ŞEHİR] için açılır turist haritası göster: katlanmış hâli önde, açık hâli arkada; simgeler numaralı, lejant köşede. Katlama çizgileri belli, kâğıt kalınlığı hissedilsin.

## English

> Show a fold-out tourist map for [CITY]: the folded state in front, the open state behind, with numbered landmarks and a corner legend. Show the fold lines and a sense of paper thickness.

## Neye dikkat edilmeli?

Numara-lejant eşleşmesi birebir olsun. Katlanmış ve açık hâl aynı haritaya ait olsun; model iki farklı harita üretmeye eğilimlidir.

---

# 2701. `/road-map` — Vintage Karayolu Haritası

## Türkçe prompt

> [BÖLGE] için vintage karayolu haritası tasarla: kırmızı ana yollar, mavi tali yollar, şehir noktaları ve mesafe rakamları. Eski benzinlik logosu tadında köşe amblemi olsun (gerçek marka değil).

## English

> Design a vintage road map for [REGION]: red highways, blue secondary roads, city dots, and distance figures. Add a corner emblem in the spirit of an old gas-station logo (not a real brand).

## Neye dikkat edilmeli?

Yol ağı gerçek coğrafyayla kabaca uyuşsun; uydurma otoyol bilen gözde hemen belli olur. Mesafe rakamları tutarlı olsun.

---

# 2702. `/rail-ticket` — Vintage Tren Bileti

## Türkçe prompt

> [GÜZERGÂH] için vintage tren bileti tasarla: perfore kenar, güzergâh ve tarih damgası, sınıf bilgisi. Bilet açıkça illüstrasyon olarak dursun; gerçek bilet izlenimi vermesin.

## English

> Design a vintage rail ticket for [ROUTE]: perforated edges, route and date stamp, and class information. Keep the ticket clearly illustrative, never resembling a real ticket.

## Neye dikkat edilmeli?

Tarih, güzergâh ve sınıf birbiriyle tutarlı olsun. Perfore ve damga gerçekçi ama sahte-resmiyet hissi vermeyecek ölçüde olsun.

---

# 2703. `/air-ticket` — Vintage Uçak Bileti

## Türkçe prompt

> Kurmaca [HAVAYOLU] için vintage uçak bileti tasarla: kuponlu yapı, el yazısı hissi veren yolcu adı alanı ve tarih damgası. Gerçek havayolu ve barkod kullanılmasın.

## English

> Design a vintage airline ticket for fictional [AIRLINE]: a coupon structure, a handwritten-feel passenger name field, and a date stamp. Do not use any real airline or barcode.

## Neye dikkat edilmeli?

Kupon bilgileri birbiriyle eşleşsin; isim ve tarih harf harf denetlenir. Belge sahte-resmiyet izlenimi vermesin.

---

# 2704. `/boarding-pass` — Kurmaca Retro Biniş Kartı

## Türkçe prompt

> Kurmaca [HAVAYOLU] için retro biniş kartı tasarla: koltuk, kapı ve uçuş numarası alanları doldurulmuş, perfore koparma çizgili. Kartpostal estetiğinde, açıkça illüstrasyon olsun.

## English

> Design a fictional retro boarding pass for [AIRLINE]: filled seat, gate, and flight-number fields with a perforated tear line. Keep a postcard aesthetic so it reads as illustration.

## Neye dikkat edilmeli?

Gerçek uçuş numarası formatı ve barkod kullanılmasın; kart sahte belge gibi durmasın. Tüm yazılar denetlenir.

---

# 2705. `/transit-ticket` — Tarihsel Şehir İçi Bilet

## Türkçe prompt

> [ŞEHİR] için tarihsel şehir içi ulaşım bileti tasarla: tramvay/otobüs damgası, hat numarası ve dönem tipografisi. Bilet küçük ve sade olsun.

## English

> Design a historical city transit ticket for [CITY]: a tram or bus stamp, a line number, and period typography. Keep the ticket small and simple.

## Neye dikkat edilmeli?

Hat numarası ve damga şehrin gerçek tarihine aykırı olmasın. Küçük yazılar okunabilirlik sınırında test edilsin.

---

# 2706. `/ferry-ticket` — Tarihsel Vapur Bileti

## Türkçe prompt

> [HAT] için tarihsel vapur bileti tasarla: iskele adları, sefer saati ve sınıf bilgisiyle. Denizcilik renkleri (lacivert-beyaz) ve sade tipografi kullanılsın.

## English

> Design a historical ferry ticket for [LINE]: with pier names, departure time, and class information. Use maritime colors (navy and white) and plain typography.

## Neye dikkat edilmeli?

İskele adları ve saat formatı döneme uysun. Bilet açıkça illüstrasyon olarak kalsın.

---

# 2707. `/pennant` — Şehir Flaması

## Türkçe prompt

> [ŞEHİR] için vintage üçgen şehir flaması (pennant) göster: keçe dokusu, aplike harflerle şehir adı ve küçük simge. Flama hafif dalgalı dursun, duvara asılı bağlamıyla sunulsun.

## English

> Show a vintage triangular city pennant for [CITY]: felt texture, appliquéd city-name letters, and a small icon. Present it slightly rippled, in a wall-hung context.

## Neye dikkat edilmeli?

Aplike harfler düzgün dikilsin; eğri harf tekniği ele verir. Şehir adı ve simge aynı şehre ait olsun.

---

# 2708. `/hotel-stationery` — Otel Antetli Kâğıdı

## Türkçe prompt

> [OTEL] için vintage otel antetli kâğıdı ve zarfı göster: üstte küçük cephe illüstrasyonu, zarif başlık tipografisi ve adres satırı. Kâğıt dokusu hissedilsin.

## English

> Show vintage hotel stationery and its envelope for [HOTEL]: a small facade illustration on top, elegant header typography, and an address line. Give a sense of paper texture.

## Neye dikkat edilmeli?

Adres formatı döneme uysun (posta kodu, telefon). Başlık ve adres yazıları harf harf denetlenir.

---

# 2709. `/airmail` — Uçak Postası Zarfı

## Türkçe prompt

> Uçak postası (airmail) zarfı göster: kırmızı-mavi verev kenar bordürü, “PAR AVION” benzeri kısa ibare ve pul köşesi. Zarf hafif yıpranmış, üzerinde el yazısı adres olsun.

## English

> Show an air-mail envelope: a red-and-blue diagonal border, a short “PAR AVION”-style marking, and a stamp corner. Keep the envelope slightly worn with a handwritten address.

## Neye dikkat edilmeli?

El yazısı adres okunabilir olsun; pul gerçek pul kopyası değil, sadeleştirilmiş illüstrasyon olsun. Kenar bordürü düzgün ve kesintisiz dönsün.

---

# 2710. `/stamp-sheet` — Kurmaca Pul Sayfası

## Türkçe prompt

> Kurmaca [ÜLKE / ŞEHİR] pullarından oluşan koleksiyon sayfası tasarla: 6–9 pul, her pulda farklı manzara ve nominal değer. Pullar açıkça illüstrasyon olsun; gerçek ülke adı ve posta idaresi yazmasın.

## English

> Design a collector sheet of fictional [COUNTRY / CITY] stamps: 6–9 stamps, each with a different view and denomination. Keep the stamps clearly illustrative, with no real country or postal authority names.

## Neye dikkat edilmeli?

Gerçek posta işareti ve ülke adı kullanılmasın; sayfa sahte-resmiyet izlenimi vermesin. Perforasyon düzgün ve eşit olsun.

---

# 2711. `/ticket-collage` — Bilet Efemera Kolajı

## Türkçe prompt

> Bir [GEZİ]'ye ait bilet ve fişleri efemera kolajı olarak düzenle: tren bileti, müze bileti, fiş ve pul aynı yüzeyde, katmanlı ama okunabilir. Hepsi aynı geziye ve döneme ait olsun.

## English

> Arrange tickets and receipts from one [TRIP] as an ephemera collage: rail ticket, museum ticket, receipts, and stamps on one surface, layered but legible. Keep everything from the same trip and era.

## Neye dikkat edilmeli?

Tarihler birbiriyle çelişmesin; kolajın anlattığı gezi tek ve tutarlı olsun. Yazı kalabalığı okunabilirliği bitirmesin.

---

# 2712. `/roadtrip-board` — Yolculuk Efemera Panosu

## Türkçe prompt

> [GÜZERGÂH] yolculuğunu efemera panosu olarak anlat: harita parçası, benzin fişi, motel kartı ve fotoğraf aynı panoda iğneli. Pano kronolojik sırayla okunsun.

## English

> Tell a [ROUTE] road trip as an ephemera board: a map fragment, gas receipts, a motel card, and photos pinned on one board. Make the board read in chronological order.

## Neye dikkat edilmeli?

Kronoloji bozulmasın; fiş tarihleri güzergâh sırasını desteklesin. İğne ve bant gibi tutturucular fiziksel olarak inandırıcı olsun.

---

# 2713. `/city-guide` — Retro Şehir Rehberi Kapağı

## Türkçe prompt

> [ŞEHİR] için retro şehir rehberi kapağı tasarla: kapak illüstrasyonu, başlık, yıl ve “resmî” hissi veren sade amblem. İç sayfa önizlemesi küçük karede gösterilsin.

## English

> Design a retro city-guide cover for [CITY]: a cover illustration, title, year, and a plain official-feeling emblem. Show an inside-page preview in a small inset.

## Neye dikkat edilmeli?

Kapak ve iç sayfa aynı tasarıma ait olsun. Yıl ile içerik dili (fotoğraf mı illüstrasyon mu) çelişmesin.

---

# 2714. `/ephemera-set` — Koordineli Şehir Efemera Seti

## Türkçe prompt

> [ŞEHİR] için koordineli seyahat efemera seti tasarla: kartpostal, bagaj etiketi, pul ve katlanır harita aynı renk ve tipografi sisteminde. Set aynı masada, düzenli kompozisyonla sunulsun.

## English

> Design a coordinated city travel ephemera set for [CITY]: a postcard, luggage label, stamp, and fold-out map in one color and typography system. Present the set neatly on one table.

## Neye dikkat edilmeli?

Sistem tutarlılığı esastır: renk, font ve amblem bütün parçalarda aynı olsun. Parçalardan biri sistem dışına taşarsa set dağılır.

---

<a id="aile-137"></a>
# §891 İndeksinin Tam Preset Karşılıkları — Portre, Moda, Mekân, Ambalaj, Müzik, Harita

§891'deki “Bu tur için slash-style kısa adlar” tablosundaki satırların bir kısmının bağımsız bölümü yoktu. Aşağıdaki bölümler bu boşluğu kapatır. Zaten tam preset karşılığı olanlar kapsanmamıştır: `/direct-flash` §1333, `/scanography` §1730, `/material-board` §1652, `/material-grid` §2667, `/sensory-closeup` §1549'tadır.

---

# 2746. `/party-snapshot` — Parti Anı Fotoğrafı

## Türkçe prompt

> [KİŞİ / GRUP]'u ev partisinde çekilmiş doğal an fotoğrafı olarak göster: doğrudan flaş, gevşek kadraj, arka planda parti detayları. Poz verilmiş stüdyo hissi olmasın.

## English

> Show [PERSON / GROUP] as a candid party snapshot: direct flash, loose framing, and party details in the background. Avoid any posed studio feel.

## Neye dikkat edilmeli?

Flaş sertliği ve kırmızı göz kontrol altında olsun; gece dokusu stüdyo parlaklığına çekilmesin. Arka plandaki yüzler tanınmayacak ölçüde flu bırakılabilir.

---

# 2747. `/connection` — Gerçek Etkileşim Portresi

## Türkçe prompt

> İki [KİŞİ]'yi gerçek bir etkileşim anında göster: göz teması, gülüşme ya da ortak bir işe bakma. Kameraya poz verme hissi olmasın; an, sahnelenmiş gibi durmasın.

## English

> Show two [PEOPLE] in a moment of genuine interaction: eye contact, shared laughter, or looking at a common task. Avoid any sense of posing for the camera; the moment should not feel staged.

## Neye dikkat edilmeli?

Eller ve bakış yönleri aynı anı anlatsın; biri kameraya bakıyorsa etkileşim bozulur. Yapay kahkaha yüzleri donuklaştırır, dozunda tutulsun.

---

# 2748. `/motion-portrait` — Hareket Bulanıklıklı Portre

## Türkçe prompt

> [KİŞİ]'yi hafif hareket bulanıklığıyla portre olarak göster: yüz tanınır kalsın, saç ve giysi hareket izi taşısın. Enstantane hissi veren doğal bir an olsun.

## English

> Show [PERSON] as a portrait with slight motion blur: keep the face recognizable while hair and clothing carry motion trails. Make it feel like a natural split-second moment.

## Neye dikkat edilmeli?

Yüz netliği korunsun; yüz de bulanıksa portre değil hata olur. Bulanıklık tek yönde olsun, dağınık titreme değil.

---

# 2749. `/reflection` — Cam Yansıması Portresi

## Türkçe prompt

> [KİŞİ]'yi cam yansımasıyla birlikte portre olarak göster: vitrin ya da pencere camında yansıma, gerçek kişiyle yansıma aynı karede dengeli olsun. Yansıma silüeti bozmasın.

## English

> Show [PERSON] as a portrait with glass reflection: a shop-window or window-pane reflection balanced with the real person in one frame. Keep the reflection from breaking the silhouette.

## Neye dikkat edilmeli?

Yansıma geometrisi tutarlı olsun: yansıyan öğeler camın arkasındaki gerçek sahneye uysun. Çift pozlama hissi istenmiyorsa katmanlar net ayrılsın.

---

# 2750. `/xerox-portrait` — Fotokopi Portre

## Türkçe prompt

> [KİŞİ] portresini fotokopi (xerox) estetiğinde göster: yüksek kontrast siyah-beyaz, toner dokusu ve hafif eğik tarama. Fanzin kapağı hissi versin.

## English

> Show a [PERSON] portrait in photocopy (Xerox) aesthetics: high-contrast black and white, toner texture, and a slightly skewed scan. Give it a zine-cover feel.

## Neye dikkat edilmeli?

Kontrast yüzü yutmasın; gözler ve ağız çizgisi okunur kalsın. Leke ve çizgiler dozunda olsun, portre çamur gibi durmasın.

---

# 2751. `/contact-sheet` — Portre Contact Sheet

## Türkçe prompt

> [KİŞİ]'nin aynı çekimden 6–9 karesini contact sheet olarak diz: kareler aynı ışık ve fonda, küçük ifade ve açı farklarıyla. Onaylı kareyi kırmızı kalem işaretiyle belirt.

## English

> Arrange 6–9 frames of [PERSON] from one shoot as a contact sheet: same lighting and backdrop with small expression and angle differences. Mark the approved frame with a red grease-pencil mark.

## Neye dikkat edilmeli?

Kimlik bütün karelerde sabit kalsın; sapan kare tek başına üretilsin. Hücre sayısı sabitlensin, film şeridi kenarlıkları tutarlı olsun.

---

# 2752. `/real-skin` — Doğal Cilt Portresi

## Türkçe prompt

> [KİŞİ]'yi doğal cilt dokusuyla portre olarak göster: gözenek, ben ve hafif asimetri korunsun; rötuş “temizlenmiş” değil “düzenlenmiş” seviyesinde kalsın. Cilt tonu gerçekçi olsun.

## English

> Show [PERSON] as a portrait with natural skin texture: preserve pores, moles, and slight asymmetry, keeping retouching at a “tidied” rather than “cleaned” level. Keep skin tone realistic.

## Neye dikkat edilmeli?

Pürüzsüzlük ile plastiklik sınırı yakındır; yakın planda doku kontrol edilsin. Cilt tonu ışıkla birlikte tutarlı değişsin, grileşmesin.

---

# 2753. `/editorial-crop` — Editorial Portre Kadrajı

## Türkçe prompt

> [KİŞİ] portresini dergi kullanımı için kadrajla: yüz karenin üst üçte birinde, bakış yönünde boşluk bırakılsın, alt yarı metin alanı olarak sade tutulsun. Dikey 3:4 kompozisyon olsun.

## English

> Crop a [PERSON] portrait for magazine use: face in the upper third, space left in the gaze direction, and the lower half kept plain as text area. Use a vertical 3:4 composition.

## Neye dikkat edilmeli?

Metin alanı gerçekten boş kalsın; model doldurmaya eğilimlidir. Başlık boşluğu masthead için yeterli olsun (§2193).

---

# 2754. `/street-style` — Sokak Stili Candid

## Türkçe prompt

> [KİŞİ]'yi sokak stili fotoğrafı olarak göster: tam boy kadraj, doğal yürüyüş anı, şehir fonu flu. Kıyafet net, yüz tanınır olsun.

## English

> Show [PERSON] as a street-style photograph: full-body framing, a natural walking moment, and a blurred city backdrop. Keep the outfit sharp and the face recognizable.

## Neye dikkat edilmeli?

Kıyafet odakta kalsın; fon bulanıklığı özneyi yutmasın. Yürüyüş pozu dengeli olsun, düşüyormuş hissi vermesin.

---

# 2755. `/outfit-formula` — Kıyafet Formülü

## Türkçe prompt

> [KİŞİ]'nin günlük kıyafet formülünü tek karede göster: üst, alt, ayakkabı ve 1–2 aksesuar etiketli ya da düzenli dizili. Formül tekrar giyilebilir sadelikte olsun.

## English

> Show [PERSON]'s daily outfit formula in one frame: top, bottom, shoes, and 1–2 accessories, labeled or neatly arranged. Keep the formula simple enough to re-wear.

## Neye dikkat edilmeli?

Parçalar aynı stile ait olsun; formülün tekrarlanabilirliği esastır. Renk uyumu abartılı styling'e kaymasın.

---

# 2756. `/capsule-wardrobe` — Kapsül Gardırop Panosu

## Türkçe prompt

> [SEZON] için 8–12 parçalık kapsül gardırop panosu hazırla: parçalar birbirleriyle kombinlenebilir olsun, renk paleti sınırlı, her parça temiz ürün fotoğrafı dilinde. Pano ızgara düzeninde olsun.

## English

> Build an 8–12 piece capsule wardrobe board for [SEASON]: keep pieces mutually combinable with a limited color palette, each in clean product-photo language. Use a grid layout.

## Neye dikkat edilmeli?

Her parça en az üç kombinasyona girmeli; girmeyen parça panodan çıkarılır. Renk paleti dışına taşan parça sistemi bozar.

---

# 2757. `/exploded-outfit` — Kıyafet Parça Çözümlemesi

## Türkçe prompt

> [KOMBİN]'i patlatılmış görünüm mantığıyla göster: katmanlar (iç-dış giyim, ayakkabı, aksesuar) montaj sırasına göre ayrılmış ama ilişkisi okunur olsun. Her katman etiketli olsun.

## English

> Show [OUTFIT] with exploded-view logic: layers (inner and outer wear, shoes, accessories) separated in assembly order while keeping their relationship readable. Label each layer.

## Neye dikkat edilmeli?

Katman sırası giyilme sırasını izlesin; karışık sıra öğreticiliği bitirir (§4 mantığı). Parçalar aynı bedene aitmiş gibi dursun.

---

# 2758. `/fabric-swatches` — Kumaş Kartelası

## Türkçe prompt

> [KOLEKSİYON] için kumaş kartelası (swatch board) hazırla: 6–9 kumaş örneği, her birinde doku yakından hissedilsin, altında kumaş adı ve içerik oranı yazsın. Kartela düzenli ızgarada olsun.

## English

> Build a fabric swatch board for [COLLECTION]: 6–9 fabric samples with closely felt textures, each labeled with fabric name and content ratio. Use a neat grid.

## Neye dikkat edilmeli?

Doku ile yazı eşleşsin; yanlış etiket koleksiyonu bitirir. Renkler ekranda değil baskıda doğrulanacaksa bu belirtilsin.

---

# 2759. `/garment-breakdown` — Giysi Konstrüksiyon Çözümlemesi

## Türkçe prompt

> [GİYSİ]'nin konstrüksiyonunu çözümleme olarak göster: kalıp parçaları, dikiş yerleri ve astar katmanı ayrı ayrı; dikiş yönleri oklarla belirtilsin. Terzilik şeması dili kullanılsın.

## English

> Show the construction breakdown of [GARMENT]: pattern pieces, seams, and lining shown separately, with stitch directions marked by arrows. Use tailoring-diagram language.

## Neye dikkat edilmeli?

Dikiş yönleri gerçek terziliğe uysun; uydurma dikiş bilen gözde hemen belli olur. Parça adları standart terimlerle yazılsın.

---

# 2760. `/reading-nook` — Kişisel Okuma Köşesi

## Türkçe prompt

> [KİŞİ] için kişiselleştirilmiş okuma köşesi tasarla: koltuk, okuma lambası, küçük raf ve battaniye; köşe kişinin ilgi alanını yansıtan 2–3 nesne içersin. Işık sıcak ve odakta kitap olsun.

## English

> Design a personalized reading nook for [PERSON]: an armchair, reading lamp, small shelf, and throw blanket, with 2–3 objects reflecting the person's interests. Keep the light warm with the book in focus.

## Neye dikkat edilmeli?

Işık kitap üzerine düşsün; loş köşede okunmayan kitap sahte durur. Kişisel nesneler gerçekten o kişiye ait olsun, katalog doldurması olmasın.

---

# 2761. `/closet-nook` — Gömme Dolap Okuma Köşesi

## Türkçe prompt

> Kullanılmayan gömme dolabı okuma köşesine dönüştür: oturma minderi, raf aydınlatması ve perde/kapı çözümü. Dar alan ferah gösterilsin ama gerçek ölçüler hissedilsin.

## English

> Convert an unused closet into a reading nook: a seat cushion, shelf lighting, and a curtain or door solution. Keep the narrow space airy while preserving a sense of real dimensions.

## Neye dikkat edilmeli?

Ölçü dürüstlüğü esastır; dolap saray gibi gösterilmesin. Havalandırma ve ışık gerçekçi çözülsün.

---

# 2762. `/micro-makeover` — Aynı Kadrajda Önce / Sonra

## Türkçe prompt

> Aynı [ODA]'yı aynı kamerayla önce/sonra olarak göster: kamera konumu, açı ve ışık saati sabit; değişen yalnız mobilya ve düzen olsun. İki kare yan yana sunulsun.

## English

> Show the same [ROOM] as a before/after from an identical camera: fixed camera position, angle, and time of day, varying only furniture and layout. Present the two frames side by side.

## Neye dikkat edilmeli?

Değişen yalnız incelenen değişken olsun (§23 mantığı); ışık değiştiyse karşılaştırma kirlenir. Eşyaların gölgeleri yeni düzene uysun.

---

# 2763. `/moody-blue` — Kasvetli Mavi İç Mekân

## Türkçe prompt

> [ODA]'yı kasvetli mavi (moody-blue) iç mekân olarak göster: lacivert-petrol duvarlar, sıcak noktasal ışıklar ve koyu ahşap. Mekân kasvetli ama yaşanır dursun.

## English

> Show [ROOM] as a moody-blue interior: navy-petrol walls, warm accent lights, and dark wood. Keep the space moody but livable.

## Neye dikkat edilmeli?

Koyu renk detayları yutmasın; ışık-gölge dengesiyle derinlik korunsun. Mavi tek tona düşerse mekân düzleşir.

---

# 2764. `/vintage-pink` — Vintage Pembe Mutfak

## Türkçe prompt

> Vintage pembe mutfak göster: retro buzdolabı, fayans desenleri ve krom detaylar; pembe baskın ama göz yormayan tonda olsun. 1950'ler mutfak dili tutarlı olsun.

## English

> Show a vintage-pink kitchen: a retro fridge, tile patterns, and chrome details, with pink dominant but easy on the eyes. Keep the 1950s kitchen language consistent.

## Neye dikkat edilmeli?

Dönem detayları (priz, batarya, zemin) aynı onyıla ait olsun. Pembe dozu kaçarsa mutfak şekerciye döner.

---

# 2765. `/grandma-kitchen` — Birikmiş Vintage Mutfak

## Türkçe prompt

> Yıllarla birikmiş vintage mutfak göster: uyumsuz ama uyumlu tabaklar, dantel perde, bakır tencereler ve tezgâhta günlük izler. Düzenli dağınıklık hissi versin.

## English

> Show a collected vintage kitchen: mismatched yet harmonious dishes, lace curtains, copper pots, and daily traces on the counter. Give a sense of ordered clutter.

## Neye dikkat edilmeli?

Dağınıklık bilinçli sınırlansın; kirli ile yaşanmış ayrımı korunsun. Her nesnenin yeri belli olsun, rastgele yığın olmasın.

---

# 2766. `/dark-cottage` — Koyu Kır Evi Mutfağı

## Türkçe prompt

> Koyu kır evi (dark cottage) mutfağı göster: siyah-yeşil dolaplar, taş tezgâh, açık raf ve asılı otlar. Işık pencereden doğal gelsin, loş ama okunur olsun.

## English

> Show a dark cottage kitchen: black-green cabinets, a stone counter, open shelving, and hanging herbs. Bring natural window light, dim but legible.

## Neye dikkat edilmeli?

Koyu yüzeylerde doku kaybolmasın; ışık mutfak üçgenini (ocak-eviye-buzdolabı) okunur kılsın. Asılı otlar taze ve yerinde dursun.

---

# 2767. `/warm-wood` — Sıcak Ahşap İç Mekân

## Türkçe prompt

> Sıcak ahşap iç mekân göster: meşe/ceviz tonları, keten tekstil ve yumuşak gün ışığı. Ahşap damarlar yönlü ve tutarlı olsun.

## English

> Show a warm wood interior: oak and walnut tones, linen textiles, and soft daylight. Keep wood grains directional and consistent.

## Neye dikkat edilmeli?

Ahşap tonları tek ailede kalsın; her mobilya farklı ağaçsa bütünlük bozulur. Damar yönü gerçek marangozluğa uysun.

---

# 2768. `/lived-in-shelf` — Doğal Birikmiş Raf

## Türkçe ek

> Kitap ve nesnelerle doğal birikmiş raf göster: diziliş kusursuz olmasın, kitap boyları karışık, arada kişisel nesneler olsun. Raf yaşanmış ama bakımlı dursun.

## English

> Show a naturally collected shelf of books and objects: imperfect arrangement with mixed book heights and personal objects in between. Keep the shelf lived-in but cared for.

## Neye dikkat edilmeli?

Kitap sırtlarındaki yazılar denetlenir; model harf uydurur. Toz ve leke abartılırsa bakımsız izlenimi verir.

---

# 2769. `/product-macro` — Dokunsal Ürün Makro

## Türkçe prompt

> [ÜRÜN]'ü dokunsal makro fotoğraf olarak göster: malzeme dokusu (dikiş, gren, lif) aşırı yakın planda, alan derinliği sığ. Ürünün bir bölümü kadraj dışında kalabilir.

## English

> Show [PRODUCT] as a tactile macro photograph: material texture (stitching, grain, fiber) in extreme close-up with shallow depth of field. Part of the product may fall outside the frame.

## Neye dikkat edilmeli?

Odak noktası malzemenin en ayırt edici yerinde olsun. Makro, üretim hatasını da büyütür; kusur varsa bilinçli gösterilsin.

---

# 2770. `/used-product` — Kullanılmış Ama Bakımlı Ürün

## Türkçe prompt

> [ÜRÜN]'ü kullanılmış ama bakımlı göster: hafif kullanım izleri (solma, küçük çizik) gerçekçi dozda, ürün temiz ve çalışır durumda. Katalog yenisi gibi durmasın.

## English

> Show [PRODUCT] as used but cared for: light wear (fading, small scratches) in realistic doses, with the product clean and functional. Avoid catalog-new looks.

## Neye dikkat edilmeli?

Yıpranma dürüst olsun; ne gizlensin ne abartılsın. İkinci el güveni detayda kurulur.

---

# 2771. `/mono-material` — Tek Malzeme Ürün Dünyası

## Türkçe prompt

> [ÜRÜN]'ü tek malzemeden kurulmuş dünyada göster: ürün ve çevresi aynı malzeme (örn. karton, kil, buz); ışık malzemenin davranışını ortaya çıkarsın. Malzeme dışında renk kullanılmasın.

## English

> Show [PRODUCT] in a mono-material world: product and surroundings in one material (e.g., cardboard, clay, ice), with lighting revealing the material's behavior. Use no color outside the material.

## Neye dikkat edilmeli?

Malzeme davranışı tutarlı olsun; buz erimiyorsa, kil çatlamıyorsa nedeni sahnede sezilsin. Ürün formdan ayırt edilsin, kamufle olmasın.

---

# 2772. `/pulp-pack` — Kalıplanmış Selüloz Ambalaj

## Türkçe prompt

> [ÜRÜN] için kalıplanmış selüloz (molded pulp) ambalaj göster: lifli yüzey, ürüne oturan yuva formu ve tek renk baskı logo. Ambalaj açılır ve kapanır şekilde sunulsun.

## English

> Show molded-pulp packaging for [PRODUCT]: a fibrous surface, a nest form fitted to the product, and single-color printed logo. Present the packaging openable and closable.

## Neye dikkat edilmeli?

Yuva ürüne tam otursun; bol ya da sıkı duran ambalaj inandırıcılığı bitirir. Lif dokusu yakından hissedilsin.

---

# 2773. `/mono-pack` — Tek Malzeme Ambalaj

## Türkçe prompt

> [ÜRÜN] için tek malzemeden ambalaj sistemi tasarla: kutu, iç yatak ve etiket aynı malzemeden; birleşim yerleri malzemenin kendi mantığıyla (katlama, geçme) çözülsün. Plastik pencere kullanılmasın.

## English

> Design a mono-material packaging system for [PRODUCT]: box, insert, and label from one material, with joints solved in the material's own logic (folding, interlocking). Use no plastic window.

## Neye dikkat edilmeli?

Geri dönüşüm iddiası malzeme gerçeğiyle uyuşsun; kaplamalı kâğıt “tek malzeme” sayılmaz. Etiket mürekkebi de sistemin parçası olsun.

---

# 2774. `/second-life-pack` — Yeniden Kullanılır Ambalaj

## Türkçe prompt

> [ÜRÜN] için ikinci hayatlı ambalaj göster: kutu saklama kabına, kılıf alışveriş çantasına dönüşsün; dönüşüm ambalajın üzerinde şemayla anlatılsın. Dönüşmüş hâl de görselde olsun.

## English

> Show reusable second-life packaging for [PRODUCT]: the box becoming a storage container and the sleeve a shopping bag, with the transformation explained in a diagram on the pack. Include the transformed state in the visual.

## Neye dikkat edilmeli?

Dönüşüm gerçekten çalışsın; şemayla ürün çelişirse iddia çöker. İkinci hayat, birinci hayattan daha kullanışsız olmasın.

---

# 2775. `/peel-reveal` — Soyularak Açılan Etiket

## Türkçe prompt

> [ÜRÜN] için soyularak açılan (peel-to-reveal) etiket göster: üst katman yarı soyulmuş, altta gizli mesaj ya da ikinci dil bilgisi görünsün. Soyulma kenarı fiziksel olarak inandırıcı olsun.

## English

> Show a peel-to-reveal label for [PRODUCT]: the top layer half-peeled with a hidden message or second-language info beneath. Keep the peel edge physically convincing.

## Neye dikkat edilmeli?

Gizli katman gerçekten okunabilir olsun; bulanık vaat güven vermez. Yapışkan izi ve katman kalınlığı görünsün.

---

# 2776. `/local-craft` — Ürün × Yerel Zanaat

## Türkçe prompt

> [ÜRÜN]'ü [BÖLGE]'nin yerel zanaatıyla buluştur: ambalaj ya da ürün detayı o zanaatın tekniğiyle (seramik, dokuma, oyma) üretilmiş olsun. Zanaat süs değil, işlevin parçası olsun.

## English

> Marry [PRODUCT] with [REGION]'s local craft: packaging or product detail produced in that craft's technique (ceramics, weaving, carving). Make the craft part of the function, not decoration.

## Neye dikkat edilmeli?

Zanaat doğru temsil edilsin; motif ve teknik o bölgeye ait olsun. Kültürel öğe kostüm gibi kullanılmasın (§1570).

---

# 2777. `/blindbox-pack` — Sürpriz Kutu Ambalaj Sistemi

## Türkçe prompt

> [SERİ] için sürpriz kutu (blind-box) ambalaj sistemi tasarla: kapalı kutu, seri kartı ve gizli varyant oranıyla. Kutular aynı, içerik sürpriz olsun; seri kartı bütün varyantları göstersin.

## English

> Design a blind-box packaging system for [SERIES]: sealed box, series card, and hidden-variant ratio. Keep boxes identical with surprise contents, showing all variants on the series card.

## Neye dikkat edilmeli?

Kutu gerçekten ayırt edilemez olsun; ağırlık ve ses ipucu veren detaylar tutarlılığı bozar. Seri kartındaki varyantlar kutudakilerle eşleşsin.

---

# 2778. `/material-anatomy` — Ürün Malzeme Anatomisi

## Türkçe prompt

> [ÜRÜN]'ün malzeme anatomisini göster: dış kabuk yarı saydam ya da kesitli, iç katmanlar etiketli; her malzeme gerçek dokusuyla ayırt edilsin. Kesit görünümü mantığı kullanılsın (§5).

## English

> Show the material anatomy of [PRODUCT]: a half-transparent or sectioned outer shell with labeled inner layers, each material distinct in real texture. Use cutaway-view logic (§5).

## Neye dikkat edilmeli?

Katman sırası gerçek ürüne uysun; uydurma katman teknik incelemede hemen belli olur. Etiketler doğru katmana bağlı olsun.

---

# 2779. `/type-cover` — Tipografi Öncülüğünde Albüm Kapağı

## Türkçe prompt

> [SANATÇI] için tipografi öncülüğünde albüm kapağı tasarla: başlık dominant, görsel minimal destekte; font seçimi türü çağrıştırsın ama klişeye kaymasın. Kare format korunsun.

## English

> Design a type-led album cover for [ARTIST]: a dominant title with minimal visual support, with font choice evoking the genre without tipping into cliché. Keep the square format.

## Neye dikkat edilmeli?

Başlık harf harf denetlenir; kapak yazısındaki tek harf hatası affedilmez. Tür klişeleri filtresi uygulansın (§1054).

---

# 2780. `/found-photo` — Buluntu Fotoğraf Kapak

## Türkçe prompt

> [ALBÜM] için buluntu fotoğraf (found-photo) estetiğinde kapak tasarla: amatör kadraj, flaş patlaması ve dönem dokusu; fotoğraf “bulunmuş” hissi versin. Başlık minimal ve köşede olsun.

## English

> Design a found-photo aesthetic cover for [ALBUM]: amateur framing, flash blowout, and period texture, giving a “discovered” feel. Keep the title minimal in a corner.

## Neye dikkat edilmeli?

Buluntu hissi sahicilikten gelsin; yapay leke abartılırsa parodi olur. Başlık fotoğrafı kapatmasın.

---

# 2781. `/scan-cover` — Scanography Kapak

## Türkçe prompt

> [ALBÜM] için tarayıcıda düzenlenmiş (scanography) kapak tasarla: nesneler tarayıcı camında, derin alan netliği sığ, kenarlarda tarayıcı karanlığı. Kare format korunsun.

## English

> Design a scanography cover for [ALBUM]: objects arranged on scanner glass with shallow depth of field and scanner darkness at the edges. Keep the square format.

## Neye dikkat edilmeli?

Tarayıcı fiziği tutarlı olsun: cama değen yer net, kalkan yer flu. Toz ve tüy dozunda kalsın.

---

# 2782. `/music-ephemera` — Müzik Efemera Seti

## Türkçe prompt

> [SANATÇI / ALBÜM] için müzik efemera seti düzenle: bilet, backstage kartı, setlist ve rozet aynı tasarım sisteminde, tek yüzeyde. Parçalar aynı döneme ve turneye ait olsun.

## English

> Arrange a music ephemera set for [ARTIST / ALBUM]: ticket, backstage pass, setlist, and badge in one design system on a single surface. Keep all pieces from the same era and tour.

## Neye dikkat edilmeli?

Tarihler ve mekânlar birbiriyle tutarlı olsun. Bilet ve kartlar sahte-resmiyet izlenimi vermesin.

---

# 2783. `/map-graphic` — Harita Odaklı Grafik

## Türkçe prompt

> [KONU]'yu harita odaklı grafik olarak anlat: harita ana görsel, veri katmanları (renk, simge, çizgi) haritanın üzerinde; lejant ve kaynak notu zorunlu olsun. Harita projeksiyonu belirtilsin.

## English

> Tell [TOPIC] as a map-led graphic: the map as hero visual with data layers (color, symbols, lines) on top, plus a mandatory legend and source note. State the map projection.

## Neye dikkat edilmeli?

Veri-harital eşleşmesi doğrulanır; yanlış konumlandırılmış veri tüm grafiği çürütür. Kaynaksız harita kullanılmaz (§1830).

---

# 2784. `/contour-art` — Gerçek Eş Yükselti Sanatı

## Türkçe prompt

> [BÖLGE]'nin gerçek eş yükselti (kontur) çizgilerini sanat baskısına dönüştür: çizgi aralıkları gerçek topoğrafyayı korusun, renklendirme yükseltiye göre kademeli olsun. Bölge adı küçük yazıyla eklensin.

## English

> Turn the real contour lines of [REGION] into an art print: keep line intervals true to the topography with elevation-graded coloring. Add the region name in small type.

## Neye dikkat edilmeli?

Konturlar gerçek veriden türesin; dekoratif dalga çizgisi topoğrafya değildir. Yükselti yönü (vadi-tepe) tersine dönmesin.

---

# 2785. `/route-memory` — Güzergâh Anı Baskısı

## Türkçe prompt

> [YOLCULUK]'u güzergâh anı baskısı olarak göster: rota çizgisi, durak noktaları ve küçük tarih notlarıyla; baskı ev duvarına asılacak sadelikte olsun. Rota gerçek coğrafyayı izlesin.

## English

> Show [JOURNEY] as a route-memory print: a route line with stop dots and small date notes, simple enough to hang on a home wall. Follow real geography.

## Neye dikkat edilmeli?

Durak sırası ve tarihleri yolculukla eşleşsin. Rota çizgisi karadan denize sapmasın (güzergâh mantığı).

---

# 2786. `/year-routes` — Yıllık Rota Haritası

## Türkçe prompt

> [KİŞİ]'nin bir yıllık rotalarını tek haritada göster: her gezi farklı renk çizgiyle, çizgi kalınlığı kalış süresiyle orantılı, lejantta yıl ve toplam mesafe. Harita sade ve okunabilir olsun.

## English

> Show one year of [PERSON]'s routes on a single map: each trip in a different colored line with thickness proportional to stay length, plus year and total distance in the legend. Keep the map clean and legible.

## Neye dikkat edilmeli?

Renk-çizgi-lejant eşleşmesi birebir olsun. Çizgiler üst üste binerse opaklık düşürülsün, bilgi kaybolmasın.

---

# 2787. `/data-object` — Veriyi Fiziksel Nesneyle Anlat

## Türkçe prompt

> [VERİ]'yi fiziksel nesnelerle anlat: her veri noktası bir nesne (bardak, blok, bitki) olsun; nesne boyutu değeri temsil etsin. Ölçek efsanesi görselde olsun.

## English

> Tell [DATA] with physical objects: each data point as an object (glass, block, plant), with object size representing value. Include a scale key in the visual.

## Neye dikkat edilmeli?

Boyut-değer eşleşmesi doğrusal ve dürüst olsun; perspektif hilesiyle küçük değer büyük gösterilmesin. Veri kaynağı belirtilsin.

---

# 2788. `/object-count` — Tekrarlanan Nesne Verisi

## Türkçe prompt

> [VERİ]'yi tekrarlanan nesne görselleştirmesiyle göster: her simge sabit bir değeri temsil etsin (örn. 1 simge = 100 birim), kısmi değerler yarım simgeyle gösterilsin. Simgeler aynı ve hizalı olsun.

## English

> Show [DATA] as a repeated-object visual: each icon representing a fixed value (e.g., 1 icon = 100 units), with partial values as half icons. Keep icons identical and aligned.

## Neye dikkat edilmeli?

Simge-değer oranı sabit ve yazılı olsun; oran değişirse grafik yalan söyler. Yarım simgeler net okunsun.

---

# 2789. `/matched-pair` — Kilitli Kamera Önce / Sonra

## Türkçe prompt

> [DEĞİŞİM]'i kilitli kamerayla önce/sonra olarak göster: kamera konumu, açı, ışık ve kadraj iki karede birebir aynı; değişen yalnız incelenen öğe olsun. İki kare yan yana ve aynı boyutta sunulsun.

## English

> Show [CHANGE] as a locked-camera before/after: identical camera position, angle, lighting, and framing in both frames, varying only the studied element. Present both frames side by side at equal size.

## Neye dikkat edilmeli?

Kilitlenmeyen tek parametre sonucu kirletir; gölge yönüyle kamera sabitliği ayrıca doğrulanır (§23 mantığı).

---

# 2790. `/identity-grid` — Aynı Kişi Stil Grid'i

## Türkçe prompt

> Aynı [KİŞİ]'yi stil grid'inde göster: 6–9 hücrede farklı stil/ışık/kıyafet, yüz kimliği sabit. Hücre sayısı sabit, ızgara hizası kusursuz olsun.

## English

> Show the same [PERSON] in a style grid: different style, lighting, or clothing across 6–9 cells with fixed facial identity. Lock the cell count with perfect grid alignment.

## Neye dikkat edilmeli?

Kimlik bütün hücrelerde aynı kalsın (§1971); sapan hücre tek başına üretilsin. Stil değişimi kimliği sürüklemesin.

---

<a id="aile-136"></a>
# Pop-up Kâğıt Mühendisliği ve Şehir Tekstilleri — İndeks Kelimelerinin Tam Preset Karşılıkları

aile-006'daki kâğıt mühendisliği ve şehir tekstili kısayolları tur indekslerinde ad olarak geçiyor, bağımsız bölümleri yoktu. Aşağıdaki bölümler bu boşluğu kapatır. Ailenin iki kuralı burada da geçerlidir: pop-up mekanizması fiziksel olarak kapanabilir ve kesim-katlama-iz ilişkisi dürüst olsun; tekstilde baskı çözünürlüğü ve tekrar raporu (rapor) belirtilsin. Şehir skyline ve tek landmark pop-up kartlarının tam presetleri zaten §724–725'tedir; tunnel book tekniği §2668'dedir.

---

# 2715. `/accordion-city` — Akordeon Şehir Şeridi

## Türkçe prompt

> [ŞEHİR] silüetini akordeon katlamalı şerit olarak tasarla: 5–7 panel, her panelde bir landmark, katlandığında kitap ayracı boyutuna insin. Panel geçişleri kesintisiz sürsün, kat izleri landmarksız alanlara gelsin.

## English

> Design a [CITY] skyline as an accordion-folded strip: 5–7 panels with one landmark each, folding down to bookmark size. Keep the panorama continuous across panels, with fold lines falling on landmark-free areas.

## Neye dikkat edilmeli?

Panorama panel sınırlarında kırılmasın; model her paneli ayrı kart gibi üretmeye eğilimlidir. Katlanmış kalınlık gerçekçi olsun, 7 panel kâğıt destesi gibi dursun.

---

# 2716. `/box-card` — Katmanlı Kutu Kart

## Türkçe prompt

> [SAHNE]'yi açıldığında kutu gibi derinleşen box card olarak göster: ön çerçeve, 2–3 ara katman ve arka plan; katmanlar şeritlerle tutturulmuş hissi versin. Kart kapalıyken düz zarfa sığsın.

## English

> Show [SCENE] as a box card that gains box-like depth when opened: a front frame, 2–3 middle layers, and a backdrop, with layers feeling strip-attached. Keep the card flat-envelope-sized when closed.

## Neye dikkat edilmeli?

Derinlik katman aralığından gelsin; bulanık arka planla taklit edilmesin. Tutturma şeritleri görünür olsun, yoksa teknik okunmaz.

---

# 2717. `/tunnel-card` — Tünel Kart

## Türkçe prompt

> [SAHNE]'yi önden bakınca derinlik üreten tünel kart (tunnel card) olarak göster: delikli ön kapak, 3–4 iç katman ve arka kapak; katmanlar kartın yan duvarlarıyla bağlı olsun. Tunnel book'tan farkı tek kart formatında olmasıdır (§2668).

## English

> Show [SCENE] as a tunnel card producing depth when viewed head-on: a die-cut front cover, 3–4 inner layers, and a back cover, with layers joined by the card's side walls. Unlike a tunnel book (§2668), it stays a single-card format.

## Neye dikkat edilmeli?

Ön kapaktaki pencere ile iç katmanlar hizalı olsun; kayık pencere tekniği ele verir. Yan duvarlar görünür olsun, yoksa kartpostal sanılır.

---

# 2718. `/v-fold` — V-Katlamalı Pop-up

## Türkçe prompt

> [NESNE / BİNA]'yı kart açıldığında V-katlamasıyla yükselen pop-up olarak göster: simetrik V mekanizması, tek parça kesim ve kat izleri. Mekanizma kartın orta kat yerinden beslensin.

## English

> Show [OBJECT / BUILDING] as a pop-up rising on a V-fold when the card opens: a symmetric V mechanism, single-piece cutting, and visible score lines. Feed the mechanism from the card's center fold.

## Neye dikkat edilmeli?

V açısı iki tarafta eşit olsun; asimetrik V kartı yamuk kapatır. Nesne kapandığında kâğıtlar üst üste binmesin, yırtılma noktası oluşmasın.

---

# 2719. `/popup-map` — Açılır Turist Haritası

## Türkçe prompt

> [ŞEHİR] turist haritasını açılır pop-up öğeli harita olarak tasarla: katlanır harita tabanı üzerinde 3–5 yükselen landmark; simgeler numaralı, lejant köşede. Kapandığında standart katlanır harita boyutuna insin.

## English

> Design a [CITY] tourist map with pop-up elements: a folding map base with 3–5 rising landmarks, numbered icons, and a corner legend. Fold flat to standard folded-map size.

## Neye dikkat edilmeli?

Harita okunabilirliği pop-up'a feda edilmesin; yükselen öğeler sokak adlarını kapatmasın. Numara-lejant eşleşmesi birebir olsun.

---

# 2720. `/popup-guide` — Açılır Şehir Rehberi

## Türkçe prompt

> [ŞEHİR] için açılır öğeli mini şehir rehberi kapağı ve iç sayfa düzeni göster: kapakta tek pop-up vignette, içte katlanır mini harita. Kapak, iç sayfa ve harita aynı tasarım sisteminde olsun.

## English

> Show the cover and inside spread of a mini city guide for [CITY] with pop-up elements: one pop-up vignette on the cover and a fold-out mini map inside. Keep the cover, spread, and map in one design system.

## Neye dikkat edilmeli?

Üç parça aynı renk ve tipografi sisteminde olsun; biri dışarı taşarsa set dağılır. Pop-up vignette kapağı kapatmaya engel olmayacak incelikte dursun.

---

# 2721. `/postcard-model` — Kartpostaldan Makete

## Türkçe prompt

> [LANDMARK] kartpostalını kesilip kurulabilen kâğıt makete dönüştüren seti göster: önde basılı kartpostal, arkada kesim çizgili parçalar ve kurulmuş küçük maket yan yana. Kesim çizgileri ve kat izleri ayrı renklerle işaretli olsun.

## English

> Show a postcard-to-model set for [LANDMARK]: the printed postcard in front, cut-line parts behind, and the assembled small model beside them. Mark cut lines and score lines in distinct colors.

## Neye dikkat edilmeli?

Parçalar gerçekten birleşebilir görünsün; havada duran çıkıntılar tekniği ele verir. Kesim ve kat çizgisi renkleri birbirine karışmasın.

---

# 2722. `/paper-toy` — Yazdırılabilir Mimari Kâğıt Oyuncak

## Türkçe prompt

> [BİNA]'yı yazdırılabilir kâğıt oyuncak (paper toy) şablonu ve kurulmuş hâliyle göster: düz şablon yapıştırma kulakçıklarıyla, kurulmuş oyuncak kübik ve sevimli oranlarda. Şablon tek A4'e sığsın.

## English

> Show [BUILDING] as a printable paper-toy template plus the assembled result: a flat template with glue tabs and a assembled toy in cubic, charming proportions. Fit the template on a single A4 sheet.

## Neye dikkat edilmeli?

Kulakçıklar ve kesim çizgileri eksiksiz olsun; eksik kulakçık kurulamaz şablon demektir. Oranlar sevimli ama bina tanınır kalsın.

---

# 2723. `/paper-city` — Yazdırılabilir Kâğıt Şehir Seti

## Türkçe prompt

> [ŞEHİR]'in 4–6 landmarkından oluşan yazdırılabilir kâğıt şehir setini göster: şablon sayfası, kurulmuş binalar ve taban planı bir arada. Binalar aynı ölçekte olsun, taban planına otursun.

## English

> Show a printable paper-city set of 4–6 [CITY] landmarks: the template sheet, assembled buildings, and a base plan together. Keep all buildings at one scale, seated on the base plan.

## Neye dikkat edilmeli?

Ölçek birliği esastır; bir bina diğerlerinin iki katıysa set bozulur. Taban planındaki yerleşim gerçek şehir ilişkisini kabaca korusun.

---

# 2724. `/package-diorama` — Ambalajdan Şehre Diorama

## Türkçe prompt

> [ÜRÜN] ambalajını açıldığında şehir sahnesine dönüşen package diorama olarak göster: kutu kapakları sahne çerçevesine dönüşsün, içteki minyatür [ŞEHİR] öğeleri ambalaj baskısıyla aynı tasarımda olsun.

## English

> Show [PRODUCT] packaging as a package diorama turning into a city scene when opened: the box flaps become the scene frame, with miniature [CITY] elements inside in the same design as the packaging print.

## Neye dikkat edilmeli?

Ambalaj ve sahne aynı renk-tipografi sisteminde olsun; kopukluk hissi verirse iki ayrı iş gibi durur. Menteşe ve kapak hareketi fiziksel olarak mümkün görünsün.

---

# 2725. `/kirigami` — Mimari Kirigami

## Türkçe prompt

> [BİNA]'yı tek kâğıt yapraktan kesilip katlanan mimari kirigami olarak göster: simetrik kesim deseni, 90 derece açılan sayfa ve yükselen yapı. Kesim çizgileri ince ve kesintisiz olsun.

## English

> Show [BUILDING] as architectural kirigami cut and folded from a single sheet: a symmetric cut pattern, a 90-degree opening page, and the rising structure. Keep cut lines thin and continuous.

## Neye dikkat edilmeli?

Yapı tek yapraktan çıkmış hissi versin; sonradan yapıştırılmış parçalar kirigami değildir. Simetri bozulursa teknik okunmaz.

---

# 2726. `/origami` — Origami Dönüşüm

## Türkçe prompt

> [ÖZNE]'yi yalnızca katlamayla kurulmuş origami olarak göster: kat izleri görünsün, kesim ve yapıştırma olmasın. Kâğıt tek renk ya da iki yüzü farklı renkli olsun.

## English

> Show [SUBJECT] as origami built by folding only: show the crease lines, with no cutting or gluing. Use single-color paper or paper with two different-colored sides.

## Neye dikkat edilmeli?

Makas izi ve yapıştırma tekniği bozar; şüpheli birleşim yerleri kat iziyle açıklansın. Fazla detay katlama mantığını aşarsa sadeleştirilsin.

---

# 2727. `/shadowbox` — Gölge Kutusu Derinliği

## Türkçe prompt

> [SAHNE]'yi önden aydınlatmalı gölge kutusu (shadowbox) olarak göster: çerçeveli kutu, 3–5 aralıklı katman ve katman aralarında gerçek gölgeler. Işık önden ve tek kaynaktan gelsin.

## English

> Show [SCENE] as a front-lit shadowbox: a framed box with 3–5 spaced layers and real shadows between layers. Light it from the front with a single source.

## Neye dikkat edilmeli?

Gölgeler katman aralığını kanıtlasın; gölgesiz katman baskı gibi durur. Işık yönü bütün katmanlarda aynı olsun.

---

# 2728. `/pop-up-book` — Pop-up Kitap Açılımı

## Türkçe prompt

> [KONU] konulu pop-up kitabın açık çift sayfasını göster: orta kat yerinden yükselen ana sahne, yanlarda küçük çek-çevir kulakçıkları. Kitap cildi ve sayfa kalınlığı görünsün.

## English

> Show an open spread of a pop-up book on [TOPIC]: the main scene rising from the center fold with small pull-tabs on the sides. Show the book binding and page thickness.

## Neye dikkat edilmeli?

Ana sahne orta kat yerinden beslensin; sayfaya yapışmış gibi duran öğeler pop-up değildir. Kulakçıklar çalışır konumda ve yönlendirici olsun.

---

# 2729. `/skyline-tote` — Skyline Bez Çanta

## Türkçe prompt

> [ŞEHİR] silüetli bez çanta (tote bag) göster: tek renk baskı, silüet çantanın ön yüzüne ortalı, kulp dikişleri görünsün. Kumaş dokusu (kanvas) hissedilsin.

## English

> Show a canvas tote bag with a [CITY] skyline: single-color print centered on the front face, with visible handle stitching. Give a sense of canvas fabric texture.

## Neye dikkat edilmeli?

Baskı çanta kıvrımlarını takip etsin; dümdüz yapışmış gibi durmasın. Silüet tanınır landmarklar içersin, genel bina kalabalığı olmasın.

---

# 2730. `/coordinate-tote` — Koordinatlı Bez Çanta

## Türkçe prompt

> [ŞEHİR] koordinatlı bez çanta tasarla: enlem-boylam büyük tipografiyle, altında küçük şehir adı ve minik harita işareti. Tipografi baskı tekniğine uygun (serigrafi hissi) olsun.

## English

> Design a coordinate tote bag for [CITY]: large-type latitude and longitude with a small city name and tiny map marker below. Keep the typography print-appropriate with a screen-print feel.

## Neye dikkat edilmeli?

Koordinatlar gerçek şehre ait olsun; uydurma rakam güveni bitirir. Rakam ve harfler harf harf denetlenir.

---

# 2731. `/map-scarf` — Şehir Haritalı Fular

## Türkçe prompt

> [ŞEHİR] haritalı ipek fular göster: harita fulara taşmayacak şekilde yerleştirilmiş, kenar bordürü haritayla uyumlu desende, kumaş kıvrımları doğal. Renkler yumuşak ve giyilebilir olsun.

## English

> Show a silk scarf printed with a [CITY] map: the map placed to fit the scarf, an edge border in a matching pattern, and natural fabric folds. Keep colors soft and wearable.

## Neye dikkat edilmeli?

Harita okunabilir kalsın; kıvrımın yuttuğu sokak adları baskı hatası gibi durur. Renkler tenle uyumlu aralıkta tutulsun.

---

# 2732. `/skyline-scarf` — Skyline Fular

## Türkçe prompt

> [ŞEHİR] silüetli fular göster: silüet fuların bir kenarı boyunca şerit gibi aksın, geri kalan kumaş sade ve tamamlayıcı renkte olsun. Kumaş ipek parlaklığında dursun.

## English

> Show a scarf with a [CITY] skyline: the silhouette running like a band along one edge, with the rest of the fabric plain in a complementary color. Give the fabric a silk sheen.

## Neye dikkat edilmeli?

Silüet şeridi kesintisiz sürsün; kopan landmark dizimi baskı hatası sanılır. Sade alan gerçekten sade kalsın, desen taşmasın.

---

# 2733. `/map-bandana` — Haritalı Bandana

## Türkçe prompt

> [ŞEHİR] haritalı bandana göster: kare kumaş, ortada madalyon gibi harita motifi, köşelerde tamamlayıcı desen. Bandana katlanmış ve düz serilmiş iki hâliyle sunulsun.

## English

> Show a [CITY]-map bandana: square cloth with a medallion-like map motif in the center and complementary corner patterns. Present it both folded and laid flat.

## Neye dikkat edilmeli?

Katlanmış ve açık hâl aynı desene ait olsun. Merkez motifi kat izinde kaybolmayacak konumda olsun.

---

# 2734. `/city-towel` — Şehir Temalı Çay Havlusu

## Türkçe prompt

> [ŞEHİR] temalı çay havlusu (tea towel) göster: keten doku, tek ya da iki renk baskı, simgesel manzara ve küçük şehir adı. Havlu asılı ve katlı iki şekilde sunulsun.

## English

> Show a [CITY]-themed tea towel: linen texture, one- or two-color print, an iconic view, and a small city name. Present the towel both hanging and folded.

## Neye dikkat edilmeli?

Baskı havlu dokusuna işlenmiş gibi dursun; üzerine yapışmış çıkartma gibi durmasın. Yazı küçük tutulup denetlensin.

---

# 2735. `/city-handkerchief` — Hediyelik Mendil

## Türkçe prompt

> [ŞEHİR] hediyelik mendili göster: ince kumaş, kenar oya/overlok detayı, köşede küçük şehir illüstrasyonu. Mendil katlı kutusunda ve açık hâliyle sunulsun.

## English

> Show a [CITY] souvenir handkerchief: fine fabric with an edged-hem detail and a small city illustration in one corner. Present it both in its folded box and opened.

## Neye dikkat edilmeli?

Köşe illüstrasyonu küçük ve zarif kalsın; büyük baskı mendil değil bandana olur. Kutu ve mendil aynı tasarımda olsun.

---

# 2736. `/landmark-pattern` — Landmark Desenli Kumaş

## Türkçe prompt

> [LANDMARK] motifli tekrarlı kumaş deseni (repeat pattern) göster: motif raporu kusursuz birleşsin, iki renkli ve baskıya uygun sadeleşmiş olsun. Desen hem yakın detay hem rulo kumaş olarak sunulsun.

## English

> Show a repeating fabric pattern with a [LANDMARK] motif: a seamlessly joining repeat, simplified into two print-ready colors. Present both a close-up detail and the fabric roll.

## Neye dikkat edilmeli?

Rapor birleşimi kusursuz olsun; kayık tekrar baskı hatasıdır. Motif sadeleşmiş ama tanınır kalsın.

---

# 2737. `/local-pattern` — Yerel Hayat Deseni

## Türkçe prompt

> [ŞEHİR]'in günlük hayatından motiflerle tekrarlı desen tasarla: pazar, ulaşım, sokak satıcısı gibi öğeler sade ikonlara indirgenmiş olsun. Desen ev tekstilinde kullanılacakmış gibi sunulsun.

## English

> Design a repeating pattern from [CITY] everyday-life motifs: market, transport, and street-vendor elements reduced to simple icons. Present it as if for home textiles.

## Neye dikkat edilmeli?

Motifler klişeye kaymasın; her öğe gerçekten o şehre ait olsun. İkonlar tek çizgi dilinde tutarlı olsun.

---

# 2738. `/street-grid` — Sokak Izgarası Tekstili

## Türkçe prompt

> [ŞEHİR] sokak ızgarasını tekstil deseni olarak göster: gerçek cadde geometrisi sadeleştirilmiş, ızgara raporlu desene dönüşmüş, tek renk baskı. Hangi şehrin ızgarası olduğu hissedilsin.

## English

> Show a [CITY] street grid as a textile pattern: real street geometry simplified into a repeat grid pattern in single-color print. Keep the grid recognizable as that city.

## Neye dikkat edilmeli?

Izgara gerçek haritadan türesin; rastgele çizgi ağı şehir hissi vermez. Nehir ve ana aks gibi ayırt ediciler korunsun.

---

# 2739. `/skyline-socks` — Skyline Çorap Deseni

## Türkçe prompt

> [ŞEHİR] silüetli çorap çifti göster: silüet bilek bandında şerit olarak, geri kalan dokuma sade ve tamamlayıcı renkte. Örgü dokusu yakından hissedilsin.

## English

> Show a pair of socks with a [CITY] skyline: the silhouette as a band around the ankle, with the rest of the knit plain in a complementary color. Show the knit texture up close.

## Neye dikkat edilmeli?

Silüet küçük ölçekte okunsun; fazla detay çorapta çamura dönüşür. İki çorap eş olsun, motif konumu simetrik dursun.

---

# 2740. `/city-cap` — Şehir Nakışlı Kep

## Türkçe prompt

> [ŞEHİR] nakışlı kep (cap) göster: ön panelde küçük skyline ya da amblem nakışı, dikiş yönleri formu takip etsin. Kumaş ve nakış ipliği dokusu ayrı ayrı hissedilsin.

## English

> Show an embroidered city cap for [CITY]: a small skyline or emblem embroidery on the front panel, with stitch directions following the form. Render fabric and thread textures distinctly.

## Neye dikkat edilmeli?

Nakış küçük alanda okunsun; fazla detay iplik yığınına dönüşür. Yazı varsa harf harf denetlenir.

---

# 2741. `/patch-tote` — Yamalı Bez Çanta

## Türkçe prompt

> Yamalarla kişiselleştirilmiş [ŞEHİR] bez çantası göster: 4–6 nakış yama (landmark, arma, slogan) çantaya dikilmiş gibi dursun, dikiş izleri görünsün. Yamalar aynı geziye ait olsun.

## English

> Show a [CITY] tote personalized with patches: 4–6 embroidered patches (landmark, crest, slogan) looking sewn on, with visible stitching. Keep all patches from the same trip.

## Neye dikkat edilmeli?

Yamalar aynı dikiş ve nakış dilinde olsun; karışık stil kolajı dağınık durur. Yama yazıları ayrı ayrı denetlenir.

---

# 2742. `/ephemera-pack` — Şehir Efemera Paketi

## Türkçe prompt

> [ŞEHİR] efemera paketi göster: kartpostal, pul, etiket ve mini harita şeffaf paket içinde düzenli dizili. Paket arkası askılı (header card) hediyelik formatında olsun.

## English

> Show a [CITY] ephemera pack: a postcard, stamps, labels, and a mini map neatly arranged inside transparent packaging with a header-card gift format.

## Neye dikkat edilmeli?

Paket içi düzenli, dışı satışa hazır dursun; dağınık paket değer hissini düşürür. Parçalar aynı tasarım sisteminde olsun.

---

# 2743. `/keepsake-box` — Şehir Hatıra Kutusu

## Türkçe prompt

> [ŞEHİR] hatıra kutusu (keepsake box) göster: kapakta şehir illüstrasyonu, kutu açık hâliyle içinde mini efemera (bilet, pul, kartpostal) görünsün. Kutu ve içindekiler aynı tasarımda olsun.

## English

> Show a [CITY] keepsake box: a city illustration on the lid with mini ephemera (ticket, stamp, postcard) visible inside the open box. Keep the box and contents in one design.

## Neye dikkat edilmeli?

Kutu boyutu içindekilere uygun olsun; dev kutuda üç pul cılız durur. Kapak ve iç düzen aynı renk sisteminde olsun.

---

# 2744. `/landmark-box` — Landmark Formunda Ambalaj

## Türkçe prompt

> [LANDMARK] formunda hediyelik ambalaj kutusu tasarla: kutu kapalıyken yapıyı andırsın, açıldığında ürün yuvası ortaya çıksın. Yapı tanınır kalsın ama karikatüre kaymasın.

## English

> Design gift packaging shaped as [LANDMARK]: the closed box should evoke the structure, revealing the product nest when opened. Keep the structure recognizable without tipping into caricature.

## Neye dikkat edilmeli?

Açılma mekanizması fiziksel olsun; kutu açıldığında yapı dağılmasın. Ürün yuvası ürüne tam otursun.

---

# 2745. `/city-matchbox` — Şehir Temalı Kibrit Kutusu Ambalajı

## Türkçe prompt

> [ŞEHİR] temalı kibrit kutusu formatında mini ambalaj göster: sürgülü kutu, üstte şehir illüstrasyonu, iç çekmecede küçük hediye (rozet, pul). Sürgü mekanizması çalışır görünsün.

## English

> Show mini packaging in a matchbox format for [CITY]: a sliding box with a city illustration on top and a small gift (badge, stamp) in the inner drawer. Make the slide mechanism look functional.

## Neye dikkat edilmeli?

Sürgü payı gerçekçi olsun; sıkışmış ya da bol duran çekmece tekniği ele verir. Üst illüstrasyon ve iç hediye aynı temada olsun.

---

<a id="aile-138"></a>
# El İşi Malzeme Dönüşümleri — İndeks Kelimelerinin Tam Preset Karşılıkları

Craft-as-Process ailesindeki malzeme kısayolları indekslerde ad olarak geçiyor, bağımsız bölümleri yoktu. Aşağıdaki bölümler bu boşluğu kapatır. Ortak kural: malzeme yüze kaplanmaz, nesne o malzemeyle kurulmuş gibi durur; malzemenin fiziksel davranışı (dikiş, sır, lif, erime) görünür olur.

---

# 2791. `/amigurumi` — Amigurumi Figür

## Türkçe prompt

> [KARAKTER]'i sık iğne örgüyle kurulmuş amigurumi figüre dönüştür: ilmek dokusu yakından hissedilsin, dolgu formu yuvarlak ve sevimli olsun, gözler düğme ya da nakış. Kafa-gövde oranı sevimli ama karakter tanınır kalsın.

## English

> Turn [CHARACTER] into an amigurumi figure built from tight crochet stitches: show the stitch texture up close with a round, stuffed, charming form and button or embroidered eyes. Keep head-body proportions cute while staying recognizable.

## Neye dikkat edilmeli?

İlmek yönü formu takip etsin; rastgele doku örgü değil kaplamadır. Uzuvlar simetrik ve gövdeye sağlam bağlı görünsün.

---

# 2792. `/wax` — Bal Mumu Dönüşüm

## Türkçe prompt

> [NESNE]'yi bal mumu (wax) heykelciğe dönüştür: yarı saydam derinlik, parmak izi yumuşaklığı ve fitil gerektirmeyen bütün form. Yüzeyde erime izi ve damla dokusu dozunda olsun.

## English

> Turn [OBJECT] into a wax sculpture: translucent depth, finger-softened surfaces, and a solid form needing no wick. Keep melt marks and drip texture in moderation.

## Neye dikkat edilmeli?

Saydamlık abartılırsa nesne cam sanılır; mum hissi yüzey yumuşaklığından gelir. Keskin mühendislik kenarları muma uymaz, yumuşatılsın.

---

# 2793. `/ceramic-relief` — Seramik Rölyef

## Türkçe prompt

> [SAHNE]'yi seramik düşük rölyef (low-relief) pano olarak göster: kabartı derinliği 2–3 kademeli, sır (glaze) parlaklığı ve kil dokusu hissedilsin. Pano çerçeveli duvar objesi olarak sunulsun.

## English

> Show [SCENE] as a ceramic low-relief panel: relief depth in 2–3 steps with glaze sheen and clay texture. Present the panel as a framed wall object.

## Neye dikkat edilmeli?

Kabartı kademeleri okunsun; düz baskı gibi duruyorsa derinlik yetersizdir. Sır parlaklığı ışığı tek kaynaktan yansıtsın.

---

# 2794. `/mini-watercolor` — Minyatür Sulu Boya

## Türkçe prompt

> [SAHNE]'yi minyatür sulu boya olarak göster: küçük format (pul/kartvizit boyu hissi), boya akışları ve kâğıt dokusu görünsün. Detay az ama öz olsun.

## English

> Show [SCENE] as a miniature watercolor: a small-format feel (stamp or business-card size) with visible paint flows and paper texture. Keep detail minimal but essential.

## Neye dikkat edilmeli?

Küçük formatta fazla detay çamura dönüşür; üç ana leke kuralı uygulansın. Kâğıt beyazları nefes alma alanı olarak korunsun.

---

# 2795. `/cardboard-room` — Karton Mini Oda

## Türkçe prompt

> [ODA]'yı karton minyatür oda olarak göster: oluklu mukavva kenarları görünsün, mobilyalar katlama-kesim mantığıyla kurulsun. Ham karton rengi korunsun, boya minimal olsun.

## English

> Show [ROOM] as a cardboard miniature room: visible corrugated edges with furniture built in cut-and-fold logic. Preserve raw cardboard color with minimal paint.

## Neye dikkat edilmeli?

Mukavva kalınlığı tutarlı olsun; kâğıt inceliğinde duvar tekniği ele verir. Mobilya odaya oranlı olsun, devasa ya da cılız kalmasın.

---

# 2796. `/soft-object` — Kumaş Malzeme Dönüşümü

## Türkçe prompt

> [NESNE]'yi kumaştan kurulmuş yumuşak nesneye dönüştür: dikiş izleri, dolgu formu ve kumaş esnemesi görünsün. Sert mühendislik formu kumaş mantığına yumuşasın.

## English

> Turn [OBJECT] into a soft object built from fabric: show seams, stuffed form, and fabric stretch. Soften rigid engineered shapes into fabric logic.

## Neye dikkat edilmeli?

Dikiş yerleri gerilimi taşısın; dikişsiz kumaş nesne inandırıcı durmaz. Dolgu formu çökük ya da taşkın olmasın.

---

# 2797. `/inflatable` — Şişme Malzeme Dönüşümü

## Türkçe prompt

> [NESNE]'yi şişme (inflatable) forma dönüştür: hava basıncı yuvarlaklığı, dikiş birleşimleri ve supap detayı olsun. Malzeme vinil/PVC parlaklığında dursun.

## English

> Turn [OBJECT] into an inflatable form: air-pressure roundness with seam joints and a valve detail. Render the material in vinyl/PVC gloss.

## Neye dikkat edilmeli?

Şişkinlik formu tek basınç mantığına uysun; yer yer çökük yer yer gergin olmaz. Supap gizlenmesin, tekniğin kanıtıdır.

---

# 2798. `/reality-warp` — Tek Kontrollü Gerçeklik Kırılması

## Türkçe prompt

> [SAHNE]'de tek fiziksel kuralı bilinçli boz: yerçekimi, ölçek ya da yansıma — yalnız biri. Geri kalan her şey normal fizikle çalışsın. Kırılma noktasına izleyici gözü yönlensin.

## English

> Break exactly one physical rule in [SCENE] on purpose: gravity, scale, or reflection — only one. Keep everything else in normal physics. Direct the viewer's eye to the break point.

## Neye dikkat edilmeli?

Tek kırılma kuralı katıdır; iki kırılma tek fikri öldürür (§1564). Normal kalan kısım ne kadar sıradansa kırılma o kadar güçlü olur.

---

# 2799. `/scale-reversal` — Kontrollü Ölçek Tersine Çevirme

## Türkçe prompt

> [SAHNE]'de iki öğenin ölçeğini bilinçli tersine çevir: küçük olan dev, büyük olan minik olsun. Ölçek kanıtı (insan, kapı, el) sahnede kalsın; tersine çevirme açıkça okunsun.

## English

> Deliberately reverse the scale of two elements in [SCENE]: the small one giant, the large one tiny. Keep a scale cue (human, door, hand) in frame so the reversal reads clearly.

## Neye dikkat edilmeli?

Ölçek kanıtı olmadan tersine çevirme fark edilmez. Işık ve doku iki ölçeğe de uysun; dev nesne oyuncak gibi durmasın.

---

# 2800. `/cross-stitch` — Kaneviçe / Etamin

## Türkçe prompt

> [MOTİF]'i kaneviçe (cross-stitch) pano olarak göster: X dikişleri tek tek okunsun, kumaş delikleri (etamin) görünsün, renkler sınırlı iplik paletinde olsun. Kasnakta ya da çerçevede sunulsun.

## English

> Show [MOTIF] as a cross-stitch panel: individually readable X stitches on visible aida cloth with a limited thread palette. Present it in a hoop or frame.

## Neye dikkat edilmeli?

X yönü tutarlı olsun; karışık yön amatör değil, hatalı durur. Motif piksel mantığına uysun; fazla eğri dikişle anlatılmasın.

---

# 2801. `/embroidered-patch` — Nakış Yama

## Türkçe prompt

> [MOTİF]'i giysiye dikilir nakış yama (patch) olarak göster: merrow kenar bordürü, twill zemin ve nakış dokusu; yama ceket üstünde dikili sunulsun.

## English

> Show [MOTIF] as an embroidered patch ready to sew on clothing: a merrowed edge border, twill ground, and stitch texture, presented sewn onto a jacket.

## Neye dikkat edilmeli?

Bordür düzgün dönsün; kesik bordür tekniği ele verir. Yama boyutu giysiye oranlı olsun.

---

# 2802. `/enamel-pin` — Mine Rozet

## Türkçe prompt

> [MOTİF]'i mine (enamel) rozet olarak göster: metal konturlar, düz mine dolgular ve parlak yüzey; arka klips detayı da görünsün. Rozet avuçta ya da ceket yakasında sunulsun.

## English

> Show [MOTIF] as an enamel pin: metal outlines with flat enamel fills and a glossy surface, including the back clutch detail. Present the pin in a palm or on a jacket lapel.

## Neye dikkat edilmeli?

Mine taşmasın, konturlar kapalı olsun; taşan renk baskı izlenimi verir. Metal rengi (altın/gümüş/siyah nikel) tek olsun.

---

# 2803. `/clay-charm` — Kil Bagaj Süsü

## Türkçe prompt

> [MOTİF]'i el yapımı kil bagaj süsü (charm) olarak göster: parmak izi dokusu, minik halka aparatı ve sırlı/sırsız yüzey seçimi. Charm çantada asılı sunulsun.

## English

> Show [MOTIF] as a handmade clay bag charm: fingerprint texture with a small loop fitting and a glazed or unglazed finish. Present the charm hanging on a bag.

## Neye dikkat edilmeli?

Halka bağlantısı sağlam görünsün; havada duran charm inandırıcı olmaz. Boyut parmak ucuyla kıyaslanabilir olsun.

---

# 2804. `/clay-stop-motion` — Kil Stop-Motion Figür

## Türkçe prompt

> [KARAKTER]'i kil stop-motion figürü olarak göster: parmak izli kil yüzeyi, tel iskelet hissi veren duruş ve sette minik sahne aksesuarı. Kare-kare çekim dokusu sezilsin.

## English

> Show [CHARACTER] as a clay stop-motion figure: fingerprinted clay surface, an armature-suggesting pose, and a tiny set accessory. Suggest a frame-by-frame shooting texture.

## Neye dikkat edilmeli?

Yüzeyde alet izi dengeli olsun; fazla pürüzsüz kil, plastik sanılır. Figür ayakta durabilir görünsün, devriliyormuş hissi vermesin.

---

<a id="aile-139"></a>
# Kitap, Doğa, Ev ve Yiyecek Minikleri — İndeks Kelimelerinin Tam Preset Karşılıkları

Kitap-doğa-ev-yiyecek eksenindeki küçük format kısayolları indekslerde ad olarak geçiyor, bağımsız bölümleri yoktu. Ortak kural: küçük format küçük iddia demektir; minik nesne minik bağlamıyla (el, raf, cep, kutu) sunulur, devasa sahneye dönüştürülmez.

---

# 2805. `/book-charm` — Minyatür Kitap Süsü

## Türkçe prompt

> [KİTAP]'ı minyatür kitap süsü (book charm) olarak göster: açılabilir kapak, minik sayfalar ve zincir aparatı; kapak başlığı okunabilir olsun. Charm avuçta sunulsun.

## English

> Show [BOOK] as a miniature book charm: an openable cover, tiny pages, and a chain fitting, with a legible cover title. Present the charm in a palm.

## Neye dikkat edilmeli?

Başlık harf harf denetlenir; minik yazı bahanesiyle uydurma harf kabul edilmez. Sayfalar gerçekten katmanlı dursun, baskı blok gibi değil.

---

# 2806. `/ex-libris` — Kitap Sahiplik Mührü

## Türkçe prompt

> [KİŞİ] için ex-libris (kitap sahiplik mührü) tasarla: isim, küçük kişisel simge ve “ex libris” ibaresi tek renk gravür dilinde. Kitap iç kapağına yapışmış sunulsun.

## English

> Design an ex-libris bookplate for [PERSON]: name, a small personal symbol, and an “ex libris” inscription in single-color engraving language. Present it pasted inside a book cover.

## Neye dikkat edilmeli?

İsim ve ibare harf harf denetlenir. Simge gerçekten o kişiye ait olsun, hazır clip-art gibi durmasın.

---

# 2807. `/library-card` — Kütüphane Kartı Estetiği

## Türkçe prompt

> [KONU] için vintage kütüphane kartı estetiğinde görsel düzenle: karton kart, damga ve tarih kutuları, daktilo fontu hissi. Kart katalog çekmecesi bağlamında sunulsun.

## English

> Arrange a visual in vintage library-card aesthetics for [TOPIC]: a cardboard card with stamps and date boxes and a typewriter-font feel. Present the card in a catalog-drawer context.

## Neye dikkat edilmeli?

Tarih damgaları tutarlı olsun; gelecek tarihli vintage kart tekniği ele verir. Daktilo yazısı hizalı ve tek aralıktaki gibi dursun.

---

# 2808. `/reading-journal` — Okuma Günlüğü

## Türkçe prompt

> [KİTAP] için okuma günlüğü sayfası düzenle: kapak çizimi, yıldız puanı, kısa not ve alıntı kutusu el yazısı hissiyle. Sayfa kullanılmış defter gibi dursun.

## English

> Lay out a reading-journal page for [BOOK]: a cover sketch, star rating, short note, and quote box with a handwritten feel. Make the page feel like a used notebook.

## Neye dikkat edilmeli?

El yazısı ve alıntı harf harf denetlenir; yanlış alıntı güveni bitirir. Puan ile not çelişmesin.

---

# 2809. `/penpal` — Mektup Arkadaşı Seti

## Türkçe prompt

> Mektup arkadaşı (pen-pal) kırtasiye seti göster: desenli mektup kâğıdı, uyumlu zarf, pul ve sticker; set aynı desende, masada düzenli sunulsun.

## English

> Show a pen-pal stationery kit: patterned letter paper with a matching envelope, stamp, and stickers, all in one design, neatly presented on a table.

## Neye dikkat edilmeli?

Desen bütün parçalarda aynı olsun; parça başına farklı desen seti bozar. Zarf ve kâğıt ölçüleri birbirine uysun.

---

# 2810. `/zine` — DIY Fanzin

## Türkçe prompt

> [KONU] için DIY fanzin sayfa açılımı göster: fotokopi dokusu, kes-yapıştır başlıklar, el yazısı notlar ve bant izleri. Sayfa düzeni bilinçli dağınık olsun.

## English

> Show a DIY zine spread on [TOPIC]: photocopy texture, cut-and-paste headlines, handwritten notes, and tape marks. Keep the layout deliberately messy.

## Neye dikkat edilmeli?

Dağınıklık bilinçli sınırlansın: en fazla iki yazı tipi, bir vurgu rengi (§2088). Başlıklar okunabilir kalsın.

---

# 2811. `/riso-poster` — Risograph Poster

## Türkçe prompt

> [KONU] için iki spot renkli risograph poster tasarla: registration kayması, mürekkep dokusu ve sınırlı renk paleti; poster duvara asılı sunulsun.

## English

> Design a two-spot-color risograph poster on [TOPIC]: registration misalignment, ink texture, and a limited palette, presented hung on a wall.

## Neye dikkat edilmeli?

Kayma dozunda olsun; fazla kayma baskı hatası sanılır. Renkler üst üste bindiği yerde riso karışımı doğru hesaplanmış gibi dursun.

---

# 2812. `/indie-flyer` — Ham Fotokopi El İlanı

## Türkçe prompt

> [ETKİNLİK] için ham fotokopi el ilanı (flyer) tasarla: yüksek kontrast, kesik başlık, koparılabilir telefon şeritleri ve fotokopi lekeleri. İlan direğe asılı sunulsun.

## English

> Design a raw photocopy flyer for [EVENT]: high contrast, a cut headline, tear-off phone strips, and copier marks. Present the flyer posted on a pole.

## Neye dikkat edilmeli?

Tarih, saat ve yer bilgileri tutarlı ve okunabilir olsun. Koparılabilir şeritler gerçekten yırtılabilir dursun.

---

# 2813. `/raw-marker` — El Marker Tipografisi

## Türkçe prompt

> [KELİME / SLOGAN]'ı el marker kalemiyle yazılmış tipografi olarak göster: mürekkep akışları, çift katman vurgular ve kâğıt dokusu. Yazı posterin öznesi olsun.

## English

> Show [WORD / SLOGAN] as hand-marker typography: ink flows, double-stroke emphasis, and paper texture. Make the lettering the subject of the poster.

## Neye dikkat edilmeli?

Harfler dengeli ve okunabilir olsun; Türkçe karakterler (ğ, ş, ı, ç) eksiksiz yazılsın. Mürekkep akışı dozunda kalsın.

---

# 2814. `/editorial-collage` — Gazete + Analog Kolaj

## Türkçe prompt

> [KONU] için gazete kupürleri ve analog öğelerle editorial kolaj yap: başlıklar, fotoğraf parçaları ve bant izleri tek kompozisyonda; kolajın tek fikri olsun.

## English

> Build an editorial collage for [TOPIC] from newspaper clippings and analog elements: headlines, photo fragments, and tape marks in one composition with a single idea.

## Neye dikkat edilmeli?

Kupür yazıları konu dışına sapmasın; rastgele gazete metni kolajı dedikoduya çevirir. Katmanlar okunabilirlik sırasına göre dizilsin.

---

# 2815. `/browser-collage` — Retro Tarayıcı Penceresi Kolajı

## Türkçe prompt

> [KONU]'yu retro tarayıcı pencereleri kolajı olarak göster: 2000'ler başı arayüz öğeleri, üst üste pencereler ve piksel font başlıklar. Dönem arayüz dili tutarlı olsun.

## English

> Show [TOPIC] as a retro browser-window collage: early-2000s interface elements with overlapping windows and pixel-font headlines. Keep the period interface language consistent.

## Neye dikkat edilmeli?

Arayüz öğeleri tek döneme ait olsun; modern ikon sızması tekniği ele verir. Pencereler okunabilirlik sırasına göre dizilsin.

---

# 2816. `/spreadsheet` — Yaratıcı Tablo Estetiği

## Türkçe prompt

> [KONU]'yu yaratıcı tablo (spreadsheet) estetiğinde göster: hücre ızgarası, renkli satırlar ve mini grafikler; tablo sanat nesnesi gibi dursun ama verisi okunabilir olsun.

## English

> Show [TOPIC] in a creative spreadsheet aesthetic: cell grids with colored rows and mini charts, composed like an art object while keeping the data legible.

## Neye dikkat edilmeli?

Hücre verileri tutarlı olsun; uydurma rakam sanat kisvesiyle de yanlıştır. Izgara hizası kusursuz olsun.

---

# 2817. `/herbarium` — Herbaryum Yaprağı

## Türkçe prompt

> [BİTKİ] için herbaryum yaprağı düzenle: preslenmiş bitki, etiket (tür adı, tarih, yer) ve arşiv kartonu. Bitki bilimsel olarak tanınır olsun.

## English

> Arrange a herbarium sheet for [PLANT]: a pressed plant with a label (species name, date, place) on archival board. Keep the plant scientifically recognizable.

## Neye dikkat edilmeli?

Tür adı ve bitki eşleşsin; yanlış etiket bilimsel güveni bitirir. Latince ad italik ve eksiksiz yazılsın.

---

# 2818. `/nature-journal` — Doğa Günlüğü Açılımı

## Türkçe prompt

> [GÖZLEM] için doğa günlüğü açılımı düzenle: eskiz, tarih-hava notu, renk örnekleri ve kısa gözlem cümlesi el yazısı hissiyle. Sayfa sahada kullanılmış gibi dursun.

## English

> Lay out a nature-journal spread for [OBSERVATION]: a sketch with date-weather notes, color swatches, and a short observation sentence in a handwritten feel. Make the page feel field-used.

## Neye dikkat edilmeli?

Gözlem cümlesi eskizle çelişmesin. Tarih ve mevsim bitkinin hâline uysun.

---

# 2819. `/seed-packet` — Vintage Tohum Paketi

## Türkçe prompt

> [BİTKİ] için vintage tohum paketi tasarla: bitki illüstrasyonu, ekim bilgileri (derinlik, mevsim) ve paket arkası talimat. Bilgiler gerçek bahçeciliğe uygun olsun.

## English

> Design a vintage seed packet for [PLANT]: a botanical illustration with sowing info (depth, season) and back-panel instructions. Keep the information horticulturally sound.

## Neye dikkat edilmeli?

Ekim bilgileri uydurulmasın; yanlış mevsim gerçek zarara yol açar. İllüstrasyon doğru türü göstersin.

---

# 2820. `/terrarium` — Gerçekçi Mini Teraryum

## Türkçe prompt

> Gerçekçi mini teraryum göster: cam kap, toprak katmanları, yosun ve minik bitkiler; nem damlacıkları camda hissedilsin. Ekosistem kendi içinde tutarlı olsun.

## English

> Show a realistic mini terrarium: a glass vessel with soil layers, moss, and tiny plants, with condensation felt on the glass. Keep the ecosystem internally consistent.

## Neye dikkat edilmeli?

Bitkiler aynı nem isteğine sahip olsun; çöl kaktüsüyle yosun aynı kapta olmaz. Cam yansıması içeriği kapatmasın.

---

# 2821. `/tiny-food` — Gerçekçi Minyatür Yemek

## Türkçe prompt

> Gerçekçi minyatür yemek göster: tabak, çatal ve porsiyon 1:12 ölçeğinde; yemek dokusu yakından inandırıcı olsun. Ölçek kanıtı (madeni para, el) sahnede olsun.

## English

> Show realistic miniature food: plate, fork, and portion at 1:12 scale with convincing close-up food texture. Include a scale cue (coin, hand) in frame.

## Neye dikkat edilmeli?

Ölçek kanıtı olmadan minyatür okunmaz. Yemek dokusu yakında plastik gibi durmasın.

---

# 2822. `/greenhouse-mini` — Minyatür Sera Dioraması

## Türkçe prompt

> Minyatür sera dioraması göster: cam paneller, içte sıralı saksılar ve sulama detayı; ışık camdan süzülmüş gibi olsun. Sera ölçeği insan eliyle kıyaslanabilir olsun.

## English

> Show a miniature greenhouse diorama: glass panels with rows of pots and a watering detail inside, with light filtering through glass. Keep the greenhouse scale comparable to a human hand.

## Neye dikkat edilmeli?

Cam yansımaları iç düzeni kapatmasın. Bitkiler aynı ışık isteğine sahip olsun.

---

# 2823. `/food-layers` — Yemek Katman Anatomisi

## Türkçe prompt

> [YEMEK]'in katman anatomisini göster: burger/sandviç/lazanya katmanları patlatılmış görünümde ayrılmış ama sırası okunur olsun. Her katman etiketli olsun.

## English

> Show the layer anatomy of [DISH]: burger, sandwich, or lasagna layers separated in exploded view while keeping the order readable. Label each layer.

## Neye dikkat edilmeli?

Katman sırası gerçek tarife uysun; sos alta inerse anatomi bozulur (§4 mantığı). Malzemeler taze ve iştah açıcı dursun.

---

# 2824. `/food-macro` — Aşırı Dokunsal Yemek Makro

## Türkçe prompt

> [YEMEK]'i aşırı dokunsal makro fotoğraf olarak göster: buhar, damla ve lif dokusu aşırı yakın planda; alan derinliği sığ. İştah hissi dokudan gelsin.

## English

> Show [DISH] as a hyper-tactile macro photograph: steam, droplets, and fiber texture in extreme close-up with shallow depth of field. Let appetite come from texture.

## Neye dikkat edilmeli?

Buhar ve damla taze pişmiş hissi versin; bayat yemek makroda affedilmez. Odak, yemeğin en ayırt edici dokusunda olsun.

---

# 2825. `/giant-food` — Tek Dev Yemek Ölçek Kayması

## Türkçe prompt

> [YEMEK]'i tek dev ölçek kaymasıyla göster: normal sahnede tek devasa yemek öğesi; insan figürleri şaşkınlık değil, doğal etkileşimde olsun. Ölçek farkı hemen okunsun.

## English

> Show [DISH] with a single giant-food scale shift: one gigantic food item in a normal scene, with human figures interacting naturally rather than amazed. Make the scale gap read instantly.

## Neye dikkat edilmeli?

Dev öğenin gölgesi ve dokusu sahneye uysun; yüzen dev yemek kolaj gibi durur. Tek kayma kuralı korunsun.

---

# 2826. `/coffee-flight` — Kahve Tadım Uçuşu

## Türkçe prompt

> Kahve tadım uçuşu (coffee flight) göster: 3–4 küçük bardak ahşap sunumda, her birinde farklı kahve tonu; yanında tadım notu kartı. Düzen simetrik ve temiz olsun.

## English

> Show a coffee tasting flight: 3–4 small cups on a wooden presenter with distinct coffee tones in each, plus a tasting-note card. Keep the arrangement symmetric and clean.

## Neye dikkat edilmeli?

Kahve tonları birbirinden ayrılsın; hepsi aynı renkse tadım anlamsızlaşır. Not kartındaki yazılar denetlenir.

---

# 2827. `/home-cafe` — Ev Kafe Köşesi

## Türkçe prompt

> Ev kafe köşesi (home café station) tasarla: kahve ekipmanları, raf düzeni ve menü panosu küçük alanda; köşe gerçekten kullanılabilir görünsün. Işık sıcak olsun.

## English

> Design a home café station: coffee gear with shelf order and a menu board in a small footprint, looking genuinely usable. Keep the light warm.

## Neye dikkat edilmeli?

Ekipman dizimi iş akışına uysun; kullanılamaz düzen dekor olarak kalır. Menü yazısı harf harf denetlenir.

---

<a id="aile-140"></a>
# Oyun, Kimlik ve Sistem Presetleri — İndeks Kelimelerinin Tam Preset Karşılıkları

Oyuncak, kimlik-dizim ve sistem-açıklama eksenindeki kısayollar indeks ve listelerde ad olarak geçiyor, bağımsız bölümleri yoktu. Ortak kural: oyun nesnesi oynanabilir, kimlik dizimi sayılabilir, sistem şeması izlenebilir olsun.

---

# 2828. `/gashapon` — Kapsül Makine Oyuncağı

## Türkçe prompt

> [SERİ] için kapsül makine (gashapon) oyuncağı göster: şeffaf kapsülde minik figür, yanında kapsül makinesi ve seri kartı. Kapsül ve figür ölçekli olsun.

## English

> Show a capsule-machine (gashapon) toy for [SERIES]: a tiny figure in a transparent capsule beside the capsule machine and series card. Keep capsule and figure in scale.

## Neye dikkat edilmeli?

Figür kapsüle gerçekten sığsın; sığmayan figür tekniği ele verir. Seri kartındaki varyantlar makinedekilerle eşleşsin.

---

# 2829. `/chibi-vinyl-toy` — Büyük Başlı Vinyl Figür

## Türkçe prompt

> [KARAKTER]'i büyük başlı (chibi) vinyl figür olarak göster: parlak vinyl yüzey, sade boya sınırları ve kutulu sunum. Kafa-gövde oranı sevimli ama karakter tanınır kalsın.

## English

> Show [CHARACTER] as a big-headed (chibi) vinyl figure: a glossy vinyl surface with clean paint boundaries, presented boxed. Keep head-body proportions cute while staying recognizable.

## Neye dikkat edilmeli?

Boya sınırları taşmasın; taşan boya kalite izlenimini bitirir. Kutu ve figür aynı tasarımda olsun.

---

# 2830. `/ceramic-bust` — Seramik Büst

## Türkçe prompt

> [KİŞİ]'yi seramik büst olarak göster: sır yüzey, kaide ve müze etiketiyle; ifade nötr ve zamansız olsun. Büst rafta, galeri ışığında sunulsun.

## English

> Show [PERSON] as a ceramic bust: a glazed surface with a plinth and museum label, keeping the expression neutral and timeless. Present the bust on a shelf in gallery light.

## Neye dikkat edilmeli?

Yüz benzerliği abartıdan değil, orandan gelsin; karikatür büst ciddiyeti bitirir. Etiket yazısı denetlenir.

---

# 2831. `/doll-box` — Figürin Paket Kutusu Yapısı

## Türkçe prompt

> Koleksiyon figürü paket kutusunun yapısını göster: pencere, blister yuva ve figür kutu içinde; kutu grafikleri figürle aynı tasarımda olsun. Kutu hem kapalı hem figür dışarıda iki hâliyle sunulsun.

## English

> Show the structure of a collectible figure's packaging: window, blister nest, and figure inside, with box graphics matching the figure's design. Present both the closed box and the figure outside it.

## Neye dikkat edilmeli?

Blister yuva figüre tam otursun; bol yuva ucuz izlenimi verir. Pencere figürün yüzünü kapatmasın.

---

# 2832. `/night-scene` — Gece Sahnesi Dönüşümü

## Türkçe prompt

> Gündüz [SAHNE]'yi gece sahnesine çevir: yapay ışıklar (sokak lambası, vitrin, pencere) tek tek yansın; gökyüzü lacivert, gölgeler derin olsun. Işık mantığı tek sahneye uysun.

## English

> Turn a daytime [SCENE] into a night scene: switch on artificial lights (street lamps, shop windows, lit windows) one by one, with a navy sky and deep shadows. Keep the lighting logic to one scene.

## Neye dikkat edilmeli?

Yanan ve sönük ışıklar tutarlı olsun; gündüz gölgesi gece sahnesinde kalmasın. Işık renkleri (sodyum turuncusu, LED beyazı) karışıksa bilinçli olsun.

---

# 2833. `/bag-charms` — Çanta Süsü Koleksiyonu

## Türkçe prompt

> Kişisel çanta süsü (bag charm) koleksiyonu göster: 4–6 charm tek çantada asılı, her biri farklı anıyı temsil etsin; bağlantı halkaları görünsün. Koleksiyon aynı kişinin zevkini yansıtsın.

## English

> Show a personal bag-charm collection: 4–6 charms on one bag, each marking a different memory, with connector rings visible. Reflect one person's taste across the collection.

## Neye dikkat edilmeli?

Charm'lar aynı malzeme dilinde olmasa da aynı özen düzeyinde olsun. Bağlantılar sağlam görünsün.

---

# 2834. `/journal-charms` — Günlük Süsü Koleksiyonu

## Türkçe prompt

> Günlük (journal) süsü koleksiyonu göster: defter spirali ve kapağında 3–5 charm, ataş ve kurdele detaylarıyla. Defter kullanılır, süsler anlamlı olsun.

## English

> Show a journal-charm collection: 3–5 charms on a notebook's spiral and cover with clip and ribbon details. Keep the notebook used and the charms meaningful.

## Neye dikkat edilmeli?

Süsler defterin kullanımını engellemesin; yazı alanını kapatan charm işlevi bitirir. Bağlantılar sayfayı yırtmayacak gibi dursun.

---

# 2835. `/map-sleeve` — Haritalı Kılıf Ambalaj

## Türkçe prompt

> [ŞEHİR] haritalı kılıf (sleeve) ambalaj tasarla: ürün kutusu üzerinde kayan harita baskılı kılıf; kılıf yarı sıyrılmış hâliyle de gösterilsin. Harita ve ürün aynı temada olsun.

## English

> Design a map-printed sleeve packaging for [CITY]: a sliding map sleeve over the product box, also shown half-slipped. Keep map and product in one theme.

## Neye dikkat edilmeli?

Kılıf kutuya tam otursun; bol kılıf ucuz durur. Harita baskısı kılıf kenarında kesilmesin, kompozisyon bütün kalsın.

---

# 2836. `/ar-postcard` — AR Destekli Şehir Kartpostalı

## Türkçe prompt

> AR destekli şehir kartpostalı göster: fiziksel kartpostal önde, üstünde telefon ekranında beliren 3B landmark katmanı; ekranda “tarat” işareti olsun. Fiziksel ve dijital katman aynı tasarımda olsun.

## English

> Show an AR-enhanced city postcard: the physical postcard in front with a 3D landmark layer appearing on a phone screen above it, including a “scan” cue on screen. Keep physical and digital layers in one design.

## Neye dikkat edilmeli?

AR katmanı kartpostala hizalı olsun; kayık katman teknolojiyi değil hatayı gösterir. AR'sız hâl tek başına da anlamlı dursun.

---

# 2837. `/photo-booth-strip` — Fotoğraf Kabini Şeridi

## Türkçe prompt

> Klasik fotoğraf kabini şeridi göster: dikey 3–4 kare, siyah-beyaz ya da sepya, kareler arası aynı kişi farklı ifadelerle. Şerit hafif parlak fotoğraf kâğıdında sunulsun.

## English

> Show a classic photo-booth strip: a vertical run of 3–4 black-and-white or sepia frames with the same person in different expressions. Present the strip on slightly glossy photo paper.

## Neye dikkat edilmeli?

Kişi bütün karelerde aynı kalsın; kabin flaşı ve fon sabit olsun. Kare sırası doğal ifade akışını izlesin.

---

# 2838. `/vintage-poster` — Vintage Poster

## Türkçe prompt

> [KONU] için vintage poster tasarla: dönem tipografisi, sınırlı renk paleti ve eskitilmiş kâğıt dokusu; poster duvara asılı sunulsun. Dönem tek onyıla ait olsun.

## English

> Design a vintage poster on [TOPIC]: period typography with a limited palette and aged paper texture, presented hung on a wall. Keep the period to a single decade.

## Neye dikkat edilmeli?

Tipografi ve görsel aynı döneme ait olsun; karışık dönem kolajı tekniği ele verir. Eskitme dozunda kalsın, yırtık posteri okunmaz kılmasın.

---

# 2839. `/identity-flatlay` — Kimlik Üstten Düzenlemesi

## Türkçe prompt

> [KİŞİ]'nin kimliğini üstten düzenleme (flat lay) ile anlat: cüzdan, anahtar, gözlük, kitap ve 2–3 kişisel nesne düzenli dizili; düzenleme o kişiye özgü olsun. Zemin sade ve tek renk olsun.

## English

> Tell [PERSON]'s identity with a flat lay: wallet, keys, glasses, a book, and 2–3 personal objects neatly arranged, specific to that person. Keep the background plain and single-colored.

## Neye dikkat edilmeli?

Nesneler gerçekten o kişiye ait olsun; katalog doldurması kimliği değil vitrini anlatır. Kartvizit gibi yazılı nesneler denetlenir.

---

# 2840. `/toolkit-flatlay` — Alet Seti Üstten Düzenlemesi

## Türkçe prompt

> [MESLEK / HOBİ] için alet seti üstten düzenlemesi göster: aletler iş akışı sırasına dizili, her alet temiz ve tanınır; zemin koyu ve kontrastlı olsun.

## English

> Show a toolkit flat lay for [PROFESSION / HOBBY]: tools arranged in workflow order, each clean and recognizable, on a dark contrasting ground.

## Neye dikkat edilmeli?

Sıralama gerçek iş akışını izlesin; rastgele diziş öğreticiliği bitirir. Eksik kritik alet hemen fark edilir, liste baştan kontrol edilsin.

---

# 2841. `/what-on-my-desk` — Masamda Ne Var

## Türkçe prompt

> [KİŞİ]'nin masasını üstten göster: monitör/klavye düzeni, defter, içecek ve kişisel nesneler doğal dağınıklıkta; masa gerçekten çalışılan bir masa gibi dursun.

## English

> Show [PERSON]'s desk from above: monitor and keyboard layout with a notebook, drink, and personal objects in natural disarray, reading as a genuinely worked-at desk.

## Neye dikkat edilmeli?

Ekrandaki içerik okunabilir ve işe ait olsun; uydurma ekran görüntüsü güveni bitirir. Dağınıklık doğal sınırlarda kalsın.

---

# 2842. `/pixel-sheet` — Piksel Sticker Sayfası

## Türkçe prompt

> Piksel art sticker sayfası tasarla: 8–12 piksel ikon aynı ızgarada, her ikon aynı piksel boyutunda; sayfa çıkartma kâğıdında sunulsun.

## English

> Design a pixel-art sticker sheet: 8–12 pixel icons on one grid with identical pixel dimensions, presented on sticker paper.

## Neye dikkat edilmeli?

Piksel boyutu bütün ikonlarda aynı olsun; karışık çözünürlük amatör durur. İkonlar tek renk paletinde tutarlı olsun.

---

# 2843. `/process-breakdown` — Zaman / Adım Çözümlemesi

## Türkçe prompt

> [ÜRETİM]'i zaman-adım çözümlemesi olarak göster: aşamalar sırayla, her aşamada girdi-çıktı ve süre bilgisi; akış tek yönde okunsun. Süreç diyagramı mantığı kullanılsın (§20).

## English

> Show [PRODUCTION] as a time-step breakdown: stages in order with input-output and duration at each stage, reading in one direction. Use process-diagram logic (§20).

## Neye dikkat edilmeli?

Süre ve sıra gerçek üretimle uyuşsun; uydurma süre planlamayı çürütür. Karar noktası varsa akış şemasına geçilsin (§21).

---

# 2844. `/system-breakdown` — İşlevsel Alt Sistem Çözümlemesi

## Türkçe prompt

> [MAKİNE / AĞ]'ı işlevsel alt sistemlere ayırarak göster: her alt sistem kutulu, bağlantılar etiketli oklarla; kutular işleve göre renklensin. Şematik dil kullanılsın (§49).

## English

> Show [MACHINE / NETWORK] divided into functional subsystems: boxed subsystems with labeled-arrow connections, colored by function. Use schematic language (§49).

## Neye dikkat edilmeli?

Bağlantı yönleri gerçek veri/enerji akışını izlesin; ters ok tüm anlamı bozar (§21 mantığı). Kutu sayısı arttıkça her bağlantı ayrı denetlensin.

---

# 2845. `/progressive-disclosure` — Aşamalı Açma

## Türkçe prompt

> [BİLGİ]'yi aşamalı açma (progressive disclosure) ile göster: ilk karede sade özet, sonraki karelerde detay katmanları; her adım tek fikir taşısın. Adımlar numaralı olsun.

## English

> Show [INFORMATION] with progressive disclosure: a plain summary in the first frame with detail layers in following frames, one idea per step. Number the steps.

## Neye dikkat edilmeli?

Her adım öncekiyle çelişmesin; detay özeti yalanlarsa güven biter. Adım sayısı ihtiyaca göre sınırlansın.

---

# 2846. `/scientific-cover-process` — Bilimsel Kapak Süreç Panosu

## Türkçe prompt

> [ARAŞTIRMA] için bilimsel kapak süreç panosu hazırla: eskiz, baskı tekniği denemeleri (serigrafi, siyanotip, gofre) ve final kapak yan yana; süreç okunabilir olsun.

## English

> Build a scientific-cover process board for [RESEARCH]: sketch, print-technique trials (screenprint, cyanotype, embossing), and the final cover side by side, with a legible process.

## Neye dikkat edilmeli?

Denemeler gerçekten denenmiş gibi dursun; süs niyetine konmuş baskı örneği süreci değil vitrini anlatır. Final kapak denemelerden türesin.

---

<a id="aile-141"></a>
# Ders Konu Galerileri — Fen Bilimleri ve Matematik

Bu aile, rehberin eğitim misyonunu konuya indirir: her bölüm bir ders kazanımına hazır prompt verir. Biçim seçimi §3 tablosuna, doğrulama §18 listesine dayanır. Her bölümde seviye (ilkokul / ortaokul) belirtilir; seviye değişince yalnız dil değil, gösterim biçimi de sadeleşir.

---

# 2847. `/cell-compare` — Fen: Bitki ve Hayvan Hücresi Karşılaştırma (Ortaokul)

## Seviye

Ortaokul 7. sınıf — Hücre ve Bölünmeler ünitesi.

## Türkçe prompt

> Bitki ve hayvan hücresini eğitim amaçlı yan yana karşılaştır. İki hücrede de hücre zarı, sitoplazma, çekirdek ve mitokondri aynı renk ve çizim diliyle gösterilsin; hücre duvarı, kloroplast ve koful yalnız bitki hücresinde olsun. Ortak yapılar ortada küçük ortak alanda buluşsun. Türkçe etiketler kullan. Ders kitabı illüstrasyonu olsun, 3B render parlaklığı kullanma.

## English

> Compare plant and animal cells side by side for education. Render the cell membrane, cytoplasm, nucleus, and mitochondria in both cells with the same colors and drawing language, showing the cell wall, chloroplasts, and vacuole only in the plant cell. Join shared structures in a small common area in the middle. Use Turkish labels and a textbook illustration style without 3D render gloss.

## Neye dikkat edilmeli?

Organel adları ve hücreye özgü yapılar ders kitabıyla birebir karşılaştırılır; model kloroplastı hayvan hücresine koymaya eğilimlidir. İki taraf aynı ölçekte olmalı, bitki hücresi devasa görünmemeli.

---

# 2848. `/circuit-pair` — Fen: Seri ve Paralel Devre (Ortaokul)

## Seviye

Ortaokul 7. sınıf — Elektrik Devreleri ünitesi.

## Türkçe prompt

> Seri ve paralel bağlı iki basit elektrik devresini yan yana şematik gösterimle karşılaştır. Her iki devrede de pil, anahtar ve iki ampul standart devre sembolleriyle çizilsin; seri devrede ampullerin sönük, paralel devrede parlak yandığı küçük parlaklık farkıyla anlatılsın. Akım yönü oklarla gösterilsin. Türkçe etiketler kullan.

## English

> Compare two simple circuits, series and parallel, side by side as schematic diagrams. Draw the battery, switch, and two bulbs with standard circuit symbols in both, suggesting dimmer bulbs in series and brighter bulbs in parallel through a small brightness cue. Show current direction with arrows and use Turkish labels.

## Neye dikkat edilmeli?

Semboller standart olsun; gerçekçi pil fotoğrafı şemayı bozar. Parlaklık farkı abartılırsa “paralel daha iyi” gibi yanlış genelleme doğar; öğretmen farkın nedenini sözlü tamamlar.

---

# 2849. `/friction-strip` — Fen: Sürtünme Kuvveti Deneyi (İlkokul–Ortaokul)

## Türkçe prompt

> Sürtünme kuvvetini gösteren basit deneyi üç kareli sıralı şerit olarak göster: tahta blok halıda, tahta blok fayans zeminde ve tekerlekli blok aynı eğik düzlemde. Her karede okla hareket yönü ve sürtünme yönü ters oklarla belirtilsin. İlkokul düzeyinde sade çizim olsun.

## English

> Show a simple friction experiment as a three-frame sequence strip: a wooden block on carpet, the same block on tile, and a wheeled block on the same ramp. Mark motion and opposing friction with arrows in each frame, in a simple primary-school drawing style.

## Neye dikkat edilmeli?

Ok yönleri fizikle uyuşsun: sürtünme her zaman harekete terstir; ters çizilmiş tek ok kavramı bitirir. Üç karede blok ve eğim aynı kalsın.

---

# 2850. `/digestion-journey` — Fen: Sindirim Sistemi Yolculuğu (Ortaokul)

## Türkçe prompt

> Besinlerin sindirim sistemi yolculuğunu dikey süreç diyagramı olarak göster: ağız, yemek borusu, mide, ince bağırsak ve kalın bağırsak sırayla; her organda gerçekleşen temel işlem tek cümleyle yazılsın. Organlar anatomik olarak doğru konumda ve oranda olsun.

## English

> Show the journey of food through the digestive system as a vertical process diagram: mouth, esophagus, stomach, small intestine, and large intestine in order, with one sentence per organ describing its main process. Keep organs in anatomically correct positions and proportions.

## Neye dikkat edilmeli?

Organ sırası ve bağlantıları ders kitabıyla doğrulanır; model bağırsakları dekoratif düğüm gibi çizmeye eğilimlidir. Enzim ve emilim cümleleri seviyeye uygun kısalıkta olsun.

---

# 2851. `/sun-earth-moon` — Fen: Güneş–Dünya–Ay ve Gölge (İlkokul)

## Türkçe prompt

> Güneş, Dünya ve Ay'ı ilkokul düzeyinde basit modelle göster: Güneş ışık kaynağı olarak sarı, Dünya mavi-yeşil, Ay gri; Ay'ın Dünya çevresindeki yörüngesi kesikli çizgiyle belirtilsin. Gece-gündüz ayrımı Dünya üzerinde açık-koyu yarılarla anlatılsın.

## English

> Show the Sun, Earth, and Moon as a simple primary-school model: a yellow Sun as light source, a blue-green Earth, and a gray Moon, with the Moon's orbit as a dashed line. Explain day and night with light and dark halves on Earth.

## Neye dikkat edilmeli?

Ölçek ve uzaklık “temsili” olduğu görselde belirtilsin; gerçek orantı sanılan model kavram yanılgısı doğurur. Ay'ın evreleri istenmiyorsa prompta açıkça yazılsın, model kendiliğinden eklemesin.

---

# 2852. `/fraction-circles` — Matematik: Kesirler (İlkokul)

## Türkçe prompt

> Kesirleri ilkokul düzeyinde görsel çalışma rehberi olarak düzenle: 1/2, 1/3 ve 1/4 aynı büyüklükte daire modelleriyle gösterilsin; boyalı dilimler payı, toplam dilim paydayı anlatsın. Her kesrin altına sayı doğrusundaki yeri küçük işaretlensin.

## English

> Organize fractions as a primary-school visual study guide: show 1/2, 1/3, and 1/4 with same-sized circle models where shaded slices show the numerator and total slices the denominator. Mark each fraction's place on a small number line below.

## Neye dikkat edilmeli?

Bütün daireler aynı büyüklükte olsun; farklı boyda bütün, kesir kavramını çürütür. Boyalı alan ile sayı birebir eşleşsin, yaklaşık boyama kabul edilmez.

---

# 2853. `/solid-nets` — Matematik: Geometrik Cisimlerin Açılımı (Ortaokul)

## Türkçe prompt

> Küp, kare prizma ve üçgen piramidin yüzey açılımını (net) göster: her cisim yanında açılımıyla eşleşmiş dursun, karşılıklı yüzler aynı renkle kodlansın. Açılımda katlama çizgileri kesikli, kesim çizgileri düz çizilsin.

## English

> Show the surface nets of a cube, square prism, and triangular pyramid: each solid beside its matching net, with opposite faces color-coded alike. Draw fold lines dashed and cut lines solid in the nets.

## Neye dikkat edilmeli?

Açılım gerçekten katlanabilir olsun; öğretmenin kâğıt çıktıyla test etmesi önerilir. Renk kodlaması cisimle açılım arasında birebir tutsun.

---

# 2854. `/bar-chart-read` — Matematik: Sütun Grafiği Okuma (Ortaokul)

## Türkçe prompt

> Sınıfın favori meyveleri konulu sütun grafiği hazırla: 4 meyve, eksenler etiketli, her sütunun değeri üstünde yazılı; en yüksek sütun vurgu renginde olsun. Grafik deftere çizilebilir sadelikte olsun.

## English

> Prepare a bar chart on the class's favorite fruits: 4 fruits with labeled axes and each bar's value written on top, the tallest bar in an accent color. Keep the chart simple enough to redraw in a notebook.

## Neye dikkat edilmeli?

Eksen ölçeği sıfırdan başlasın; kesik eksen farkı abartır ve grafik okuryazarlığını zedeler. Değer-sütun eşleşmesi tek tek denetlensin.

---

# 2855. `/symmetry-axis` — Matematik: Simetri ve Örüntü (İlkokul)

## Türkçe prompt

> Simetri konusunu kelebek ve yaprak örnekleriyle göster: simetri ekseni kırmızı kesikli çizgiyle belirtilsin, eksenin iki yanı ayna görüntüsü olsun. Altına öğrencinin tamamlayacağı yarım bırakılmış üçüncü örnek eklensin.

## English

> Teach symmetry with butterfly and leaf examples: mark the symmetry axis with a red dashed line with mirrored halves on each side. Add a third half-finished example below for the student to complete.

## Neye dikkat edilmeli?

Ayna simetrisi piksel piksel tutsun; yaklaşık simetri “neredeyse doğru”yu öğretir. Yarım örnek gerçekten tamamlanabilir zorlukta olsun.

---

# 2856. `/area-grid` — Matematik: Alan Ölçme Izgarada (İlkokul–Ortaokul)

## Türkçe prompt

> Dikdörtgen ve L-biçimli bölgenin alanını birim kare ızgarası üzerinde göster: tam kareler bir renkle, yarım kareler başka renkle işaretlensin; sayma yolu oklarla numaralandırılsın. Izgara çizgileri net ve eşit aralıklı olsun.

## English

> Show the area of a rectangle and an L-shaped region on a unit-square grid: full squares in one color, half squares in another, with the counting path numbered by arrows. Keep grid lines sharp and evenly spaced.

## Neye dikkat edilmeli?

Yarım kareler gerçekten yarım olsun; yaklaşık bölünmüş kareler saymayı öğretmez. Toplam, görseldeki sayımla birebir tutsun.

---

<a id="aile-142"></a>
# İşlenmiş Örnekler — Zayıftan Kontrollüye (§17 Yöntemi Uygulamada)

§17'deki üç düzey (zayıf / açık / kontrollü) burada altı konuda işlenir. Her bölümde aynı konu üç hâliyle verilir; farkı yaratanın sıfat çokluğu değil, belirsizliği kapatan cümleler olduğu gösterilir. Her örneğin sonunda §18 kontrol sorularından hangilerinin bu konuda kritik olduğu yazılır.

---

# 2857. İşlenmiş örnek: Volkan kesiti

## Zayıf

> Bir volkan çiz.

Biçim yok, seviye yok, etiket dili yok; model sinematik patlama sahnesi de üretebilir, karikatür de.

## Açık

> Bir volkanın iç yapısını kesit görünümünde göster.

Biçim belli (§5); ama hangi yapılar, hangi dilde, hangi üslupla belli değil.

## Kontrollü

> Bir volkanın iç yapısını eğitim amaçlı kesit görünümünde göster. Dağın dış silueti korunurken bir bölümü açılmış gibi olsun. Magma odası, ana volkan bacası, yan bacalar, krater, lav akışı ve çevredeki kaya katmanları görülebilsin. Yapıları kısa Türkçe etiketlerle belirt. Jeoloji ders kitabı çizimi kadar açık ve ölçülü olsun.

## Neden çalıştı?

Kontrol üç yerden gelir: yapı listesi (eksik kavram engellenir), etiket dili (sınıfta kullanılabilirlik) ve üslup sınırı (dramatik sahne engellenir). Kritik §18 soruları: etiket doğru yapıda mı, model parça uydurmuş mu, görsel seviyeye uygun mu.

---

# 2858. İşlenmiş örnek: Su döngüsü

## Zayıf

> Su döngüsünü göster.

Model okları rastgele dağıtabilir, karayı ve denizi karıştırabilir.

## Açık

> Su döngüsünü döngü diyagramı olarak göster.

Döngü biçimi belli (§10); süreç listesi ve ok mantığı hâlâ modele bırakılmış.

## Kontrollü

> Su döngüsünü ilkokul düzeyinde döngü diyagramı olarak göster. Buharlaşma, yoğunlaşma, yağış, yüzey akışı ve yer altı suyunu aynı tutarlı manzarada göster. Okları yalnız gerçek süreç ilişkileri için kullan. Her aşamayı kısa Türkçe etiketle.

## Neden çalıştı?

Süreç listesi kapanışı ve “oklar yalnız gerçek ilişki için” kısıtı, döngü diyagramının en sık hatasını (dekoratif ok) baştan engeller. Kritik §18 soruları: ok yönleri doğru mu, süreç sırası doğru mu.

---

# 2859. İşlenmiş örnek: Mitoz ve mayoz

## Zayıf

> Mitoz ve mayozu çiz.

İki süreç üst üste binebilir, biri unutulabilir, renkler rastgele atanır.

## Açık

> Mitoz ve mayozu yan yana karşılaştır.

Karşılaştırma biçimi belli (§13); neyin karşılaştırılacağı belli değil.

## Kontrollü

> Mitoz ve mayoz bölünmeyi yan yana karşılaştır. Sol tarafta mitoz, sağ tarafta mayoz olsun. Kromozom sayısındaki değişim, oluşan hücre sayısı ve genetik benzerlik görsel olarak karşılaştırılabilsin. İki taraf aynı ölçek, açı ve çizim dilinde olsun. Türkçe etiketler kullan.

## Neden çalıştı?

Karşılaştırma ölçütleri (sayı, hücre adedi, benzerlik) ve “aynı ölçek-dil” kısıtı yazıldı; ölçüt yazılmayan karşılaştırma süslemeye kayar. Kritik §18 soruları: ölçek yanıltıcı mı, temel kavram eksik mi.

---

# 2860. İşlenmiş örnek: Yazının gelişimi

## Zayıf

> Yazının tarihini görselleştir.

Model dönemleri karıştırabilir, parşömen klişesine gömülebilir.

## Açık

> Yazının gelişimini zaman çizelgesi olarak göster.

Zaman biçimi belli (§22); hangi duraklar ve hangi üslup belli değil.

## Kontrollü

> Yazının gelişimini yatay zaman çizelgesi olarak göster. Sümer çivi yazısı, Mısır hiyeroglifleri, Fenike, Yunan ve Latin alfabeleri ile matbaa ve dijital yazıyı kronolojik diz. Her durakta yaklaşık tarih ve tek cümlelik Türkçe açıklama olsun. Dekoratif antik süsleme kullanma, zaman ilişkisini okunur kıl.

## Neden çalıştı?

Durak listesi dönem karışmasını, “süsleme yok” kısıtı klişeyi engeller. Kritik §18 soruları: sıra doğru mu, dekorasyon bilgiyi gölgeliyor mu.

---

# 2861. İşlenmiş örnek: Ekosistem kavram haritası

## Zayıf

> Ekosistemle ilgili kavram haritası yap.

Model kavramları etiketsiz çizgilerle bağlar; harita zihin haritasına kayar.

## Açık

> Ekosistem kavram haritası oluştur.

Kavram haritası biçimi belli (§24); ilişki ifadeleri hâlâ eksik.

## Kontrollü

> “Ekosistem” merkezli kavram haritası oluştur. Üreticiler, tüketiciler, ayrıştırıcılar, enerji akışı ve madde döngüsünü ekle. Bağlantıların üzerine “içerir”, “enerji sağlar”, “maddeyi geri kazandırır” gibi kısa ilişki ifadeleri yaz. Türkçe kullan.

## Neden çalıştı?

Kavram haritasını harita yapan şey bağlantı anlamıdır; ilişki ifadeleri yazılınca model çizgiyi süs olmaktan çıkarır. Kritik §18 sorusu: bağlantıların anlamı doğru mu.

---

# 2862. İşlenmiş örnek: Devre malzemeleri

## Zayıf

> Elektrik devresi malzemelerini göster.

Model rastgele pil-kablo yığını üretebilir, ölçekler tutmaz.

## Açık

> Devre malzemelerini üstten düzenlemeyle göster.

Düzen biçimi belli (§29); hangi malzemeler ve hangi düzen kuralı belli değil.

## Kontrollü

> Pil, anahtar, ampul, bağlantı kabloları ve duyu üstten düzenleme (flat lay) ile göster. Nesneler ızgara düzeninde, aralarında eşit boşlukla dizilsin; her nesnenin altına kısa Türkçe adı yazılsın. Ölçekler gerçeğe uygun olsun, dekoratif nesne eklenmesin.

## Neye dikkat edilmeli?

Bu örnekte kontrol listeden gelir: eksiksiz malzeme sayımı ve ızgara kuralı. Kritik §18 soruları: temel kavram eksik mi, ölçek yanıltıcı mı, dekorasyon bilgiyi gölgeliyor mu.

---

<a id="aile-143"></a>
# Çalışılmış A/B Örnekleri — İkinci Grup

§2631–2636'daki ilk grubun devamıdır; yöntem ve protokol aynıdır (§2637–2638). Bu grup iç mekân minyatürü, dönem portresi ve sticker setini kapsar.

---

# 2863. Çalışılmış örnek: `/photo-to-isometric-room` — izometrik oda A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı oda fotoğrafını iki modelde `/photo-to-isometric-room` ile dönüştürüp farkları kaydetmek. Açılım promptu §2119'dadır.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/photo-to-isometric-room — use the uploaded photo as layout reference, preserve furniture arrangement and colors`

### Nano Banana varyantı

> Yüklenen fotoğrafı yerleşim referansı olarak kullan. Odayı duvarları kesilmiş izometrik minyatüre dönüştür; mobilya dizimi ve renkler korunsun. Minyatür, masa üstü koleksiyon objesi ölçeğinde, sade zeminde gösterilsin.

## Beklenen fark

- Mekân düzeninde Nano Banana referansa daha sıkı tutunur; ChatGPT mobilyaları “güzelleştirip” yerlerini oynatabilir.
- Metin içeren nesneler (kitap sırtı, poster) iki modelde de bozulabilir; yazı denetimi şarttır.

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: mobilya dizimi aynı mı, duvar kesimi temiz mi, ölçek tutarlı mı? Düzen kaydıysa referans cümlesi güçlendirilir.

### Sonuç görseli

`images/ab-07-isoroom-chatgpt.png`  
`images/ab-07-isoroom-nanobanana.png`

---

# 2864. Çalışılmış örnek: `/yearbook-portrait` — yearbook portresi A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı portreyi iki modelde `/yearbook-portrait` ile dönüştürüp farkları kaydetmek. Açılım promptu §2050'dedir.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/yearbook-portrait — 90s yearbook style, preserve identity, studio backdrop`

### Nano Banana varyantı

> Yüklenen fotoğrafı kimlik referansı olarak kullan. Kişiyi 90'lar yearbook portresine dönüştür: dönem saç ve giysi dili, stüdyo fonu, grenli film dokusu. Yüz benzerliği korunsun.

## Beklenen fark

- Dönem dokusunda (gren, renk kayması) Nano Banana daha tutarlıdır; ChatGPT modern cilt rötuşunu döneme taşıyabilir.
- Kimlik: iki modelde de yüz benzerliği cümlesi açık yazılmalı, yoksa dönem stili kimliği ezer.

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: yüz tanınır mı, dönem detayları tek onyıla ait mi, cilt dokusu doğal mı? Rötuş baskınsa “rötuşsuz” kısıtı eklenir.

### Sonuç görseli

`images/ab-08-yearbook-chatgpt.png`  
`images/ab-08-yearbook-nanobanana.png`

---

# 2865. Çalışılmış örnek: `/sticker-sheet` — sticker seti A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı karakteri iki modelde `/sticker-sheet` ile sete dönüştürüp farkları kaydetmek. Açılım promptu §1973'tedir.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/sticker-sheet — same character in 6 stickers, white borders, die-cut look, preserve outfit and face`

### Nano Banana varyantı

> Yüklenen fotoğraftaki karakteri 6'lı sticker setine dönüştür: bütün çıkartmalarda yüz ve kıyafet aynı kalsın; beyaz kesim konturu ve çıkartma kâğıdı dokusu görünsün.

## Beklenen fark

- Karakter tutarlılığında ChatGPT tek hamlede daha stabil olabilir; Nano Banana'da sapan çıkartma tek değişiklikle ayrıca üretilir.
- Kesim konturu iki modelde de bozulabilir; kenar temizliği yakın planda denetlenir.

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: karakter bütün çıkartmalarda aynı mı, kontur temiz mi, çıkartma sayısı doğru mu? Sapan çıkartma varsa set değil o çıkartma yeniden üretilir.

### Sonuç görseli

`images/ab-09-sticker-chatgpt.png`  
`images/ab-09-sticker-nanobanana.png`

---

<a id="aile-144"></a>
# Ders Konu Galerileri — Türkçe ve Sosyal Bilgiler

aile-141'in devamıdır; kalıp aynıdır: seviye etiketi, hazır TR+EN prompt, §18'e bağlı değerlendirme notu. Dil dersinde yazı denetimi (§995 kuralı) her bölümde ayrıca uygulanır; sosyal bilgilerde harita ve tarih bilgisi kaynaktan doğrulanır.

---

# 2866. `/punctuation-poster` — Türkçe: Noktalama İşaretleri (İlkokul)

## Seviye

İlkokul 3–4. sınıf — Noktalama işaretleri.

## Türkçe prompt

> Noktalama işaretlerini ilkokul posteri olarak göster: nokta, virgül, soru işareti, ünlem, iki nokta ve kesme işareti büyük ve tek tek; her işaretin yanında bir kelimelik görevi (“durdurur”, “sorar”, “ayırt eder”) ve minik örnek cümle olsun. Renkler işarete göre kodlansın.

## English

> Show punctuation marks as a primary-school poster: period, comma, question mark, exclamation mark, colon, and apostrophe, each large and separate, with a one-word function (“durdurur”, “sorar”, “ayırt eder”) and a tiny example sentence beside each. Color-code by mark.

## Neye dikkat edilmeli?

Örnek cümlelerdeki noktalama harf harf denetlenir; posterdeki tek yanlış, yanlış öğretir. İşaret biçimleri standart klavye-tipografi biçiminde olsun.

---

# 2867. `/verb-lanes` — Türkçe: Fiilde Kip ve Zaman (Ortaokul)

## Türkçe prompt

> Fiil kiplerini zaman çizgisi mantığıyla göster: geçmiş, şimdiki ve gelecek zaman ile dilek kipleri ayrı kulvarlarda; her kulvarda aynı fiilin çekimli hâli örnek cümleyle verilsin. Kulvar başlıkları Türkçe olsun.

## English

> Show verb moods and tenses with timeline logic: past, present, and future tenses plus optative moods in separate lanes, each lane giving the conjugated form of the same verb in an example sentence. Use Turkish lane headings.

## Neye dikkat edilmeli?

Çekimler dilbilgisi kitabıyla doğrulanır; model kip eklerini karıştırmaya eğilimlidir. Aynı fiil bütün kulvarlarda kullanılsın, fiil değişmesin.

---

# 2868. `/idiom-cards` — Türkçe: Deyimler Görsel Kartları (İlkokul–Ortaokul)

## Türkçe prompt

> 4 deyimi görsel kart serisi olarak göster: her kartta deyimin gerçek anlamını anlatan küçük sahne ve altında deyimin kendisi (“gözden düşmek”, “kulağına küpe olmak” gibi). Gerçek anlam ile mecaz anlam kartta ayrı satırlarda dursun.

## English

> Show 4 idioms as a visual card series: each card with a small scene depicting the idiom's literal sense and the idiom itself below (e.g., “gözden düşmek”, “kulağına küpe olmak”). Keep literal and figurative senses on separate lines.

## Neye dikkat edilmeli?

Sahne gerçek anlamı, yazı mecaz anlamı taşısın; ikisi karışırsa deyim öğretilemez. Deyim yazımı harf harf denetlenir.

---

# 2869. `/paragraph-schema` — Türkçe: Paragraf Yapısı (Ortaokul)

## Türkçe prompt

> Paragraf yapısını şematik gösterimle anlat: giriş, gelişme ve sonuç bölümleri renkli bloklarla; her bloğun görevi tek cümleyle, bloklar arası geçiş okla gösterilsin. Örnek paragraf sağda küçük kutuda olsun.

## English

> Explain paragraph structure schematically: introduction, body, and conclusion as colored blocks with each block's function in one sentence and transitions shown by arrows. Place a sample paragraph in a small box on the right.

## Neye dikkat edilmeli?

Örnek paragrafın yapısı şemayla birebir eşleşsin; eşleşmeyen örnek şemayı çürütür. Geçiş ifadeleri örnekte gerçekten geçsin.

---

# 2870. `/word-class-cards` — Türkçe: Sözcük Türleri Renk Kodlaması (Ortaokul)

## Türkçe prompt

> İsim, sıfat, fiil ve zarfı renk kodlu kartlarla göster: her türün rengi, tek cümlelik görevi ve aynı örnek cümlede renkli işaretlenmiş hâli olsun. Örnek cümle bütün kartlarda aynı kalsın.

## English

> Show nouns, adjectives, verbs, and adverbs as color-coded cards: each type with its color, a one-sentence function, and the same example sentence marked in colors. Keep the example sentence identical across cards.

## Neye dikkat edilmeli?

Örnek cümledeki işaretleme dilbilgisi açısından doğru olsun; tek yanlış renk tüm sistemi çürütür. Renkler metinde ve kartta birebir tutsun.

---

# 2871. `/regions-map` — Sosyal: Türkiye'nin Coğrafi Bölgeleri (Ortaokul)

## Seviye

Ortaokul 5–6. sınıf — Ülkemizin coğrafi bölgeleri.

## Türkçe prompt

> Türkiye'nin yedi coğrafi bölgesini açıklamalı harita olarak göster: her bölge farklı yumuşak renkte, bölge adları harf harf doğru, her bölgede 2 küçük simge (ürün, yer şekli) olsun. Komşu denizler ve sınırlar sade çizilsin.

## English

> Show Türkiye's seven geographical regions as an annotated map: each region in a distinct soft color with letter-perfect region names and 2 small icons per region (product, landform). Draw neighboring seas and borders simply.

## Neye dikkat edilmeli?

Bölge sınırları ve adları güncel müfredatla doğrulanır; model sınır uydurmaya eğilimlidir. Simgeler gerçekten o bölgeye ait olsun.

---

# 2872. `/civ-strip` — Sosyal: Anadolu Uygarlıkları Şeridi (Ortaokul)

## Türkçe prompt

> Anadolu uygarlıklarını yatay zaman şeridi olarak göster: Hitit, Frig, Lidya, İyon, Urartu ve Pers kronolojik dizilsin; her uygarlıkta başkent ve bir ayırt edici eser/kalıntı küçük görselle verilsin. Tarihler yaklaşık olarak yazılsın.

## English

> Show Anatolian civilizations as a horizontal time strip: Hittite, Phrygian, Lydian, Ionian, Urartian, and Persian in chronological order, each with its capital and one distinguishing artifact or ruin in a small visual. Write approximate dates.

## Neye dikkat edilmeli?

Sıra ve başkentler ders kitabıyla doğrulanır; model uygarlık adını yanlış esere bağlar. Tarihler “yaklaşık” ibaresiyle verilsin.

---

# 2873. `/admin-tree` — Sosyal: Yönetim Birimleri Hiyerarşisi (Ortaokul)

## Türkçe prompt

> Merkezi ve yerel yönetim birimlerini hiyerarşi ağacı olarak göster: il, ilçe, belediye ve muhtarlık kademeleri kutularla; her kademede yöneticinin unvanı (vali, kaymakam, belediye başkanı, muhtar) yazsın. Bağlantı okları yukarıdan aşağıya insin.

## English

> Show central and local administrative units as a hierarchy tree: province, district, municipality, and neighborhood levels as boxes with each administrator's title (vali, kaymakam, belediye başkanı, muhtar). Run connecting arrows top-down.

## Neye dikkat edilmeli?

Unvan-kademe eşleşmesi güncel mevzuata uygun olsun. Kutu hiyerarşisi tek yönde okunsun, çapraz bağlantı olmasın.

---

# 2874. `/climate-zones` — Sosyal: Türkiye'de İklim Tipleri (Ortaokul)

## Türkçe prompt

> Türkiye'de iklim tiplerini harita üzerinde göster: Karadeniz, Akdeniz ve karasal iklim alanları farklı renklerde; her alanın yağış-sıcaklık karakteri tek cümleyle lejantta yazsın. Geçiş alanları belirtilsin.

## English

> Show Türkiye's climate types on a map: Black Sea, Mediterranean, and continental zones in distinct colors, with each zone's rainfall-temperature character in one legend sentence. Mark transition areas.

## Neye dikkat edilmeli?

İklim sınırları yaklaşık olduğu lejantta belirtilsin; keskin sınır çizgisi kavram yanılgısı doğurur. Renk-lejant eşleşmesi birebir olsun.

---

# 2875. `/economy-symbols` — Sosyal: Ekonomik Faaliyetler Haritası (Ortaokul)

## Türkçe prompt

> Türkiye'de ekonomik faaliyetleri simgeli harita olarak göster: tarım, hayvancılık, sanayi, turizm ve madencilik için ayrı simgeler; simgeler ilgili bölgelere yerleştirilsin, lejantta her simgenin anlamı yazsın.

## English

> Show economic activities in Türkiye as a symbol map: distinct symbols for agriculture, livestock, industry, tourism, and mining placed in relevant regions, with each symbol's meaning in the legend.

## Neye dikkat edilmeli?

Simge-bölge eşleşmesi gerçek ekonomiyle uyuşsun; turizm simgesi sanayi bölgesinde durmasın. Simge sayısı haritayı okunmaz kılmasın.

---

<a id="aile-145"></a>
# Ders Konu Galerileri — İngilizce ve Müzik

aile-141 ve aile-144'ün devamıdır; kalıp aynıdır: seviye etiketi, hazır TR+EN prompt, §18'e bağlı değerlendirme notu. Yabancı dilde örnek cümleler ders kitabıyla doğrulanır; müzikte nota ve ritim gösterimi standart notasyona uyar.

---

# 2876. `/vocab-cards` — İngilizce: Kelime Kartları (İlkokul–Ortaokul)

## Seviye

İlkokul 4. sınıf ve üstü — Kelime bilgisi.

## Türkçe prompt

> İngilizce [ÜNİTE] kelimeleri için görsel kelime kartları hazırla: her kartta kelime, küçük illüstrasyon ve Türkçe karşılığı ayrı satırlarda olsun. 8 kart ızgara düzeninde sunulsun.

## English

> Prepare visual vocabulary cards for English [UNIT] words: each card with the word, a small illustration, and the Turkish equivalent on separate lines. Present 8 cards in a grid.

## Neye dikkat edilmeli?

Kelime-illüstrasyon eşleşmesi birebir olsun; yanlış resim yanlış öğretir. Türkçe karşılıklar ders kitabındaki anlamla tutsun.

---

# 2877. `/tense-lanes` — İngilizce: Zamanlar Kulvarları (Ortaokul)

## Seviye

Ortaokul 6–8. sınıf — Tenses.

## Türkçe prompt

> İngilizce zamanları (Simple Present, Present Continuous, Simple Past, Future) kulvar şeridi olarak göster: her kulvarda zaman çizelgesi işareti, olumlu-olumsuz-soru örnek cümle ve zaman zarfı olsun. Örnek fiil bütün kulvarlarda aynı kalsın.

## English

> Show English tenses (Simple Present, Present Continuous, Simple Past, Future) as lane strips: each lane with a timeline marker, affirmative-negative-question examples, and time expressions. Keep the example verb identical across lanes.

## Neye dikkat edilmeli?

Örnek cümleler dilbilgisi açısından kusursuz olsun; tek yanlış cümle kuralı çürütür. Zaman zarfları doğru kulvarda dursun.

---

# 2878. `/dialogue-comic` — İngilizce: Diyalog Çizgi Romanı (Ortaokul)

## Türkçe prompt

> [DURUM] için 4 karelik İngilizce diyalog çizgi romanı hazırla: konuşma balonlarında kısa doğal cümleler, her karede sahne değişimi minimal olsun. Zor kelimelerin Türkçe karşılığı sayfa altında küçük sözlükte verilsin.

## English

> Prepare a 4-panel English dialogue comic for [SITUATION]: short natural sentences in speech balloons with minimal scene change per panel. Give hard words' Turkish equivalents in a small glossary below.

## Neye dikkat edilmeli?

Cümleler seviyeye uygun kısalıkta olsun; balon yazısı harf harf denetlenir. Sözlükteki karşılıklar diyalogdaki anlamla tutsun.

---

# 2879. `/phonics-chart` — İngilizce: Ses-Harf Tablosu (İlkokul)

## Türkçe prompt

> İngilizce ses-harf eşleşmeleri için phonics tablosu hazırla: her satırda harf/harf grubu, örnek kelime ve küçük illüstrasyon olsun. Benzer sesler yan yana gruplanmasın, karışmaması için ayrılsın.

## English

> Prepare a phonics chart for English letter-sound matches: each row with the letter or group, an example word, and a small illustration. Separate similar sounds instead of grouping them together.

## Neye dikkat edilmeli?

Örnek kelimeler hedef sesi gerçekten taşısın; istisna kelimeler tabloya alınmasın. Telaffuz ve yazım eşleşmesi öğretmenle doğrulanır.

---

# 2880. `/daily-routines` — İngilizce: Günlük Rutinler Şeridi (İlkokul)

## Türkçe prompt

> Günlük rutinleri İngilizce sıralı şerit olarak göster: uyanma, kahvaltı, okul, oyun ve uyku 5 karede; her karede saat, İngilizce cümle (I wake up at seven gibi) ve küçük illüstrasyon olsun.

## English

> Show daily routines as an English sequence strip: waking, breakfast, school, play, and sleep in 5 frames, each with the time, an English sentence (e.g., I wake up at seven), and a small illustration.

## Neye dikkat edilmeli?

Saat-cümle-görsel üçlüsü tutarlı olsun; saat yediyse sahne sabah ışığında olsun. Cümleler bugünkü müfredat kalıplarıyla tutsun.

---

# 2881. `/rhythm-bars` — Müzik: Ritim Kalıpları (İlkokul–Ortaokul)

## Seviye

İlkokul 3. sınıf ve üstü — Ritim.

## Türkçe prompt

> 4 temel ritim kalıbını görsel şerit olarak göster: dörtlük, sekizlik, ikilik ve es kalıpları; her kalıpta nota değerleri, vuruş sayıları ve el çırpma işareti olsun. Kalıplar zorluk sırasına dizilsin.

## English

> Show 4 basic rhythm patterns as a visual strip: quarter, eighth, half, and rest patterns, each with note values, beat counts, and clapping marks. Order patterns by difficulty.

## Neye dikkat edilmeli?

Nota değerleri ve vuruş sayıları müzik teorisiyle birebir tutsun; tek yanlış değer ritmi çürütür. Vuruş işaretleri net ve sayılabilir olsun.

---

# 2882. `/instrument-families` — Müzik: Çalgı Aileleri (İlkokul–Ortaokul)

## Türkçe prompt

> Çalgıları telli, üflemeli, vurmalı ve tuşlu aileler olarak sınıflandırma tablosu şeklinde göster: her ailede 3 örnek çalgı küçük illüstrasyonla; ses üretim biçimi tek cümleyle yazılsın.

## English

> Present instruments as a classification chart of string, wind, percussion, and keyboard families: 3 example instruments per family as small illustrations, with one sentence each on sound production.

## Neye dikkat edilmeli?

Çalgı-aile eşleşmesi doğru olsun; piyano telli-vurmalı tartışması seviyeye göre sadeleştirilip öğretmene bırakılsın. İllüstrasyonlar gerçek çalgıyı andırsın.

---

# 2883. `/note-ladder` — Müzik: Nota Merdiveni (İlkokul)

## Türkçe prompt

> Do'dan Do'ya nota merdiveni göster: porte üzerinde 8 nota, her basamakta nota adı ve parmak numarası (flüt/blok flüt için); merdiven yukarı çıktıkça ses inceldiği okla belirtilsin.

## English

> Show a note ladder from Do to Do: 8 notes on a staff with note names and finger numbers (for flute/recorder) per step, marking rising pitch with an upward arrow.

## Neye dikkat edilmeli?

Nota konumları porte üzerinde doğru çizgide olsun; tek çizgi kayması yanlış öğretir. Parmak numaraları ilgili çalgıya uygun olsun.

---

# 2884. `/dynamics-signs` — Müzik: Gürlük İşaretleri (Ortaokul)

## Türkçe prompt

> Gürlük (nüans) işaretlerini kart serisi olarak göster: piano, forte, crescendo ve decrescendo; her kartta işaret, adı ve “nasıl çalınır” tek cümlesi olsun. İşaret biçimleri standart notasyonda olsun.

## English

> Show dynamics signs as a card series: piano, forte, crescendo, and decrescendo, each card with the sign, its name, and one sentence on how to play it. Keep signs in standard notation.

## Neye dikkat edilmeli?

İşaret biçimleri standart dışı çizilmesin; crescendo açısı ve yönü doğru olsun. Ad-tanım eşleşmesi denetlensin.

---

# 2885. `/composer-strip` — Müzik: Besteci Zaman Şeridi (Ortaokul)

## Türkçe prompt

> 4 besteciyi zaman şeridinde göster: her bestecide dönem, ülke ve bir ünlü eser küçük illüstrasyonla; şerit kronolojik dizilsin. Dönem adları (Barok, Klasik gibi) doğru yazılsın.

## English

> Show 4 composers on a timeline: each with era, country, and one famous work as a small illustration, arranged chronologically. Spell era names (Baroque, Classical) correctly.

## Neye dikkat edilmeli?

Dönem-besteci eşleşmesi müzik tarihiyle doğrulanır. Eser adları orijinal dilinde ve doğru yazılsın.

---

<a id="aile-146"></a>
# Ders Konu Galerileri — Beden Eğitimi ve Görsel Sanatlar

Galeri dizisinin devamıdır; kalıp aynıdır: seviye etiketi, hazır TR+EN prompt, §18'e bağlı değerlendirme notu. Hareket gösterimlerinde eklem ve denge gerçekçiliği (§75–77 mantığı), sanat gösterimlerinde teknik doğruluk aranır.

---

# 2886. `/warmup-cards` — Beden: Isınma Kartları (İlkokul–Ortaokul)

## Seviye

İlkokul 2. sınıf ve üstü — Isınma hareketleri.

## Türkçe prompt

> 6 ısınma hareketini kart serisi olarak göster: her kartta hareketin adı, başlangıç-bitiş pozu okla ve tekrar sayısı; figür sade çizgi insan olsun. Kartlar ısınma sırasına dizilsin.

## English

> Show 6 warm-up moves as a card series: each card with the move's name, start-end poses with arrows, and repetition count, using a simple line figure. Order cards in warm-up sequence.

## Neye dikkat edilmeli?

Pozlar anatomik olarak mümkün olsun; eklemi zorlayan çizim sakatlığa davetiye çıkarır. Ok yönü hareket yönüyle birebir tutsun.

---

# 2887. `/game-rules` — Beden: Oyun Kuralları Şeması (İlkokul–Ortaokul)

## Türkçe prompt

> [OYUN]'un kurallarını tek sayfalık görsel şema olarak anlat: saha dizimi, başlama, sayı ve faul kuralları 4 kutuda; her kutuda minik saha çizimi olsun. Dil ilkokul düzeyinde sade olsun.

## English

> Explain [GAME]'s rules as a one-page visual diagram: field setup, start, scoring, and foul rules in 4 boxes, each with a tiny field sketch. Keep language at primary level.

## Neye dikkat edilmeli?

Kural sayısı oyunun gerçeğiyle tutsun; uydurma kural bahçede kavga çıkarır. Saha ölçüleri orantılı olsun.

---

# 2888. `/movement-sequence` — Beden: Hareket Sıralı Şeridi (Ortaokul)

## Türkçe prompt

> [HAREKET]'i (örn. şut, smaç, takla) 4 kareli sıralı şerit olarak göster: kesikli aşama tekniğiyle aynı figürün art arda pozu; kilit an (topa vuruş) büyük karede vurgulansın.

## English

> Show [MOVE] (e.g., kick, spike, roll) as a 4-frame sequence strip: the same figure in successive poses with ghosted steps, emphasizing the key instant (ball contact) in a larger frame.

## Neye dikkat edilmeli?

Figür bütün karelerde aynı kişi ve kıyafette olsun; zemin çizgisi sürekliliği korusun (§75–77). Kilit an anatomik olarak doğru yakalansın.

---

# 2889. `/team-positions` — Beden: Takım Dizilişi (Ortaokul)

## Türkçe prompt

> [SPOR] için takım diziliş şeması göster: saha üstten, oyuncular numaralı noktalarla, her mevkinin adı lejantta; topun başlama konumu işaretli olsun.

## English

> Show a team lineup diagram for [SPORT]: top-down field with players as numbered dots, position names in a legend, and the ball's starting spot marked.

## Neye dikkat edilmeli?

Oyuncu sayısı branşa uygun olsun; eksik ya da fazla oyuncu şemayı çürütür. Numara-lejant eşleşmesi birebir olsun.

---

# 2890. `/safety-poster` — Beden: Güvenlik Kuralları Posteri (İlkokul–Ortaokul)

## Türkçe prompt

> Spor salonu güvenlik kurallarını poster olarak göster: doğru-yanlış karşılaştırmalı 4 kural (ısınmadan başlama, uygun ayakkabı, saha çizgisine dikkat, malzeme iadesi); her kuralda yeşil tik ve kırmızı çarpı ikonlu mini sahne olsun.

## English

> Show gym safety rules as a poster: 4 do/don't rules (no starting without warm-up, proper shoes, minding court lines, returning equipment), each a mini scene with green-check and red-cross icons.

## Neye dikkat edilmeli?

Doğru-yanlış sahneleri aynı mekânda geçsin; değişen yalnız davranış olsun (§68 mantığı). Kurallar okulun gerçek kurallarıyla tutsun.

---

# 2891. `/color-wheel` — Görsel Sanatlar: Renk Çemberi (İlkokul–Ortaokul)

## Seviye

İlkokul 3. sınıf ve üstü — Renk bilgisi.

## Türkçe prompt

> Renk çemberini eğitim posteri olarak göster: ana, ara ve tamamlayıcı renkler doğru konumda; her rengin adı Türkçe yazılsın. Sıcak-soğuk ayrımı çemberin iki yarısında belirtilsin.

## English

> Show the color wheel as an educational poster: primary, secondary, and complementary colors in correct positions with Turkish names. Mark the warm-cool split across the wheel halves.

## Neye dikkat edilmeli?

Renk konumları renk teorisiyle birebir tutsun; kayık çember yanlış öğretir. Tamamlayıcı çiftler karşılıklı dursun.

---

# 2892. `/perspective-demo` — Görsel Sanatlar: Perspektif Gösterimi (Ortaokul)

## Türkçe prompt

> Tek kaçışlı perspektifi şematik gösterimle anlat: ufuk çizgisi, kaçış noktası ve ona giden raylar; önde küp, ortada ev, geride ağaç aynı perspektifte dizilsin. Yardımcı çizgiler ince ve silik olsun.

## English

> Teach one-point perspective schematically: horizon line, vanishing point, and converging rails, with a cube in front, a house mid-ground, and a tree behind in one perspective. Keep construction lines thin and faint.

## Neye dikkat edilmeli?

Bütün nesneler tek kaçış noktasına gitsin; iki kaçışlı çizim tek kaçışlı anlatımı çürütür. Nesne boyutları derinlikle tutarlı küçülsün.

---

# 2893. `/pattern-design` — Görsel Sanatlar: Örüntü Tasarımı (İlkokul–Ortaokul)

## Türkçe prompt

> Öğrencinin tamamlayacağı örüntü tasarım şablonu hazırla: tekrar raporu belli motif dizisi, ilk iki tekrar örnekli, üçüncü tekrar boş bırakılmış olsun. Motif kültürel olarak nötr geometrik şekillerden seçilsin.

## English

> Prepare a pattern-design template for students to complete: a motif sequence with a clear repeat, the first two repeats exemplified and the third left blank. Choose culturally neutral geometric motifs.

## Neye dikkat edilmeli?

Rapor birleşimi kusursuz olsun; bozuk rapor öğrenciyi değil şablonu suçlu çıkarır. Boş bölüm gerçekten tamamlanabilir zorlukta olsun.

---

# 2894. `/portrait-proportions` — Görsel Sanatlar: Portre Oranları (Ortaokul)

## Türkçe prompt

> Yüz oranlarını öğretim şeması olarak göster: göz çizgisi ortada, burun-ağız-çene aralıkları işaretli; önden görünümde kılavuz çizgiler numaralı olsun. Şema gerçekçi yüzle yan yana dursun.

## English

> Show facial proportions as a teaching diagram: eyes on the midline with marked nose-mouth-chin intervals and numbered guide lines on a front view. Place the diagram beside a realistic face.

## Neye dikkat edilmeli?

Oranlar standart öğretim oranlarıyla tutsun; modele özgü abartılı yüz şema olamaz. Kılavuz numaralarıyla açıklama metni eşleşsin.

---

# 2895. `/printmaking-steps` — Görsel Sanatlar: Baskı Adımları (Ortaokul)

## Türkçe prompt

> Linol baskı sürecini 4 adımlı şerit olarak göster: desen çizimi, oyma, mürekkep merdane ve baskı; her adımda alet ve malzeme doğru çizilsin. Güvenlik uyarısı (oygu bıçağı yönü) son karede belirtilsin.

## English

> Show the linocut process as a 4-step strip: drawing, carving, ink rolling, and printing, with correct tools and materials per step. State the safety note (gouge direction) in the last frame.

## Neye dikkat edilmeli?

Alet tutuşları güvenli olsun; yanlış tutuş öğreten görsel derste kullanılmaz. Adım sırası gerçek süreçle birebir tutsun.

---

<a id="aile-147"></a>
# Ders Konu Galerileri — Din Kültürü ve Bilişim

Galeri dizisinin devamıdır; kalıp aynıdır: seviye etiketi, hazır TR+EN prompt, §18'e bağlı değerlendirme notu. Din kültürü bölümlerinde saygılı ve doğru temsil esastır; hiçbir inanç karikatürize edilmez, ibadet mekân ve metinleri özenle denetlenir. Bilişimde arayüz ve donanım adları güncel gerçeklikle tutar.

---

# 2896. `/values-poster` — Din Kültürü: Değerler Posteri (İlkokul–Ortaokul)

## Seviye

İlkokul 4. sınıf ve üstü — Değerler eğitimi.

## Türkçe prompt

> Saygı, yardımlaşma, dürüstlük ve sorumluluk değerlerini poster olarak göster: her değer için günlük hayattan küçük sahne ve tek cümlelik açıklama; 4 kart ızgara düzeninde sunulsun.

## English

> Show respect, helpfulness, honesty, and responsibility as a values poster: a small everyday scene plus a one-sentence explanation per value, arranged as 4 cards in a grid.

## Neye dikkat edilmeli?

Sahneler gerçek okul-aile hayatından olsun; soyut sembol yığını değer öğretmez. Cümleler seviyeye uygun kısalıkta olsun.

---

# 2897. `/worship-places` — Din Kültürü: İbadethaneler (Ortaokul)

## Seviye

Ortaokul 5–6. sınıf — İbadet mekânları.

## Türkçe prompt

> Farklı inançların ibadet mekânlarını saygılı tanıtım panosu olarak göster: cami, kilise ve sinagog dış görünüşleriyle yan yana; her birinde mekânın adı ve tek cümlelik saygılı tanıtım olsun. Mimari doğru çizilsin.

## English

> Present different faiths' houses of worship as a respectful info board: mosque, church, and synagogue side by side in exterior views, each with its name and a one-sentence respectful description. Draw the architecture correctly.

## Neye dikkat edilmeli?

Mimari öğeler (minare, kubbe, çan kulesi) doğru ve yerinde olsun; hiçbir mekân diğerinden küçük ya da özensiz gösterilmesin. Metinler saygılı dilde ve harf harf denetlensin.

---

# 2898. `/holy-books` — Din Kültürü: Kutsal Kitaplar (Ortaokul)

## Türkçe prompt

> Kutsal kitapları tanıtım kartları olarak göster: Kur'an-ı Kerim, İncil ve Tevrat için ayrı kart; her kartta kitabın adı, mensup olduğu din ve saygılı tek cümlelik tanıtım olsun. Kitaplar özenli ve eşit sunulsun.

## English

> Present holy books as info cards: separate cards for the Qur'an, the Bible, and the Torah, each with the book's name, its faith, and a respectful one-sentence description. Present all books with equal care.

## Neye dikkat edilmeli?

Ad yazımları ve atıflar harf harf denetlenir; hata incitici olur. Hiçbir kitap diğerinden büyük ya da süslü gösterilmesin.

---

# 2899. `/festivals-board` — Din Kültürü: Dini Bayramlar Panosu (İlkokul–Ortaokul)

## Türkçe prompt

> Dini bayramları pano olarak göster: Ramazan ve Kurban bayramları için ayrı bölümler; her bölümde bayrama özgü 2–3 öğe (bayramlaşma, yardımlaşma, sofralar) küçük sahnelerle anlatılsın.

## English

> Show religious festivals as a board: separate sections for Ramadan and Eid al-Adha festivities, each told with 2–3 signature elements (greetings, charity, festive tables) in small scenes.

## Neye dikkat edilmeli?

Öğeler gerçekten o bayrama ait olsun; bayramlar birbirine karışmasın. Sahneler sevinç ve paylaşma duygusunu abartısız versin.

---

# 2900. `/kindness-strip` — Din Kültürü: Güzel Davranış Şeridi (İlkokul)

## Türkçe prompt

> Güzel davranışları 4 kareli sıralı şerit olarak göster: yaşlıya yardım, paylaşma, doğayı koruma ve doğru sözlülük; her karede tek eylem ve tek cümlelik açıklama olsun.

## English

> Show good deeds as a 4-frame sequence strip: helping the elderly, sharing, protecting nature, and truthfulness, with one action and one explanatory sentence per frame.

## Neye dikkat edilmeli?

Eylem-cümle eşleşmesi birebir olsun; cümle karede gösterilmeyeni anlatmasın. Figürler sevecen ama karikatürsüz olsun.

---

# 2901. `/computer-parts` — Bilişim: Bilgisayar Parçaları (İlkokul–Ortaokul)

## Seviye

İlkokul 4. sınıf ve üstü — Bilgisayarın bölümleri.

## Türkçe prompt

> Bilgisayarın temel parçalarını numaralı açıklama (numbered callouts) ile göster: kasa, monitör, klavye, fare ve yazıcı; her parçanın görevi tek cümleyle yazılsın. Parçalar gerçek oranlarında olsun.

## English

> Show basic computer parts with numbered callouts: case, monitor, keyboard, mouse, and printer, each with a one-sentence function. Keep parts in realistic proportions.

## Neye dikkat edilmeli?

Parça adları güncel Türkçe bilişim terimleriyle yazılsın. Numara-etiket eşleşmesi birebir olsun (§34 mantığı).

---

# 2902. `/safe-internet` — Bilişim: Güvenli İnternet Posteri (İlkokul–Ortaokul)

## Türkçe prompt

> Güvenli internet kurallarını poster olarak göster: bilinmeyen bağlantılara tıklamama, kişisel bilgi paylaşmama, zorbalıkta öğretmene başvurma ve ekran süresi; her kural doğru-yanlış mini sahneli olsun.

## English

> Show safe-internet rules as a poster: no clicking unknown links, no sharing personal info, telling a teacher about bullying, and screen time, each rule as a do/don't mini scene.

## Neye dikkat edilmeli?

Korku dili kullanılmasın; kurallar koruyucu tonda anlatılsın. Doğru-yanlış sahneleri aynı mekânda geçsin (§68 mantığı).

---

# 2903. `/algorithm-steps` — Bilişim: Algoritma Adımları (Ortaokul)

## Türkçe prompt

> [GÜNLÜK İŞ]'i (örn. çay demleme, diş fırçalama) algoritma adımları olarak akış şemasıyla göster: başla-bitir kutuları, işlem adımları ve bir karar noktası; adımlar numaralı ve sırayla okunsun.

## English

> Show [EVERYDAY TASK] (e.g., brewing tea, brushing teeth) as algorithm steps in a flowchart: start-end boxes, process steps, and one decision point, numbered and reading in order.

## Neye dikkat edilmeli?

Akış kopmadan bitsin; her yol bir sona ulaşsın (§21 mantığı). Karar noktasının iki çıkışı da tanımlı olsun.

---

# 2904. `/folder-tree` — Bilişim: Dosya Klasör Düzeni (Ortaokul)

## Türkçe prompt

> Dosya klasör düzenini hiyerarşi ağacı olarak göster: ana klasör, alt klasörler ve örnek dosya adlarıyla; adlandırma kuralları (Türkçe karakter yok, tarih formatı) yanda kutuda yazsın.

## English

> Show file-folder organization as a hierarchy tree: a main folder with subfolders and sample file names, plus naming rules (no Turkish characters, date format) in a side box.

## Neye dikkat edilmeli?

Örnek adlar kurala uysun; kuralı çiğneyen örnek öğretimi çürütür. Ağaç derinliği 3 düzeyi geçmesin.

---

# 2905. `/keyboard-map` — Bilişim: Klavye Haritası (İlkokul–Ortaokul)

## Türkçe prompt

> Türkçe F klavyeyi öğretim haritası olarak göster: tuşlar gerçek dizilimde, home-row (temel sıra) vurgulu; parmak atamaları renkli noktalarla işaretlensin.

## English

> Show the Turkish F keyboard as a teaching map: keys in real layout with the home row highlighted and finger assignments marked by colored dots.

## Neye dikkat edilmeli?

Tuş dizimi gerçek F klavyeyle birebir tutsun; tek kayık tuş alışkanlığı bozar. Parmak-renk eşleşmesi lejantta açıkça yazsın.

---

<a id="aile-148"></a>
# Ders Akış Senaryoları — 40 Dakikada Kısayol Zinciri

Tekil presetler hazırdı; eksik olan bunları derse dizmekti. Her bölüm bir branşta 40 dakikalık akıştır: giriş çengeli, kavram görseli, etkinlik ve çıkış kontrolü. Tablodaki kısayollar rehberin ilgili bölümlerine gönderir; akışın kendisi öğretmene Türkçedir, bu yüzden bu ailede EN blok yoktur. Süreler öneridir, sınıfın hızına göre kaydırılır.

## Nasıl kullanılır (önemli)

`/lesson-fen` gibi akış kısayolları modele yapıştırılmaz; bunlar okuma kısayoludur. Kullanım: tabloda ilgili adıma gelinir, o adımdaki kısayol kendi bölümünden açılıp oradaki hazır promptla üretim yapılır. Tek hamlede “bana 40 dakikalık ders üret” denmez; akış adım adım uygulanır (§19'un tek değişiklik disiplini burada da geçerlidir).

---

# 2906. `/lesson-fen` — Fen Dersi Akışı (40′)

## Hedef

Öğrenci ders sonunda kavramı görselle anlatabilir ve mini deney föyünü doldurur.

| Dakika | Adım | Kısayol | Üretim notu |
|---|---|---|---|
| 0–5 | Çengel soru görseli | Tahta sorusu (görsel gerekmez) | Tek soru, tek görsel; cevabı verme |
| 5–20 | Kavram görseli | Konu galerisi: `/cell-compare`, `/circuit-pair`, `/friction-strip` | §18 doğrulaması dersten önce yapılır |
| 20–33 | Etkinlik föyü | `/worksheet-student` + `/teacher-overlay` | Föy, görseldeki kavramı ölçsün |
| 33–40 | Çıkış kartı | `/exit-ticket` | 2 soru; ertesi dersin girişini besler |

## Neye dikkat edilmeli?

Akışta en çok kırılan halka kavram-etkinlik uyumudur: föy, gösterilen görselin kavramını ölçmüyorsa akış kopar. Görseller dersten önce §18'den geçirilir, derste yalnızca kullanılır.

---

# 2907. `/lesson-mat` — Matematik Dersi Akışı (40′)

## Hedef

Öğrenci işlemi görselle kurar, kuralı kendisi söyler.

| Dakika | Adım | Kısayol | Üretim notu |
|---|---|---|---|
| 0–5 | Sayı hissi ısınması | Sözlü sayı sohbeti (görsel gerekmez) | Kısa, sözlü, görselsiz başlanabilir |
| 5–20 | Kavram modeli | `/fraction-circles`, `/solid-nets`, `/bar-chart-read` | Model tahtada elle de kurulur |
| 20–33 | Alıştırma seti | `/worksheet-student` | İlk 2 soru modelle birebir eşleşsin |
| 33–40 | Çıkış kartı | `/exit-ticket` | “Bugünün kuralını bir cümleyle yaz” |

## Neye dikkat edilmeli?

Model ile alıştırma aynı örnekle başlasın; modelde elma, alıştırmada armut varsa transfer kopar. Kuralı öğretmen değil, modelden gören öğrenci söylesin.

---

# 2908. `/lesson-turkce` — Türkçe Dersi Akışı (40′)

## Hedef

Öğrenci kuralı örnekte görür, kendi cümlesinde kullanır.

| Dakika | Adım | Kısayol | Üretim notu |
|---|---|---|---|
| 0–5 | Hatalı cümle avı | Tahtaya 2 hatalı cümle | Görsel gerekmez, merak yeter |
| 5–20 | Kural posteri | `/punctuation-poster`, `/verb-lanes`, `/word-class-cards` | Poster ders boyu asılı kalır |
| 20–33 | Üretim etkinliği | `/worksheet-student` | Öğrenci kendi cümlesini yazar |
| 33–40 | Akran kontrolü | Komşuyla kâğıt değişimi + kontrol listesi | Komşu, kurala göre kontrol eder |

## Neye dikkat edilmeli?

Posterdeki örnek ile öğrencinin üreteceği cümle türü aynı olsun. Yazı denetimi iki katmanlıdır: öğretmenin posteri (§995) ve öğrencinin cümlesi.

---

# 2909. `/lesson-sosyal` — Sosyal Bilgiler Dersi Akışı (40′)

## Hedef

Öğrenci harita ve şeridi okur, bilgiyi kendi cümlesiyle özetler.

| Dakika | Adım | Kısayol | Üretim notu |
|---|---|---|---|
| 0–5 | Harita tahmini | `/regions-map` kapağı kapalı soru | “Sence bu bölge neden sarı?” |
| 5–20 | Harita + şerit | `/regions-map`, `/civ-strip`, `/climate-zones` | Lejant birlikte okunur |
| 20–33 | Eşleştirme | `/matching-weather` diliyle eşleştirme föyü | Simge-bilgi eşleşmesi ölçülür |
| 33–40 | Özet cümlesi | `/exit-ticket` | “Bugün öğrendiğim 1 şey” |

## Neye dikkat edilmeli?

Harita okuryazarlığı adım adım kurulur: önce lejant, sonra simge, sonra yorum. Doğrudan yoruma atlanırsa ezber başlar.

---

# 2910. `/lesson-ingilizce` — İngilizce Dersi Akışı (40′)

## Hedef

Öğrenci kalıbı duyar, görür, söyler ve yazar.

| Dakika | Adım | Kısayol | Üretim notu |
|---|---|---|---|
| 0–5 | Dinleme çengeli | Öğretmen sesi + `/vocab-cards` | Görsel sesi destekler, tersi değil |
| 5–20 | Kalıp panosu | `/tense-lanes`, `/dialogue-comic` | Kalıp tahtada sabit kalır |
| 20–33 | Eşli konuşma | `/dialogue-comic` rolleri | Öğrenciler rolleri değişir |
| 33–40 | Mini yazma | `/exit-ticket` | 2 cümleyle günlüğe yazılır |

## Neye dikkat edilmeli?

Görsel, sesi bastırmasın: dinleme anında pano kapalı olabilir. Yazım aşamasına geçmeden sözlü üretim tamamlanır.

---

# 2911. `/lesson-muzik` — Müzik Dersi Akışı (40′)

## Hedef

Öğrenci ritmi görür, çalar, yazar.

| Dakika | Adım | Kısayol | Üretim notu |
|---|---|---|---|
| 0–5 | Ritim yankısı | Öğretmen çalar, sınıf tekrarlar | Görselsiz başlanır |
| 5–20 | Nota panosu | `/rhythm-bars`, `/note-ladder` | Pano enstrümanla birlikte okunur |
| 20–33 | Grup icrası | `/instrument-families` rolleri | Her grup bir aileyi çalar |
| 33–40 | Dinleme günlüğü | `/exit-ticket` | “En zor ritim ve neden” |

## Neye dikkat edilmeli?

Pano ile icra aynı anda olmaz: önce bak-dınle, sonra çal. Ritim kartları enstrümana göre seçilsin, piyanoya davul ritmi verilmesin.

---

<a id="aile-149"></a>
# Sınıf Yönetimi, Ölçme ve Veli İletişimi

Ders akışlarının (§aile-148) kullandığı yan ürünler burada tam preset olur: çıkış kartı, rubrik, pano ve bültenler. Ortak kural: yönetim görseli ceza değil davet diliyle yazılır; ölçme görseli öğretimi değil öğrenmeyi ölçer; veli görseli tek bakışta anlaşılır.

---

# 2912. `/rules-poster` — Sınıf Kuralları Posteri

## Türkçe prompt

> Sınıf kurallarını poster olarak göster: 5 olumlu cümle (“Söz alarak konuşuruz” gibi), her kuralda minik sahne; yasak dili (“yapma”, “etme”) kullanılmasın. Poster kapı yanına asılacak boyutta okunur olsun.

## English

> Show classroom rules as a poster: 5 positively phrased rules (e.g., “Söz alarak konuşuruz”) each with a tiny scene, avoiding prohibitive language. Keep it legible at door-side size.

## Neye dikkat edilmeli?

Kurallar sınıfça belirlenmiş gibi dursun; tepeden inme liste aidiyet üretmez. Olumlu cümle kuralı katıdır, tek “yapma” posteri bozar.

---

# 2913. `/seating-chart` — Oturma Planı

## Türkçe prompt

> [SINIF] için oturma planı şeması hazırla: sıra düzeni kuşbakışı, her koltukta isim kartı alanı boş bırakılsın; öğretmen masası ve tahta konumu işaretli olsun. Plan fotokopiye uygun sade çizgide olsun.

## English

> Prepare a seating-chart diagram for [CLASS]: a top-down desk layout with blank name-card slots per seat, marking the teacher's desk and board. Keep lines plain and photocopy-friendly.

## Neye dikkat edilmeli?

İsimler elle yazılacağı için kart alanları boş ve yeterli büyüklükte olsun. Plan sınıfın gerçek ölçüsüne uysun.

---

# 2914. `/duty-board` — Görev Panosu

## Türkçe prompt

> Haftalık sınıf görev panosu hazırla: tahta silgisi, dosya dağıtımı, bitki sulama ve pano düzeni görevleri; her görevde sorumlu adı için boş kart ve gün sütunları olsun. Görevler adil dağılacak yapıda sunulsun.

## English

> Build a weekly classroom duty board: board cleaning, file distribution, plant watering, and display duties, each with blank name cards and day columns. Structure duties for fair rotation.

## Neye dikkat edilmeli?

Rotasyon şeması panoda görünsün; aynı isimler aynı görevde takılı kalmasın. Kartlar silinebilir-yazılabilir malzemeye uygun boyutta olsun.

---

# 2915. `/exit-ticket` — Çıkış Kartı

## Türkçe prompt

> Ders çıkışı için çıkış kartı (exit ticket) şablonu hazırla: “Bugün öğrendiğim 1 şey”, “Hâlâ kafama takılan 1 soru” ve isim satırı; kart A6 boyutunda, kesim çizgili olsun.

## English

> Build an exit-ticket template for lesson endings: “1 thing I learned today”, “1 question still on my mind”, and a name line, sized A6 with cut lines.

## Neye dikkat edilmeli?

Kart 2 dakikada doldurulur uzunlukta olsun; uzun kart kuyruk yapar. Sorular öğretmenin ertesi ders planını beslesin, arşivde çürümesin.

---

# 2916. `/rubric-visual` — Görsel Rubrik

## Türkçe prompt

> [ÖDEV / PROJE] için 3 düzeyli görsel rubrik hazırla: her ölçütte “başlangıç”, “gelişiyor”, “hedefte” sütunları; her hücrede tek cümlelik gözlenebilir davranış yazsın. Öğrenci dili kullanılsın.

## English

> Build a 3-level visual rubric for [ASSIGNMENT / PROJECT]: “starting”, “developing”, and “on-target” columns per criterion with one observable behavior sentence per cell. Use student language.

## Neye dikkat edilmeli?

Davranışlar gözlenebilir olsun; “güzel olmuş” gibi öznel ifadeler rubriğe giremez. Düzeyler arası fark tek bakışta anlaşılsın.

---

# 2917. `/merit-badge` — Başarı Rozeti

## Türkçe prompt

> [DAVRANIŞ / BECERİ] için başarı rozeti tasarla: rozet formu, kısa unvan (“Kitap Kurdu” gibi) ve okul adı alanı; rozet deftere yapıştırılacak boyutta olsun. Tasarım sevinç versin, rütbe hissi vermesin.

## English

> Design a merit badge for [BEHAVIOR / SKILL]: a badge shape with a short title (e.g., “Kitap Kurdu”) and a school-name field, sized for notebooks. Make it joyful, not rank-like.

## Neye dikkat edilmeli?

Rozet davranışı ödüllendirsin, çocuğu etiketlemesin. Unvan yazımı harf harf denetlenir.

---

# 2918. `/parent-newsletter` — Veli Bülteni

## Türkçe prompt

> [DÖNEM] veli bülteni tek sayfa tasarla: bu ayın konuları, evde destek önerileri ve önemli tarihler 3 blokta; dil sade ve davetkâr olsun. Okuma süresi 2 dakikayı geçmesin.

## English

> Design a one-page parent newsletter for [TERM]: this month's topics, home-support tips, and key dates in 3 blocks, in plain inviting language. Keep reading time under 2 minutes.

## Neye dikkat edilmeli?

Jargon kullanılmasın; “kazanım” yerine “çocuğunuz şunu öğrenecek” yazılsın. Tarihler okul takvimiyle birebir tutsun.

---

# 2919. `/homework-board` — Ödev Panosu

## Türkçe prompt

> Haftalık ödev panosu şablonu hazırla: gün sütunları, ders satırları ve teslim kutucukları; pano uzaktan okunur büyüklükte olsun. Boş şablon fotokopiye uygun olsun.

## English

> Build a weekly homework-board template: day columns with subject rows and hand-in checkboxes, legible from a distance. Keep the blank template photocopy-friendly.

## Neye dikkat edilmeli?

Yazı boyutu en arka sıradan okunsun. Ders renkleri pano genelinde tutarlı olsun.

---

# 2920. `/announce-poster` — Duyuru Posteri

## Türkçe prompt

> [ETKİNLİK] için okul duyuru posteri tasarla: ne-nerede-ne zaman üçlüsü büyük ve ilk bakışta okunur; ayrıntı küçük yazıyla altta olsun. Poster koridor mesafesinden dikkat çeksin.

## English

> Design a school announcement poster for [EVENT]: a big at-a-glance what-where-when trio with details in small type below. Make the poster catch attention from corridor distance.

## Neye dikkat edilmeli?

Üçlü bilgi eksiksiz olsun; eksik saatli duyuru işe yaramaz. Tarih ve yer okul kayıtlarıyla tutsun.

---

# 2921. `/class-calendar` — Sınıf Takvimi

## Türkçe prompt

> [AY] için sınıf takvimi şablonu hazırla: sınav, gezi ve teslim tarihleri işaretli; her hafta satırında küçük not alanı olsun. Takvim pano boyutunda okunur olsun.

## English

> Build a classroom calendar template for [MONTH]: exams, trips, and deadlines marked, with a small note area per week row. Keep it legible at display size.

## Neye dikkat edilmeli?

Tarihler okul takvimiyle birebir tutsun; çelişen takvim güveni bitirir. Yazı alanı elle yazmaya uygun büyüklükte olsun.

---

<a id="aile-150"></a>
# Öğrenci Prompt Okuryazarlığı — Öğrenciye Prompt Yazmayı Öğretmek

Bu aile öğretmene değil, öğretmen aracılığıyla öğrenciye seslenir; sınıf panosuna asılacak ya da deftere yapıştırılacak dildedir. Altın kural §2655'tendir: gerçek yüz yok, kişisel fotoğraf yok, konu öğretmen onaylı. Güvenlik kuralı her bölümde tekrarlanır çünkü tekrar, bu yaş grubunda yöntemdir.

---

# 2922. `/prompt-parts` — Promptun Üç Parçası

## Türkçe prompt

> Öğrencilere promptun üç parçasını öğreten poster hazırla: KONU (ne çizilecek), BİÇİM (nasıl gösterilecek) ve KURAL (ne yapılmayacak); her parça için bir örnek cümle olsun. Poster ilkokul 4. sınıf düzeyinde sade dille yazılsın.

## English

> Build a poster teaching students the three parts of a prompt: SUBJECT (what to draw), FORM (how to show it), and RULE (what not to do), with one example sentence per part. Write at 4th-grade reading level.

## Neye dikkat edilmeli?

Örnekler öğrencinin dünyasından olsun (uçurtma, kedi, okul); soyut örnek kuralı öğretmez. Güvenlik kuralı posterde sabit dursun: gerçek yüz yok.

---

# 2923. `/safe-prompt` — Güvenli Prompt Kuralları

## Türkçe prompt

> Öğrenciler için güvenli prompt kuralları posteri hazırla: gerçek kişi fotoğrafı kullanma, adres-okul adı yazma, korkutucu ve şiddetli içerik isteme, öğretmenin onaylamadığı konuya girme; her kuralda doğru-yanlış mini sahne olsun.

## English

> Build a safe-prompting rules poster for students: no real-person photos, no addresses or school names, no scary or violent content, and no unapproved topics, each rule as a do/don't mini scene.

## Neye dikkat edilmeli?

Korkutma dili kullanılmasın; kurallar koruyucu tonda anlatılsın (§2902 dili). Poster her bilgisayar başında görünür olsun.

---

# 2924. `/prompt-fix-game` — Bozuk Promptu Düzelt Oyunu

## Türkçe prompt

> “Bozuk promptu düzelt” oyunu için 6 kart hazırla: her kartta zayıf bir prompt (“güzel bir şey çiz”) ve 3 düzeltme seçeneği; doğru seçenek biçimi netleştiren olsun. Kartlar oyun hamuru kıvamında eğlenceli dille yazılsın.

## English

> Build 6 cards for a “fix the broken prompt” game: each card with a weak prompt (“güzel bir şey çiz”) and 3 fix options, the correct one clarifying the form. Write cards in playful game language.

## Neye dikkat edilmeli?

Doğru cevap tek ve açık olsun; iki doğru şık tartışmayı oyundan çalar. Kartlar seviyeye uygun kısalıkta olsun.

---

# 2925. `/my-first-poster` — İlk Posterim Şablonu

## Türkçe prompt

> Öğrencinin ilk posteri için doldurmalı şablon hazırla: KONU, BİÇİM ve KURAL satırları boş; altta “öğretmen onayı” kutucuğu olsun. Şablon A5 boyutunda, fotokopiye uygun olsun.

## English

> Build a fill-in template for a student's first poster: blank SUBJECT, FORM, and RULE lines with a “teacher approval” checkbox below. Size A5 and photocopy-friendly.

## Neye dikkat edilmeli?

Onay kutucuğu atlanamayacak konumda olsun; onaysız üretim oyunun dışındadır. Satırlar ilkokul el yazısına uygun genişlikte olsun.

---

# 2926. `/prompt-journal` — Prompt Günlüğü

## Türkçe prompt

> Öğrenci prompt günlüğü sayfa şablonu hazırla: yazdığım prompt, çıkan sonuç, neyi beğendim, neyi değiştiririm — 4 kutulu; sayfa haftalık kullanılır. Dil günlük konuşma tonunda olsun.

## English

> Build a student prompt-journal page template: my prompt, the result, what I liked, what I'd change — 4 boxes for weekly use. Keep a conversational tone.

## Neye dikkat edilmeli?

Günlük notla değil resimle de tutulabilsin; çizim kutusu yazı kadar yer kapsasın. Öğretmen günlüğü okur, not vermez — kural sayfada yazsın.

---

### Üçüncü grup (A/B)

Aynı yöntemle üç örnek daha (§2637–2638 protokolü).

---

# 2927. Çalışılmış örnek: `/photo-to-board-game` — masa oyunu A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı fotoğrafı iki modelde `/photo-to-board-game` ile dönüştürüp farkları kaydetmek. Açılım promptu §2124'tedir.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/photo-to-board-game — use the uploaded photo as theme reference, playable board, readable rules area`

### Nano Banana varyantı

> Yüklenen fotoğrafı tema referansı olarak kullan. Fotoğraftan oynanabilir masa oyunu tasarla: rota, oyun taşları, zar alanı ve kısa kural bölümü okunabilir olsun.

## Beklenen fark

- Oynanabilirlikte Nano Banana fiziksel mantığa daha çok uyar; ChatGPT görsel afişe kayabilir.
- Kural metinleri iki modelde de bozulabilir; kısa tutulur ve denetlenir.

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: oyun gerçekten oynanır mı, tema fotoğrafla bağlı mı, yazılar okunur mu? Oynanmayan oyun posterdır, masa oyunu değil.

### Sonuç görseli

`images/ab-10-boardgame-chatgpt.png`  
`images/ab-10-boardgame-nanobanana.png`

---

# 2928. Çalışılmış örnek: `/mirror-selfie` — ayna selfie'si A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı selfie'yi iki modelde `/mirror-selfie` ile dönüştürüp farkları kaydetmek. Açılım promptu §2307'dedir.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/mirror-selfie — keep identity and outfit, coherent mirror reflection, visible phone`

### Nano Banana varyantı

> Yüklenen selfie'yi kimlik referansı olarak kullan. Gerçek ayna selfie'si üret: yansımada telefonu tutan el, flaş parlaması ve ters yazılar tutarlı olsun; kimlik ve kıyafet korunsun.

## Beklenen fark

- Yansıma geometrisinde iki model de hata yapar; hangisinin daha tutarlı olduğu kare kare değişir, genelleme yapılmaz.
- Kimlik cümlesi iki modelde de açık yazılmalı.

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: yansıma geometrisi tutarlı mı, yazılar ters mi, kimlik korunmuş mu? Düz görünen yazı hatalıdır (aile-085).

### Sonuç görseli

`images/ab-11-mirror-chatgpt.png`  
`images/ab-11-mirror-nanobanana.png`

---

# 2929. Çalışılmış örnek: `/tiny-world-jar` — kavanoz dünya A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı sahneyi iki modelde `/tiny-world-jar` ile dönüştürüp farkları kaydetmek. Açılım promptu §2329'dadır.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/tiny-world-jar — source scene inside a glass jar, preserve layout, real scale cue`

### Nano Banana varyantı

> Yüklenen sahneyi cam kavanoz içinde minyatür dünyaya dönüştür: kaynak yerleşim korunsun, kavanoz camı ve kapak fiziksel olsun; ölçek için tek gerçek boyutlu referans nesne eklensin.

## Beklenen fark

- Cam fiziğinde (yansıma, kırılma) iki model de zorlanır; sade cam daha güvenli sonuç verir.
- Ölçek kanıtı unutulursa minyatür okunmaz; referans nesne cümlesi iki promptta da durmalı.

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: yerleşim korunmuş mu, cam inandırıcı mı, ölçek okunur mu? Cam abartılırsa sahne görünmez.

### Sonuç görseli

`images/ab-12-tinyworld-chatgpt.png`  
`images/ab-12-tinyworld-nanobanana.png`

---

<a id="aile-151"></a>
# Branş Paketleri — Hazır Kısayol Demetleri

Bu ailede yeni kısayol icat edilmez; her bölüm bir branşın en sık kullanacağı mevcut presetleri tek demette toplar. Paket, dönemin ilk haftası öğretmene verilir; öğretmen yıl boyu bu demetten seçer. Her pakette 6 kısayol ve her biri için tek cümlelik “ne zaman” notu vardır.

---

# 2930. Fen Paketi — 6 Kısayol

- `/cell-compare` — hücre karşılaştırma gerektiğinde (§2847).
- `/circuit-pair` — elektrik devrelerinde (§2848).
- `/friction-strip` — deney föyü hazırlanırken (§2849).
- `/worksheet-student` — öğrenci etkinlik sayfası için (§1288).
- `/exit-ticket` — ders çıkışı kontrolü için (§2915).
- `/digestion-journey` — sistemler ünitesinde (§2850).

## Neye dikkat edilmeli?

Paket dışına taşan ihtiyaçta yeni ad icat edilmez; önce galeri (§aile-141) ve katalog taranır. Paketteki her kısayol dönem başında bir kez test edilir.

---

# 2931. Matematik Paketi — 6 Kısayol

- `/fraction-circles` — kesir anlatımında (§2852).
- `/solid-nets` — cisim açılımında (§2853).
- `/bar-chart-read` — grafik okumada (§2854).
- `/area-grid` — alan ölçmede (§2856).
- `/worksheet-student` — alıştırma seti için (§1288).
- `/exit-ticket` — “kuralı bir cümleyle yaz” çıkışı için (§2915).

## Neye dikkat edilmeli?

Modelle alıştırma aynı örnekle başlar; paketteki sıra (model → alıştırma → çıkış) bozulmaz.

---

# 2932. Türkçe Paketi — 6 Kısayol

- `/punctuation-poster` — noktalama haftasında (§2866).
- `/verb-lanes` — kip-zaman karşılaştırmada (§2867).
- `/idiom-cards` — deyim serisinde (§2868).
- `/word-class-cards` — sözcük türlerinde (§2870).
- `/worksheet-student` — üretim etkinliği için (§1288).
- `/exit-ticket` — akran kontrolü sonrası çıkış için (§2915).

## Neye dikkat edilmeli?

Posterdeki örnekle öğrencinin üreteceği cümle türü aynı tutulur. Yazı denetimi iki katmanlıdır.

---

# 2933. Sosyal Bilgiler Paketi — 6 Kısayol

- `/regions-map` — bölgeler ünitesinde (§2871).
- `/civ-strip` — uygarlıklar şeridinde (§2872).
- `/climate-zones` — iklim tiplerinde (§2874).
- `/economy-symbols` — ekonomik faaliyetlerde (§2875).
- `/worksheet-student` — eşleştirme föyü için (§1288).
- `/exit-ticket` — özet cümlesi çıkışı için (§2915).

## Neye dikkat edilmeli?

Harita okuryazarlığı sırayla kurulur: lejant, simge, yorum. Doğrudan yoruma atlanmaz.

---

# 2934. İngilizce Paketi — 6 Kısayol

- `/vocab-cards` — ünite kelimelerinde (§2876).
- `/tense-lanes` — zamanlar karşılaştırmada (§2877).
- `/dialogue-comic` — konuşma etkinliğinde (§2878).
- `/phonics-chart` — ses-harf çalışmasında (§2879).
- `/worksheet-student` — mini yazma için (§1288).
- `/exit-ticket` — 2 cümlelik günlük çıkışı için (§2915).

## Neye dikkat edilmeli?

Görsel sesi bastırmasın; dinleme anında pano kapalı olabilir. Sözlü üretim yazıdan önce tamamlanır.

---

# 2935. Müzik Paketi — 5 Kısayol

- `/rhythm-bars` — ritim kalıplarında (§2881).
- `/note-ladder` — nota öğretiminde (§2883).
- `/instrument-families` — çalgı sınıflandırmada (§2882).
- `/dynamics-signs` — gürlük işaretlerinde (§2884).
- `/exit-ticket` — dinleme günlüğü çıkışı için (§2915).

## Neye dikkat edilmeli?

Pano ile icra aynı anda olmaz: önce bak-dinle, sonra çal.

---

# 2936. Beden Eğitimi Paketi — 5 Kısayol

- `/warmup-cards` — ısınma serisinde (§2886).
- `/movement-sequence` — hareket öğretiminde (§2888).
- `/team-positions` — diziliş şemasında (§2889).
- `/safety-poster` — güvenlik hatırlatmada (§2890).
- `/exit-ticket` — nabız yoklaması çıkışı için (§2915).

## Neye dikkat edilmeli?

Pozlar anatomik olarak mümkün çizilir; eklemi zorlayan görsel derste kullanılmaz.

---

# 2937. Görsel Sanatlar Paketi — 5 Kısayol

- `/color-wheel` — renk bilgisinde (§2891).
- `/perspective-demo` — perspektif anlatımında (§2892).
- `/pattern-design` — örüntü şablonunda (§2893).
- `/portrait-proportions` — oran şemasında (§2894).
- `/printmaking-steps` — baskı sürecinde (§2895).

## Neye dikkat edilmeli?

Şablonlar gerçekten tamamlanabilir zorlukta olur; yapılamayan şablon motivasyonu bitirir.

---

### Dördüncü grup (A/B)

Aynı yöntemle üç örnek daha (§2637–2638 protokolü).

---

# 2938. Çalışılmış örnek: `/fashion-doll` — fashion doll A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı selfie'yi iki modelde `/fashion-doll` ile dönüştürüp farkları kaydetmek. Açılım promptu §2340'tadır.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/fashion-doll — keep identity and outfit colors, physical doll proportions, window-box presentation`

### Nano Banana varyantı

> Yüklenen selfie'yi kimlik referansı olarak kullan. Kişiyi fiziksel fashion doll'a dönüştür: bebek oranları oyuncak mantığına uysun, yüz ve giysi rengi korunsun; pencereli kutuda sunulsun.

## Beklenen fark

- Oyuncak oranlarında iki model de kimi zaman gerçekçi vücuda kayar; kutu sunumu tutarlılığı artırır.
- Giysi rengi iki modelde de ayrıca kilitlenmeli, yoksa bebek “yeniden giydirilir”.

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: yüz tanınır mı, oranlar oyuncak mı, kutu fiziksel mi? Gerçekçi vücutlu “bebek”, bebek değildir.

### Sonuç görseli

`images/ab-13-doll-chatgpt.png`  
`images/ab-13-doll-nanobanana.png`

---

# 2939. Çalışılmış örnek: `/korean-four-cut` — four-cut şerit A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı selfie'yi iki modelde `/korean-four-cut` ile dönüştürüp farkları kaydetmek. Açılım promptu §2361'dedir.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/korean-four-cut — same person across 4 frames, same booth lighting, photo-strip layout`

### Nano Banana varyantı

> Yüklenen selfie'yi kimlik referansı olarak kullan. Aynı kişiyi dörtlü photo-strip'e dönüştür: dört karede yüz, ışık ve kadraj aynı kabinde çekilmiş gibi tutarlı olsun.

## Beklenen fark

- Kare tutarlılığında referans kilidi güçlü olan model öne geçer; sapan kare tek başına üretilir.
- Kabin ışığı iki modelde de stüdyoya kayabilir; flaş sertliği denetlenir.

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: dört karede kimlik aynı mı, ışık sabit mi, kostüm değişmemiş mi? Karelerden biri saparsa set değil o kare yenilenir.

### Sonuç görseli

`images/ab-14-fourcut-chatgpt.png`  
`images/ab-14-fourcut-nanobanana.png`

---

# 2940. Çalışılmış örnek: `/newspaper-front-page` — gazete manşet A/B

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

## Amaç

Aynı fotoğrafı iki modelde `/newspaper-front-page` ile dönüştürüp farkları kaydetmek. Açılım promptu §2370'tedir.

### ChatGPT varyantı

> (fotoğrafı ekleyin) `/newspaper-front-page — front-page layout, short verified headline, no real masthead`

### Nano Banana varyantı

> Yüklenen fotoğrafı gazete ön sayfasına dönüştür: manşet kısa ve doğrulanmış, gerçek gazete logosu kullanılmasın; sayfa düzeni baskı mantığına uysun.

## Beklenen fark

- Manşet yazımında iki model de harf uydurabilir; kısa başlık riski azaltır.
- Gerçek logo taklidi iki modelde de engellenmeli; jenerik masthead istenir.

## Neye dikkat edilmeli?

Her iki çıktıda da bakılacak üç nokta: başlık harf harf doğru mu, logo jenerik mi, sayfa baskı mantığında mı? Sahte-resmiyet izlenimi veren öğe çıkarılır.

### Sonuç görseli

`images/ab-15-news-chatgpt.png`  
`images/ab-15-news-nanobanana.png`

---

<a id="aile-152"></a>
# Hızlı Başlangıç — Rehbere Yeni Giren Öğretmene

Bu aile okuma sırası önerir; 2.900 bölümlük rehber ilk günden taranmaz. Üç bölüm 15 dakika, ilk hafta ve ilk ay ritmini kurar. Yeni kısayol icat edilmez; mevcut bölümlere gönderilir.

---

# 2941. 15 Dakikada İlk Görsel

Rehberi ilk kez açan öğretmen şunu yapar:

1. Branş paketini bulur (aile-151): kendi branşının 5–6 kısayolunu okur.
2. Paketten tek kısayol seçer (örn. `/fraction-circles`), bölümündeki hazır promptu kopyalar.
3. Kendi konusuna uyarlar: yalnız köşeli parantezli yeri değiştirir, geri kalan cümleye dokunmaz.
4. Üretir ve §18'in üç sorusunu sorar: etiket doğru yerde mi, eksik kavram var mı, seviye uygun mu?

## Neye dikkat edilmeli?

İlk gün tek görsel yeterlidir; beş görsel birden üretmek değerlendirme körlüğü doğurur. İlk üretimde üslup cümlesi değiştirilmez.

---

# 2942. İlk Hafta: 5 Preset Kuralı

İlk hafta her ders için en fazla 5 preset kullanılır: 1 kavram görseli, 1 etkinlik föyü, 1 çıkış kartı ve en fazla 2 yedek. Yedekler paketin dışından seçilmez. Hafta sonunda çıkış kartları toplanıp hangi kavramın oturmadığı bulunur; ikinci hafta pakete yalnız o kavramın alternatifi eklenir.

## Neye dikkat edilmeli?

Preset sayısı değil, tekrar ritmi öğretir. Aynı kavram iki farklı presetle değil, aynı preset iki farklı örnekle pekiştirilir.

---

# 2943. Yeni Başlayanların 5 Hatası

1. **Sıfat yığmak:** “güzel, detaylı, muhteşem” yazmak yerine yapı cümlesi eklenir (§17).
2. **Etiketsiz üretmek:** Türkçe etiketsiz görsel sınıfta kullanılmaz; prompta etiket dili yazılır.
3. **Doğrulamadan dağıtmak:** Her görsel §18'den geçmeden öğrenciye ulaşmaz.
4. **Gerçek yüzle denemek:** Denemeler kurgusal özneyle yapılır; öğrenci fotoğrafı ilk gün araca yüklenmez (§2655).
5. **Hepsini bir derste denemek:** Haftada 5 preset sınırı konur (§2942).

## Neye dikkat edilmeli?

Bu liste sınıf panosuna değil, öğretmenin defterine yazılır; hatalar öğretmene aittir, öğrenciye gösterilmez.

---

<a id="aile-153"></a>
# Google Pics ile Ders Görseli Üretimi (Eylül 2026)

Google'ın Eylül 2026'da Workspace'e açtığı Pics aracı, Nano Banana modelini belgenin içine taşır. Bu aile Pics'e özgü iş akışını anlatır; genel prompt dili rehberin tamamında aynıdır. Erişim ve kota bilgileri hızlı değişir; her dönem başı güncel sayfadan doğrulanır.

---

# 2944. Pics'e Giriş — Nerede, Kimler İçin

## Kalıcı

**Kalıcı başvuru bilgisi; model sürümleri değiştikçe güncellenir.**

Pics bağımsız web uygulaması olarak ve Docs/Slides içi panel olarak çalışır; Eylül 2026 itibarıyla duyurusu yapılan Drive entegrasyonunun güncel durumu kontrol edilmelidir. Erişim Google AI Pro/Ultra abonelikleri ile kurumsal Workspace hesaplarına kademeli açılır. Öğretmen için anlamı: mevcut lisans kapsamına göre ek lisans gerekmeyebilir; güncel paket koşulları doğrulanmalıdır.

## Neye dikkat edilmeli?

Kişisel hesapla kurum hesabının yetkisi farklı olabilir; ders dosyasına geçmeden önce okul hesabında erişim test edilir. Öğrenci verisi içeren dosyalarda kurumun veri politikası geçerlidir (§2655).

---

# 2945. Docs İçinde Kavram Görseli Üretme

İmlecin bulunduğu yere Pics panelinden doğal dille istek yazılır; örneğin bu rehberdeki hazır promptlardan biri (`/cell-compare` açılımı gibi) aynen yapıştırılır. Görsel belgeye doğrudan yerleşir; beğenilmeyen sonuç aynı panelden, belge değiştirilmeden yeniden üretilir.

## Neye dikkat edilmeli?

Belgeye yerleşen her görsel §18'den geçirilir (etiket, eksik kavram, seviye); hızlı üretim hızlı doğrulamayı ortadan kaldırmaz. Etiket dili promptta açıkça yazılır, sonradan eklenmez.

---

# 2946. Slides İçinde Sunum Görseli Döngüsü

Slaytın notuna istenen görsel yazılır, üretim slayta yerleşir; revizyon “şunu değiştir” cümlesiyle aynı panelden yapılır. Tutarlı seri için (aynı ünitenin 5 slaytı) ilk onaylanan görsel referans gösterilerek devam edilir (§2625 mantığı).

## Neye dikkat edilmeli?

Seride stil kayması olursa referans kare sabitlenip slaytlar tek tek üretilir. Slayt oranı (16:9/4:3) üretimden önce seçilir; sonradan kırpma kompozisyonu bozar.

---

# 2947. Nesne Ayırma ile Düzenleme

Pics'in ayırt edici işlevi nesne ayırmadır (object segmentation): görseldeki tek öğe seçilip yalnız o değiştirilir, geri kalan korunur. Kullanım: Düzeltilecek öğe adlandırılır (“soldaki ikinci etiket”), değişiklik tek cümleyle yazılır; §19'un tek değişiklik disiplini burada da geçerlidir.

## Neye dikkat edilmeli?

Ayırma her dokuda çalışmaz; ince detay ve iç içe nesnelerde seçim taşar. Taşma olursa bölge büyütülüp yeniden seçilir, tüm görsel baştan üretilmez.

---

# 2948. Görseldeki Yazıyı Düzeltme ve Çevirme

Pics görseldeki yazıyı fontu koruyarak düzeltir ve çevirir. Kullanım: Düzeltilen kelime tırnak içinde aynen yazılır, yeni metin ayrıca verilir. Türkçe karakterler (ğ, ş, ı, ç) düzeltme sonrası harf harf denetlenir (§995 kuralı).

## Neye dikkat edilmeli?

Uzun cümlelerin düzeltilmesi harf uydurma riskini artırır; başlık ve etiket kısa tutulur. Çeviride anlam kayması öğretmence denetlenir, modele bırakılmaz.

---

# 2949. Varyant Üretimi ve Seçim Disiplini

Pics tek prompttan çoklu varyant üretir. Kullanım: 3–4 varyant istenir, seçim §18'in üç sorusuyla yapılır (etiket, eksik kavram, seviye). Seçilmeyen varyantlar silinir; arşivde “belki kullanılır” dosyası biriktirilmez.

## Neye dikkat edilmeli?

Varyant çokluğu karar yorgunluğu doğurur; tur başına tek seçim yapılır. Seçilen görselin promptu ve tarihi kaydedilir (A/B kaydı, §2637).

---

<a id="aile-154"></a>
# Pedagojik Derinleştirme — Neden Bu Biçim?

Bu aile, biçim seçimlerinin altındaki öğrenme bilimini metin düzeyinde toplar. Yeni kısayol icat edilmez; mevcut bölümlere gerekçe ve sınır eklenir. Dördü de üretimden önce okunur, üretimden sonra kontrol listesi gibi kullanılır.

---

# 2950. Bilişsel Yük Kontrol Listesi (Mayer İlkeleriyle)

Çoklu ortamla öğrenme araştırmasının (Mayer) prompt karşılığı:

- [ ] **Gereksizi ele:** Konuyla ilgisiz her öğe silinir (slop filtresi §163'ün pedagojik adı budur).
- [ ] **İşaretle:** Önemli öğe ok, renk ya da numarayla vurgulanır; vurgusuz görselde öğrenci neye bakacağını bilemez.
- [ ] **Yakın tut:** Etiket, gösterdiği yapıya bitişik durur; lejant avı bilişsel yükü artırır.
- [ ] **Böl:** Karmaşık süreç tek kareye değil, adım dizisine bölünür (§9, §60).
- [ ] **Önce sözlü, sonra yazılı:** Anlatım görseli, açıklama metninden önce gelir; ikisi aynı anda verilmez.

## Neye dikkat edilmeli?

Bu liste §18'in yerine değil, önüne geçer: önce yük azaltılır, sonra doğruluk denetlenir. Beş maddenin üçü tutmuyorsa biçim değiştirilir (§19).

---

# 2951. Kavram Yanılgısı Kalkanı

Modellerin görselde pekiştirdiği klasik yanılgılar ve engelleyici cümleler:

| Yanılgı | Engelleyici prompt cümlesi |
|---|---|
| Mevsimler Güneş'e uzaklıktan olur | “Mevsimlerin eksen eğikliğinden kaynaklandığı not olarak yazılsın; uzaklık gösterilmesin” |
| Hücredeki her şey aynı boyuttadır | “Organel boyutları birbirine oranlı olsun” |
| Devre telleri enerjiyi taşır gibi akar | “Akım yönü okla, elektron abartısı olmadan gösterilsin” |
| Evrim merdivendir | “Dallanma ağaç olarak çizilsin, basamak dizisi olmasın” |
| Güneş-Dünya-Ay gerçek ölçektedir | “Ölçek temsili olduğu görselde belirtilsin” |
| Harita sınırı keskindir | “Yaklaşık sınır olduğu lejantta yazsın” |

## Neye dikkat edilmeli?

Tablo çekirdek listedir; öğretmenin branşındaki kritik yanılgılar listeye eklenir. Yanılgı cümlesi prompta aynen yazılır, ima edilmez.

---

# 2952. Bloom Düzeyi × Biçim Matrisi

Hedef düzeye göre biçim seçilir; konu kadar düzey de belirleyicidir:

| Düzey | Uygun biçimler | Örnek kısayol |
|---|---|---|
| Hatırlama | Etiketli şema, kart destesi | `/label-lock` düzeni, kart destesi |
| Anlama | Kavram haritası, karşılaştırma | Kavram haritası (§24), `/cell-compare` |
| Uygulama | Worksheet, doldurulabilir diyagram | `/worksheet-student`, `/fillable-diagram` |
| Analiz | Önce/sonra, neden-sonuç | `/matched-pair`, neden-sonuç diyagramı (§54) |
| Değerlendirme | Rubrik, akran kontrolü | `/rubric-visual`, `/exit-ticket` |
| Yaratma | Öğrenci üretimi posteri | `/my-first-poster`, `/prompt-journal` |

## Neye dikkat edilmeli?

Düzey atlanmaz: değerlendirme görseli, hatırlama görseli olmadan verilmez. Matris ders planına (§aile-148) düzey sütunu olarak eklenir.

---

# 2953. UDL Uyarlamaları — Herkes İçin Görsel

Evrensel tasarım (UDL) için prompta eklenen değiştirici cümle kalıpları:

- **Dikkat yükünü azaltma (DEHB):** “Tek karede tek fikir olsun; yan öğe ve dekoratif detay kullanılmasın.”
- **Okuma yükünü azaltma (disleksi):** “Yazılar kısa ve büyük olsun; satır arası geniş, zemin-yazı kontrastı yüksek olsun.”
- **Adım bölme:** “Süreç en fazla 4 adıma bölünsün; her adım numaralı olsun.”
- **Tahmin edilebilirlik:** “Düzen soldan sağa, yukarıdan aşağıya okunsun; sürpriz yerleşim olmasın.”
- **Duyusal hassasiyet:** “Yüksek kontrastlı neon ve yanıp sönen öğe kullanılmasın.”

## Neye dikkat edilmeli?

Uyarlama, basitleştirme değildir: kavram korunur, yük azaltılır. Sınıfın ihtiyacı bilinmiyorsa en sade sürüm varsayılan yapılır.

---

<a id="aile-155"></a>
# Ders Konu Galerileri — Okul Öncesi

Galeri dizisinin en küçük yaş grubudur; kalıp aynıdır ama kurallar serttir: yazı en aza iner, tek karede tek kavram olur, yönergeler öğretmene Türkçedir (çocuk okumaz, bakar ve yapar). UDL ilkeleri (§2953) burada varsayılandır, istisna değil.

---

# 2954. `/toddler-colors` — Renkleri Öğreniyorum (Okul Öncesi)

## Seviye

36–72 ay — Renk kavramı.

## Türkçe prompt

> Okul öncesi için renk posteri hazırla: 4 ana renk (kırmızı, mavi, sarı, yeşil) büyük dairelerle; her dairenin içinde o renkte tek nesne (elma, balon gibi) olsun. Yazı yalnız renk adından ibaret, büyük harflerle olsun.

## English

> Prepare a color poster for preschool: 4 main colors (red, blue, yellow, green) as large circles, each containing one object in that color (apple, balloon). Keep text to color names only, in capital letters.

## Neye dikkat edilmeli?

Nesne-rengi eşleşmesi tartışmasız olsun; çilek kırmızısı yerine elma kırmızısı gibi net örnekler seçilsin. Ton farkı bu yaşta öğretilmez, tek ton kullanılır.

---

# 2955. `/shape-hunt` — Şekil Avı (Okul Öncesi)

## Türkçe prompt

> Okul öncesi için şekil avı sayfası hazırla: daire, kare, üçgen ve dikdörtgen büyük ve renkli; sayfanın altında “sınıfta bul” görevi için boş kutucuklar olsun. Şekiller kalın konturlu ve içleri boş olmasın.

## English

> Prepare a shape-hunt page for preschool: big colorful circle, square, triangle, and rectangle, with empty checkboxes below for a “find in class” task. Keep shapes thick-outlined and filled.

## Neye dikkat edilmeli?

Şekiller standart oryantasyonda olsun (üçgen tepesi yukarıda); döndürülmüş şekil bu yaşta ayrı şekil sanılır. Görev kutucukları parmakla işaretlenecek büyüklükte olsun.

---

# 2956. `/animal-sounds` — Hayvan Sesleri (Okul Öncesi)

## Türkçe prompt

> Okul öncesi için hayvan sesleri kartları hazırla: 6 kart, her kartta bir hayvan illüstrasyonu ve ses taklidi (“möö”, “hav hav”); hayvanlar sevimli ama gerçek türüne uygun çizilsin.

## English

> Prepare animal-sound cards for preschool: 6 cards, each with one animal illustration and its sound word (“möö”, “hav hav”); draw animals cute but true to species.

## Neye dikkat edilmeli?

Ses kelimeleri Türkçe çocuk dilindeki halleriyle yazılsın. Hayvan türü doğru olsun; kedi-köpek karışıklığı bu yaşta kalıcı olur.

---

# 2957. `/weather-window` — Hava Durumu Penceresi (Okul Öncesi)

## Türkçe prompt

> Okul öncesi için hava durumu penceresi posteri hazırla: güneşli, yağmurlu, karlı ve rüzgârlı 4 pencere; her pencerede hava ve uygun giysi (şemsiye, atkı) birlikte gösterilsin.

## English

> Prepare a weather-window poster for preschool: 4 windows for sunny, rainy, snowy, and windy weather, each showing the weather with matching clothing (umbrella, scarf).

## Neye dikkat edilmeli?

Hava-giysi eşleşmesi doğru olsun; güneşli pencereye bot konulmasın. Pencereler günlük kontrol için mıknatıslı kart düzeninde düşünülerek tasarlansın.

---

# 2958. `/story-seed` — Hikâye Tohumu (Okul Öncesi)

## Türkçe prompt

> Okul öncesi hikâye anlatımı için tek sahnelik “hikâye tohumu” görseli hazırla: merak uyandıran tek sahne (ormanda kapı, gökte balon sepeti), soru cümlesi öğretmene ait ayrı kartta olsun. Sahne mutlu ve güvenli hissetsin.

## English

> Prepare a single-scene “story seed” visual for preschool storytelling: one intriguing scene (a door in the forest, a balloon basket in the sky) with the prompt question on a separate teacher card. Keep the scene happy and safe.

## Neye dikkat edilmeli?

Sahnede korku öğesi olmasın; karanlık, diş ve keskin nesnelerden kaçınılır. Soru kartı çocuğa değil öğretmene yazılır.

---
