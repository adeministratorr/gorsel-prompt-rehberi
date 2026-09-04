> [← Genel İçindekiler](gorsel-prompt-rehberi.md) · [Süleyman’a Umut Ol — Dayanışma Çağrısı](gorsel-prompt-rehberi.md#suleymana-umut-ol)

<a id="aile-024"></a>
# Blueprint, Patent Drawing, Teknik Talimat, Xerox ve Scanography — 2026 Ek Taraması

2026'da internette dolaşan görsel prompt listelerinde yeni bir kümelenme çok görünür hâle geldi:

> `/blueprint`
>
> `/schematic`
>
> `/technicaldrawing`
>
> `/diagram`

Bunlar bazı topluluk listelerinde doğrudan slash-prefixed kısa komutlar gibi yazılıyor.

Bu rehberde önceki `/lego` açıklamasında olduğu gibi aynı ayrım korunmalıdır:

> **Bunlar ChatGPT'nin belgelenmiş evrensel resmî image command'ları değildir.**
>
> İnternette kullanılan **prompt shorthand / preset label** biçimleridir.

Özellikle teknik çizimde ikinci bir uyarı daha önemlidir:

> **AI-generated technical-looking image ≠ manufacturing drawing.**

Bir image model:

- görünüş planlayabilir,
- teknik çizim dilini taklit edebilir,
- parçaları açıklayabilir,
- callout sistemi önerebilir,

ancak tek bir fotoğraftan güvenilir:

- ölçü,
- tolerans,
- GD&T,
- malzeme,
- üretim detayı

çıkardığı varsayılmamalıdır.

2026'da yayımlanan teknik çizim rehberleri de aynı ayrımı açıkça yapıyor: modelin “üretime hazır boyutlandırılmış teknik resim” verdiğini varsaymak yerine, geometri ve standartların gerçek CAD/ölçüm verisiyle doğrulanması gerekir.

---

# 1701. `/blueprint` — Blueprint Görsel Dili

## Topluluk kısayolu

`/blueprint`

## Teknik anlam

Blueprint tarihsel olarak belirli çoğaltma süreçlerinden gelen bir teknik çizim türüdür. Güncel prompt kullanımında ise çoğunlukla:

> teknik çizgi + ölçü/callout hissi + mavi/beyaz görsel dil

anlamında kullanılır.

## Türkçe prompt

> [NESNE/YAPI]'yı teknik blueprint presentation olarak göster.
>
> Kullan:
>
> - temiz orthographic veya isometric görünüm,
> - ince teknik çizgiler,
> - yalnız gerekli center/construction çizgileri,
> - kısa part callout'lar,
> - sade title area.
>
> Ölçüler gerçek veri verilmediyse sayı uydurma.
>
> “Blueprint” görünmesi için bütün yüzeyi grid, formül ve sahte ölçülerle doldurma.

## English

> Present [OBJECT/STRUCTURE] as a technical blueprint-style drawing using a clean orthographic or isometric view, restrained technical linework, only necessary construction lines, concise part callouts, and a simple title area.
>
> Do not invent dimensions when real measurements are not supplied.
>
> Avoid filling the page with decorative grids, equations, and fake measurements.

## Neye dikkat edilmeli?

Çizgi kalınlıkları ve ölçülendirme tek sisteme uysun; paftadaki her yazı [§995](30-katalog-aile-009-016.md#sec-995)'teki kapak notundaki gibi denetlenir.

---
# 1702. `/exploded-blueprint` — Patlatılmış Blueprint

## Trend

**T1/T2 — 2026 prompt arşivlerinde çok görünür.**

## Türkçe

> Kaynak [ÜRÜN]'ün ana geometrisini koruyarak parçalarını montaj eksenleri boyunca exploded technical view olarak ayır.
>
> Her parça:
>
> - gerçek yerleşim ilişkisini korusun,
> - tek numara taşısın,
> - aynı perspective sisteminde kalsın.
>
> Sağ/alt bölgede kısa parts list olabilir.
>
> Kaynak fotoğrafta görünmeyen iç parçaları gerçekmiş gibi icat etme.

## English

> Preserve the primary geometry of [PRODUCT] and separate its parts along believable assembly axes as an exploded technical view.
>
> Give each component one number and keep every part within the same perspective system.
>
> A concise parts list may appear at the side or bottom.
>
> Do not invent hidden internal components as factual when they are not supported by the source.

---

# 1703. `/patent-drawing` — Patent Çizimi Görsel Dili

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [NESNE]'yi patent drawing'den esinlenen siyah-beyaz teknik line illustration olarak göster.
>
> Kullan:
>
> - beyaz arka plan,
> - gölgesiz veya çok sınırlı teknik shading,
> - numaralı callout,
> - farklı görünüşler gerektiğinde ayrı figürler.
>
> Patent numarası, başvuru sahibi veya hukukî belge metni uydurma.
>
> Çıktıyı gerçek patent başvurusu olarak sunma.

## English

> Show [OBJECT] as a black-and-white technical line illustration inspired by patent drawings, using a white background, minimal technical shading, numbered callouts, and separate figures where different views are needed.
>
> Do not invent patent numbers, applicants, or legal-document text.
>
> Do not present the output as a genuine patent filing.

---

# 1704. `/orthographic-drawing` — Ortografik Teknik Görünüş

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [NESNE]'yi aynı scale ve hizalamada:
>
> - front,
> - top,
> - side
>
> orthographic views ile göster.
>
> Perspektif kaçışı kullanma.
>
> Görünüşler aynı nesne geometrisini temsil etsin.
>
> Fotoğraftan bilinmeyen arka/alt geometriyi kesin bilgi gibi üretme.

## English

> Show [OBJECT] in matched front, top, and side orthographic views at one consistent scale and alignment.
>
> Avoid perspective convergence.
>
> Make all views represent the same geometry.
>
> Do not present unknown rear or underside geometry inferred from a single photograph as certain.

---

# 1705. `/dimensioned-drawing` — Boyutlandırılmış Görünüm

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Kritik sınır

Bu prompt:

> **görsel açıklama**

içindir.

Üretime hazır teknik resim değildir.

## Türkçe

> [NESNE]'nin kullanıcı tarafından verilen ölçülerini temiz dimensioned technical drawing üzerinde göster.
>
> Yalnız verilen:
>
> - toplam genişlik,
> - yükseklik,
> - kalınlık,
> - delik aralığı,
> - çap
>
> gibi gerçek ölçüleri kullan.
>
> Eksik ölçüleri tamamlamak için sayı tahmin etme.

## English

> Place only user-supplied dimensions of [OBJECT] on a clean technical drawing, such as overall width, height, thickness, hole spacing, or diameter.
>
> Do not estimate missing dimensions to make the drawing appear complete.

---

# 1706. `/section-hatch` — Teknik Kesit Tarama Dili

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [PARÇA/YAPI]'nın section view'unda kesilen malzeme alanlarını tutarlı hatch ile göster.
>
> Komşu parçaların hatch yönü gerektiğinde farklılaştırılabilir.
>
> Hollow/boş alanı tarama.
>
> Hatch pattern'ı malzeme standardı olarak yorumlanacaksa gerçek teknik standarda göre ayrıca doğrula.

## English

> Use consistent section hatching on cut material areas of [PART/STRUCTURE].
>
> Differentiate adjacent parts where necessary.
>
> Do not hatch hollow space.
>
> Verify any hatch intended to communicate a formal material standard against the relevant drawing convention.

---

# 1707. `/detail-callout` — Büyütülmüş Teknik Detay

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Ana teknik çizim üzerinde kritik [BİRLEŞİM/PARÇA]'yı daire veya sınır ile işaretle ve ayrı büyütülmüş detail view olarak göster.
>
> Ana ve detail görünüş aynı geometriyi taşısın.
>
> Detail görünüşte yeni parça icat etme.

## English

> Mark the critical [JOINT/PART] on the main technical drawing and show it separately as an enlarged detail view.
>
> Preserve the same geometry between the main and detail views.
>
> Do not invent new components inside the detail.

---

# 1708. `/bill-of-materials` — Parts / Bill of Materials Görseli

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ÜRÜN]'ün doğrulanmış parça listesini numbered table olarak göster.
>
> Alanlar:
>
> item no,
> part name,
> quantity,
> material yalnız biliniyorsa.
>
> Parts table'daki numaralar exploded view callout'larıyla bire bir eşleşsin.
>
> Bilinmeyen malzeme ve adetleri tahmin etme.

## English

> Present the verified part list for [PRODUCT] as a numbered table with item number, part name, quantity, and material only when known.
>
> Make item numbers match the exploded-view callouts exactly.
>
> Do not guess materials or quantities.

---

# 1709. `/assembly-manual` — Montaj Kılavuzu

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ÜRÜN] montajını 4–8 adımlık teknik instruction sheet olarak göster.
>
> Her adımda:
>
> - yalnız aktif parçalar,
> - hareket yönü,
> - bağlantı noktası,
> - gerektiğinde tool
>
> gösterilsin.
>
> Aynı parçayı farklı adımlarda farklı geometriyle üretme.
>
> Exploded presentation ile gerçek montaj sırasını karıştırma.

## English

> Show [PRODUCT] assembly as a 4–8 step technical instruction sheet.
>
> At each step show only active parts, movement direction, connection point, and tool where needed.
>
> Preserve component geometry across steps.
>
> Do not confuse an exploded presentation with actual assembly order.

---

# 1710. `/service-manual` — Servis / Bakım Kılavuzu Görseli

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [CİHAZ]'ın belirli [BAKIM İŞLEMİ]'ni servis manual illustration olarak göster.
>
> Sadece işlemle ilgili parçaları vurgula.
>
> Güvenlik gerektiren işlemlerde kullanıcı tarafından sağlanan doğrulanmış prosedürü esas al.
>
> Elektrik, basınç, ısı veya mekanik risk içeren adımları modelin kendi başına uydurmasına izin verme.

## English

> Illustrate the specified [MAINTENANCE TASK] for [DEVICE] in service-manual form, highlighting only the components relevant to the task.
>
> For safety-critical procedures, follow only a verified supplied procedure.
>
> Do not let the image model invent steps involving electrical, pressure, thermal, or mechanical hazards.

---

# 1711. `/instruction-sheet` — Tek Sayfalık Teknik Talimat

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [GÖREV]'i tek sayfalık instruction sheet olarak düzenle.
>
> En fazla 6 ana adım.
>
> Her adım:
>
> - kısa fiil,
> - tek görsel,
> - gerekli yön oku.
>
> Paragraf yerine işlem odaklı kısa dil kullan.

## English

> Arrange [TASK] as a one-page instruction sheet with no more than six primary steps.
>
> Give every step one concise action verb, one visual, and a directional arrow only where needed.
>
> Prefer action-focused language over paragraphs.

---

# 1712. `/wiring-layout` — Kablo / Bağlantı Yerleşimi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [SİSTEM]'de kullanıcı tarafından verilen gerçek bağlantıları sade wiring layout olarak göster.
>
> Kablo:
>
> - başlangıç,
> - bitiş,
> - port,
> - renk/etiket
>
> bilgisi doğrulanmış veriye dayansın.
>
> Gerçek cihaz pinout'u bilinmiyorsa uydurma bağlantı çizme.

## English

> Show the verified connections in [SYSTEM] as a restrained wiring layout.
>
> Base cable origin, destination, port, and color or label only on supplied information.
>
> Do not invent pinouts or electrical connections for unknown hardware.

---

# 1713. `/reverse-engineering-board` — Tersine İnceleme Panosu

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Kaynak [NESNE]'yi reverse-engineering observation board olarak göster.
>
> Board:
>
> - genel görünüm,
> - ölçülmüş dış boyutlar,
> - görünür bağlantılar,
> - malzeme gözlemleri,
> - bilinmeyen alanlar
>
> içersin.
>
> Bilinmeyen iç geometriyi “inferred / unknown” olarak ayır.

## English

> Present the source [OBJECT] as a reverse-engineering observation board containing overall views, measured external dimensions, visible joints, material observations, and unknown regions.
>
> Clearly separate inferred or unknown internal geometry from measured information.

---

# 1714. `/technical-drawing-audit` — Teknik Görsel Denetimi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

Bir teknik görsel için kontrol:

1. Bütün görünüşler aynı nesneyi mi gösteriyor?
2. Callout numaraları parts list ile eşleşiyor mu?
3. Oklar gerçekten doğru parçaya gidiyor mu?
4. Ölçüler kullanıcı/veri kaynağından mı?
5. Bilinmeyen iç parçalar ayrılmış mı?
6. Perspective ile orthographic karışmış mı?
7. Kesit düzlemi mantıklı mı?
8. Üretim için gereken toleranslar gerçekten var mı?
9. Görsel yalnız “teknik görünüyor” diye doğru kabul ediliyor mu?

---

# 1715. `/blueprint-slop-filter` — Blueprint / Technical AI Slop Filtresi

Kaçınılması gerekenler:

- sahte ölçüler,
- uydurma tolerans,
- rastgele formül,
- dekoratif grid,
- bütün parçalara gereksiz callout,
- isometric + perspective + orthographic karışımı,
- kaynağa ait olmayan iç mekanizma,
- üretime hazır olduğunu iddia etmek,
- “blueprint” = mavi arka plan filtresi sanmak.

---

# 1716. İnternetteki `/blueprint`, `/schematic`, `/technicaldrawing` Listelerini Nasıl Okumalı?

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

2026’da yayımlanan bazı prompt modifier cheat sheet'lerinde:

> `/blueprint`
>
> `/schematic`
>
> `/technicaldrawing`
>
> `/diagram`
>
> `/cutaway`

gibi ifadeler slash command biçiminde listeleniyor.

Bu rehberde doğru yorum:

> **community shorthand**

Resmî bir ChatGPT görsel syntax'ı olduğu varsayılmamalı.

Rehber kullanım biçimi:

> `/blueprint — product photo → technical line drawing, preserve source geometry, no invented dimensions`

ve ardından tam prompt.

---

<a id="aile-025"></a>
# Xerox, Photocopy, Paste-up ve Scanner Görsel Dili

2026'nın analog/anti-polish yönlerinde photocopy ve Xerox dili yalnız “grunge filter” olarak değil, **gerçek çoğaltma sürecinin görüntüyü dönüştürmesi** olarak yeniden görünür.

Temmuz 2026'da Rencontres d'Arles çevresinde sergilenen *Hard Copy* projesi, çağdaş fotoğrafçıların görüntülerini Xerox süreçleri üzerinden yeniden yorumladı. Buradaki ilgi:

- ton kaybı,
- yüksek kontrast,
- toner davranışı,
- tekrar kopyalamada generation loss,
- fiziksel ölçek,
- ucuz ve hızlı çoğaltım

gibi süreç özelliklerinden geliyor.

Zine araştırmaları da fotokopi makinesinin punk/DIY estetiğindeki rolünü yalnız görünüş değil, **üretim ve dağıtım biçimi** üzerinden açıklıyor.

---

# 1717. `/xerox-photo` — Xerox Fotoğraf

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe prompt

> [FOTOĞRAF]'ı gerçek siyah-beyaz photocopier/Xerox çoğaltımı gibi dönüştür.
>
> Kullan:
>
> - yüksek kontrast,
> - sınırlı gri ton,
> - toner yoğunluğu,
> - ince detay kaybı,
> - hafif paper/roller davranışı.
>
> Kaynak yüz ve ana silhouette tanınabilir kalsın.
>
> Rastgele scratch/grunge overlay kullanma.

## English

> Transform [PHOTO] as if reproduced on a real black-and-white photocopier using high contrast, limited gray range, toner density, fine-detail loss, and subtle paper or roller behavior.
>
> Preserve the recognizable face and main silhouette.
>
> Avoid random scratch or grunge overlays.

---

# 1718. `/xerox-generation-loss` — Kopyanın Kopyası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Aynı [FOTOĞRAF/METİN]'i dört nesil fotokopi boyunca göster:
>
> 1. original print,
> 2. first copy,
> 3. copy of copy,
> 4. fourth-generation copy.
>
> Her nesilde:
>
> - ince detay azalabilir,
> - siyah alan genişleyebilir,
> - toner artefact artabilir.
>
> Dört kareye dört farklı “grunge texture” yapıştırma.

## English

> Show [PHOTO/TEXT] across four photocopy generations:
>
> original print → first copy → copy of copy → fourth-generation copy.
>
> Let fine detail degrade, black areas gain, and toner artifacts accumulate progressively.
>
> Do not apply four unrelated grunge textures.

---

# 1719. `/xerox-collage` — Fotokopi Kolajı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> 3–6 fiziksel fotoğraf/metin parçasını kesilmiş photocopy fragments olarak tek sayfada birleştir.
>
> Her parça aynı toner/kağıt dünyasında olsun.
>
> Overlap ve kesim kenarı gerçek fiziksel paste-up gibi görünsün.
>
> Her boşluğu doldurma.

## English

> Assemble 3–6 cut photocopy photo or text fragments into one physical collage page.
>
> Keep them within one toner and paper world.
>
> Make overlaps and cut edges feel physically pasted.
>
> Preserve deliberate empty space.

---

# 1720. `/paste-up` — Fiziksel Paste-up Sayfası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [POSTER/ZINE SAYFASI]'nı dijital grid yerine fiziksel paste-up yöntemiyle kurulmuş gibi göster.
>
> Ayrı:
>
> - fotoğraf parçaları,
> - basılı metin şeritleri,
> - başlık,
> - küçük işaretler
>
> kesilip manuel yerleştirilmiş olsun.
>
> Yapıştırma sırası ve overlap fiziksel olarak anlaşılır olsun.

## English

> Build [POSTER/ZINE PAGE] as a physical paste-up rather than a digital grid.
>
> Use separately cut photographic fragments, printed text strips, headline pieces, and small marks, with believable assembly order and overlap.

---

# 1721. `/cut-paste-type` — Kes-Yapıştır Tipografi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KISA BAŞLIK]'ı basılı farklı kaynaklardan kesilmiş fiziksel harf/kelime parçalarıyla oluştur.
>
> Okunabilirlik korunmalı.
>
> Her harfi farklı font/renk yapmak zorunda değilsin.
>
> “Ransom note” klişesine otomatik dönüşme.

## English

> Build [SHORT HEADLINE] from physically cut printed letter or word fragments while preserving readability.
>
> Do not force every character to use a different font and color or automatically turn the result into a ransom-note cliché.

---

# 1722. `/stencil-type` — Stencil / Şablon Tipografi

## Türkçe

> [KELİME]'yi fiziksel stencil ile boya uygulanmış gibi göster.
>
> Harf iç boşluklarının tutulması için gerçek stencil bridge mantığı olsun.
>
> Sprey overspray çok sınırlı kalabilir.
>
> Dijital distressed font kullanıp “stencil” deme.

## English

> Render [WORD] as physically stenciled paint using real bridge logic to hold enclosed counters.
>
> Allow only restrained overspray.
>
> Do not substitute a distressed digital font and call it stencil.

## Neye dikkat edilmeli?

Bilgi kilidi: kaynak, tarih ve gösterim yöntemi görselde belirtilsin; kaynaksız infografik kullanılmaz ([§1830](#sec-1830)).

---
# 1723. `/punk-flyer` — DIY Punk / Gig Flyer

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## 2026 trend

Punk/grunge revival raporlarında:

- photocopy,
- stencil,
- cut-out type,
- distorted photo,
- handwritten marks,
- limited spot color

yeniden güçlü.

## Türkçe

> [ETKİNLİK] için düşük maliyetli fiziksel DIY flyer üretim mantığı kullan.
>
> Siyah-beyaz photocopy tabanı + en fazla tek spot renk.
>
> Bir ana fotoğraf, sert başlık, tarih/yer bilgisi ve az sayıda elle müdahale yeterli olsun.
>
> Bilgi okunabilirliğini “punk” adına tamamen yok etme.

## English

> Design a low-cost DIY flyer for [EVENT] using black-and-white photocopy reproduction with at most one spot color.
>
> Use one main photograph, a strong headline, clear date and place, and only a few hand interventions.
>
> Do not destroy essential legibility in the name of punk aesthetics.

---

# 1724. `/xerox-poster` — Büyük Fotokopi Poster

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [FOTOĞRAF/MESAJ]'ı yüksek kontrast photocopy image + tek güçlü tipografi ile poster olarak oluştur.
>
> Toner kırılması ve copy artefact yalnız görüntünün çoğaltımından gelsin.
>
> Sahte yüzey çizikleri ekleme.

## English

> Create a poster using one high-contrast photocopied image and one strong typographic element.
>
> Let toner breakup and copy artifacts emerge from reproduction rather than fake surface scratching.

---

# 1725. `/zine-spread` — Zine Açılımı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KONU]'yu iki sayfalık bağımsız zine spread olarak düzenle.
>
> Sayfalar birlikte çalışsın fakat aynı layout'un aynası olmasın.
>
> Kullan:
>
> - 1 ana görsel,
> - 2–4 küçük parça,
> - kısa metin,
> - sayfa numarası gerekiyorsa.
>
> Zine'i “kaotik olmak zorunda” gibi tasarlama.

## English

> Design [TOPIC] as a two-page independent zine spread.
>
> Make the pages work together without mirroring the same layout.
>
> Use one primary image, 2–4 smaller fragments, concise text, and page numbering where needed.
>
> Do not treat chaos as a requirement of zine design.

---

# 1726. `/one-sheet-zine` — Tek Kâğıttan Katlanan Mini Zine

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Tek A4/Letter kâğıttan kesilip katlanabilecek 8-panelli mini zine layout oluştur.
>
> Sayfa yönleri katlama sonrası doğru dönsün.
>
> Ön/arka kapak ve sayfa sırası fiziksel katlama mantığına uygun olsun.
>
> Sadece sekiz kutulu poster yapma.

## English

> Create an eight-panel mini-zine layout that can be cut and folded from one A4 or Letter sheet.
>
> Make page orientation and sequence correct after folding.
>
> Treat front and back covers as part of the physical imposition rather than making an eight-box poster.

---

# 1727. `/zine-imposition` — Zine Baskı Yerleşimi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ZINE] için baskı/katlama öncesi imposition sheet göster.
>
> Okuyucunun gördüğü sayfa sırası ile baskı kâğıdındaki sıra arasındaki fark açık olsun.
>
> Gerçek katlama biçimine göre sayfa yönlerini döndür.

## English

> Show an imposition sheet for [ZINE] before printing and folding.
>
> Distinguish reading order from print-sheet order and rotate pages according to the actual fold.

---

# 1728. `/photocopy-contact-sheet` — Photocopy Photo Contact

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> 9–16 fotoğrafı aynı photocopy sheet üzerinde küçük proof/contact görüntüler olarak göster.
>
> Tüm fotoğraflar aynı reproduction sürecinden geçsin.
>
> Bir veya iki kare grease pencil/circle ile seçilebilir.

## English

> Show 9–16 photographs as small proof or contact images on one photocopied sheet.
>
> Apply one consistent reproduction process.
>
> Mark only one or two selected frames with a restrained grease-pencil circle.

---

# 1729. `/flatbed-scan` — Flatbed Scanner Görüntüsü

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [NESNE/FOTOĞRAF/KÂĞIT]'ı flatbed scanner camına doğrudan yerleştirilmiş gibi göster.
>
> Perspektif yok denecek kadar az olsun.
>
> Cama temas eden bölgeler çok net; yüzeyden yükselen bölümler hızla yumuşayabilir.
>
> Kamera gölgesi veya lens bokeh'i ekleme.

## English

> Show [OBJECT/PHOTO/PAPER] as if placed directly on flatbed-scanner glass.
>
> Use almost no perspective.
>
> Keep contact areas extremely sharp while elements rising away from the glass soften quickly.
>
> Avoid camera shadows and lens bokeh.

---

<a id="sec-1730"></a>
# 1730. `/scanography` — Scanner Art / Scanography

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [NESNELER]'i flatbed scanner üzerinde fiziksel kompozisyon olarak düzenle.
>
> Tarama kaynağının:
>
> - sığ alan derinliği,
> - cam teması,
> - düz frontal light,
> - siyah/açık scanner lid background
>
> davranışını koru.
>
> Normal top-down fotoğrafa scanner texture ekleme.

## English

> Arrange [OBJECTS] as a physical composition on a flatbed scanner, preserving shallow scanner depth, glass contact, frontal scan illumination, and a plausible scanner-lid background.
>
> Do not simulate scanography by applying scanner texture to a normal top-down photograph.

---

# 1731. `/scanner-motion` — Tarama Sırasında Hareket

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [NESNE/EL]'i scanner head hareket ederken sınırlı biçimde oynatılmış gibi göster.
>
> Hareket distortion'ı tarama yönü boyunca zamanla uzasın.
>
> Photoshop liquify gibi her yöne rastgele bükme.

## English

> Show [OBJECT/HAND] moving slightly while the scanner head passes, creating time-based distortion along the scan direction.
>
> Avoid arbitrary multi-directional liquify warping.

---

# 1732. `/scanner-object-portrait` — Scanner ile Nesne Portresi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Tek [NESNE]'yi scanner camı üzerinde ana portre gibi göster.
>
> Cama değen yüzey maksimum detay; üstte kalan yapı daha karanlık/yumuşak olabilir.
>
> Nesneyi ürün stüdyosu gibi rim light ile aydınlatma.

## English

> Portrait one [OBJECT] directly on scanner glass, with maximum detail at contact surfaces and softer or darker structure farther from the glass.
>
> Avoid product-studio rim lighting.

---

# 1733. `/scan-collage` — Scanner İçinde Fiziksel Kolaj

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> 4–7 kesilmiş kâğıt, fotoğraf, kumaş veya küçük düz nesneyi scanner camında gerçek fiziksel overlap ile birleştir.
>
> Katmanlar scanner ışığı ve cama uzaklık nedeniyle farklı davranabilsin.
>
> Dijital Photoshop layer paneli gibi kusursuz kesim kullanma.

## English

> Combine 4–7 cut-paper, photo, textile, or small flat objects physically on scanner glass with real overlap.
>
> Let layers differ according to scanner illumination and distance from the glass.
>
> Avoid perfect Photoshop-style digital cutouts.

---

# 1734. `/copy-scan-slop-filter` — Xerox / Scanner AI Slop Filtresi

Kaçınılması gerekenler:

- Xerox = grunge texture,
- scan = top-down photo,
- toner = film grain,
- generation loss = random scratches,
- zine = okunamaz kaos,
- paste-up = digital card grid,
- scanner hareketi = liquify,
- her analog çıktıya tape/coffee stain eklemek.

---

# 1735. Yeni üst aile: `Copy / Scan Grammar`

Aile:

- `/xerox-photo`
- `/xerox-generation-loss`
- `/xerox-collage`
- `/paste-up`
- `/photocopy-contact-sheet`
- `/flatbed-scan`
- `/scanography`
- `/scanner-motion`

Ortak soru:

> **Görüntü nasıl çoğaltıldı veya nasıl yakalandı?**

Bu ailede “retro efekt” yerine:

> toner + exposure + glass contact + physical cut + reproduction generation

gibi gerçek süreç özellikleri yazılır.

---

<a id="aile-026"></a>
# Editorial Publication Grammar — Tek Sayfa Değil, Sayfa Dizisi

Editorial design ile poster tasarımı arasındaki ana fark:

> **okur tek bir kompozisyona değil, art arda gelen sayfalara maruz kalır.**

2026 editorial design değerlendirmelerinde iki yön aynı anda güçlü:

- daha sıcak, tactile ve ayırt edilebilir görsel kimlik,
- daha sıkı okunabilirlik, grid ve tipografik disiplin.

Bu yüzden magazine/zine/book promptlarında amaç:

> her sayfayı “wow” yapmak değil,
>
> **ritim kurmak**tır.

---

# 1736. `/editorial-opener` — Bölüm / Makale Açılışı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [MAKALE/BÖLÜM] için iki sayfalık editorial opener oluştur.
>
> Kullan:
>
> - tek güçlü başlık,
> - kısa deck/subtitle,
> - bir ana görsel,
> - yeterli başlangıç boşluğu.
>
> İlk sayfaya bütün makale özetini doldurma.

## English

> Create a two-page editorial opener for [ARTICLE/SECTION] using one strong headline, a concise deck or subtitle, one primary image, and enough opening space.
>
> Do not overload the opener with the entire article summary.

---

# 1737. `/feature-spread` — Uzun Makale Açılımı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [MAKALE]'nin ana gövdesi için iki sayfalık feature spread tasarla.
>
> Grid:
>
> - okunabilir body text,
> - 1 ana görsel,
> - en fazla 2 destek görsel,
> - kısa caption
>
> taşısın.
>
> Her görseli farklı çerçeve ve efektle sunma.

## English

> Design a two-page feature spread for [ARTICLE] using readable body text, one primary image, no more than two supporting images, and concise captions.
>
> Avoid giving every image a different frame or effect.

---

# 1738. `/pull-quote-spread` — Pull Quote Sayfası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Uzun metin akışında yalnız gerçekten önemli tek kısa cümleyi pull quote olarak büyüt.
>
> Quote ana makalede gerçekten varsa kullan.
>
> Sayfayı doldurmak için yeni slogan uydurma.

## English

> Enlarge one genuinely important short sentence from the article as a pull quote.
>
> Use only text that actually exists in the source.
>
> Do not invent a slogan to fill the page.

---

# 1739. `/photo-essay-sequence` — Fotoğraf Hikâyesi Sayfa Dizisi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [FOTOĞRAF SERİSİ]'ni 6–12 sayfalık photo essay olarak sırala.
>
> Ritmi:
>
> wide → medium → detail → pause → peak → closing
>
> gibi kur.
>
> En güçlü fotoğrafları art arda yığma.
>
> Aynı tür kareler arasında boşluk/pacing bırak.

## English

> Sequence [PHOTO SERIES] as a 6–12 page photo essay with rhythm such as wide → medium → detail → pause → peak → closing.
>
> Do not stack every strongest image consecutively.
>
> Use pacing between similar frames.

---

# 1740. `/caption-system` — Caption Sistemi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Yayın boyunca caption'ları tek sistemle düzenle.
>
> İçerik gerektiğinde:
>
> - ne/kim,
> - yer,
> - tarih,
> - credit
>
> sırasını kullansın.
>
> Fotoğrafta görülmeyen bilgiyi uydurma.
>
> Caption typography body text'ten ayrışsın ama yarışmasın.

## English

> Use one caption system throughout the publication, containing what or who, place, date, and credit only where relevant.
>
> Do not invent information not supported by the source.
>
> Keep caption typography distinct from body text without competing with it.

---

# 1741. `/contents-page` — İçindekiler Sayfası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [YAYIN]'ın contents page'ini gerçek navigasyon aracı olarak tasarla.
>
> Bölüm adı + sayfa numarası öncelikli.
>
> En fazla birkaç küçük görsel cue kullan.
>
> İçindekileri editorial poster hâline getirip sayfa numaralarını zor bulunur yapma.

## English

> Design the contents page of [PUBLICATION] as a real navigation tool with section names and page numbers as the priority.
>
> Use only a few small visual cues.
>
> Do not turn the contents page into a poster where page numbers are difficult to find.

---

# 1742. `/index-page` — Dizin / Kaynak Sayfası

## Türkçe

> [YAYIN]'ın index/reference bölümünü taranabilir alfabetik veya tematik yapıda düzenle.
>
> Çok sütun kullanılabilir ancak satır takibi kolay olsun.
>
> Dizin sayfasını görsel collage ile bölme.

## English

> Structure the index or reference section of [PUBLICATION] in a scannable alphabetical or thematic system.
>
> Multiple columns may be used while preserving easy line tracking.
>
> Avoid breaking the index with decorative collage.

## Neye dikkat edilmeli?

Bilgi kilidi: kaynak, tarih ve gösterim yöntemi görselde belirtilsin; kaynaksız infografik kullanılmaz ([§1830](#sec-1830)).

---
# 1743. `/archive-issue` — Arşiv Sayısı / Dosya Görünümü

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KONU]'yu arşiv yayını gibi düzenle:
>
> tarih,
> belge,
> fotoğraf,
> kısa kayıt,
> kaynak.
>
> Arşiv materyalinin farklı dönemlerini aynı “vintage filter” ile eşitleme.
>
> Her kaynağın kendi fiziksel karakterini koru.

## English

> Structure [TOPIC] like an archival issue using dates, documents, photographs, concise records, and sources.
>
> Do not flatten materials from different periods under one vintage filter.
>
> Preserve the physical character of each source.

---

# 1744. `/publication-rhythm` — Yayın Ritmi Kontrolü

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

Bir 12+ sayfalık yayın için sor:

1. Kaç ağır/dolu sayfa art arda geliyor?
2. Nefes alan sayfa var mı?
3. Aynı layout gereğinden fazla tekrar ediyor mu?
4. Her bölüm başlangıcı tanınabilir mi?
5. Görsel ve metin oranı içerikle uyumlu mu?
6. Caption sistemi tutarlı mı?
7. Okurun nerede olduğunu anlaması kolay mı?

---

# 1745. `/spread-continuity` — Sayfalar Arası Devamlılık

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Aynı yayın boyunca:
>
> - grid,
> - margin,
> - body typography,
> - caption,
> - folio/page number,
> - recurring graphic cue
>
> kurallarını sabit tut.
>
> Her spread'i bağımsız Behance projesi gibi yeniden tasarlama.

## English

> Preserve grid, margins, body typography, caption system, folios, and recurring graphic cues across the publication.
>
> Do not redesign every spread as an unrelated portfolio piece.

---

# 1746. `/editorial-publication-slop-filter` — Yayın Tasarımı AI Slop Filtresi

Kaçınılması gerekenler:

- her sayfa poster,
- her spread farklı font,
- her fotoğraf farklı treatment,
- lorem ipsum'u gerçek içerik gibi bırakmak,
- sayfa numarasını unutmak,
- çok küçük body text,
- dekoratif caption,
- sürekli full-bleed,
- ritim yerine sürekli “impact”.

---

<a id="aile-027"></a>
# 2026 Etiket Bilgi Mimarisi — Extended Content Label

2026 label/packaging değerlendirmelerinde **Extended Content Labels (ECL)**, regülasyon ve çoklu bilgi gereksinimleri nedeniyle daha görünür hâle geliyor.

Bu aile:

- peel-back label,
- booklet label,
- fold-out label

gibi formatları kapsayabilir.

Buradaki amaç:

> küçük pakete daha çok bilgiyi okunabilir biçimde sığdırmak.

Ama:

> **bilgiyi saklamak**

değildir.

---

# 1747. `/extended-content-label` — Genişletilmiş İçerik Etiketi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ÜRÜN] için küçük yüzeyde çoklu bilgi taşıyan extended-content label tasarla.
>
> Dış yüzey:
>
> - marka,
> - ürün adı,
> - kritik kısa bilgi.
>
> İç katman:
>
> - kullanım,
> - içerik,
> - regülasyon,
> - çoklu dil
>
> gibi ikincil ayrıntılar.
>
> Açma yönü açıkça anlaşılır olsun.

## English

> Design an extended-content label for [PRODUCT].
>
> Keep the outer face focused on brand, product name, and essential concise information.
>
> Use inner layers for secondary details such as instructions, ingredients, regulatory text, or multiple languages.
>
> Make the opening direction obvious.

---

# 1748. `/peel-back-label` — Soyulup Açılan Etiket

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ŞİŞE/KUTU]'da üst katmanı köşeden kaldırılan peel-back label tasarla.
>
> Küçük “peel here” affordance ve tekrar kapanma gerekiyorsa fiziksel yapısı anlaşılır olsun.
>
> Kritik güvenlik bilgisini yalnız erişilmesi zor alt katmanda bırakma.

## English

> Design a peel-back label for [BOTTLE/PACKAGE] with a clear small opening affordance and physically plausible resealing where needed.
>
> Do not hide critical safety information only on a difficult-to-access inner layer.

---

# 1749. `/booklet-label` — Kitapçık Etiket

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ÜRÜN]'ün sınırlı yüzeyinde 4–8 küçük sayfalık booklet label tasarla.
>
> Sayfalar gerçek cilt/adhesive alanına göre açılabilsin.
>
> Tipografi küçük olduğu için bilgi hiyerarşisini özellikle güçlü kur.
>
> Görsel dekor için kullanılabilir alanı abartma.

## English

> Design a 4–8 page booklet label for [PRODUCT] within limited package area.
>
> Make page turning physically plausible around the binding or adhesive zone.
>
> Use particularly strong hierarchy at small type sizes.
>
> Do not overestimate the space available for decoration.

---

# 1750. `/compliance-layer` — Regülasyon Bilgi Katmanı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [AMBALAJ]'da zorunlu/regulatory bilgiyi marka tasarımından ayrı ama sistem içinde okunabilir katman olarak düzenle.
>
> Gerçek yasal gereklilik kullanıcı/veri kaynağından gelmeli.
>
> Sahte sertifika, sembol veya zorunlu ibare uydurma.

## English

> Organize mandatory or regulatory information on [PACKAGE] as a readable layer distinct from, but integrated with, the brand design.
>
> Real legal requirements must come from supplied or verified sources.
>
> Do not invent certification marks, symbols, or mandatory statements.

---

# 1751. `/nutrition-panel-layout` — Besin Bilgi Paneli Yerleşimi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Kullanıcı tarafından verilen besin verisini temiz nutrition panel layout içinde düzenle.
>
> Sayılar ve birimler bire bir korunmalı.
>
> Gerçek ülke mevzuatına uygunluk gerekiyorsa ilgili standarda ayrıca doğrula.
>
> Image modelden besin değeri hesaplamasını isteme.

## English

> Place user-supplied nutrition data into a clean information panel while preserving numbers and units exactly.
>
> Verify against the relevant jurisdictional standard when formal compliance is required.
>
> Do not ask the image model to calculate nutrition values.

---

# 1752. `/multilingual-pack-label` — Çok Dilli Ambalaj Etiketi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [DİLLER] için aynı ambalajda dil hiyerarşisi oluştur.
>
> Her dil:
>
> - eşit doğruluk,
> - yeterli okunabilirlik,
> - açık ayrım
>
> taşısın.
>
> Bir dili dekoratif küçültüp okunmaz hâle getirme.
>
> Çeviri doğruluğu ayrıca doğrulanmalı.

## English

> Create a multilingual label hierarchy for [LANGUAGES] on the same package.
>
> Give every language accurate content, adequate legibility, and clear separation.
>
> Do not reduce one language to decorative unreadable microtype.
>
> Verify translations separately.

---

# 1753. `/label-information-hierarchy` — Etiket Bilgi Hiyerarşisi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ÜRÜN ETİKETİ]'ni bilgi önceliğine göre beş katmana ayır:
>
> 1. marka,
> 2. ürün,
> 3. variant/quantity,
> 4. essential instruction,
> 5. regulatory/detail.
>
> Her bilgiyi aynı font ağırlığında sunma.

## English

> Structure [PRODUCT LABEL] into five information levels:
>
> 1. brand,
> 2. product,
> 3. variant or quantity,
> 4. essential instruction,
> 5. regulatory or detailed information.
>
> Do not give every text element equal visual weight.

---

# 1754. `/label-family` — SKU / Etiket Ailesi

## Türkçe

> Aynı [MARKA]'nın 6 SKU etiketini tek family olarak tasarla.
>
> Sabit:
>
> - logo,
> - grid,
> - bilgi sırası,
> - temel typography.
>
> Değişken:
>
> - variant adı,
> - kontrollü renk,
> - tek ingredient/product cue.
>
> Her SKU'yu tamamen farklı marka gibi yapma.

## English

> Design six SKU labels for [BRAND] as one family.
>
> Keep logo, grid, information order, and base typography fixed.
>
> Vary only the variant name, controlled color, and one ingredient or product cue.
>
> Do not make every SKU look like a separate brand.

## Neye dikkat edilmeli?

Bilgi kilidi: kaynak, tarih ve gösterim yöntemi görselde belirtilsin; kaynaksız infografik kullanılmaz ([§1830](#sec-1830)).

---
# 1755. `/label-slop-filter` — Etiket AI Slop Filtresi

Kaçınılması gerekenler:

- küçük yazıyı okunamaz yapmak,
- sahte sertifika,
- uydurma ingredient/nutrition,
- QR'ı dekor olarak yapıştırmak,
- bütün bilgi aynı hiyerarşide,
- çoklu dili küçücük yazmak,
- “premium” = foil,
- ECL mekanizmasını fiziksel olarak çözememek.

---

<a id="aile-028"></a>
# Prompt Dili Deneyi — Türkçe, İngilizce ve Hibrit Aynı Görselde Nasıl Karşılaştırılır?

Rehberin başında İngilizce teknik terimlerin bazen yararlı olabileceği anlatılmıştı.

Burada bunu iddia değil **test protokolü** hâline getirelim.

Önemli:

> Amaç “İngilizce daha iyi prompt üretir” sonucunu kanıtlamak değildir.

Amaç:

> Modelin yerleşik görsel terimleri farklı dillerde ne kadar doğru yorumladığını karşılaştırmak.

---

# 1756. `/language-ab-test` — Prompt Dili Karşılaştırma Testi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Test konusu

> Bir çiçeğin anatomik görünümü.

### Türkçe

> Bir çiçeğin çanak yaprak, taç yaprak, başçık, sapçık, tepecik, boyuncuk ve yumurtalık bölümlerini sade eğitim illüstrasyonu olarak göster. İnce açıklama çizgileri kullan. Etiketleri Türkçe yaz. Beyaz arka plan. Dekoratif öğe kullanma.

### English

> Create a clean educational anatomy illustration of a flower showing sepals, petals, anther, filament, stigma, style, and ovary. Use thin leader lines and clear labels. White background. No decorative elements.

### Hibrit

> Bir çiçeği **botanical anatomy plate** olarak göster. Çanak yaprak, taç yaprak, başçık, sapçık, tepecik, boyuncuk ve yumurtalığı ince **leader lines** ile etiketle. Etiket dili Türkçe. Beyaz arka plan. Dekoratif öğe kullanma.

## Neye dikkat edilmeli?

**`/language-ab-test`** biçiminde iki tarafın aynı ölçek, aynı açı ve benzer ışıkla gösterilmesi karşılaştırmanın ön koşuludur; ölçek farklıysa fark abartılır veya silinir. Model yan yana koyduğu iki örneği ayrı stillerde üretebilir; stil farkı bilginin parçası değilse promptta kısıtlanır. Şüphe hâlinde yeniden üretin ya da biçim değiştirin ([§19](10-temeller-001-222.md#sec-19)).

---

# 1757. `/language-test-score` — Dil Testi Değerlendirme Rubriği

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

Her üç prompt aynı model ve mümkün olduğunca aynı koşullarda değerlendirilir:

| Ölçüt | 0–2 |
|---|---:|
| Yapısal doğruluk | 0–2 |
| Etiket doğruluğu | 0–2 |
| İstenen görsel genre'ı anlama | 0–2 |
| Leader-line yerleşimi | 0–2 |
| Gereksiz dekor eklememe | 0–2 |

Toplam:

> 10 puan.

Tek örnekten genel dil üstünlüğü sonucu çıkarılmaz.

---

# 1758. `/source-genre` — Görsel Kaynak Türünü Belirtme

Görsel promptlarda çoğu zaman “style” yerine **source genre** daha açıklayıcıdır.

Örnekler:

| Amaç | Kaynak türü |
|---|---|
| bitki anatomisi | botanical plate |
| hayvan türleri | field guide plate |
| makine | technical manual |
| arkeoloji | excavation record / museum catalog |
| coğrafya | school atlas / thematic map |
| deney | lab manual |
| moda | lookbook / technical flat |
| yemek | cookbook / recipe card |
| tarih | archival plate / museum interpretation |
| malzeme | material sample board |
| mimari | competition board / construction detail |
| ürün | catalog / teardown / service manual |

Bu nedenle:

> `make it beautiful`

yerine:

> `present it like a botanical field guide plate`

çok daha işlevsel bir yönlendirme olabilir.

---

# 1759. `/genre-first` — Stilden Önce Kaynak Türü

## Türkçe

> [KONU]'yu önce kullanılacağı görsel kaynak türüyle tanımla:
>
> textbook figure,
> museum label,
> technical manual,
> field guide,
> editorial illustration,
> catalog,
> worksheet,
> scientific plate.
>
> Ardından stil özelliklerini ekle.
>
> Genre ile style'ı aynı şey sanma.

## English

> Define [TOPIC] first by its intended source genre—textbook figure, museum label, technical manual, field guide, editorial illustration, catalog, worksheet, or scientific plate—then add stylistic properties.
>
> Do not confuse genre with style.

## Neye dikkat edilmeli?

Bilgi kilidi: kaynak, tarih ve gösterim yöntemi görselde belirtilsin; kaynaksız infografik kullanılmaz ([§1830](#sec-1830)).

---
# 1760. Yeni Üst Aileler — Bu Turun Özeti

## `Technical Documentation Visual`

- `/blueprint`
- `/patent-drawing`
- `/orthographic-drawing`
- `/dimensioned-drawing`
- `/assembly-manual`
- `/service-manual`
- `/bill-of-materials`

Ana kural:

> **technical-looking ≠ technically verified**

## `Copy / Scan Visual`

- `/xerox-photo`
- `/xerox-generation-loss`
- `/paste-up`
- `/scanography`
- `/flatbed-scan`

Ana kural:

> **analog görünüş, analog sürecin sonucudur.**

## `Publication Sequence Visual`

- `/editorial-opener`
- `/feature-spread`
- `/photo-essay-sequence`
- `/publication-rhythm`
- `/spread-continuity`

Ana kural:

> **tek güzel sayfa değil, okunabilir sayfa dizisi.**

## `Regulatory Information Visual`

- `/extended-content-label`
- `/peel-back-label`
- `/booklet-label`
- `/compliance-layer`
- `/multilingual-pack-label`

Ana kural:

> **tasarım, zorunlu bilgiyi gizlemez.**

## `Genre-first Prompting`

Önce:

> bu görsel hangi yayın/meslek/öğretim geleneğine ait?

Sonra:

> nasıl görünmeli?

---

# 1761. Bu turdaki slash-style indeks (aile-028)

| Kısayol | Aile |
|---|---|
| `/blueprint` | technical blueprint-style presentation |
| `/exploded-blueprint` | exploded technical blueprint |
| `/patent-drawing` | patent-inspired line drawing |
| `/orthographic-drawing` | matched technical views |
| `/dimensioned-drawing` | supplied dimensions only |
| `/section-hatch` | technical section hatching |
| `/detail-callout` | enlarged detail |
| `/bill-of-materials` | verified parts table |
| `/assembly-manual` | sequential assembly instruction |
| `/service-manual` | maintenance illustration |
| `/instruction-sheet` | one-page technical instruction |
| `/wiring-layout` | verified wiring layout |
| `/reverse-engineering-board` | measured vs unknown object analysis |
| `/technical-drawing-audit` | technical visual review |
| `/xerox-photo` | photocopied photograph |
| `/xerox-generation-loss` | copy-of-copy degradation |
| `/xerox-collage` | physical photocopy collage |
| `/paste-up` | manually assembled page |
| `/cut-paste-type` | cut printed typography |
| `/stencil-type` | physical stencil lettering |
| `/punk-flyer` | low-cost DIY event flyer |
| `/xerox-poster` | photocopy-led poster |
| `/zine-spread` | independent publication spread |
| `/one-sheet-zine` | foldable one-sheet zine |
| `/zine-imposition` | print/fold page arrangement |
| `/photocopy-contact-sheet` | copied photo proof sheet |
| `/flatbed-scan` | scanner-captured object |
| `/scanography` | scanner-based composition |
| `/scanner-motion` | movement during scanning |
| `/scanner-object-portrait` | scanner object portrait |
| `/scan-collage` | physical scanner collage |
| `/editorial-opener` | article/section opening |
| `/feature-spread` | long-form editorial spread |
| `/pull-quote-spread` | source-derived pull quote |
| `/photo-essay-sequence` | paced photo narrative |
| `/caption-system` | publication caption grammar |
| `/contents-page` | publication navigation |
| `/index-page` | index/reference navigation |
| `/archive-issue` | archival publication |
| `/publication-rhythm` | page-sequence pacing audit |
| `/spread-continuity` | cross-spread system lock |
| `/extended-content-label` | multilayer content label |
| `/peel-back-label` | peel-open label |
| `/booklet-label` | multi-page package label |
| `/compliance-layer` | mandatory information layer |
| `/nutrition-panel-layout` | supplied nutrition data layout |
| `/multilingual-pack-label` | multilingual label hierarchy |
| `/label-information-hierarchy` | information-priority system |
| `/label-family` | consistent SKU labels |
| `/language-ab-test` | Turkish/English/hybrid test |
| `/language-test-score` | language-test rubric |
| `/source-genre` | visual source convention |
| `/genre-first` | source genre before style |

---

<a id="aile-029"></a>
# Harita Dili, Tematik Kartografya ve “Hangi Görsel Türünü Seçmeliyim?” — 2026 Ek Taraması

2026’da Esri’nin güncel kartografya yayınları temel bir noktayı yeniden öne çıkarıyor:

> **Harita yalnız “yer gösteren görsel” değildir; veri, ölçek, projeksiyon, sembol, hiyerarşi ve okuma amacı birlikte tasarlanır.**

Esri’nin 2026’da yayımlanan *Map Use: Map Reading and Design* dokuzuncu baskısı ile Spring 2026 kartografya yazıları özellikle şu beş ilkeyi öne çıkarıyor:

- legibility,
- visual contrast,
- figure–ground,
- visual hierarchy,
- proportion.

Aynı yıl güncellenen thematic-map rehberleri de veri sınıflandırma aralıklarının bile haritanın anlattığı sonucu ciddi biçimde değiştirebildiğini hatırlatıyor.

Bu nedenle harita promptlarında:

> `make a beautiful map`

çok zayıf bir taleptir.

Önce şu sorular cevaplanmalıdır:

1. Harita neyi anlatacak?
2. Konum mu, dağılım mı, oran mı, hareket mi?
3. Kullanıcı hangi ölçekte okuyacak?
4. Veri nicel mi nitel mi?
5. Hangi base layer geri planda kalmalı?
6. Hangi bilgi en yüksek visual plane’de olmalı?

---

# 1762. `/map-purpose` — Haritanın Amacını Önce Tanımla

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [HARİTA KONUSU] için önce tek ana kullanıcı sorusunu tanımla:
>
> - Nerede?
> - Ne kadar?
> - Hangisi daha fazla?
> - Nasıl dağılıyor?
> - Nereden nereye hareket ediyor?
> - Ne kadar sürede ulaşılır?
> - Zaman içinde nasıl değişti?
>
> Harita türünü bu soruya göre seç.
>
> Aynı haritada bütün sorulara cevap vermeye çalışma.

## English

> Define one primary user question for [MAP TOPIC] first:
>
> Where is it?  
> How much is there?  
> Which area has more?  
> How is it distributed?  
> Where does movement occur?  
> What can be reached within a given time?  
> How has it changed over time?
>
> Select the map form according to that question.
>
> Do not force one map to answer every question.

---

# 1763. `/reference-map` — Referans Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [BÖLGE]'yi reference map olarak göster.
>
> Öncelik:
>
> - ana yerleşimler,
> - yollar,
> - su,
> - topoğrafik/administrative referanslar.
>
> Tematik veri ana amaç değil.
>
> Layer hiyerarşisi doğal coğrafi ve kullanım önemine göre kurulsun.

## English

> Show [REGION] as a reference map prioritizing settlements, roads, water, terrain, and relevant administrative context.
>
> Thematic data should not dominate.
>
> Build layer hierarchy according to geographic and navigational importance.

---

# 1764. `/thematic-map` — Tematik Harita

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [DEĞİŞKEN]'in coğrafi dağılımını thematic map olarak göster.
>
> Base map düşük kontrastta geri çekilsin.
>
> Tematik katman en yüksek görsel öncelikte olsun.
>
> Legend veri sınıflarını açıkça anlatsın.
>
> Konuyla ilgisiz yol, bina ve etiketleri azalt.

## English

> Show the geographic distribution of [VARIABLE] as a thematic map.
>
> Keep the basemap low-contrast and secondary.
>
> Place the thematic layer on the highest visual plane.
>
> Use a clear legend and remove unrelated map detail.

---

# 1765. `/choropleth` — Alanları Değerle Renklendirme

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Kullanım

İdari bölgeler gibi alanlara ait:

- oran,
- yüzde,
- normalize edilmiş değer

için.

## Türkçe prompt

> [BÖLGELER] için [ORAN/YÜZDE] verisini choropleth map olarak göster.
>
> Tek sequential veya diverging color scale kullan.
>
> Ham nüfus/sayıyı alan rengiyle göstermeden önce normalize edilip edilmemesi gerektiğini kontrol et.
>
> Class breaks gerçek veri dağılımına ve haritanın amacına göre seçilmeli.
>
> Veri yoksa sınıf değerleri uydurma.

## English

> Show [RATE/PERCENTAGE] across [AREAS] as a choropleth map using one sequential or diverging scale.
>
> Check whether raw counts should be normalized before encoding them by area color.
>
> Choose class breaks according to the real distribution and communication purpose.
>
> Do not invent class values without data.

---

# 1766. `/choropleth-class-check` — Sınıf Aralığı Denetimi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## 2026 kartografya notu

Aynı veri:

- equal interval,
- quantile,
- natural breaks,
- custom threshold

ile farklı görünür.

## Türkçe

> Choropleth üretmeden önce sınıflandırma yöntemini açıkça belirt.
>
> Eşik değerleri politik, bilimsel veya operasyonel anlam taşıyorsa yalnız doğrulanmış threshold kullan.
>
> Görsel olarak daha dramatik sonuç için class breaks ile oynama.

## English

> State the classification method explicitly before creating the choropleth.
>
> Use only verified thresholds when class boundaries have policy, scientific, or operational meaning.
>
> Do not manipulate class breaks merely to create a more dramatic map.

---

# 1767. `/proportional-symbol-map` — Orantılı Sembol Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Kullanım

Konuma bağlı **ham miktar/sayı** için.

## Türkçe

> [NOKTALAR]'daki [SAYI] değerlerini proportional symbols ile göster.
>
> Sembol alanı değeri temsil etsin.
>
> Büyük semboller küçükleri tamamen kapatıyorsa overlap düzenini veya opacity’yi kontrollü çöz.
>
> Sembol çapını değere doğrudan lineer bağlayıp alanı yanlış büyütme.

## English

> Show [COUNT] values at [LOCATIONS] using proportional symbols where symbol area encodes magnitude.
>
> Manage overlap carefully when large symbols obscure small ones.
>
> Do not map the raw value directly to circle diameter and thereby distort perceived area.

---

# 1768. `/dot-density-map` — Nokta Yoğunluk Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [OLAY/NÜFUS] dağılımını dot-density map olarak göster.
>
> Her nokta = [GERÇEK BİRİM DEĞERİ].
>
> Noktaların bölge içinde gerçek bireysel konumları temsil etmediğini gerekiyorsa legend/not ile açıkla.
>
> Nokta değerini uydurma.

## English

> Show the distribution of [EVENT/POPULATION] using a dot-density map where each dot represents [REAL UNIT VALUE].
>
> Clarify where necessary that dots do not necessarily represent exact individual locations within areas.
>
> Do not invent the dot value.

---

# 1769. `/graduated-symbol-map` — Sınıflandırılmış Sembol Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [DEĞER]'i 4–6 symbol-size sınıfıyla göster.
>
> Legend her boyut sınıfının gerçek aralığını açıklasın.
>
> Birbirine çok yakın 10 farklı daire boyutu kullanma.

## English

> Show [VALUE] using 4–6 graduated symbol-size classes with clear real ranges in the legend.
>
> Avoid using many barely distinguishable symbol sizes.

---

# 1770. `/flow-map` — Akış Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KAYNAK] ile [HEDEFLER] arasındaki hareketi flow map olarak göster.
>
> Çizgi:
>
> - yön,
> - miktar,
> - başlangıç/varış
>
> ilişkisini gerçek veriye göre taşısın.
>
> Her rotayı aynı kalınlıkta dekoratif eğri yapma.
>
> Büyük akışlar küçük akışları tamamen örtmesin.

## English

> Show movement between [ORIGIN] and [DESTINATIONS] as a flow map.
>
> Encode direction and magnitude from real data.
>
> Do not draw every route as the same decorative curved line.
>
> Keep large flows from fully obscuring smaller ones.

---

# 1771. `/desire-line-map` — Origin–Destination Bağlantı Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [NOKTALAR] arasındaki doğrudan origin–destination bağlantılarını desire-line map olarak göster.
>
> Bu çizgiler gerçek yol güzergâhı değil ilişki/akış bağlantısı olarak açıkça anlaşılmalı.

## English

> Show direct origin–destination relationships among [LOCATIONS] as desire lines.
>
> Make it clear that these straight connections represent relationships or flows rather than actual travel routes.

---

# 1772. `/route-map` — Gerçek Güzergâh Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ROTA]'yı gerçek yol/ağ geometrisi üzerinde route map olarak göster.
>
> Başlangıç, bitiş ve kritik ara noktalar açık olsun.
>
> Desire line ile gerçek güzergâhı karıştırma.
>
> Gerçek navigasyon gerekiyorsa güncel route data kullanılmalı.

## English

> Show [ROUTE] along the real road or network geometry with clear start, end, and key intermediate points.
>
> Do not confuse a straight desire line with the actual route.
>
> Use current routing data for real navigation.

---

# 1773. `/transit-map` — Toplu Taşıma Şeması

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [METRO/OTOBÜS/AĞ]'ı navigasyonu kolaylaştıran schematic transit map olarak göster.
>
> Coğrafi doğruluğu tamamen terk etmeden:
>
> - hat ilişkisi,
> - interchange,
> - sıra,
> - terminal
>
> bilgisini önceliklendir.
>
> İstasyon isimleri gerçek veri yoksa uydurulmasın.

## English

> Show [METRO/BUS/NETWORK] as a schematic transit map prioritizing line relationships, interchange points, station sequence, and terminals over exact geography.
>
> Do not invent station names or network data.

---

# 1774. `/transit-line-diagram` — Tek Hat Şeması

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Tek [HAT]'ın istasyon sırasını line diagram olarak göster.
>
> Transfer noktaları, yön ve terminal açık olsun.
>
> Harita gerekmiyorsa coğrafi base map ekleme.

## English

> Show the station sequence of one [LINE] as a line diagram with transfer points, direction, and terminals.
>
> Do not add a geographic basemap when it does not help the task.

---

# 1775. `/isochrone-map` — Ulaşılabilirlik Süre Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [BAŞLANGIÇ NOKTASI]'ndan gerçek ulaşım/ağ verisine dayalı:
>
> 10,
> 20,
> 30 dakika
>
> erişilebilirlik alanlarını nested isochrones olarak göster.
>
> Ulaşım türü açıkça yazılsın:
>
> yürüyüş / araç / bisiklet / transit.
>
> Gerçek route/time data yoksa ulaşım süresi uydurma.

## English

> Show 10-, 20-, and 30-minute reachable areas from [ORIGIN] as nested isochrones based on real network or travel-time data.
>
> State the travel mode clearly.
>
> Do not invent travel times without routing data.

---

# 1776. `/catchment-map` — Hizmet / Erişim Alanı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [OKUL/HASTANE/İSTASYON/HİZMET]'in gerçek catchment/service area'sını göster.
>
> Alan sınırı hangi metoda göre hesaplandıysa belirt:
>
> mesafe,
> süre,
> administrative boundary,
> observed users.
>
> Rastgele dairesel radius çizip “service area” deme.

## English

> Show the real catchment or service area of [SCHOOL/HOSPITAL/STATION/SERVICE].
>
> State whether the boundary comes from distance, travel time, administrative definition, or observed users.
>
> Do not draw an arbitrary circle and call it a service area.

---

# 1777. `/contour-map` — Eşyükselti / Kontur Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ARAZİ]'yi eşit elevation interval'a sahip contour lines ile göster.
>
> Ana/index contour gerektiğinde daha güçlü çizgi olabilir.
>
> Elevation values gerçek topographic data olmadan uydurulmasın.
>
> Konturları dekoratif dalga pattern'ına dönüştürme.

## English

> Show [TERRAIN] using contour lines at a consistent elevation interval, with stronger index contours where appropriate.
>
> Do not invent elevation values without topographic data.
>
> Avoid turning contours into decorative wave patterns.

---

# 1778. `/hillshade` — Rölyef Gölgelendirme

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [ARAZİ]'yi hillshade relief olarak göster.
>
> Işık yönü sabit ve kartografik olarak tutarlı olsun.
>
> Hillshade tematik verinin önüne geçmesin.
>
> Gerçek elevation model yoksa bunun yalnız illustrative terrain olduğunu belirt.

## English

> Show [TERRAIN] using hillshade with one consistent cartographic light direction.
>
> Keep relief secondary to thematic data.
>
> If no elevation model is supplied, treat the result as illustrative terrain rather than measured topography.

---

# 1779. `/hypsometric-tint` — Yüksekliğe Göre Renk

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Yüksekliği hypsometric tint ile göster.
>
> Renk geçişleri gerçek elevation bands'e dayansın.
>
> “Yeşil = alçak, kahverengi = yüksek” geleneğini bağlamına göre kullan; her arazi için otomatik zorunlu değildir.

## English

> Encode elevation using hypsometric tint based on real elevation bands.
>
> Use conventional green-to-brown elevation colors only where appropriate rather than as an automatic rule.

---

# 1780. `/bathymetric-map` — Deniz / Göl Derinlik Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [SU KÜTLESİ]'nin derinliğini bathymetric map olarak göster.
>
> Depth contours ve renk sınıfları gerçek bathymetry verisine dayanmalı.
>
> Kara elevation ve su depth legend'ını karıştırma.

## English

> Show depth in [WATER BODY] using a bathymetric map with real depth contours and data-based color classes.
>
> Keep terrestrial elevation and water-depth legends distinct.

---

# 1781. `/geologic-map` — Jeoloji Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [BÖLGE]'deki doğrulanmış rock/formation units'i geologic map olarak göster.
>
> Her birim:
>
> - ayrı renk/pattern,
> - legend,
> - age/unit label
>
> taşısın.
>
> Fault/fold/contact çizgileri yalnız gerçek geological data varsa eklenmeli.
>
> Jeolojik formasyon uydurma.

## English

> Show verified rock or formation units in [REGION] as a geologic map with distinct color or pattern, legend, and age or unit labels.
>
> Add faults, folds, and contacts only when supported by real geological data.
>
> Do not invent formations.

---

# 1782. `/geologic-cross-section` — Jeolojik Kesit

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Haritadaki [A–B HATTI] boyunca geologic cross-section göster.
>
> Surface topography ile subsurface layers birbiriyle ilişkili olsun.
>
> Vertical exaggeration varsa açıkça belirt.
>
> Yer altı geometri/kalınlıkları veri olmadan uydurulmasın.

## English

> Show a geologic cross-section along [A–B LINE], relating surface topography to subsurface layers.
>
> State any vertical exaggeration explicitly.
>
> Do not invent subsurface geometry or thickness without supporting data.

---

# 1783. `/land-use-map` — Arazi Kullanım Haritası

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [BÖLGE]'deki land-use classes'i nitel categorical map olarak göster.
>
> Tarım, yerleşim, orman, sanayi vb kategoriler kolay ayırt edilsin.
>
> Nicel sequential color scale kullanma.
>
> Sınıflandırma veri kaynağını koru.

## English

> Show land-use classes in [REGION] as a qualitative categorical map with clearly distinguishable classes such as agriculture, settlement, forest, or industry.
>
> Avoid quantitative sequential color scales for nominal categories.

---

# 1784. `/land-cover-change` — Arazi Örtüsü Değişimi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Aynı bölgenin [TARİH 1] ve [TARİH 2] land-cover durumunu matched maps olarak göster.
>
> Sınıf renkleri, projection, extent ve scale aynı kalsın.
>
> Üçüncü panelde yalnız gerçek change areas gösterilebilir.

## English

> Show land cover for the same region at [DATE 1] and [DATE 2] using matched maps with the same class colors, projection, extent, and scale.
>
> A third panel may show only real change areas.

---

# 1785. `/map-small-multiples` — Harita Small Multiples

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [DEĞİŞKEN]'i farklı zaman/kategori için 4–12 küçük matched map'te göster.
>
> Tüm haritalarda:
>
> - extent,
> - projection,
> - legend,
> - color scale
>
> aynı kalsın.
>
> Her panelde farklı styling kullanma.

## English

> Show [VARIABLE] across 4–12 matched small-multiple maps for different times or categories.
>
> Keep extent, projection, legend, and color scale identical.
>
> Do not restyle every panel independently.

---

# 1786. `/map-change-sequence` — Zaman İçinde Harita Dizisi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [OLAY]'ın mekânsal değişimini 4–8 tarihli map sequence olarak göster.
>
> Aynı map frame ve legend kullan.
>
> Değişen alanları yalnız gerektiğinde highlight et.
>
> Kamera/extent değiştirilerek değişim abartılmasın.

## English

> Show spatial change in [EVENT] across 4–8 dated maps using one consistent map frame and legend.
>
> Highlight changes only where necessary.
>
> Do not exaggerate change by altering extent or viewpoint.

---

# 1787. `/map-label-hierarchy` — Harita Etiket Hiyerarşisi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## 2026 kartografya ilkeleriyle uyumlu

## Türkçe

> Haritadaki label'ları önem sırasına göre düzenle:
>
> 1. ana tema/yer,
> 2. büyük yerleşim,
> 3. ikincil yer,
> 4. fiziksel feature,
> 5. yardımcı bilgi.
>
> Font size/weight farkı ölçülü olsun.
>
> Her etiketi aynı görsel düzleme çıkarma.

## English

> Structure map labels by importance:
>
> primary theme or place, major settlements, secondary places, physical features, and supporting information.
>
> Use restrained size and weight differences.
>
> Do not place every label on the same visual plane.

---

# 1788. `/basemap-recede` — Base Map'i Geri Çek

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## 2026 Esri StoryMaps yaklaşımı

## Türkçe

> Base map yalnız yön ve bağlam sağlasın.
>
> Tematik katman öncelikliyse:
>
> - road detail,
> - POI,
> - labels,
> - terrain contrast
>
> azaltılabilir.
>
> Base map'in tematik layer ile görsel rekabet etmesine izin verme.

## English

> Let the basemap provide only orientation and geographic context.
>
> When the thematic layer is primary, reduce road detail, points of interest, labels, and terrain contrast.
>
> Do not let the basemap compete visually with the data.

---

# 1789. `/map-figure-ground` — Figure–Ground Ayrımı

## Türkçe

> Ana çalışma alanını çevresinden figure–ground mantığıyla ayır.
>
> Kullan:
>
> - screening,
> - muted surround,
> - sınır,
> - controlled vignette
>
> gibi yalnız bir yöntem.
>
> Büyük drop shadow ile ülkeyi “floating island” yapma.

## English

> Separate the primary study area from its surroundings using one restrained figure–ground method such as screening, muted context, boundary emphasis, or controlled vignette.
>
> Avoid giant drop shadows that make the region look like a floating island.

## Neye dikkat edilmeli?

Bilgi kilidi: kaynak, tarih ve gösterim yöntemi görselde belirtilsin; kaynaksız infografik kullanılmaz ([§1830](#sec-1830)).

---
# 1790. `/map-projection-choice` — Projeksiyon Seçimini Belirt

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Haritanın amacına göre projection seçimini açıkça belirt.
>
> Dünya haritasında:
>
> - alan,
> - şekil,
> - mesafe,
> - yön
>
> özelliklerinden hangisinin öncelikli olduğunu yaz.
>
> Web Mercator'u her harita için otomatik varsayma.

## English

> State the map projection according to purpose.
>
> For world maps, clarify whether area, shape, distance, or direction is the priority.
>
> Do not default automatically to Web Mercator for every task.

---

# 1791. `/equal-area-map` — Alan Karşılaştırması İçin Eşit Alan Projeksiyonu

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Ülkeler/bölgeler arası alan-temelli thematic comparison için equal-area projection kullan.
>
> Haritada alan büyüklüğü veri yorumunu etkiliyorsa şekil bozulmasından çok alan korunması öncelikli olsun.

## English

> Use an equal-area projection for thematic comparisons where geographic area affects interpretation.
>
> Prioritize area preservation over exact shape.

---

# 1792. `/map-scale-lock` — Harita Ölçeğini Sabitle

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Karşılaştırmalı iki veya daha fazla haritada aynı extent ve scale kullan.
>
> Bir bölgeyi daha dramatik göstermek için zoom seviyesini değiştirme.

## English

> Preserve the same extent and scale across comparative maps.
>
> Do not change zoom level to make one region appear more dramatic.

---

# 1793. `/map-data-lock` — Harita Veri Kilidi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Haritadaki:
>
> - sınır,
> - değer,
> - tarih,
> - coordinate,
> - route,
> - category
>
> yalnız kullanıcı tarafından sağlanan veya doğrulanmış geospatial data'dan gelsin.
>
> Eksik coğrafi bilgiyi image modelin tamamlamasına güvenme.

## English

> Use only supplied or verified geospatial data for boundaries, values, dates, coordinates, routes, and categories.
>
> Do not rely on image generation to fill missing geographic facts.

---

# 1794. `/map-source-note` — Harita Kaynak Notu

## Türkçe

> Haritanın altında küçük:
>
> veri kaynağı,
> tarih,
> projection,
> gerekiyorsa class method
>
> alanı bırak.
>
> Kaynağı tasarım uğruna görünmez yapma.

## English

> Leave a small source note beneath the map for data source, date, projection, and classification method where relevant.
>
> Do not hide source information for aesthetic reasons.

## Neye dikkat edilmeli?

Bilgi kilidi: kaynak, tarih ve gösterim yöntemi görselde belirtilsin; kaynaksız infografik kullanılmaz ([§1830](#sec-1830)).

---
# 1795. `/map-slop-filter` — Harita AI Slop Filtresi

Kaçınılması gerekenler:

- uydurma sınır,
- yanlış coastline,
- sahte koordinat,
- her thematic map'te rainbow scale,
- base map'in ana veriden daha güçlü olması,
- Web Mercator'u otomatik kullanmak,
- 3B perspective ile değer algısını bozmak,
- decorative pin icon kalabalığı,
- class breaks'i açıklamamak,
- legenda uymayan renk,
- haritayı infographic sticker board'a çevirmek.

---

# 1796. Yeni üst aile: `Cartographic Grammar`

Aile:

- `/reference-map`
- `/thematic-map`
- `/choropleth`
- `/proportional-symbol-map`
- `/dot-density-map`
- `/flow-map`
- `/transit-map`
- `/isochrone-map`
- `/contour-map`
- `/geologic-map`

Ana formül:

> **question + geographic unit + data type + encoding + projection + scale + legend + source**

---

<a id="aile-030"></a>
# “Infographic” Tek Bir Görsel Türü Değildir

Adobe’nin Haziran 2026 infographic rehberi de iyi infographic’in temelini:

- information hierarchy,
- doğru format seçimi,
- uygun chart,
- renk,
- okunabilirlik

üzerinden tanımlıyor.

Bu yüzden:

> `make an infographic`

çoğu zaman yeterli değildir.

Önce:

> **hangi bilgi ilişkisi?**

sorulmalıdır.

---

# 1797. `/visual-format-selector` — Görsel Türü Seçici

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [İÇERİK]'teki ana bilgi ilişkisini belirle:
>
> - yapı,
> - parça,
> - süreç,
> - sıra,
> - zaman,
> - karşılaştırma,
> - miktar,
> - dağılım,
> - coğrafya,
> - ilişki/ağ,
> - hiyerarşi,
> - kavram/metafor.
>
> Sonra en az bir uygun format seç.

## English

> Identify the primary information relationship in [CONTENT]:
>
> structure, parts, process, sequence, time, comparison, quantity, distribution, geography, network, hierarchy, or concept/metaphor.
>
> Then select the appropriate visual format.

---

# 1798. `/diagram-vs-illustration` — Diyagram mı İllüstrasyon mu?

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Diagram

Amaç:

> **ilişkiyi açıklamak.**

Önemli:

- ok,
- sıra,
- katman,
- bağlantı,
- label.

## Illustration

Amaç:

> **bir şeyi veya fikri görsel olarak temsil etmek.**

Önemli:

- form,
- sahne,
- metafor,
- görsel anlatım.

### Rehber kuralı

> “Nasıl çalışıyor?” → diagram.
>
> “Nasıl görünüyor / ne hissettiriyor?” → illustration.

---

# 1799. `/diagram-vs-infographic` — Diyagram mı Infographic mi?

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Diagram

Tek yapı/ilişkiyi açıklar.

## Infographic

Birden fazla bilgi türünü:

- text,
- chart,
- number,
- diagram,
- icon

ile tek bilgi hiyerarşisinde birleştirebilir.

### Kural

Bir tek mekanizmayı anlatıyorsan:

> infographic gerekmeyebilir.

---

# 1800. `/chart-vs-infographic` — Chart mı Infographic mi?

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Chart

> sayısal veriyi kodlar.

## Infographic

> sayısal veriyi bağlam içinde anlatabilir.

### Kural

Kullanıcının sorusu:

> “Değerler nasıl karşılaştırılıyor?”

ise önce chart.

> “Bu verinin ne anlama geldiğini nasıl anlatırım?”

ise chart + explanatory infographic düşünülebilir.

---

# 1801. `/map-vs-diagram` — Harita mı Şema mı?

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Map

Coğrafi konum/mesafe/alan önemlidir.

## Diagram

Topolojik sıra veya ilişki önemlidir.

Örnek:

Metro:

- gerçek coğrafya → map.
- durak sırası/transfer → schematic transit diagram.

---

# 1802. `/photo-vs-illustration` — Fotoğraf mı İllüstrasyon mu?

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Fotoğraf

Gerçek görünüş ve fiziksel kanıt önemliyse.

## İllüstrasyon

- görünmeyeni göstermek,
- sadeleştirmek,
- soyut kavram,
- tarihsel rekonstrüksiyon,
- yapısal açıklama

gerekiyorsa daha uygun olabilir.

### Kural

> Gerçeklik iddiası yükseldikçe kaynak doğrulaması da yükselmelidir.

---

# 1803. `/annotated-photo` — Açıklamalı Fotoğraf

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Gerçek kaynak fotoğrafı koru ve yalnız 3–7 kritik özellik için callout ekle.
>
> Yeni nesne/özellik çizerek fotoğrafı değiştirme.
>
> Annotation, görüntüde gerçekten görülebilen ayrıntıya işaret etsin.

## English

> Preserve the real source photograph and add callouts for only 3–7 critical visible features.
>
> Do not draw new objects or features into the photograph.
>
> Make every annotation point to something genuinely visible.

---

# 1804. `/infographic` — Kontrollü Infographic

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe prompt

> [KONU]'yu infographic olarak düzenle ancak önce bilgi hiyerarşisini kur.
>
> En fazla:
>
> - 1 ana mesaj,
> - 3–5 ana bölüm,
> - 1–2 veri görseli,
> - gerekli kısa açıklama
>
> kullan.
>
> Her bölüm için ayrı ikon, card ve gradient üretme.
>
> Veri yoksa sahte yüzde/sayı ekleme.

## English

> Structure [TOPIC] as an infographic with one primary message, 3–5 major sections, no more than 1–2 data visualizations, and only necessary concise explanation.
>
> Avoid separate icons, cards, and gradients for every section.
>
> Do not invent percentages or statistics.

---

# 1805. `/stat-card` — Tek Sayısal Bulguyu Gösterme

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Kullanıcı tarafından verilen [SAYI/ORAN]'ı tek stat card olarak göster.
>
> Büyük değer + kısa açıklama + kaynak/tarih.
>
> Arka plana dekoratif chart ekleme.
>
> Bir sayı için tam infographic üretme.

## English

> Show user-supplied [NUMBER/RATE] as one stat card using a large value, concise explanation, and source or date.
>
> Do not add decorative charts in the background.
>
> Avoid building an entire infographic for one number.

---

# 1806. `/comparison-infographic` — Karşılaştırma Infographic'i

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [A] ve [B]'yi yalnız aynı kategoriler üzerinden karşılaştır.
>
> 4–7 comparison row yeterli.
>
> Her satırda aynı birim ve ölçek kullan.
>
> A ve B için farklı ölçüm kriterleri kullanma.

## English

> Compare [A] and [B] using only matched categories.
>
> Use 4–7 comparison rows with consistent units and scales.
>
> Do not evaluate A and B using different criteria.

---

# 1807. `/process-infographic` — Süreç Infographic'i

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [SÜREÇ]'i 4–7 adımda göster.
>
> Her adım:
>
> - numara,
> - kısa fiil,
> - tek görsel/diagram
>
> taşısın.
>
> Süreci timeline, cycle ve flowchart öğelerini aynı anda kullanarak karmaşıklaştırma.

## English

> Show [PROCESS] in 4–7 steps using one number, concise action verb, and one visual or diagram per step.
>
> Do not mix timeline, cycle, and flowchart conventions unnecessarily.

---

# 1808. `/timeline-infographic` — Zaman Odaklı Infographic

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [OLAYLAR]'ı kronolojik tek eksen üzerinde göster.
>
> Tarihler gerçek veriyle eşleşsin.
>
> Olay yoğunluğu çok farklıysa spacing'in gerçek zaman ölçeği mi yoksa ordinal sequence mi olduğunu belirt.

## English

> Show [EVENTS] on one chronological axis with verified dates.
>
> If spacing does not represent actual time intervals, make it clear that the sequence is ordinal rather than time-scaled.

---

# 1809. `/hierarchy-infographic` — Hiyerarşi Görseli

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [SİSTEM]'de üst–alt ilişkisini 3–5 level hierarchy olarak göster.
>
> Box sayısı arttıkça font küçültme yerine yapıyı sadeleştir.
>
> Hierarchy ile network'ü karıştırma.

## English

> Show the parent–child structure of [SYSTEM] across 3–5 hierarchy levels.
>
> Simplify when the number of nodes grows rather than shrinking all text.
>
> Do not confuse hierarchy with a network.

---

# 1810. `/list-infographic` — Görsel Liste

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [5–10 MADDE]'yi infographic list olarak düzenle.
>
> Her madde için büyük ayrı illustration zorunlu değil.
>
> Numara, kısa başlık ve tek satır açıklama yeterli olabilir.
>
> Listeyi decorative card dashboard'a dönüştürme.

## English

> Present [5–10 ITEMS] as a visual list using numbers, concise headings, and one-line descriptions.
>
> A separate illustration for every item is not required.
>
> Avoid turning the list into a decorative card dashboard.

---

# 1811. `/chart-first-infographic` — Önce Grafik

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [VERİ]'nin ana chart'ını önce tasarla.
>
> Infographic'in başlık, annotation ve açıklama öğeleri chart'ı desteklesin.
>
> Chart'ı küçük köşeye sıkıştırıp dekoratif illüstrasyonu ana öğe yapma.

## English

> Design the primary chart for [DATA] first.
>
> Let the title, annotations, and explanation support the chart.
>
> Do not shrink the chart into a corner while decorative illustration becomes the main element.

---

# 1812. `/annotated-chart` — Açıklamalı Grafik

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Gerçek [CHART]'ın üzerinde yalnız 2–5 kritik veri noktasına kısa annotation ekle.
>
> Annotation:
>
> - ne oldu,
> - ne zaman,
> - neden önemli
>
> gibi tek açıklama taşısın.
>
> Her noktayı etiketleme.

## English

> Add concise annotations to only 2–5 critical points on the real [CHART], explaining what happened, when, or why it matters.
>
> Do not label every point.

---

# 1813. `/small-multiple-chart` — Small Multiple Grafik

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KATEGORİLER]'i aynı chart türü ve scale ile 4–12 küçük panelde karşılaştır.
>
> Tüm panel eksenleri eşleşsin.
>
> Her panel için otomatik farklı y-axis kullanma.

## English

> Compare [CATEGORIES] across 4–12 small-multiple charts using the same chart type and scale.
>
> Keep axes matched.
>
> Do not auto-scale each y-axis independently.

---

# 1814. `/slope-chart` — İki Zaman Noktası Değişim Grafiği

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KATEGORİLER]'in [TARİH A] ile [TARİH B] arasındaki değişimini slope chart olarak göster.
>
> Başlangıç ve bitiş değerleri aynı scale üzerinde olsun.
>
> Çok fazla kategori varsa yalnız anlamlı subset kullan.

## English

> Show change in [CATEGORIES] between [DATE A] and [DATE B] using a slope chart on one common scale.
>
> If too many categories create clutter, use a meaningful subset.

---

# 1815. `/bump-chart` — Sıralama Değişimi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KATEGORİLER]'in zaman içindeki rank değişimini bump chart olarak göster.
>
> Y ekseni rank olmalı; raw value ile karıştırma.
>
> Kullanıcı değer büyüklüğü istiyorsa başka chart ekle.

## English

> Show changes in rank over time for [CATEGORIES] using a bump chart.
>
> Keep the y-axis as rank rather than raw value.
>
> Use another chart when magnitude is also important.

---

# 1816. `/dot-plot` — Nokta Grafiği

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KATEGORİLER]'i aynı numeric axis üzerinde dot plot ile karşılaştır.
>
> Bar fill yerine konumu ana encoding yap.
>
> Çok yakın değerlerde label/spacing okunabilirliği koru.

## English

> Compare [CATEGORIES] on one numeric axis using a dot plot where position is the primary encoding.
>
> Preserve readability when values are close.

---

# 1817. `/lollipop-chart` — Lollipop Grafik

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KATEGORİLER]'i bar chart yerine hafif lollipop chart ile göster.
>
> Stem ince, dot ana değer göstergesi olsun.
>
> Çok fazla kategori varsa chart'ı dekoratif çizgi ormanına dönüştürme.

## English

> Show [CATEGORIES] using a restrained lollipop chart with thin stems and dots as the primary value markers.
>
> Avoid clutter with too many categories.

---

# 1818. `/range-plot` — Aralık Grafiği

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Her [KATEGORİ] için min–max veya başlangıç–bitiş aralığını aynı eksen üzerinde göster.
>
> Aralığın neyi temsil ettiği legend/label ile açık olsun.
>
> Midpoint varsa ayrı işaretle.

## English

> Show minimum–maximum or start–end range for each [CATEGORY] on one shared axis.
>
> Clarify what the range represents.
>
> Mark any midpoint separately.

---

# 1819. `/distribution-plot` — Dağılımı Göster

## Türkçe

> Yalnız ortalama bar'ı yerine [VERİ]'nin dağılımını göster.
>
> Uygun olduğunda:
>
> - individual points,
> - box plot,
> - histogram,
> - density
>
> seçeneklerinden biri kullanılabilir.
>
> Veri yapısına uymayan decorative violin plot üretme.

## English

> Show the distribution of [DATA] rather than only a mean bar.
>
> Use individual points, box plot, histogram, or density where appropriate.
>
> Do not choose a decorative distribution form that does not fit the data.

## Neye dikkat edilmeli?

Bilgi kilidi: kaynak, tarih ve gösterim yöntemi görselde belirtilsin; kaynaksız infografik kullanılmaz ([§1830](#sec-1830)).

---
# 1820. `/table-first` — Grafik Yerine Tablo

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Önemli karar

Bazı sorular için grafik kötü seçimdir.

## Türkçe

> Kullanıcı kesin değerleri tek tek okumalıysa veya kategori sayısı azsa, chart yerine temiz table düşün.
>
> Tabloyu gereksiz heatmap/ikonlarla infographic'e dönüştürme.

## English

> When readers need exact values or the category count is small, consider a clean table instead of a chart.
>
> Do not decorate the table into an unnecessary heatmap or icon infographic.

---

# 1821. `/chart-type-by-task` — Göreve Göre Grafik Seçimi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

| Soru | Öncelikli grafik |
|---|---|
| Kategoriler ne kadar farklı? | bar / dot plot |
| Zaman içinde nasıl değişiyor? | line |
| Dağılım nasıl? | histogram / dot / box |
| İki zaman noktası nasıl değişti? | slope |
| Sıralama nasıl değişti? | bump |
| Parça-bütün ilişkisi? | stacked bar / 100% stacked |
| İki değişken ilişkili mi? | scatter |
| Aralık ne? | range plot |
| Kesin değer okunacak mı? | table |
| Coğrafi dağılım mı? | map |

Bu tablo “her şeyi pie chart yapma” sorununu azaltır.

---

# 1822. `/pie-chart-check` — Pasta Grafik Kontrolü

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Pie/donut yalnız:
>
> - gerçek part-to-whole,
> - az kategori,
> - toplam = %100
>
> olduğunda düşün.
>
> 8–12 dilimli pie chart üretme.
>
> Kategori karşılaştırması önemliyse bar/dot daha uygun olabilir.

## English

> Use pie or donut only for genuine part-to-whole relationships with few categories summing to 100%.
>
> Avoid pie charts with many slices.
>
> Prefer bars or dots when precise category comparison matters.

---

# 1823. `/dual-axis-warning` — Çift Eksen Uyarısı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> İki farklı birimi aynı chart'ta dual axis ile göstermeden önce gerçekten gerekli olup olmadığını kontrol et.
>
> İki seri ayrı small multiples ile daha açık anlatılabiliyorsa onu tercih et.
>
> Ölçekleri manipüle ederek sahte ilişki oluşturma.

## English

> Before using a dual-axis chart for different units, check whether separate matched panels would communicate more clearly.
>
> Do not manipulate scales to imply a misleading relationship.

---

# 1824. `/zero-baseline-check` — Sıfır Başlangıç Kontrolü

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Bar chart'ta uzunluk değer temsil ediyorsa baseline çoğu durumda zero'dan başlamalı.
>
> Line chart'ta bağlama göre truncated axis kullanılabilir ancak açıkça okunmalı.
>
> Görsel dramatizasyon için ekseni gizlice kesme.

## English

> When bar length encodes magnitude, the baseline should usually begin at zero.
>
> Truncated axes may be appropriate for line charts in context, but must remain explicit.
>
> Do not secretly crop axes for drama.

---

# 1825. `/uncertainty-lock` — Belirsizlik Kilidi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Veri:
>
> - confidence interval,
> - margin of error,
> - range,
> - missing values
>
> içeriyorsa görselde kaybolmasın.
>
> Eksik veriyi sıfır gibi gösterme.

## English

> Preserve confidence intervals, margins of error, ranges, and missing values when present.
>
> Do not represent missing data as zero.

---

# 1826. `/missing-data-style` — Eksik Veriyi Açıkça Göster

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Missing/no-data bölgelerini gerçek sıfır değerinden görsel olarak ayır.
>
> Harita veya chart legend'ında ayrı “no data” kategorisi kullan.

## English

> Distinguish missing or unavailable data visually from true zero values.
>
> Use a separate “no data” category in chart or map legends.

---

# 1827. `/source-footnote` — Veri Kaynağı Dipnotu

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Veri görselinin altında:
>
> - source,
> - date,
> - unit,
> - gerekiyorsa method
>
> bilgisi için küçük alan bırak.
>
> Kaynağı yalnız metadata içinde saklama.

## English

> Leave a concise source note beneath the visualization for source, date, unit, and method where relevant.
>
> Do not hide provenance only in metadata.

---

# 1828. `/chart-accuracy-lock` — Grafik Doğruluk Kilidi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Chart'taki bütün:
>
> - değer,
> - label,
> - axis,
> - unit,
> - date,
> - category
>
> supplied data ile bire bir eşleşsin.
>
> Image-generation modelinin veri noktası uydurmasına izin verme.

## English

> Make every chart value, label, axis, unit, date, and category match supplied data exactly.
>
> Do not let the image-generation model invent data points.

---

# 1829. `/chart-not-imagegen` — Sayısal Grafik İçin Image Generation Kullanma

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Kritik rehber notu

Eğer çıktı:

- exact bar chart,
- exact line chart,
- scatter plot,
- histogram,
- map with verified values,
- statistical figure

ise:

> **grafiği image-generation modeliyle üretmek doğru ana yöntem değildir.**

Kullan:

- spreadsheet,
- Python/R,
- Datawrapper,
- Flourish,
- GIS,
- chart library.

Image-generation modeli daha sonra:

- illustration,
- background,
- supporting visual,
- cover art

için kullanılabilir.

### Kısa kural

> **Sayısal doğruluk → data tool.**
>
> **Görsel temsil → image model.**

---

<a id="sec-1830"></a>
# 1830. `/infographic-source-lock` — Infographic Kaynak Kilidi

## Türkçe

> Infographic'teki sayı, iddia, tarih ve karşılaştırmalar yalnız kullanıcı tarafından verilen veya doğrulanmış kaynaktan gelsin.
>
> Tasarım boşluğu doldurmak için:
>
> “%87”
> “3x faster”
> “1 in 5”
>
> gibi sahte headline statistic üretme.

## English

> Use only supplied or verified sources for numbers, claims, dates, and comparisons in the infographic.
>
> Do not fabricate headline statistics such as “87%,” “3x faster,” or “1 in 5” to fill design space.

## Neye dikkat edilmeli?

Bilgi kilidi: kaynak, tarih ve gösterim yöntemi görselde belirtilsin; kaynaksız infografik kullanılmaz ([§1830](#sec-1830)).

---
# 1831. `/legend-first` — Legend'ı En Baştan Planla

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Renk, boyut, shape veya pattern veri taşıyorsa legend'ı görsel tamamlandıktan sonra ekleme.
>
> Encoding ile birlikte tasarla.
>
> Legend'da kullanılan sembol ile haritadaki/grafikteki sembol bire bir eşleşsin.

## English

> When color, size, shape, or pattern carries data, design the legend alongside the encoding rather than adding it afterward.
>
> Make legend symbols match the visualization exactly.

---

# 1832. `/color-not-alone` — Bilgiyi Yalnız Renkle Kodlama

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Erişilebilirlik

## Türkçe

> Kritik kategorileri yalnız hue farkıyla ayırma.
>
> Gerektiğinde:
>
> - label,
> - shape,
> - pattern,
> - line style
>
> gibi ikinci cue kullan.
>
> Özellikle print ve color-vision farklılıklarını düşün.

## English

> Do not distinguish critical categories by hue alone.
>
> Where needed, add labels, shape, pattern, or line style as a second cue.
>
> Account for print and color-vision differences.

---

# 1833. `/data-ink-reduction` — Gereksiz Görsel Mürekkebi Azalt

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Veri okumaya katkı sağlamayan:
>
> - ağır grid,
> - 3B bevel,
> - gradient,
> - shadow,
> - decorative icon,
> - chart frame
>
> öğelerini kaldır.
>
> Görsel sadeleşirken gerekli axis/legend bilgisini kaybetme.

## English

> Remove heavy grids, 3D bevels, gradients, shadows, decorative icons, and chart frames that do not help data reading.
>
> Simplify without removing necessary axes or legends.

---

# 1834. `/progressive-data-story` — Veriyi Aşamalı Anlat

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Karmaşık [VERİ]'yi tek infographic'e sıkıştırmak yerine:
>
> 1. bağlam,
> 2. ana chart,
> 3. kritik annotation,
> 4. comparison,
> 5. sonuç
>
> sırasıyla göster.
>
> Scrollytelling veya carousel kullanılabilir.

## English

> Instead of compressing complex [DATA] into one infographic, reveal it progressively:
>
> context → primary chart → critical annotation → comparison → conclusion.
>
> Use scrollytelling or carousel where appropriate.

---

# 1835. `/data-story-card` — Tek Bulgulu Veri Kartı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Tek kartta yalnız:
>
> - bir bulgu,
> - bir chart/cue,
> - bir kısa açıklama,
> - kaynak
>
> olsun.
>
> Bir carousel serisinde her kart farklı bir soru cevaplasın.

## English

> Keep each data-story card focused on one finding, one chart or cue, one concise explanation, and the source.
>
> Let each card in a carousel answer a different question.

---

# 1836. `/infographic-slop-filter` — Infographic AI Slop Filtresi

Kaçınılması gerekenler:

- her bölüm card,
- her madde icon,
- her veri pie chart,
- sahte yüzde,
- decorative dashboard,
- 3B chart,
- rainbow palette,
- gereksiz timeline,
- chart yerine büyük sayı balonları,
- kaynaksız statistic,
- infographic = her şeyi tek A4'e sıkıştırmak.

---

# 1837. Yeni üst aile: `Quantitative Visual`

Aile:

- bar,
- line,
- dot plot,
- histogram,
- scatter,
- range,
- small multiple,
- thematic map,
- table.

Ana kural:

> **görsel form, veri tipinden ve kullanıcı sorusundan türemeli.**

---

# 1838. Yeni üst aile: `Format Decision Grammar`

Temel karar ağacı:

### Fiziksel yapı mı?
→ illustration / anatomy / cutaway / exploded.

### Süreç mi?
→ step-by-step / flowchart / sequence.

### Zaman mı?
→ timeline / line chart.

### Sayısal karşılaştırma mı?
→ chart / table.

### Coğrafi dağılım mı?
→ map.

### Kavramsal fikir mi?
→ editorial illustration / concept map.

### Çoklu bilgi + bağlam mı?
→ infographic.

### Gerçek fiziksel kanıt mı?
→ photo / annotated photo.

### Öğrenme etkinliği mi?
→ worksheet / visual notes / diagram.

Bu karar ağacı, promptta yanlış format seçimini azaltır.

---

# 1839. `/format-purpose-line` — Prompt Başına Amaç Satırı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Yeni rehber kalıbı

Her karmaşık promptun ilk satırında şu yapı kullanılabilir:

> **Purpose: [what should the viewer understand/do?]**

Örnek:

> `Purpose: compare how unemployment rate differs by province.`

Ardından:

> `Format: choropleth map.`

Bu, modelin sadece “güzel görsel” üretmesini engeller.

---

# 1840. `/encoding-purpose-line` — Veri Encoding Satırı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Örnek

> `Value → circle area`
>
> `Category → color`
>
> `Time → x-position`
>
> `Uncertainty → error bar`

Bir data visualization promptunda bu ilişkileri açıkça yazmak:

> modelin estetik keyfîliğini azaltır.

---

# 1841. Bu turdaki slash-style indeks (aile-030)

| Kısayol | Aile |
|---|---|
| `/map-purpose` | define map question first |
| `/reference-map` | general geographic reference |
| `/thematic-map` | one geographic variable |
| `/choropleth` | rate/percentage by area |
| `/choropleth-class-check` | classification audit |
| `/proportional-symbol-map` | count by symbol area |
| `/dot-density-map` | distribution by unit dots |
| `/graduated-symbol-map` | classified symbol sizes |
| `/flow-map` | directional geographic flow |
| `/desire-line-map` | origin–destination relation |
| `/route-map` | actual network route |
| `/transit-map` | schematic transit network |
| `/transit-line-diagram` | one line/station sequence |
| `/isochrone-map` | travel-time accessibility |
| `/catchment-map` | service/catchment area |
| `/contour-map` | elevation contours |
| `/hillshade` | shaded terrain relief |
| `/hypsometric-tint` | elevation color bands |
| `/bathymetric-map` | water depth |
| `/geologic-map` | geologic units |
| `/geologic-cross-section` | subsurface section |
| `/land-use-map` | categorical land use |
| `/land-cover-change` | matched temporal land cover |
| `/map-small-multiples` | repeated matched maps |
| `/map-change-sequence` | spatial change over time |
| `/map-label-hierarchy` | label visual order |
| `/basemap-recede` | de-emphasize basemap |
| `/map-figure-ground` | area-of-interest emphasis |
| `/map-projection-choice` | projection by purpose |
| `/equal-area-map` | area-preserving comparison |
| `/map-scale-lock` | matched map scale |
| `/map-data-lock` | verified geospatial data only |
| `/map-source-note` | map provenance |
| `/visual-format-selector` | choose visual by relationship |
| `/diagram-vs-illustration` | explanatory relation vs representation |
| `/diagram-vs-infographic` | one relation vs multi-info composition |
| `/chart-vs-infographic` | numeric encoding vs contextual story |
| `/map-vs-diagram` | geography vs topology |
| `/photo-vs-illustration` | evidence vs constructed explanation |
| `/annotated-photo` | source photo + factual callouts |
| `/infographic` | controlled information hierarchy |
| `/stat-card` | one supplied statistic |
| `/comparison-infographic` | matched comparison |
| `/process-infographic` | process summary |
| `/timeline-infographic` | chronological summary |
| `/hierarchy-infographic` | parent-child structure |
| `/list-infographic` | structured visual list |
| `/chart-first-infographic` | chart-led explanation |
| `/annotated-chart` | chart + key annotations |
| `/small-multiple-chart` | matched chart panels |
| `/slope-chart` | two-point change |
| `/bump-chart` | rank over time |
| `/dot-plot` | categorical numeric comparison |
| `/lollipop-chart` | lightweight categorical comparison |
| `/range-plot` | min/max or start/end |
| `/distribution-plot` | show spread/distribution |
| `/table-first` | exact-value table choice |
| `/chart-type-by-task` | task-based chart selection |
| `/pie-chart-check` | part-to-whole guardrail |
| `/dual-axis-warning` | dual-axis caution |
| `/zero-baseline-check` | axis integrity |
| `/uncertainty-lock` | preserve uncertainty |
| `/missing-data-style` | no-data ≠ zero |
| `/source-footnote` | visible data provenance |
| `/chart-accuracy-lock` | exact chart-data match |
| `/chart-not-imagegen` | use data tools for exact charts |
| `/infographic-source-lock` | verified infographic claims |
| `/legend-first` | design legend with encoding |
| `/color-not-alone` | accessible redundant encoding |
| `/data-ink-reduction` | remove non-informative decoration |
| `/progressive-data-story` | staged data explanation |
| `/data-story-card` | one-finding information card |
| `/format-purpose-line` | state visual purpose first |
| `/encoding-purpose-line` | state data-to-visual mapping |

---

<a id="aile-031"></a>
# Erişilebilir Görsel Yazarlığı, Alt Text, Long Description ve Educational Comics — 2026 Ek Taraması

W3C Web Accessibility Initiative’in Nisan 2026’da güncellediği **Images Tutorial**, görselleri tek bir “alt text yaz” kuralıyla ele almıyor. Görselin **sayfadaki işlevine** göre farklı davranmak gerekiyor:

- informative image,
- decorative image,
- functional image,
- image of text,
- complex image,
- group of images.

Özellikle:

- chart,
- graph,
- flowchart,
- organizational chart,
- diagram,
- information-rich illustration,
- map

gibi **complex images** için kısa bir `alt` cümlesinin tek başına yetmeyebileceği; kısa tanım + ayrıntılı text equivalent / long description yaklaşımının gerekebileceği belirtiliyor.

Bu rehber için sonuç:

> **Erişilebilirlik, görsel üretildikten sonra yazılan bir alt text işi değildir.**
>
> Görselin hangi bilgiyi yalnız görsel kanaldan taşıdığı daha prompt aşamasında düşünülmelidir.

Ayrıca W3C’nin 2026 güncel tasarım rehberlerinde bilgi için **rengin tek başına kullanılmaması** gerektiği yeniden vurgulanıyor. Grafik nesnelerin sınırları bilgi taşıyorsa yeterli non-text contrast veya alternatif ayırıcılar gerekebilir.

---

# 1842. `/image-purpose-audit` — Görselin İşlevini Belirle

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

Alt text yazmadan önce ilk soru:

> Bu görsel bu bağlamda ne yapıyor?

## Kategoriler

### Informative

Yeni bilgi taşıyor.

### Decorative

Metne yeni bilgi eklemiyor.

### Functional

Buton/link/eylem işlevi taşıyor.

### Image of text

Okunması gereken metni görüntü olarak içeriyor.

### Complex

Tek cümlede aktarılamayacak kadar yapısal/verisel bilgi taşıyor.

## Türkçe prompt

> [GÖRSEL]'i erişilebilirlik açısından sınıflandır:
>
> informative / decorative / functional / image-of-text / complex.
>
> Kararı yalnız görselin görünüşüne göre değil, sayfadaki kullanım amacına göre ver.
>
> Ardından uygun text-alternative yaklaşımını öner.

## English

> Classify [IMAGE] for accessibility as informative, decorative, functional, image-of-text, or complex.
>
> Base the decision on the image’s purpose in context rather than appearance alone.
>
> Then recommend the appropriate text-alternative strategy.

---

# 1843. `/alt-text` — Kısa Alt Text

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## W3C ilkesiyle uyumlu

Alt text’in amacı:

> görüntüyü şiirsel biçimde tarif etmek değil,
>
> **bağlam için gerekli bilgiyi aktarmaktır.**

## Türkçe prompt

> [GÖRSEL] için kısa alt text yaz.
>
> Önce bu görselin sayfadaki amacını dikkate al.
>
> En önemli bilgiyi cümlenin başında ver.
>
> Görselde bağlam açısından önemsiz:
>
> - renk,
> - kıyafet,
> - arka plan,
> - dekor
>
> ayrıntılarını otomatik ekleme.
>
> “Görselde...”, “bir resim...” gibi gereksiz giriş kullanma.

## English

> Write concise alt text for [IMAGE] based on its purpose in context.
>
> Put the most important information first.
>
> Omit colors, clothing, background, and decorative details unless they are relevant to the meaning.
>
> Avoid unnecessary openings such as “image of” or “picture of.”

---

# 1844. `/alt-text-purpose-first` — Bağlama Göre Alt Text

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

Aynı fotoğrafın alt text’i kullanım yerine göre değişebilir.

Örneğin bir kuş fotoğrafı:

### Park sitesi

> Gölet kenarında bir yaban ördeği.

### Kuş türleri rehberi

> Erkek yeşilbaş ördeğin yeşil başı, beyaz boyun halkası ve kestane göğsü.

### Fotoğraf kompozisyon dersi

> Kuş sağ alt üçte konumlanmış; su yüzeyi kadrajın büyük bölümünü kaplıyor.

Ana kural:

> **Alt text görseli değil, görselin o bağlamdaki işlevini tarif eder.**

---

# 1845. `/decorative-alt` — Dekoratif Görsel Kararı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## W3C notu

Görsel gerçekten yalnız dekoratifse:

> web uygulamasında genellikle `alt=""`

gibi null alternative kullanılabilir.

## Prompt

> Bu görsel adjacent text'e yeni bir bilgi eklemiyorsa dekoratif olarak değerlendir.
>
> Aynı bilgiyi screen reader'a ikinci kez okutacak tekrar alt text üretme.

---

# 1846. `/functional-alt` — İşlevsel Görsel Alt Metni

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

Bir ikon veya görsel butonsa:

> neye benzediği değil ne yaptığı önemlidir.

## Örnek

Zarf ikonu:

Zayıf:

> `envelope icon`

Daha işlevsel:

> `Send email`

## Türkçe prompt

> [İKON/GÖRSEL BUTON]'un görünüşünü değil gerçekleştirdiği eylemi alt text / accessible name olarak tarif et.

## English

> Describe the action or destination of [ICON/IMAGE BUTTON] rather than its visual appearance.

---

# 1847. `/complex-image-description` — Karmaşık Görsel Açıklaması

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Kullanım

- diagram,
- chart,
- map,
- scientific figure,
- process illustration,
- hierarchy,
- detailed infographic.

## Türkçe prompt

> [KARMAŞIK GÖRSEL] için iki katmanlı erişilebilir açıklama oluştur:
>
> 1. kısa tanım — görsel neyi gösteriyor?
> 2. uzun açıklama — izleyicinin görselden öğrenmesi gereken yapı, ilişki, değer ve sonuçlar.
>
> Uzun açıklamayı piksel piksel tarif etme.
>
> Görselin bilgi mantığını metne çevir.

## English

> Create a two-layer accessible description for [COMPLEX IMAGE]:
>
> 1. short description — what the image shows,
> 2. long description — the structure, relationships, values, and conclusions a viewer needs to understand.
>
> Do not describe the image pixel by pixel.
>
> Translate the information logic into text.

---

# 1848. `/chart-long-description` — Grafik Long Description

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe yapı

Bir chart için long description şu sırayla yazılabilir:

1. chart türü,
2. ne karşılaştırılıyor,
3. eksenler/birimler,
4. ana trend,
5. önemli zirve/düşüş,
6. istisna/outlier,
7. gerekiyorsa bütün değerlerin tablo bağlantısı.

## Prompt

> [CHART] için erişilebilir long description yaz.
>
> Önce ana sonucu ver.
>
> Sonra scale, series ve kritik değerleri açıkla.
>
> Grafikteki her grid çizgisini veya dekoratif elementi tarif etme.

## English

> Write an accessible long description for [CHART].
>
> State the primary takeaway first, then explain scale, series, important values, peaks, declines, and notable exceptions.
>
> Do not describe decorative chart elements.

---

# 1849. `/map-long-description` — Harita Long Description

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [HARİTA] için long description oluştur.
>
> Açıklama:
>
> - alan/extent,
> - tematik değişken,
> - legend mantığı,
> - en belirgin mekânsal örüntü,
> - önemli istisnalar
>
> üzerinde dursun.
>
> Her şehir veya sınır çizgisini sıralama.

## English

> Write a long description for [MAP] focusing on geographic extent, thematic variable, legend logic, primary spatial pattern, and important exceptions.
>
> Do not enumerate every place name or boundary.

---

# 1850. `/diagram-long-description` — Diyagram Long Description

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [DİYAGRAM]'ı metinle takip edilebilir yapıya dönüştür.
>
> Önce ana bileşenleri sırala.
>
> Sonra:
>
> A → B,
> B → C,
> C → D
>
> gibi gerçek bağlantı ve yönleri açıkla.
>
> Layout bilgisi anlam taşımıyorsa “sol üstte kutu var” gibi konumsal ayrıntıya boğma.

## English

> Translate [DIAGRAM] into a text-followable structure.
>
> Identify the main components first and then explain genuine directional relationships such as A → B → C.
>
> Avoid spatial descriptions like “box in the upper left” unless position itself carries meaning.

---

# 1851. `/complex-image-table` — Görselin Verisini Tabloyla Sunma

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## W3C yaklaşımıyla uyumlu

Özellikle chart için:

> long description + gerçek veri tablosu

çok güçlü bir alternatiftir.

## Türkçe

> Görselde kesin sayısal değerler varsa açıklamaya ek olarak aynı veriyi gerçek table formatında ver.
>
> Table görseldeki değerlerle bire bir eşleşsin.
>
> Görüntü modelinden tablo değerlerini yeniden tahmin etmesini isteme.

## English

> When the image contains exact numeric values, provide the same data as a real table in addition to the description.
>
> Make the table match the source data exactly.
>
> Do not ask the image model to infer the values.

---

# 1852. `/alt-and-caption-separate` — Alt Text ile Caption'ı Ayır

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Caption

Gören ve görmeyen herkes için görünür yayın metni olabilir.

## Alt text

Görselin bağlamdaki bilgi/işlev alternatifidir.

## Kural

Aynı cümleyi:

> caption + alt

olarak gereksiz iki kez okutma.

## Prompt

> [GÖRSEL] için önce caption'ın hangi bilgiyi zaten verdiğini belirle.
>
> Alt text'te yalnız caption tarafından aktarılmayan gerekli görsel bilgiyi tamamla.

---

# 1853. `/alt-no-duplicate` — Yakındaki Metni Tekrar Etme

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Görselin yanında aynı bilgi zaten gerçek metinle verilmişse alt text'i aynı paragrafın tam kopyası yapma.
>
> Gerektiğinde null alt veya yalnız eksik görsel bilgiyi kullan.

## English

> If adjacent real text already conveys the same information, do not duplicate the entire passage in alt text.
>
> Use a null alternative or only the missing visual information where appropriate.

---

# 1854. `/image-text-extract` — Görsel İçindeki Metni Erişilebilir Kıl

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## W3C

Gerekmedikçe:

> okunacak gerçek metni image içine gömmek yerine gerçek text kullanmak daha esnektir.

## Türkçe prompt

> [POSTER/GÖRSEL]'de okunması zorunlu metni ayrıca plain text olarak çıkar.
>
> Image generation sonucu oluşan metne tek güvenilir kaynak gibi davranma.
>
> Logo dışındaki uzun yazıları mümkünse tasarım aracında gerçek text layer olarak ekle.

## English

> Extract all text that must be read from [POSTER/IMAGE] into real text content.
>
> Do not rely on image-generated lettering as the only authoritative text source.
>
> Add longer copy as real text layers in a design tool where practical.

---

# 1855. `/text-in-image-lock` — Görsel İçindeki Yazı Kilidi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Görselde mutlaka bulunması gereken kısa metinleri kullanıcı tarafından verilen exact copy olarak koru.
>
> Yazım, sayı, tarih ve özel adları değiştirme.
>
> Uzun body text'i image modeline render ettirmek yerine layout placeholder olarak bırak.

## English

> Preserve short required image text exactly as supplied, including spelling, numbers, dates, and proper names.
>
> Use placeholders for long body copy rather than relying on image generation to typeset it accurately.

---

# 1856. `/color-not-only` — Bilgiyi Yalnız Renge Bağlama

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## W3C WCAG 1.4.1

## Türkçe prompt

> [GRAFİK/DİYAGRAM/HARİTA]'da kategori veya durumları yalnız renk farkıyla ayırma.
>
> Rengi şu ikincil işaretlerden biriyle destekle:
>
> - label,
> - number,
> - shape,
> - pattern,
> - line style.
>
> Legend aynı ikincil işareti de göstersin.

## English

> Do not distinguish categories or states in [CHART/DIAGRAM/MAP] by color alone.
>
> Reinforce color using labels, numbers, shapes, patterns, or line styles.
>
> Repeat the same secondary cue in the legend.

---

# 1857. `/graphic-contrast-check` — Grafik Nesne Kontrastı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## 2026 W3C teknik güncellemesi

Bilgi için gerekli adjoining graphical areas yeterince ayrışmalıdır.

## Türkçe

> Anlamı kavramak için birbirinden ayrılması gereken grafik alanların sınırlarını kontrol et.
>
> Yakın renkler kullanılıyorsa:
>
> - border,
> - whitespace,
> - pattern,
> - direct labels
>
> gibi ek ayrım kullan.
>
> Kontrast testi gerçek final renk değerleriyle ayrıca yapılmalıdır.

## English

> Check boundaries between graphical areas that must be distinguished to understand the information.
>
> When colors are close, add borders, whitespace, patterns, or direct labels.
>
> Test contrast using the actual final color values.

---

# 1858. `/grayscale-check` — Gri Ton Kontrolü

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [GÖRSEL]'in grayscale/monochrome kopyasında kritik kategorilerin hâlâ ayırt edilip edilmediğini kontrol et.
>
> Renk kalkınca anlam tamamen kayboluyorsa shape, label veya pattern ekle.

## English

> Check whether critical categories in [VISUAL] remain distinguishable in grayscale.
>
> If meaning disappears without hue, add shape, labels, or patterns.

---

# 1859. `/print-safe-visual` — Baskıda Çalışan Görsel

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [GÖRSEL]'i ekran kadar A4/A3 baskıda da okunabilir yap.
>
> Kontrol:
>
> - küçük font,
> - ince line,
> - düşük contrast,
> - çok açık tint,
> - transparent overlay.
>
> Kritik bilgi ekran parlaklığına bağımlı olmasın.

## English

> Make [VISUAL] readable in A4 or A3 print as well as on screen.
>
> Check small type, thin lines, low contrast, pale tints, and transparent overlays.
>
> Do not make critical information depend on display brightness.

---

# 1860. `/black-white-version` — Siyah-Beyaz Alternatif

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Aynı [WORKSHEET/DIAGRAM/POSTER]'ın siyah-beyaz baskı sürümünü oluştur.
>
> Renk kodlarını:
>
> pattern,
> line style,
> number,
> direct label
>
> ile değiştir.
>
> Yalnız saturation sıfırlama.

## English

> Create a true black-and-white version of [WORKSHEET/DIAGRAM/POSTER].
>
> Replace color coding with patterns, line styles, numbers, or direct labels.
>
> Do not merely desaturate the color version.

---

# 1861. `/large-print-version` — Büyük Baskı / Düşük Görme Varyantı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [MATERYAL]'in large-print sürümünü üret.
>
> İçerik aynı kalsın ancak:
>
> - daha büyük text,
> - daha geniş satır aralığı,
> - daha fazla whitespace,
> - daha az column,
> - daha güçlü contrast
>
> kullan.
>
> Sayfayı aynı ölçekte yalnız büyütme; yeniden düzenle.

## English

> Recompose [MATERIAL] as a large-print version using larger type, more line spacing, more whitespace, fewer columns, and stronger contrast.
>
> Do not simply scale up the original page.

---

# 1862. `/responsive-visual` — Responsive Görsel Düzeni

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Aynı information visual'ı:
>
> desktop,
> tablet,
> mobile
>
> için yeniden düzenle.
>
> Mobilde:
>
> - daha az eşzamanlı panel,
> - direct labels,
> - stacked sequence,
> - daha büyük dokunma/okuma alanı
>
> kullan.
>
> Geniş yatay infografiği yalnız küçültme.

## English

> Recompose the same information visual for desktop, tablet, and mobile.
>
> On mobile use fewer simultaneous panels, direct labels, stacked sequencing, and larger readable or interactive areas.
>
> Do not merely shrink a wide infographic.

---

# 1863. `/crop-safe` — Farklı Kadrajlarda Bilgi Güvenliği

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [SOSYAL GÖRSEL]'in 1:1, 4:5 ve 9:16 crop'larında kritik yüz, ürün, başlık ve logo güvenli alanda kalsın.
>
> Edge decoration crop olabilir; kritik bilgi crop olmamalı.

## English

> Keep the critical face, product, headline, and logo within safe areas across 1:1, 4:5, and 9:16 crops.
>
> Allow edge decoration to crop, but not essential information.

---

# 1864. `/zoom-readable` — Yakınlaştırıldığında Bozulmayan Açıklama

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> Karmaşık görselde küçük bilgi kümelerini ayrı logical sections halinde düzenle.
>
> Kullanıcı zoom yaptığında hangi detayın hangi başlığa ait olduğu kaybolmasın.
>
> 40 küçük callout'ı tek merkezden dağıtma.

## English

> Organize detail in a complex visual into logical sections so relationships remain clear when users zoom.
>
> Avoid radiating dozens of tiny callouts from one center point.

---

# 1865. `/accessible-image-package` — Erişilebilir Görsel Çıktı Paketi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Master format

Bir karmaşık eğitim/bilgi görseli için tek image yeterli olmayabilir.

## Türkçe

> [GÖRSEL] için aşağıdaki erişilebilir paket yapısını üret:
>
> 1. ana görsel,
> 2. kısa alt text,
> 3. gerekiyorsa long description,
> 4. veri varsa table,
> 5. siyah-beyaz/print sürümü,
> 6. yüksek okunabilirlik sürümü,
> 7. kaynak/not.
>
> Aynı bilgiyi yedi kez tekrar etmek yerine her formatın rolünü ayır.

## English

> Build an accessible output package for [VISUAL] containing:
>
> 1. primary image,
> 2. concise alt text,
> 3. long description where necessary,
> 4. data table where relevant,
> 5. black-and-white or print version,
> 6. high-legibility version,
> 7. source note.
>
> Give each representation a distinct role rather than redundantly repeating everything.

---

# 1866. `/accessibility-slop-filter` — Erişilebilir Görsel AI Slop Filtresi

Kaçınılması gerekenler:

- her görsele uzun alt text,
- decorative image'i detaylı tarif etmek,
- alt text'te renk listesi,
- “image of...” ile her cümleye başlamak,
- chart'ı yalnız renk değiştirmekle erişilebilir sanmak,
- grayscale = desaturate,
- accessibility = font büyütme,
- long description = görseldeki her pikseli anlatmak,
- gerçek data table yerine image içindeki tablo,
- alt text'i caption'ın aynısı yapmak.

---

# 1867. Yeni üst aile: `Accessible Visual Authoring`

Aile:

- `/image-purpose-audit`
- `/alt-text`
- `/complex-image-description`
- `/chart-long-description`
- `/map-long-description`
- `/diagram-long-description`
- `/color-not-only`
- `/graphic-contrast-check`
- `/grayscale-check`
- `/large-print-version`
- `/responsive-visual`
- `/accessible-image-package`

Temel formül:

> **purpose + visual information + equivalent alternative + redundant cue + adaptable format**

Ana soru:

> **Görseli göremeyen, rengi ayırt edemeyen, düşük görüşle kullanan veya küçük ekranda okuyan biri aynı kritik bilgiyi nasıl alacak?**

---

<a id="aile-032"></a>
# Sequential Art ve Educational Comics

2026’da yayımlanan eğitim araştırmalarında comics / graphic medicine yalnız “eğlenceli resimli içerik” olarak değil, **sequential visual storytelling** yaklaşımı olarak inceleniyor.

Haziran 2026’da yayımlanan mixed-method anatomy çalışmasında comic-based visual storytelling kullanan öğrenci grubunda daha yüksek öğrenme kazanımı ve daha düşük bilişsel yük raporlandı. Çalışmanın kendisi belirli bir örneklem ve bağlamla sınırlı olsa da önemli mekanizma şuydu:

> **narrative anchoring + visual sequence + verbal/visual integration**

Temmuz 2026’da yayımlanan başka bir medical-education çalışması da comic-making etkinliklerini refleksiyon, iletişim ve profesyonel kimlik çalışması açısından ele aldı.

Bu bulgulardan çıkarılması gereken şey:

> **“Her dersi çizgi romana çevir” değildir.**
>
> Sequential art özellikle:
>
> - zaman,
> - olay,
> - karar,
> - deneyim,
> - etkileşim,
> - neden–sonuç
>
> anlatıldığında yararlı olabilir.

---

# 1868. `/comic-sequence` — Temel Çizgi Roman Dizisi

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe prompt

> [OLAY/SÜREÇ]'i 4–8 panellik sequential comic olarak anlat.
>
> Her panel:
>
> - yeni bir olay/karar,
> - açık karakter eylemi,
> - bir önceki panelle continuity
>
> taşısın.
>
> Aynı olayı farklı açılardan gereksiz tekrar etme.
>
> Metin panellerin anlatamadığı bilgiyi tamamlasın.

## English

> Tell [EVENT/PROCESS] as a 4–8 panel sequential comic.
>
> Give each panel one new event or decision, clear character action, and continuity with the previous panel.
>
> Avoid repeating the same event from unnecessary angles.
>
> Use text only to add information the images do not already convey.

---

# 1869. `/educational-comic` — Öğretici Çizgi Roman

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [KAVRAM]'ı karakterlerin gerçek problem çözme süreci içinde educational comic olarak anlat.
>
> Önce learning objective belirle.
>
> Hikâye bu hedefe hizmet etsin.
>
> Ders bilgisini karakterlerin uzun konuşma balonlarına yapıştırma.
>
> Kavram mümkün olduğunca eylem, sonuç ve görsel ilişki üzerinden anlaşılsın.

## English

> Teach [CONCEPT] through an educational comic built around characters solving a real problem.
>
> Define the learning objective first.
>
> Let the narrative serve that objective.
>
> Do not paste textbook paragraphs into speech balloons.
>
> Communicate the concept through action, consequence, and visual relationships wherever possible.

---

# 1870. `/science-comic` — Bilimsel Süreç Çizgi Romanı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [BİLİMSEL SÜREÇ]'i 6 panellik comic sequence olarak göster.
>
> Bilimsel yapı ve sıralama gerçek kalmalı.
>
> Karakter/kişileştirme kullanılacaksa kavramı yanlışlaştırmamalı.
>
> Moleküllere/organellere kişilik verirken gerçek işlev ilişkisini bozma.

## English

> Show [SCIENTIFIC PROCESS] as a six-panel comic sequence while preserving scientific structure and order.
>
> If personification is used, do not let it distort the actual mechanism or functional relationships.

---

# 1871. `/history-comic` — Tarihsel Olay Çizgi Romanı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [TARİHSEL OLAY]'ı doğrulanmış olay sırasına dayalı kısa sequential narrative olarak göster.
>
> Diyalog:
>
> - doğrudan kaynak varsa kısa alıntı,
> - yoksa açıkça dramatize edilmiş/paraphrased
>
> olmalı.
>
> Tarihsel kişilere kaynağı olmayan kesin cümleler söyletme.

## English

> Present [HISTORICAL EVENT] as a short sequential narrative grounded in a verified event sequence.
>
> Use direct dialogue only when sourced; otherwise keep dialogue clearly dramatized or paraphrased.
>
> Do not attribute unsourced exact statements to historical people.

---

# 1872. `/procedure-comic` — İşlem / Beceri Çizgi Romanı

## Trend

**Trend taramasından eklendi; kısa ömürlü olabilir.**

## Türkçe

> [GÜVENLİ PROSEDÜR]'ü karakterin uyguladığı 4–8 panellik instructional comic olarak göster.
>
> Her panel bir gerçek işlem adımı olsun.
>
> El/araç/nesne konumları continuity taşısın.
>
> Güvenlik-kritik prosedürde yalnız doğrulanmış adımları kullan.

## English

> Show [SAFE PROCEDURE] as a 4–8 panel instructional comic performed by a character.
>
> Give each panel one real action step and preserve continuity of hands, tools, and objects.
>
> For safety-critical procedures, use only verified steps.

---

# 1873. `/concept-conflict-comic` — Kavramsal Çatışma Çizgi Romanı

## Eğitim

## Türkçe

> İki karakter [KONU] hakkında farklı görüş savunsun.
>
> Bir panelde gözlem/problem,
> iki panelde farklı açıklamalar,
> son panelde kanıt/test sonucu göster.
>
> Doğru cevabı baştan karakter görünüşüyle ele verme.

## English

> Let two characters propose different explanations for [TOPIC].
>
> Use one panel for observation or problem, two for competing explanations, and a final panel for evidence or test results.
>
> Do not visually signal the correct answer in advance through character styling.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1874. `/comic-case-study` — Vaka Çizgi Romanı

## Türkçe

> [VAKA]'yı başlangıç → karar → sonuç → reflection şeklinde 4–6 panellik case comic olarak göster.
>
> Bir karar noktasında öğrenciye:
>
> “Burada ne yapardın?”
>
> gibi soru alanı bırakılabilir.
>
> Sonucu ilk panellerde açık etme.

## English

> Present [CASE] as a 4–6 panel sequence:
>
> setup → decision → outcome → reflection.
>
> Optionally pause at the decision point with a learner question such as “What would you do here?”
>
> Do not reveal the outcome too early.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1875. `/graphic-medicine` — Graphic Medicine Görsel Anlatımı

## Kullanım

Sağlık deneyimi, hasta iletişimi, bakım süreci, mesleki refleksiyon.

## Türkçe

> [SAĞLIK DENEYİMİ]'ni insan deneyimini merkeze alan graphic-medicine tarzı sequential narrative olarak anlat.
>
> Tıbbi bilgi doğru, insan deneyimi nüanslı olsun.
>
> Hastayı diagnosis stereotype veya “lesson object” hâline getirme.
>
> Sağlık bilgisi veriliyorsa gerçek kaynakla doğrulanmalı.

## English

> Present [HEALTH EXPERIENCE] as a human-centered graphic-medicine sequential narrative.
>
> Keep medical information accurate and human experience nuanced.
>
> Do not reduce the patient to a diagnosis stereotype or teaching prop.
>
> Verify health information separately.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1876. `/silent-comic` — Yazısız Çizgi Roman

## Türkçe

> [OLAY]'ı yalnız panel kompozisyonu, beden dili, nesne ve mekân değişimiyle 4–8 panelde anlat.
>
> Speech bubble ve caption kullanma.
>
> Her panelde karakterin kimliği ve yönü korunmalı.

## English

> Tell [EVENT] across 4–8 panels using only composition, body language, objects, and environmental change.
>
> Use no speech balloons or captions.
>
> Preserve character identity and direction across panels.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1877. `/one-page-comic` — Tek Sayfalık Comic

## Türkçe

> [HİKÂYE]'yi tek sayfada 5–9 panellik açık reading order ile anlat.
>
> Panel boyutları ritme göre değişebilir.
>
> Okuma sırasını deneysel layout uğruna belirsizleştirme.

## English

> Tell [STORY] on one page using 5–9 panels with a clear reading order.
>
> Let panel size vary according to pacing.
>
> Do not make reading order ambiguous merely for experimental composition.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1878. `/three-panel-comic` — Üç Karelik Mikro Hikâye

## Türkçe

> [FİKİR]'i üç panelde:
>
> setup → turn → result
>
> yapısıyla anlat.
>
> Her panel yeni bilgi taşısın.
>
> Üç kareyi aynı kişinin üç pozuna dönüştürme.

## English

> Tell [IDEA] in three panels using:
>
> setup → turn → result.
>
> Make each panel add new information.
>
> Do not use three frames merely as three poses of the same person.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1879. `/comic-panel-size` — Panel Boyutu ile Ritim

## Türkçe

> Önemli olay için daha büyük panel, hızlı ara olaylar için küçük panel kullan.
>
> Panel boyutunu yalnız görsel çeşitlilik için değiştirme.
>
> Alan kullanımının zaman/önem hissini desteklemesini sağla.

## English

> Use a larger panel for an important moment and smaller panels for quicker transitional beats.
>
> Let panel size support pacing and importance rather than visual variety alone.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1880. `/comic-gutter` — Gutter / Kareler Arası Boşluk

## Kavram

Comic’te panel arası boşluk:

> izleyicinin iki kare arasında zihinsel olarak zamanı/eylemi tamamladığı alan olabilir.

## Türkçe

> Panel geçişlerinde ne kadar zaman/eylem atlandığını düşün.
>
> Çok büyük olay değişimini tek küçük gutter ile anlaşılmaz bırakma.
>
> Gerekirse ara panel ekle.

## English

> Consider how much time or action the reader must infer across each gutter.
>
> Do not hide a major event transition between two insufficiently connected panels.
>
> Add an intermediate panel where necessary.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1881. `/comic-continuity-lock` — Çizgi Roman Süreklilik Kilidi

## Türkçe

> Tüm comic boyunca:
>
> - karakter yüzü,
> - saç,
> - kıyafet,
> - boy oranı,
> - önemli prop,
> - oda/çevre,
> - ekran yönü
>
> sabit kalsın.
>
> Yalnız hikâyenin gerektirdiği değişiklikleri yap.

## English

> Preserve character face, hair, clothing, body proportions, important props, environment, and screen direction across the comic.
>
> Change only what the story requires.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1882. `/comic-eyeline` — Bakış Yönü Tutarlılığı

## Türkçe

> Karakterler konuşurken karşılıklı eyeline ilişkisini koru.
>
> Biri diğerine bakıyorsa reverse panelde bakış yönünü fiziksel olarak tutarlı üret.
>
> Karakterleri kareler arasında sağ-sol rastgele değiştirme.

## English

> Preserve eyeline relationships between speaking characters.
>
> Keep reverse views spatially coherent and avoid random left-right swapping.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1883. `/speech-balloon` — Konuşma Balonu

## Türkçe

> Speech balloon'u konuşan kişiye açık tail ile bağla.
>
> Bir balonda en fazla birkaç kısa cümle kullan.
>
> Balon:
>
> - yüzü,
> - kritik el eylemini,
> - önemli nesneyi
>
> kapatmasın.
>
> Uzun ders paragrafını balona koyma.

## English

> Connect each speech balloon clearly to the speaker.
>
> Keep dialogue concise and avoid covering faces, critical hand actions, or important objects.
>
> Do not place textbook paragraphs inside balloons.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1884. `/thought-balloon` — Düşünce / İç Ses

## Türkçe

> İç düşünce yalnız gerçekten anlatı için gerekliyse kullan.
>
> Düşünce ile yüksek sesli konuşmanın grafik dili farklı olsun.
>
> Her panelde iç ses kullanma.

## English

> Use internal thought only when narratively necessary and distinguish it visually from spoken dialogue.
>
> Avoid internal monologue in every panel.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1885. `/caption-box` — Anlatıcı / Zaman Kutusu

## Türkçe

> Caption box'u yalnız:
>
> - zaman,
> - yer,
> - kısa anlatıcı bilgisi
>
> için kullan.
>
> Görselde zaten açık olan eylemi yeniden yazma.

## English

> Use caption boxes only for time, place, or concise narrator information.
>
> Do not restate actions that are already visually obvious.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1886. `/sound-effect-type` — Ses Efekti Yazısı

## Türkçe

> Onomatopoeia'yı yalnız gerçek işitsel olaya bağla.
>
> Yazı formu:
>
> - ses şiddeti,
> - yön,
> - süre
>
> ile ilişkili olabilir.
>
> Her hareketi büyük “BAM/WHOOSH” yazısına dönüştürme.

## English

> Use onomatopoeia only for real sound events and let letter scale or direction reflect loudness, direction, or duration where appropriate.
>
> Do not turn every action into oversized “BAM” or “WHOOSH” lettering.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1887. `/comic-camera-language` — Comic İçinde Çekim Ölçeği

## Türkçe

> Comic sequence içinde:
>
> establishing → medium → close-up → detail
>
> gibi shot değişimini bilgi amacıyla kullan.
>
> Her panel aynı orta plan olmasın.
>
> Sadece “cinematic” görünmek için anlamsız açı değiştirme.

## English

> Use shot changes such as establishing, medium, close-up, and detail to serve information and pacing.
>
> Avoid making every panel the same medium shot or changing angles only for cinematic flair.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1888. `/comic-reaction-panel` — Tepki Karesi

## Türkçe

> Hikâyede karar/sonuç önemliyse kısa reaction panel kullanılabilir.
>
> Tepki:
>
> - beden,
> - yüz,
> - duraklama
>
> üzerinden gelsin.
>
> Her önemli cümleden sonra reaction close-up kullanma.

## English

> Use a brief reaction panel when a decision or consequence deserves a pause.
>
> Convey reaction through body, face, or stillness.
>
> Avoid reaction close-ups after every important line.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1889. `/comic-insert` — Nesne Ayrıntı Paneli

## Türkçe

> Hikâyede kritik nesneyi kısa insert panel ile göster:
>
> anahtar,
> belge,
> deney sonucu,
> mesaj,
> kırılmış parça
>
> gibi.
>
> Sonraki olay bu detayla ilişkili olsun.

## English

> Use a short insert panel for a critical object such as a key, document, experiment result, message, or broken component.
>
> Make the detail relevant to what follows.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1890. `/before-after-comic` — Dönüşüm Çizgi Romanı

## Türkçe

> [DÖNÜŞÜM]'ü:
>
> önce → neden/eylem → sonra
>
> şeklinde 3–5 panelde göster.
>
> Kamera veya ölçek farkıyla sonucu yapay biçimde dramatikleştirme.

## English

> Show [TRANSFORMATION] across 3–5 panels:
>
> before → cause/action → after.
>
> Do not exaggerate the outcome by changing camera or scale.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1891. `/comic-question-stop` — Öğrenci Karar Noktası

## Türkçe

> Comic'i kritik karar panelinde durdur.
>
> Sonraki sonucu göstermeden:
>
> “Sence ne olur?”
> veya
> “Hangi seçenek daha doğru?”
>
> gibi tek soru sor.
>
> Cevap ayrı panel/öğretmen katmanında verilebilir.

## English

> Pause the comic at a critical decision point before revealing the outcome.
>
> Ask one prediction or choice question.
>
> Reveal the answer in a separate panel or teacher layer.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1892. `/comic-answer-layer` — Öğretmen / Cevap Sürümü

## Türkçe

> Öğrenci comic sayfasının layout'unu değiştirme.
>
> Teacher version'da yalnız:
>
> - doğru karar,
> - kısa neden,
> - kritik kavram
>
> için annotation ekle.

## English

> Preserve the student comic layout exactly.
>
> In the teacher version add only the correct decision, concise reasoning, and critical concept annotation.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1893. `/comic-accessible-description` — Comic Long Description

Sequential art için alt text özellikle zordur.

## Türkçe

> Comic için yalnız “altı panelli çizgi roman” yazma.
>
> Long description'ı panel sırasına göre oluştur:
>
> Panel 1 — durum  
> Panel 2 — eylem  
> Panel 3 — sonuç...
>
> Diyalog önemliyse exact veya anlam eşdeğerli metin olarak ver.
>
> Görsel jest/beden dili anlam taşıyorsa onu da dahil et.

## English

> Do not describe a comic only as “a six-panel comic.”
>
> Write a long description in panel order:
>
> Panel 1 — setup  
> Panel 2 — action  
> Panel 3 — consequence...
>
> Include dialogue where meaningful and describe gestures or body language when they carry narrative information.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1894. `/comic-mobile-stack` — Mobil Comic Düzeni

## Türkçe

> Aynı comic'i mobilde tek sütun panel stack olarak yeniden düzenle.
>
> Panel içi text ve yüzler telefonda okunacak kadar büyük kalsın.
>
> Desktop sayfayı yalnız küçültme.

## English

> Recompose the same comic for mobile as a single-column panel stack.
>
> Keep text and faces readable at phone size.
>
> Do not merely shrink the desktop page.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1895. `/vertical-scroll-comic` — Dikey Scroll Comic

## Türkçe

> [HİKÂYE]'yi dikey scroll okuma için tasarla.
>
> Panel yüksekliği ve aradaki boşluk zaman/pause hissi verebilir.
>
> Her paneli 9:16 poster hâline getirme.
>
> Uzun boşlukları yalnız dramatik etki için aşırı kullanma.

## English

> Design [STORY] for vertical scrolling.
>
> Use panel height and spacing to control time and pauses.
>
> Do not turn every panel into a full 9:16 poster or overuse long empty gaps for drama.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1896. `/comic-print-page` — Baskı Comic Sayfası

## Türkçe

> Comic'i basılı sayfa için:
>
> - güvenli margin,
> - yeterli gutter,
> - okunabilir balloon text,
> - baskıya uygun line weight
>
> ile düzenle.
>
> Ekran zoom'una güvenme.

## English

> Prepare the comic page for print using safe margins, sufficient gutters, readable balloon text, and print-appropriate line weight.
>
> Do not rely on screen zoom.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1897. `/comic-style-lock` — Stil Sürekliliği

## Türkçe

> Tüm panel dizisinde:
>
> - line weight,
> - rendering,
> - color palette,
> - character proportions,
> - balloon style
>
> aynı sistemde kalsın.
>
> Her paneli farklı sanatçı çizmiş gibi üretme.

## English

> Preserve one line weight, rendering approach, color palette, character-proportion system, and balloon style throughout the sequence.
>
> Avoid making each panel look like it was drawn by a different artist.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1898. `/comic-fact-lock` — Bilgi Doğruluğu Kilidi

## Türkçe

> Eğitim comic'inde:
>
> - tarih,
> - bilimsel kavram,
> - anatomi,
> - sayı,
> - teknik süreç
>
> yalnız doğrulanmış bilgiye dayansın.
>
> Narrative akış uğruna factual relationship'i değiştirme.

## English

> In educational comics, keep dates, scientific concepts, anatomy, numbers, and technical processes grounded in verified information.
>
> Do not alter factual relationships merely to improve the story.

## Neye dikkat edilmeli?

Kareler arası süreklilik (yüz, giysi, bakış yönü) kilitlensin; balon yazıları Türkçe karakterleriyle harf harf denetlensin.

---
# 1899. `/comic-slop-filter` — Çizgi Roman AI Slop Filtresi

Kaçınılması gerekenler:

- her panel aynı poz,
- karakter yüzünün değişmesi,
- kıyafetin renk değiştirmesi,
- konuşma balonunun yanlış kişiye bağlanması,
- okunmayan balloon text,
- her panelde reaksiyon close-up,
- bütün bilgiyi diyaloga yüklemek,
- anime hız çizgilerini her sahnede kullanmak,
- panel sırasını belirsiz bırakmak,
- öğretici comic = konuşan organ maskotu sanmak.

---

# 1900. Yeni üst aile: `Sequential Visual Grammar`

Aile:

- `/comic-sequence`
- `/wordless-sequence`
- `/procedure-comic`
- `/comic-case-study`
- `/three-panel-comic`
- `/vertical-scroll-comic`
- `/shot-sequence`

Ortak formül:

> **state A + meaningful change + state B + continuity**

Ana soru:

> **Bir sonraki kare neden var?**

Eğer cevap yoksa panel gereksiz olabilir.

---

# 1901. Yeni üst aile: `Educational Narrative Visual`

Aile:

- `/educational-comic`
- `/science-comic`
- `/history-comic`
- `/concept-conflict-comic`
- `/comic-case-study`
- `/graphic-medicine`
- `/educational-story-scene`

Ortak kural:

> **hikâye öğrenme hedefinin önüne geçmez.**

---

# 1902. `/narrative-vs-diagram` — Hikâye mi Diyagram mı?

## Diagram seç

Eğer ana soru:

> Nasıl çalışıyor?
>
> Parçalar nasıl bağlı?
>
> Adımlar neler?

ise.

## Narrative seç

Eğer ana soru:

> Bir kişi bu süreçte ne yaşıyor?
>
> Karar nasıl veriliyor?
>
> Olay nasıl gelişiyor?
>
> Sonuç neye yol açıyor?

ise.

### Hibrit

Bir comic panel içinde küçük diyagram kullanılabilir.

Ama:

> comic + infographic + flowchart + poster

hepsini aynı sayfaya sıkıştırma.

---

# 1903. `/comic-vs-storyboard` — Comic mi Storyboard mu?

## Comic

Nihai okuyucu içindir.

- speech,
- pacing,
- page/scroll composition,
- narrative reading.

## Storyboard

Üretim ekibi içindir.

- camera,
- action,
- timing,
- movement,
- production planning.

### Kural

> Storyboard “bitmemiş comic” değildir.
>
> Comic de “renklendirilmiş storyboard” değildir.

---

# 1904. Bu turdaki slash-style indeks (aile-032)

| Kısayol | Aile |
|---|---|
| `/image-purpose-audit` | informative/decorative/functional/complex decision |
| `/alt-text` | concise contextual text alternative |
| `/alt-text-purpose-first` | context-driven alt text |
| `/decorative-alt` | decorative-image handling |
| `/functional-alt` | action/destination alternative |
| `/complex-image-description` | short + long text equivalent |
| `/chart-long-description` | accessible chart narrative |
| `/map-long-description` | accessible map narrative |
| `/diagram-long-description` | text-followable diagram |
| `/complex-image-table` | exact data table alternative |
| `/alt-and-caption-separate` | prevent redundant reading |
| `/alt-no-duplicate` | avoid adjacent-text duplication |
| `/image-text-extract` | make embedded text available as real text |
| `/text-in-image-lock` | preserve exact short image text |
| `/color-not-only` | redundant non-color encoding |
| `/graphic-contrast-check` | graphical boundary contrast |
| `/grayscale-check` | no-color meaning audit |
| `/print-safe-visual` | screen + print readability |
| `/black-white-version` | real monochrome redesign |
| `/large-print-version` | large-print recomposition |
| `/responsive-visual` | device-specific information layout |
| `/crop-safe` | social-format safe area |
| `/zoom-readable` | complex visual zoom structure |
| `/accessible-image-package` | image + alternatives package |
| `/comic-sequence` | sequential visual narrative |
| `/educational-comic` | learning-objective comic |
| `/science-comic` | accurate scientific sequence |
| `/history-comic` | evidence-aware history comic |
| `/procedure-comic` | action-based instructional comic |
| `/concept-conflict-comic` | competing explanations |
| `/comic-case-study` | case → decision → outcome |
| `/graphic-medicine` | health narrative comic |
| `/silent-comic` | wordless sequential narrative |
| `/one-page-comic` | page-based comic |
| `/three-panel-comic` | setup → turn → result |
| `/comic-panel-size` | pacing through panel scale |
| `/comic-gutter` | inferred time/action between panels |
| `/comic-continuity-lock` | character/environment continuity |
| `/comic-eyeline` | spatial gaze consistency |
| `/speech-balloon` | concise spoken dialogue |
| `/thought-balloon` | internal voice |
| `/caption-box` | time/place/narrator information |
| `/sound-effect-type` | meaningful onomatopoeia |
| `/comic-camera-language` | shot variation for sequence |
| `/comic-reaction-panel` | intentional narrative pause |
| `/comic-insert` | critical object detail |
| `/before-after-comic` | controlled transformation story |
| `/comic-question-stop` | learner prediction pause |
| `/comic-answer-layer` | teacher answer overlay |
| `/comic-accessible-description` | panel-order long description |
| `/comic-mobile-stack` | phone-ready comic |
| `/vertical-scroll-comic` | scroll-native sequence |
| `/comic-print-page` | print-ready comics layout |
| `/comic-style-lock` | consistent rendering system |
| `/comic-fact-lock` | verified educational content |
| `/narrative-vs-diagram` | select story vs structure |
| `/comic-vs-storyboard` | reader artifact vs production plan |

---

<a id="aile-033"></a>
# Viral Fotoğraf Annotation, “What’s in My Bag”, Masaüstü Figürin ve Arşiv Nesnesi — Eylül 2026 Ek Taraması

Eylül 2026 taramasında dört ayrı ama birbirine bağlanan görsel aile öne çıkıyor:

- fotoğraf üzerine **hand-drawn annotation / daily notes overlay**,
- klasik flat lay’den hareketli **“What’s in My Bag / Bag Catch”** anlatımına geçiş,
- kişi/pet/karakteri **masaüstü koleksiyon figürüne** dönüştüren viral master prompt,
- fotoğrafı yalnız içerik değil **fiziksel ve arşivlenmiş bir nesne** olarak sunma.

Canva’nın 2026 **Notes App Chic** eğilimi kamera rulosu, notlar klasörü ve scrapbook öğelerinin aynı görsel dilde birleşmesini özellikle öne çıkarıyor. Canva ayrıca DIY/scrapbook aramalarında kendi platformunda yıllık %90 artış bildirmiştir. Bu veri Canva platformuna aittir; küresel pazar büyüklüğü olarak yorumlanmamalıdır.

2026 sosyal medya prompt listelerinde ise fotoğrafın üzerine ince çizim, ok, kısa el yazısı ve kişisel günlük notları ekleyen format ayrı bir viral aile olarak dolaşıyor.

Bu bölümün ana ilkesi:

> **Annotation, fotoğrafı süslemek için değil; fotoğrafta zaten bulunan bir ayrıntıyı seçmek, açıklamak veya kişisel bağlam vermek için kullanılmalıdır.**

---

# 1905. `/daily-notes-overlay` — Günlük Not Annotation

## Trend

**T1/T2 — 2026 sosyal fotoğraf trendi.**

## Türkçe prompt

> Kaynak fotoğrafı ana görsel olarak tamamen koru.
>
> Fotoğrafın çevresine 4–7 kısa handwritten daily-note annotation ekle.
>
> Notlar yalnız:
>
> - fotoğrafta görülen bir nesne,
> - kıyafet ayrıntısı,
> - gerçek mekânsal detay,
> - kullanıcı tarafından verilen kısa kişisel not
>
> ile ilişkili olsun.
>
> İnce el çizgisi, kısa ok ve küçük underline kullanılabilir.
>
> Fotoğrafta olmayan olay, duygu, tarih, marka veya anı uydurma.
>
> Sayfayı doodle defterine dönüştürme.

## English

> Preserve the source photograph completely and add only 4–7 concise handwritten daily-note annotations around it.
>
> Tie every note to a visible object, outfit detail, real spatial feature, or short personal note supplied by the user.
>
> Use restrained hand-drawn lines, arrows, and underlines.
>
> Do not invent events, emotions, dates, brands, or memories absent from the source.
>
> Avoid turning the image into a doodle notebook.

---

# 1906. `/photo-sketch-overlay` — Fotoğraf + İnce Eskiz Katmanı

## Türkçe

> Kaynak [FOTOĞRAF]'ı değiştirmeden üzerinde yalnız seçilmiş 3–5 ayrıntıyı ince freehand line drawing ile takip et.
>
> Çizim:
>
> - silhouette,
> - kıyafet seam,
> - obje contour,
> - mimari çizgi
>
> gibi gerçek forma bağlı olsun.
>
> Fotoğrafın üzerine ikinci hayalî sahne çizme.

## English

> Keep [PHOTO] unchanged and trace only 3–5 selected visible details with restrained freehand linework, such as silhouette, garment seam, object contour, or architectural line.
>
> Anchor the drawing to the real form.
>
> Do not draw a second imaginary scene over the photograph.

## Neye dikkat edilmeli?

Annotation katmanı fotoğrafı kapatmasın; el yazısı bilgi kilidiyle ([§1911](#sec-1911)) her not kaynaktan doğrulansın.

---
# 1907. `/outfit-annotation-photo` — Kıyafet Annotation Fotoğrafı

## Türkçe

> [KİŞİ FOTOĞRAFI]'nı koru ve yalnız gerçek outfit parçalarını kısa annotation ile göster:
>
> jacket,
> shirt,
> trouser/skirt,
> shoe,
> accessory.
>
> Marka yalnız kullanıcı veriyorsa yazılsın.
>
> Kumaş/ürün modeli görünüşten kesin anlaşılmıyorsa tahmin etme.
>
> Moda moodboard sticker'ları ekleme.

## English

> Preserve [PERSON PHOTO] and annotate only the real visible outfit pieces such as jacket, shirt, trousers or skirt, shoes, and accessories.
>
> Mention brands only when supplied by the user.
>
> Do not infer exact fabric or product model from appearance when uncertain.
>
> Avoid unrelated fashion-moodboard stickers.

## Neye dikkat edilmeli?

Annotation katmanı fotoğrafı kapatmasın; el yazısı bilgi kilidiyle ([§1911](#sec-1911)) her not kaynaktan doğrulansın.

---
# 1908. `/design-annotation-photo` — Tasarım Kararı Annotation

## Kullanım

Mimari, ürün, mobilya, grafik tasarım eleştirisi.

## Türkçe

> Kaynak [TASARIM FOTOĞRAFI]'nda yalnız gerçekten görülebilen 4–6 tasarım kararını annotation ile işaretle:
>
> form,
> material transition,
> proportion,
> joint,
> spacing,
> hierarchy.
>
> Her not kısa ve gözleme dayalı olsun.
>
> Tasarımcının niyetini kaynak yoksa kesin bilgi gibi yazma.

## English

> Annotate only 4–6 design decisions genuinely visible in [DESIGN PHOTO], such as form, material transition, proportion, joint, spacing, or hierarchy.
>
> Keep notes concise and observational.
>
> Do not present assumed designer intent as fact without a source.

## Neye dikkat edilmeli?

Annotation katmanı fotoğrafı kapatmasın; el yazısı bilgi kilidiyle ([§1911](#sec-1911)) her not kaynaktan doğrulansın.

---
# 1909. `/photo-margin-notes` — Kenar Boşluğunda Not

## Türkçe

> Fotoğrafın kendisini temiz bırak.
>
> Annotation'ları yalnız beyaz/neutral dış margin içine yerleştir.
>
> İnce leader line gerektiğinde fotoğrafa girebilir.
>
> Bu format fotoğrafı bozmadan editorial annotation hissi versin.

## English

> Keep the photograph itself visually clean and place annotations only in a white or neutral outer margin.
>
> Let only restrained leader lines enter the image where needed.
>
> Preserve an editorial annotation feel without covering the photograph.

## Neye dikkat edilmeli?

Annotation katmanı fotoğrafı kapatmasın; el yazısı bilgi kilidiyle ([§1911](#sec-1911)) her not kaynaktan doğrulansın.

---
# 1910. `/annotation-layer-lock` — Annotation Katmanı Kilidi

## Türkçe

> Fotoğraf = immutable source layer.
>
> Annotation = ayrı overlay layer.
>
> Annotation eklerken:
>
> - yüz,
> - ürün,
> - mimari,
> - kıyafet,
> - ışık,
> - arka plan
>
> değiştirilmesin.
>
> Yalnız overlay ekle.

## English

> Treat the photograph as an immutable source layer and annotation as a separate overlay layer.
>
> Do not alter face, product, architecture, clothing, lighting, or background while adding annotations.
>
> Add only the overlay.

## Neye dikkat edilmeli?

Annotation katmanı fotoğrafı kapatmasın; el yazısı bilgi kilidiyle ([§1911](#sec-1911)) her not kaynaktan doğrulansın.

---
<a id="sec-1911"></a>
# 1911. `/handwritten-fact-lock` — El Yazısı Bilgi Kilidi

## Türkçe

> Handwritten annotation içindeki:
>
> - isim,
> - tarih,
> - fiyat,
> - marka,
> - ürün,
> - yer
>
> gibi factual bilgiler yalnız kullanıcı tarafından sağlanan veya doğrulanmış veriden gelsin.
>
> Estetik boşluğu doldurmak için “Sunday 10:45”, “Paris”, “favorite jacket” gibi sahte notlar üretme.

## English

> Use only supplied or verified information for handwritten names, dates, prices, brands, products, or places.
>
> Do not invent notes such as “Sunday 10:45,” “Paris,” or “favorite jacket” merely to fill visual space.

## Neye dikkat edilmeli?

Annotation katmanı fotoğrafı kapatmasın; el yazısı bilgi kilidiyle ([§1911](#sec-1911)) her not kaynaktan doğrulansın.

---
# 1912. `/notes-app-photo-board` — Notes App Chic Fotoğraf Panosu

## Trend

**T1 — Canva 2026 Notes App Chic.**

## Türkçe

> [3–7 FOTOĞRAF]'ı kamera rulosu + kısa not + rough crop mantığında tek kişisel board üzerinde düzenle.
>
> Kullan:
>
> - gerçek fotoğraflar,
> - 2–4 kısa not,
> - bir screenshot benzeri text block gerekiyorsa,
> - sınırlı crop/overlap.
>
> Her görsele tape, torn edge ve doodle ekleme.
>
> Board düzenli mükemmellik yerine çalışma hâlindeki düşünce hissi taşısın.

## English

> Arrange [3–7 PHOTOS] on one personal board combining camera-roll imagery, concise notes, and restrained rough cropping.
>
> Use real photographs, 2–4 short notes, an optional screenshot-like text block, and limited overlap.
>
> Do not add tape, torn edges, and doodles to every image.
>
> Let the board feel like thinking in progress rather than polished perfection.

---

# 1913. `/camera-roll-story` — Kamera Rulosundan Hikâye

## Türkçe

> [FOTOĞRAF SETİ]'nden 6–10 kare seçerek gerçek camera-roll story oluştur.
>
> Yalnız en estetik kareleri seçme.
>
> Kurucu kare, küçük ayrıntı, hareket, sıradan ara an ve kapanış karesi birlikte bulunabilir.
>
> Fotoğraf sırası gerçek olay/zaman akışını bozmasın.

## English

> Build a 6–10 image camera-roll story from [PHOTO SET].
>
> Do not select only the most polished images.
>
> Include an establishing frame, small detail, action, ordinary in-between moment, and closing image where appropriate.
>
> Preserve the real chronology or event logic.

## Neye dikkat edilmeli?

Annotation katmanı fotoğrafı kapatmasın; el yazısı bilgi kilidiyle ([§1911](#sec-1911)) her not kaynaktan doğrulansın.

---
# 1914. `/annotation-slop-filter` — Fotoğraf Annotation AI Slop Filtresi

Kaçınılması gerekenler:

- rastgele ok,
- her objeyi etiketlemek,
- fotoğrafta olmayan kişisel not,
- kaynak görseli yeniden çizmek,
- her kenara doodle,
- sticker + tape + star + heart zorunluluğu,
- okunmayan handwriting,
- annotation için gerçek fotoğrafı crop/deform etmek,
- “authentic” görünmesi için sahte tarih/konum.

---

<a id="aile-034"></a>
# “What’s in My Bag” — Nesnelerle Kimlik Anlatımı

“What’s in my bag” formatı uzun süredir var olan bir editorial/social format olsa da 2026’da iki farklı kola ayrılıyor:

### Static

> bag + contents as flat lay / object portrait.

### Motion

> nesnelerin tek tek çantaya düşmesi/yakalanması.

Mayıs 2026’da Picsart’ın yayınladığı **Bag Catch Edit** rehberi, klasik flat-lay sürümünden farklı olarak nesnelerin birer birer çantaya düştüğü 9:16 video formatını güncel trend olarak öne çıkarıyor.

Bu ailede önemli etik sınır:

> Çantadaki nesnelerden kişinin kişiliği, sağlık durumu, siyasi görüşü, gelir düzeyi veya özel yaşamı hakkında çıkarım yapılmaz.

Nesneler:

> **kullanıcının verdiği seçimlerdir.**

---

# 1915. `/whats-in-my-bag` — What’s in My Bag

## Türkçe prompt

> [ÇANTA]'yı açık veya yanında yer alan gerçek içeriğiyle birlikte temiz editorial “what’s in my bag” görseli olarak göster.
>
> Yalnız kullanıcı tarafından verilen 6–12 nesneyi kullan.
>
> Her nesne:
>
> - ayrı okunabilir,
> - gerçek ölçek ilişkisine yakın,
> - çantaya fiziksel olarak sığabilir
>
> olsun.
>
> Kişiyi tanımlamak için ilave “cool lifestyle” nesneleri uydurma.

## English

> Show [BAG] with its real supplied contents as a clean editorial “what’s in my bag” visual.
>
> Use only the 6–12 objects provided by the user.
>
> Keep every object readable, approximately scale-consistent, and physically plausible for the bag.
>
> Do not invent aspirational lifestyle objects to characterize the owner.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1916. `/bag-flatlay` — Çanta + İçindekiler Flat Lay

## Türkçe

> [ÇANTA] ve [NESNELER]'i tam top-down flat lay olarak göster.
>
> Çanta ana anchor olsun.
>
> İçerik çevresinde yeterli whitespace bırak.
>
> Nesneleri sırf kompozisyon için tekrar etme veya küçültme.

## English

> Show [BAG] and [OBJECTS] in a true top-down flat lay.
>
> Keep the bag as the primary anchor with enough whitespace around individual items.
>
> Do not duplicate or shrink objects merely to improve composition.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1917. `/bag-inventory` — Çanta Envanteri

## Türkçe

> [ÇANTA]'daki nesneleri numaralı inventory sheet olarak göster.
>
> Çanta + 1–N items.
>
> Sağ/alt bölümde yalnız kısa gerçek item adları olsun.
>
> Bu format identity moodboard değil, envanter mantığında çalışsın.

## English

> Show the contents of [BAG] as a numbered inventory sheet with the bag plus items 1–N.
>
> Use concise real item names in a side or bottom list.
>
> Treat it as inventory rather than an identity moodboard.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1918. `/bag-exploded-layout` — Çantadan Dışarı Açılan İçerik

## Türkçe

> [ÇANTA]'yı merkezde tut ve içindeki nesneleri çantadan dışarı mantıksal/yerleşimsel olarak yayılan exploded layout şeklinde göster.
>
> Bu mekanik exploded view değildir; nesneler çantanın parçaları değil içeriğidir.
>
> Her nesneye kısa leader line gerekmez.

## English

> Keep [BAG] central and arrange its contents outward in an exploded-layout presentation.
>
> This is not a mechanical exploded view; the objects are contents rather than bag components.
>
> Leader lines are optional and should remain restrained.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1919. `/bag-pocket-map` — Hangi Nesne Hangi Bölmede?

## Türkçe

> [ÇANTA]'nın açık cutaway/section görünümünde kullanıcı tarafından verilen nesnelerin hangi cep/bölmeye yerleştirildiğini göster.
>
> Nesne boyutları çantanın gerçek hacmiyle mantıklı olsun.
>
> Çantada gerçekte olmayan cep/bölme icat etme.

## English

> Show [BAG] in an open cutaway or sectional view with supplied objects placed into their actual pockets or compartments.
>
> Keep object sizes physically plausible.
>
> Do not invent pockets or compartments absent from the source bag.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1920. `/bag-catch-storyboard` — Bag Catch Edit Storyboard

## Trend

**T1/T2 — 2026 vertical social video format.**

## Türkçe

> 9:16 “bag catch” video için 8 karelik storyboard oluştur.
>
> Kare 1:
> kişi/çanta başlangıç pozisyonu.
>
> Kare 2–7:
> her karede yalnız bir nesne yukarıdan düşer ve çanta tarafından yakalanır.
>
> Kare 8:
> final bag + kısa ending pose.
>
> Her nesnenin:
>
> - boyutu,
> - düşüş yönü,
> - çantaya giriş noktası
>
> tutarlı olsun.
>
> Bir karede birden çok nesne yağdırma.

## English

> Create an eight-frame storyboard for a 9:16 “bag catch” edit.
>
> Frame 1 establishes the person or bag.
>
> Frames 2–7 introduce only one falling item per frame, caught by the bag.
>
> Frame 8 resolves with the final bag and a concise ending pose.
>
> Keep object size, fall direction, and entry point coherent.
>
> Do not rain multiple objects into the frame at once.

---

# 1921. `/bag-catch-item-stickers` — Bag Catch Nesne Sticker Seti

## Türkçe

> Kullanıcının verdiği [NESNELER]'in her birini aynı viewpoint/scale logic içinde ayrı clean-cut sticker asset olarak hazırla.
>
> Nesne kimliği korunmalı.
>
> Ek “aesthetic essentials” uydurma.

## English

> Prepare each supplied [OBJECT] as a separate clean-cut sticker asset using one consistent viewpoint and scale logic.
>
> Preserve object identity.
>
> Do not invent extra aesthetic essentials.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1922. `/bag-story-card` — Çantanın Nesnelerle Hikâyesi

## Türkçe

> [ÇANTA + NESNELER]'i tek editorial card üzerinde göster.
>
> Kullanıcı tarafından verilen yalnız 2–3 nesnenin neden önemli olduğunu kısa gerçek notlarla belirt.
>
> Nesnelerden kişilik analizi veya sosyal statü çıkarma.

## English

> Present [BAG + OBJECTS] on one editorial card and explain only 2–3 user-supplied reasons why selected objects matter.
>
> Do not infer personality or social status from the objects.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1923. `/bag-slop-filter` — What’s in My Bag AI Slop Filtresi

Kaçınılması gerekenler:

- herkese AirPods/parfüm/kamera eklemek,
- nesneleri çantaya fiziksel olarak sığmayacak boyutta yapmak,
- kişilik analizi uydurmak,
- bütün nesneleri pastel sticker'a çevirmek,
- aynı nesneyi iki kez üretmek,
- marka/logoyu değiştirmek,
- çanta bölmelerini icat etmek,
- flat lay ile inventory'yi karıştırmak.

---

<a id="aile-035"></a>
# Masaüstü Figürin + Paket + 3B Modelleme Ekranı — Viral Master Prompt

Google’ın kendi 2025 Nano Banana trend özetinde “figurines” ayrı bir popüler kullanım olarak yer aldı. 2026’da bu format hâlâ güçlü biçimde dolaşıyor ve temelde şu sahne tekrar ediyor:

> kişi/pet/karakter → küçük ticari figür → şeffaf akrilik base → masaüstü → yanında oyuncak kutusu → arkada 3B modelleme ekranı.

Temmuz–Ağustos 2026 tarihli prompt rehberleri bu yapıyı hâlâ “viral figurine trend” olarak yayınlıyor.

Bu formatı rehberde yalnız kopyalanan master prompt olarak değil, **hangi ayrıntı ne işe yarıyor?** mantığıyla arşivlemek daha yararlıdır.

---

# 1924. `/desk-figurine` — Masaüstü Koleksiyon Figürü

## Türkçe prompt

> Kaynak [KİŞİ/PET/KARAKTER]'i yaklaşık 1:7 ölçek hissi veren fiziksel koleksiyon figürüne dönüştür.
>
> Figür gerçek masa üzerinde dursun.
>
> Kullan:
>
> - fiziksel PVC/resin benzeri materyal,
> - küçük şeffaf dairesel akrilik base,
> - gerçek ölçek hissi,
> - masaüstü ürün fotoğrafçılığı.
>
> Kaynak yüz/işaret/kıyafet ayrıntılarını koru.
>
> Figürü bobblehead veya chibi yapma, aksi özellikle istenmedikçe.

## English

> Transform the source [PERSON/PET/CHARACTER] into a physical collectible figurine with an approximately 1:7 scale impression, placed on a real desk.
>
> Use believable PVC or resin material, a small transparent circular acrylic base, convincing physical scale, and desk-based product photography.
>
> Preserve key facial, marking, and outfit details from the source.
>
> Avoid bobblehead or chibi proportions unless explicitly requested.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1925. `/figurine-box` — Figürin Paket Kutusu

## Türkçe

> Figürün yanında aynı karaktere ait kurmaca, markasız collectible packaging box göster.
>
> Kutuda:
>
> - tek kısa isim,
> - karakter artwork/portrait,
> - basit ürün serisi işareti
>
> yeterli olsun.
>
> Gerçek oyuncak markası logosu kullanma.
>
> Kutudaki yüz ve kıyafet figürle aynı kimliği taşısın.

## English

> Place a fictional non-branded collectible package beside the figurine.
>
> Use only one short name, character artwork or portrait, and a restrained series marker.
>
> Avoid real toy-brand logos.
>
> Keep the face and wardrobe on the package consistent with the figurine.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1926. `/figurine-monitor` — Modelleme Süreci Ekranı

## Viral formatın ayırt edici unsuru

## Türkçe

> Figürün arkasındaki monitörde aynı figürün sade 3B sculpt/modeling viewport'unu göster.
>
> Ekrandaki model:
>
> - aynı pose,
> - aynı karakter,
> - henüz material/render uygulanmamış sculpt
>
> hissi taşısın.
>
> Okunabilir gerçek yazılım UI veya kod üretmek zorunda değil.
>
> Monitor içeriği ayrı karaktere dönüşmesin.

## English

> Show a restrained 3D sculpting or modeling viewport of the same figurine on the monitor behind it.
>
> Preserve the same character and pose while giving the model an unfinished sculpt appearance before final materials.
>
> Accurate readable software UI or code is not necessary.
>
> Do not let the monitor display drift into a different character.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1927. `/figurine-source-lock` — Figürin Kimlik Kilidi

## Türkçe

> Figürin dönüşümünde yalnız materyal ve fiziksel ölçek değişsin.
>
> Korunacak:
>
> - yüz/surat yapısı,
> - saç/tüy,
> - kıyafet,
> - ana renkler,
> - ayırt edici aksesuar.
>
> “Daha oyuncak gibi” görünmesi için kimliği yeniden tasarlama.

## English

> Change only material treatment and physical scale during the figurine transformation.
>
> Preserve facial structure, hair or fur, wardrobe, primary colors, and distinctive accessories.
>
> Do not redesign identity merely to make the subject look more toy-like.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1928. `/figurine-scale-proof` — Ölçeği Kanıtlayan Çevre

## Türkçe

> Figürin küçük görünmekle kalmasın; ölçeği gerçek çevre nesneleriyle kanıtla.
>
> Yalnız 2–3 gerçek cue kullan:
>
> - keyboard key,
> - monitor base,
> - pencil,
> - notebook edge.
>
> Dev kahve kupası gibi komik zorunlu scale cue ekleme.

## English

> Prove the figurine’s small physical scale through only 2–3 real environmental cues such as keyboard keys, monitor base, pencil, or notebook edge.
>
> Avoid exaggerated oversized props used solely for comedic scale.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1929. `/figurine-production-board` — Figürin Üretim Panosu

## Türkçe

> Aynı figürü dört matched aşamada göster:
>
> 1. source/reference,
> 2. gray sculpt,
> 3. painted prototype,
> 4. packaged final figure.
>
> Kimlik ve pose tüm aşamalarda sabit kalsın.
>
> Bu süreç gerçek fabrika üretimi iddiası değil, concept visualization olarak sunulsun.

## English

> Show the same figurine across four matched stages:
>
> 1. source or reference,
> 2. gray sculpt,
> 3. painted prototype,
> 4. packaged final figure.
>
> Preserve identity and pose.
>
> Present the sequence as concept visualization rather than evidence of an actual manufacturing process.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1930. `/figurine-pet-desk` — Evcil Hayvan Masaüstü Figürü

## Türkçe

> Kaynak [EVCİL HAYVAN]'ın tüy deseni, kulak şekli, göz rengi ve beden oranını koruyarak küçük collectible figure oluştur.
>
> Aynı hayvanı generic cute pet'e dönüştürme.
>
> Yanında kurmaca paket ve küçük scale cue kullanılabilir.

## English

> Create a small collectible figure of the source [PET] while preserving fur pattern, ear shape, eye color, and body proportions.
>
> Do not turn the animal into a generic cute pet.
>
> A fictional package and small scale cue may be included.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1931. `/figurine-couple-desk` — İki Kişilik Figür Seti

## Türkçe

> Reference A ve B'deki iki kişiyi aynı ölçek ve base system içinde iki ayrı figür olarak göster.
>
> Her kişinin yüz kimliği kendi referansında kalsın.
>
> Yüzleri birbirine karıştırma.
>
> Paket tek çift seti veya iki ayrı kutu olabilir.

## English

> Show the two people from references A and B as separate figurines within one matched scale and base system.
>
> Preserve each person’s own identity.
>
> Do not blend faces.
>
> Use either one duo package or two matched boxes.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1932. `/figurine-no-brand` — Marka Kopyalamadan Koleksiyon Figürü

## Türkçe

> Gerçek oyuncak markasının:
>
> - logosunu,
> - kutu gridini,
> - ayırt edici trade dress'ini
>
> bire bir kopyalama.
>
> “commercial collectible packaging” gibi genel fiziksel dili kullan ve özgün kurmaca marka sistemi oluştur.

## English

> Do not reproduce a real toy brand’s logo, packaging grid, or distinctive trade dress.
>
> Use the general physical language of commercial collectible packaging and create an original fictional system.

## Neye dikkat edilmeli?

Nesneler öznenin gerçek eşyalarıyla sınırlı kalsın; model “ilgili görünsün” diye ait olmayan marka ve nesne ekler.

---
# 1933. `/figurine-slop-filter` — Figürin AI Slop Filtresi

Kaçınılması gerekenler:

- mum/plastik erimiş yüz,
- bobblehead zorunluluğu,
- dev kafa,
- packaging üzerinde farklı kişi,
- monitörde farklı karakter,
- base üzerinde anlamsız yazı,
- rastgele gerçek marka logosu,
- pakette okunmaz paragraf,
- ölçek kanıtı olmayan “minyatür” render,
- source identity'yi stil uğruna kaybetmek.

---

<a id="aile-036"></a>
# Fotoğrafı “Dosya” Değil Fiziksel ve Arşivsel Nesne Olarak Görmek

Generative AI çağında fotoğrafın yalnız görsel içeriği değil, **fiziksel taşıyıcısı, arkasındaki yazı, mount'u, katalog numarası, hasarı ve provenance bilgisi** giderek daha önemli.

2026’da yayımlanan *ArchiveGPT* çalışması, arkeoloji ve mimari fotoğraflarının karton mount üzerine yapıştırıldığı, el veya daktilo ile bilgi eklendiği tarihsel arşiv kartları üzerinde vision-language model değerlendirmesi yaptı. Çalışma, fotoğraf içeriği ile insan tarafından oluşturulan açıklama/katalog bilgisinin birlikte ele alınmasının önemini gösteriyor.

Ağustos 2026’da yayımlanan *Curatorial data formation in exhibition practice* çalışması da sergi sırasında hangi kayıtların üretildiği ve seçildiğinin gelecekteki arşivin kendisini şekillendirdiğine dikkat çekiyor.

Bu ailede ana kural:

> **AI, arşiv nesnesinin görünüşünü simüle edebilir; provenance ve katalog bilgisini icat edemez.**

---

# 1934. `/archive-photo-mount` — Arşiv Fotoğraf Kartı

## Türkçe prompt

> Kaynak [FOTOĞRAF]'ı fiziksel archival photo mount üzerine monte edilmiş belge olarak göster.
>
> Mount üzerinde yalnız kullanıcı tarafından sağlanan:
>
> - kısa başlık,
> - tarih,
> - yer,
> - katalog numarası,
> - kaynak
>
> alanları bulunsun.
>
> Fotoğrafın fiziksel kenarı ile mount ayrı malzeme olarak okunabilsin.
>
> Sahte kurum damgası veya katalog numarası uydurma.

## English

> Present the source [PHOTO] as a physical photograph mounted on an archival card.
>
> Include only supplied title, date, place, catalog number, and source fields.
>
> Keep the photographic print and card mount materially distinct.
>
> Do not invent institutional stamps or catalog numbers.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1935. `/archive-photo-verso` — Fotoğrafın Arka Yüzü

## Türkçe

> [FOTOĞRAF]'ın recto ve verso görünümünü iki matched panelde göster.
>
> Ön yüzde fotoğraf.
>
> Arka yüzde yalnız kaynakta gerçekten bulunan veya kullanıcı tarafından verilen:
>
> - yazı,
> - stamp,
> - catalog note,
> - photographer mark.
>
> Eski görünmesi için sahte kurşun kalem notu uydurma.

## English

> Show matched recto and verso views of [PHOTO].
>
> Keep the front as the photograph and place only real or supplied writing, stamps, catalog notes, or photographer marks on the back.
>
> Do not invent pencil notes merely to make the object appear old.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1936. `/archive-sleeve` — Arşiv Koruma Kılıfı

## Koruma notu

National Archives fotoğraf saklama rehberi; uygun durumlarda inert polyester, polypropylene veya polyethylene sleeve ve uygun archival paper enclosure kullanımından bahseder. PVC ve sıradan ofis malzemeleri arşiv saklama standardı olarak kullanılmamalıdır.

## Türkçe prompt

> [FOTOĞRAF]'ı şeffaf archival sleeve içinde belge fotoğrafı olarak göster.
>
> Kılıf:
>
> - fotoğrafı koruyan,
> - görüntüyü çıkarmadan görmeye izin veren,
> - sade ve etiketsiz
>
> fiziksel enclosure gibi olsun.
>
> Kılıfı parlak retail plastic packaging'e dönüştürme.

## English

> Show [PHOTO] documented inside a clear archival sleeve that protects the object while allowing viewing without removal.
>
> Keep the enclosure visually restrained and archival rather than glossy retail packaging.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1937. `/archive-paper-envelope` — Kâğıt Arşiv Zarfı

## Türkçe

> [FOTOĞRAF/BELGE]'yi archival paper enclosure ile birlikte göster.
>
> Zarf üzerinde yalnız küçük catalog ID/collection information alanı olsun.
>
> Kraft craft-envelope estetiği üretme.
>
> Gerçek koruma malzemesi gerekiyorsa ilgili archival standard ayrıca doğrulanmalıdır.

## English

> Show [PHOTO/DOCUMENT] with a restrained archival paper enclosure using only a small catalog or collection information area.
>
> Avoid a decorative kraft-craft envelope aesthetic.
>
> Verify actual preservation materials separately when real conservation use is intended.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1938. `/archive-contact-sheet` — Arşiv Contact Sheet

## Türkçe

> Aynı çekim serisine ait 12–36 kareyi archival contact/proof sheet olarak göster.
>
> Frame sequence korunsun.
>
> Yalnız seçilmiş 1–3 kare grease pencil/circle ile işaretlenebilir.
>
> Fotoğrafları farklı dönem/çekimlerden rastgele karıştırma.

## English

> Show 12–36 frames from one real photographic sequence as an archival contact or proof sheet.
>
> Preserve frame order.
>
> Mark only 1–3 selected frames with restrained grease-pencil circles.
>
> Do not mix unrelated periods or shoots.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1939. `/archive-negative-sleeve` — Negatif Şerit Arşivi

## Türkçe

> [35MM/120] film şeritlerini numbered archival negative sleeve içinde göster.
>
> Frame numarası ve gerçek negatif yoğunluk farkları görülebilsin.
>
> Pozitif fotoğrafı sadece renk ters çevirerek “negative archive” yapma.

## English

> Show [35MM/120] film strips inside a numbered archival negative sleeve, preserving frame numbering and believable negative-density variation.
>
> Do not simulate a negative archive by simply inverting a positive image.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1940. `/archive-box` — Arşiv Kutusu / Dosya Sistemi

## Türkçe

> [KOLEKSİYON]'u fiziksel archive box içinde klasörlere ayrılmış olarak göster.
>
> Folder tab'larında kısa gerçek:
>
> tarih,
> seri,
> konu,
> ID
>
> bilgisi bulunabilir.
>
> İçerik düzeni araştırılabilir/findable olsun.
>
> Kutuyu nostalgia prop'a dönüştürme.

## English

> Show [COLLECTION] organized in folders within a physical archive box.
>
> Use concise real date, series, subject, or ID information on folder tabs.
>
> Make the system findable and research-oriented rather than nostalgic decoration.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1941. `/archive-index-card` — Arşiv İndeks Kartı

## Türkçe

> [ARŞİV ÖĞESİ] için küçük catalog/index card tasarla.
>
> Yalnız gerçek metadata:
>
> identifier,
> title,
> date,
> creator/source,
> format,
> location.
>
> Estetik uğruna sahte typed metadata ekleme.

## English

> Design a small catalog or index card for [ARCHIVAL ITEM] using only real metadata such as identifier, title, date, creator or source, format, and location.
>
> Do not add fictional typed metadata for aesthetics.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1942. `/archive-condition-record` — Kondisyon Belgeleme

## Türkçe

> [FOTOĞRAF/BELGE/NESNE]'yi conservation condition record olarak göster.
>
> Gerçek gözleme dayalı:
>
> - tear,
> - crease,
> - stain,
> - fading,
> - loss,
> - previous repair
>
> bölgeleri numaralı küçük annotation ile gösterilebilir.
>
> Hasar uydurma.
>
> “Vintage” görünmesi için eseri daha fazla yıpratma.

## English

> Document [PHOTO/DOCUMENT/OBJECT] as a conservation condition record using numbered annotations only for genuinely observed tears, creases, stains, fading, losses, or earlier repairs.
>
> Do not invent damage or distress the object aesthetically.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1943. `/archive-before-after` — Koruma Öncesi / Sonrası

## Türkçe

> Aynı [ARŞİV NESNESİ]'ni matched before/after conservation documentation olarak göster.
>
> Kamera, crop, scale ve lighting eşleşsin.
>
> Sonraki görüntüyü daha dramatik/temiz göstermek için ışığı değiştirme.
>
> Yapılmayan müdahaleyi varmış gibi gösterme.

## English

> Show matched before-and-after conservation documentation of the same [ARCHIVAL OBJECT].
>
> Keep camera, crop, scale, and lighting consistent.
>
> Do not change lighting to exaggerate improvement or depict conservation work that did not occur.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1944. `/provenance-chain` — Kaynak / Sahiplik / Aktarım Zinciri

## Türkçe

> [NESNE/BELGE]'nin doğrulanmış provenance chain'ini timeline olarak göster.
>
> Her node:
>
> - tarih,
> - kişi/kurum,
> - olay/transfer,
> - kaynak
>
> taşısın.
>
> Zincirde boşluk varsa “unknown / undocumented” olarak bırak.
>
> Hikâyeyi tamamlamak için ara sahip uydurma.

## English

> Show the verified provenance chain of [OBJECT/DOCUMENT] as a timeline with date, person or institution, transfer or event, and source at each node.
>
> Mark gaps as unknown or undocumented.
>
> Do not invent intermediary owners to complete the story.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1945. `/archive-evidence-layer` — Arşiv Kanıt Katmanı

## Türkçe

> [ARŞİV SUNUMU]'nda bilgiyi dört seviyede ayır:
>
> 1. physical evidence,
> 2. written archival record,
> 3. expert inference,
> 4. reconstruction/speculation.
>
> Bu seviyeleri görsel olarak karıştırma.
>
> AI-generated reconstruction'ı archival photograph gibi sunma.

## English

> Separate information in [ARCHIVAL PRESENTATION] into:
>
> 1. physical evidence,
> 2. written archival record,
> 3. expert inference,
> 4. reconstruction or speculation.
>
> Do not visually collapse these evidence levels.
>
> Never present an AI-generated reconstruction as an archival photograph.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1946. `/source-vs-reconstruction` — Kaynak Görsel / Rekonstrüksiyon Ayrımı

## Türkçe

> Sayfayı iki matched alana ayır:
>
> A — original source/document.
> B — reconstruction/interpretation.
>
> B alanında açık “reconstruction / interpretation” etiketi kullan.
>
> Kaynak ile üretilmiş görsel arasındaki sınırı bulanıklaştırma.

## English

> Divide the page into matched areas:
>
> A — original source or document,
> B — reconstruction or interpretation.
>
> Label B explicitly as reconstruction or interpretation.
>
> Do not blur the boundary between source material and generated imagery.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1947. `/museum-object-record` — Müze Nesnesi Kayıt Kartı

## Türkçe

> [ESER/NESNE]'yi catalog record olarak göster:
>
> object image,
> accession/catalog ID,
> title/object name,
> date/period,
> material,
> dimensions,
> source/provenance.
>
> Yalnız gerçek metadata kullan.
>
> Exhibition marketing copy ekleme.

## English

> Present [ARTIFACT/OBJECT] as a catalog record containing object image, accession or catalog ID, title or object name, date or period, material, dimensions, and source or provenance.
>
> Use only real metadata.
>
> Avoid exhibition-marketing language.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1948. `/archive-display-wall` — Arşiv Sergi Duvarı

## Türkçe

> [ARŞİV SETİ]'ni sergi duvarında:
>
> - original photographs/documents,
> - küçük labels,
> - 1–2 contextual panels
>
> ile göster.
>
> Arşiv materyalini aynı boyutta poster serisine dönüştürme.
>
> Farklı fiziksel format ve yaşlanma özelliklerini koru.

## English

> Display [ARCHIVAL SET] on an exhibition wall using original photographs or documents, concise labels, and only 1–2 contextual panels.
>
> Do not redesign all archival items into same-size posters.
>
> Preserve differences in physical format and age.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1949. `/archive-selection-board` — Küratoryal Seçim Panosu

## 2026 araştırma bağlantısı

Sergide hangi kayıtların seçildiği gelecekteki kültürel kaydı da etkileyebilir.

## Türkçe

> [ARŞİV]'den sergi seçimini review board üzerinde göster.
>
> Her öğe:
>
> selected,
> reserve,
> excluded,
> needs verification
>
> gibi açık status taşıyabilir.
>
> Seçim kriterlerini kısa notla belirt.
>
> “Güzel fotoğraf”ı tek kriter yapma.

## English

> Show exhibition selection from [ARCHIVE] on a review board using explicit statuses such as selected, reserve, excluded, or needs verification.
>
> State concise selection criteria.
>
> Do not make visual attractiveness the only criterion.

## Neye dikkat edilmeli?

Kaynakla rekonstrüksiyon ayrı katmanda dursun; kondisyon ve sahiplik zinciri belgelenmeden vitrin anlatısı kurulmasın.

---
# 1950. `/archive-authenticity-slop-filter` — Arşiv AI Slop Filtresi

Kaçınılması gerekenler:

- sahte katalog numarası,
- sahte kurum damgası,
- uydurma el yazısı,
- bilinmeyen tarihi doldurmak,
- bütün fotoğraflara sepia,
- archive = dusty cardboard,
- gerçek hasarı “restore” ederek silmek,
- AI reconstruction'ı source image gibi sunmak,
- provenance boşluğunu hikâyeyle doldurmak,
- arşiv materyalini vintage moodboard'a indirgemek.

---

# 1951. Yeni üst aile: `Annotated Reality`

Aile:

- `/daily-notes-overlay`
- `/photo-sketch-overlay`
- `/outfit-annotation-photo`
- `/design-annotation-photo`
- `/photo-margin-notes`
- `/annotated-photo`
- `/look-closer-label`

Ortak kural:

> **source image remains evidence; annotation remains interpretation.**

---

# 1952. Yeni üst aile: `Object Identity Through Contents`

Aile:

- `/whats-in-my-bag`
- `/bag-inventory`
- `/bag-pocket-map`
- `/what-on-my-desk`
- `/identity-flatlay`
- `/toolkit-flatlay`

Ortak sınır:

> Nesne seçimi kullanıcıdan gelir.
>
> Model bu nesnelerden hassas veya kişisel özellik çıkarmaz.

---

# 1953. Yeni üst aile: `Viral Master Prompt Anatomy`

Bir internet master prompt'unu rehbere eklerken yalnız metni saklamak yerine şu bileşenlere ayır:

1. **source** — hangi referans?
2. **identity lock** — ne korunuyor?
3. **transformation** — neye dönüşüyor?
4. **physical proof** — dönüşümü ne inandırıcı kılıyor?
5. **scene** — nerede?
6. **supporting object** — kutu, ekran, base vb.
7. **camera** — nasıl çekiliyor?
8. **text risk** — hangi metin kısa tutulmalı?
9. **brand/copyright risk** — ne genelleştirilmeli?
10. **failure modes** — yüz, el, scale, text, material.

Örneğin viral figürin promptunun özü:

> **reference identity + 1:7 collectible + acrylic base + desk scale cue + fictional package + sculpt monitor + product photo**

Bu yapı, kopyalanan tek uzun prompttan daha yeniden kullanılabilirdir.

---

# 1954. Yeni üst aile: `Archive-aware Visual`

Aile:

- `/archive-photo-mount`
- `/archive-photo-verso`
- `/archive-sleeve`
- `/archive-contact-sheet`
- `/archive-negative-sleeve`
- `/archive-index-card`
- `/archive-condition-record`
- `/provenance-chain`
- `/archive-evidence-layer`
- `/source-vs-reconstruction`

Ana kural:

> **belge görünümü üretmek kolaydır; belge niteliği ve provenance üretilemez.**

---

# 1955. `/physical-photo-object` — Fotoğrafı Fiziksel Nesne Olarak Göster

## Türkçe

> [FOTOĞRAF]'ı ekrandaki pixels olarak değil gerçek fiziksel fotoğraf nesnesi olarak göster.
>
> Formatı açıkça seç:
>
> - loose print,
> - mounted print,
> - contact print,
> - Polaroid-like instant print,
> - cabinet card,
> - album page,
> - archive sleeve.
>
> Kâğıt kalınlığı, kenar ve yüzey davranışı bu fiziksel formata uygun olsun.

## English

> Present [PHOTO] as a real physical photographic object rather than pixels on a screen.
>
> Choose one explicit format such as loose print, mounted print, contact print, instant print, cabinet card, album page, or archival sleeve.
>
> Make paper thickness, edges, and surface behavior consistent with that physical format.

## Neye dikkat edilmeli?

Nesnenin fiziksel kondisyonu (kıvrım, solma, zarf) gizlenmesin; orijinal-restore ayrımı aynı karede etiketlensin.

---
# 1956. `/cabinet-card` — Tarihsel Cabinet Card Görsel Dili

## Evergreen / tarihsel format

Cabinet card, 19. yüzyıl sonlarında yaygınlaşan fotoğrafın karton mount üzerine takıldığı belirli tarihsel formattır.

## Türkçe

> [PORTRE]'yi tarihsel cabinet-card formatından esinlenen mounted photograph olarak göster.
>
> Fotoğraf kalın kart üzerinde fiziksel olarak monte edilmiş olsun.
>
> Studio name/location gibi bilgi yalnız kullanıcı tarafından verilirse kullan.
>
> Döneme uymayan modern sans-serif, QR veya dijital efekt ekleme.
>
> Gerçek tarihsel belge olduğunu iddia etme.

## English

> Present [PORTRAIT] as a mounted photograph inspired by the historical cabinet-card format.
>
> Mount the print physically on heavier card.
>
> Include studio name or location only when supplied.
>
> Avoid anachronistic QR codes, modern interface elements, or unsupported historical claims.

## Neye dikkat edilmeli?

Nesnenin fiziksel kondisyonu (kıvrım, solma, zarf) gizlenmesin; orijinal-restore ayrımı aynı karede etiketlensin.

---
# 1957. `/album-page-photo` — Fotoğraf Albümü Sayfası

## Türkçe

> [FOTOĞRAFLAR]'ı gerçek fiziksel album page üzerinde düzenle.
>
> Aynı aile/olay sayfasında:
>
> - 2–5 fotoğraf,
> - kısa tarih/isim notu,
> - yeterli boşluk
>
> kullan.
>
> Her sayfaya sticker, çiçek, tape ve scrapbook süsü eklemek zorunda değilsin.

## English

> Arrange [PHOTOS] on a real physical album page using 2–5 photographs, concise date or name notes, and sufficient spacing.
>
> Avoid forcing stickers, flowers, tape, and scrapbook decoration onto every page.

## Neye dikkat edilmeli?

Nesnenin fiziksel kondisyonu (kıvrım, solma, zarf) gizlenmesin; orijinal-restore ayrımı aynı karede etiketlensin.

---
# 1958. `/photo-ephemera-page` — Fotoğraf + Gerçek Ephemera

## Türkçe

> [FOTOĞRAF]'ı aynı olaya gerçekten ait olduğu kullanıcı tarafından sağlanan 1–3 ephemera ile birlikte göster:
>
> ticket,
> receipt,
> invitation,
> map fragment,
> note.
>
> Sahte hatıra belgesi uydurma.
>
> Fiziksel format farklılıkları korunsun.

## English

> Present [PHOTO] with 1–3 genuinely related user-supplied pieces of ephemera such as a ticket, receipt, invitation, map fragment, or note.
>
> Do not invent fake memorabilia.
>
> Preserve differences in physical format.

## Neye dikkat edilmeli?

Nesnenin fiziksel kondisyonu (kıvrım, solma, zarf) gizlenmesin; orijinal-restore ayrımı aynı karede etiketlensin.

---
# 1959. `/photo-object-condition` — Fotoğrafın Fiziksel Kondisyonu

## Türkçe

> Kaynak fiziksel fotoğrafta gerçekten görülen:
>
> corner bend,
> silvering,
> tear,
> surface scratch,
> fading
>
> gibi condition özelliklerini belgeleyici biçimde koru.
>
> Görseli estetik olarak “temizlerken” orijinal condition bilgisini kaybetme.
>
> Restoration gerekiyorsa ayrı sürüm oluştur.

## English

> Preserve genuinely visible physical condition features of the source photograph, such as corner bends, silvering, tears, surface scratches, or fading, when documenting the object.
>
> Do not erase condition evidence merely to make the image cleaner.
>
> Create restoration as a separate version when needed.

## Neye dikkat edilmeli?

Nesnenin fiziksel kondisyonu (kıvrım, solma, zarf) gizlenmesin; orijinal-restore ayrımı aynı karede etiketlensin.

---
# 1960. `/archive-original-vs-restored` — Orijinal / Restore Edilmiş Ayrımı

## Türkçe

> İki matched panel kullan:
>
> A — source/original condition.
>
> B — restored interpretation.
>
> B'yi açıkça “restored” olarak etiketle.
>
> Orijinali değiştirilmiş sürümle değiştirme.

## English

> Use matched panels:
>
> A — source or original condition,
> B — restored interpretation.
>
> Label B explicitly as restored.
>
> Never replace the archival source with the altered version.

## Neye dikkat edilmeli?

Nesnenin fiziksel kondisyonu (kıvrım, solma, zarf) gizlenmesin; orijinal-restore ayrımı aynı karede etiketlensin.

---
# 1961. Bu turdaki slash-style indeks (aile-036)

| Kısayol | Aile |
|---|---|
| `/daily-notes-overlay` | handwritten daily annotation |
| `/photo-sketch-overlay` | sketch traced over real photo |
| `/outfit-annotation-photo` | outfit callout image |
| `/design-annotation-photo` | design-observation callouts |
| `/photo-margin-notes` | annotations outside image |
| `/annotation-layer-lock` | immutable photo + overlay |
| `/handwritten-fact-lock` | verified handwritten facts |
| `/notes-app-photo-board` | camera roll + notes + rough layout |
| `/camera-roll-story` | photo-dump narrative sequence |
| `/whats-in-my-bag` | bag + supplied contents |
| `/bag-flatlay` | top-down bag contents |
| `/bag-inventory` | numbered bag inventory |
| `/bag-exploded-layout` | contents distributed around bag |
| `/bag-pocket-map` | content-to-compartment mapping |
| `/bag-catch-storyboard` | vertical falling-item video plan |
| `/bag-catch-item-stickers` | isolated item assets |
| `/bag-story-card` | selected object stories |
| `/desk-figurine` | viral desk collectible figure |
| `/figurine-box` | fictional collectible package |
| `/figurine-monitor` | matching sculpt viewport |
| `/figurine-source-lock` | preserve source identity |
| `/figurine-scale-proof` | real environmental scale cues |
| `/figurine-production-board` | source → sculpt → prototype → box |
| `/figurine-pet-desk` | pet collectible scene |
| `/figurine-couple-desk` | two-person collectible set |
| `/figurine-no-brand` | non-branded collectible system |
| `/archive-photo-mount` | mounted archival photograph |
| `/archive-photo-verso` | front/back physical documentation |
| `/archive-sleeve` | clear archival enclosure |
| `/archive-paper-envelope` | archival paper housing |
| `/archive-contact-sheet` | sequential archival proof sheet |
| `/archive-negative-sleeve` | sleeved negative strips |
| `/archive-box` | foldered archival storage |
| `/archive-index-card` | catalog metadata card |
| `/archive-condition-record` | physical condition documentation |
| `/archive-before-after` | matched conservation documentation |
| `/provenance-chain` | documented ownership/source chain |
| `/archive-evidence-layer` | evidence/inference/reconstruction separation |
| `/source-vs-reconstruction` | original vs generated interpretation |
| `/museum-object-record` | collection catalog record |
| `/archive-display-wall` | archival exhibition wall |
| `/archive-selection-board` | curatorial selection review |
| `/physical-photo-object` | photograph as physical artifact |
| `/cabinet-card` | historic mounted-card photograph |
| `/album-page-photo` | physical photo-album page |
| `/photo-ephemera-page` | photo + real related ephemera |
| `/photo-object-condition` | preserve photographic condition |
| `/archive-original-vs-restored` | source/restoration pair |

## Bu turdaki kaynak sinyalleri

- Canva — **Design Trends 2026 / Notes App Chic**  
  https://www.canva.com/design-trends/
- Canva Newsroom — **Design Trends 2026**  
  https://www.canva.com/newsroom/news/design-trends-2026/
- Picsart — **Bag Catch Edit: What’s in My Bag Trend**  
  https://picsart.com/blog/bag-catch-edit-trend/
- Google — **Nano Banana visual trends / Figurines**  
  https://blog.google/products-and-platforms/products/gemini/nano-banana-google-trends-2025/
- Morphed — **AI Figurine Prompt 2026**  
  https://morphed.app/blog/ai-figurine-prompt
- Nature HSS Communications — **ArchiveGPT, 2026**  
  https://www.nature.com/articles/s41599-026-08367-6
- Archival Science — **Curatorial data formation in exhibition practice, 2026**  
  https://link.springer.com/article/10.1007/s10502-026-09560-x
- U.S. National Archives — **Photograph preservation / enclosures**  
  https://www.archives.gov/preservation/holdings-maintenance/photographs

---

<a id="aile-037"></a>
# Çekirdek Görsel Prompt Ailelerine Dönüş — 3×3 Grid, Sticker Sheet, Younger-Self, Headshot, Sketch ve Gerçek Model Sözdizimi

Bu bölüm rehberin ana amacına geri döner:

> **İnternette gerçekten dolaşan kısa görsel prompt kalıpları, viral dönüşümler ve doğrudan belirgin görsel sonuç veren terimler.**

2026 prompt arşivleri ve topluluk paylaşımlarında özellikle şu aileler sık görülüyor:

- 3×3 identity grid,
- expression grid,
- outfit/look grid,
- face sticker sheet,
- childhood + adult self,
- professional headshot,
- photo restoration,
- pencil / pen sketch,
- action figure / figurine,
- style reference.

Burada önemli bir ayrım daha eklenmelidir:

### Rehber içi shorthand

> `/expression-grid`

gibi ifadeler bizim kolay hatırlama etiketimizdir.

### Gerçek model parametresi

Midjourney’de:

> `--sref`
>
> `--sw`

gibi belgelenmiş parametreler gerçekten ürün sözdiziminin parçasıdır.

Bu iki şeyi aynı kategoride göstermemek gerekir.

---

# 1962. `/3x3-grid` — 3×3 Kimlik Grid'i

## Trend

**T1/T2 — Nano Banana / Gemini prompt topluluklarında 2026 boyunca çok görünür.**

## Türkçe prompt

> Kaynak [KİŞİ]'yi tek 3×3 grid içinde dokuz ayrı karede göster.
>
> Tüm karelerde:
>
> - aynı kişi,
> - aynı temel yüz yapısı,
> - aynı yaş,
> - aynı ten tonu,
> - aynı ayırt edici yüz özellikleri
>
> korunmalı.
>
> Her hücre tek bağımsız portre olsun.
>
> İnce ve tutarlı grid boşlukları kullan.
>
> Yüzleri birbirine karıştırma veya hücre sınırlarını bozma.

## English

> Create one 3×3 grid containing nine separate portraits of the source [PERSON].
>
> Preserve the same identity, underlying facial structure, age, skin tone, and distinctive features across all cells.
>
> Treat every cell as one independent portrait with consistent spacing.
>
> Do not blend faces across cells or break grid boundaries.

---

# 1963. `/expression-grid` — Dokuz Farklı İfade

## Viral kullanım

Topluluk promptlarında en yaygın 3×3 varyantlardan biri:

> same face + nine expressions.

## Türkçe

> Aynı kişinin 3×3 grid içinde dokuz doğal yüz ifadesini göster.
>
> Örnek:
>
> neutral,
> small smile,
> laugh,
> surprised,
> thoughtful,
> skeptical,
> focused,
> playful,
> calm.
>
> İfade değişirken yüz anatomisini yeniden tasarlama.
>
> Özellikle:
>
> - burun,
> - göz aralığı,
> - çene,
> - yüz oranı
>
> sabit kalsın.

## English

> Show the same person in a 3×3 grid with nine natural expressions such as neutral, subtle smile, laugh, surprised, thoughtful, skeptical, focused, playful, and calm.
>
> Preserve facial anatomy as expression changes.
>
> Keep nose shape, eye spacing, jaw structure, and overall facial proportions consistent.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin ([§1971](#sec-1971)); aynı kişi bütün hücrelerde aynı kalsın, sapan hücre tek başına üretilsin.

---
# 1964. `/outfit-grid` — Dokuz Kıyafet, Aynı Kişi

## Türkçe

> Aynı kişiyi dokuz farklı outfit ile 3×3 grid içinde göster.
>
> Yüz, saç çizgisi ve beden oranı sabit kalsın.
>
> Her hücrede yalnız outfit değişsin.
>
> Kamera mesafesi, framing ve temel poz eşleşsin.
>
> Outfit karşılaştırmasını background ve poz değişiklikleriyle karıştırma.

## English

> Show the same person in nine different outfits within a 3×3 grid.
>
> Preserve face, hairline, and body proportions.
>
> Change only the outfit in each cell while keeping camera distance, framing, and basic pose matched.
>
> Do not mix outfit comparison with unrelated background or pose changes.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin ([§1971](#sec-1971)); aynı kişi bütün hücrelerde aynı kalsın, sapan hücre tek başına üretilsin.

---
# 1965. `/pose-grid` — Poz Grid'i

## Türkçe

> Aynı kişi ve aynı kıyafetle dokuz farklı doğal pose göster.
>
> Kimlik, outfit, background ve ışık değişmesin.
>
> Değişken yalnız pose olsun.
>
> Beden oranlarının kareler arasında değişmesine izin verme.

## English

> Show nine different natural poses of the same person wearing the same outfit.
>
> Keep identity, outfit, background, and lighting fixed.
>
> Change only the pose.
>
> Preserve body proportions across all cells.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin ([§1971](#sec-1971)); aynı kişi bütün hücrelerde aynı kalsın, sapan hücre tek başına üretilsin.

---
# 1966. `/camera-angle-grid` — Kamera Açısı Grid'i

## Türkçe

> Aynı kişi, aynı poz ve aynı kıyafet için dokuz kontrollü camera-angle varyantı oluştur.
>
> Örneğin:
>
> eye-level,
> slight high angle,
> slight low angle,
> three-quarter left,
> three-quarter right,
> side profile.
>
> Açı değişirken yüz kimliği kaymasın.

## English

> Create a controlled grid of camera-angle variations for the same person, pose, and outfit, such as eye-level, slight high angle, slight low angle, three-quarter left, three-quarter right, and side profile.
>
> Preserve identity as viewpoint changes.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin ([§1971](#sec-1971)); aynı kişi bütün hücrelerde aynı kalsın, sapan hücre tek başına üretilsin.

---
# 1967. `/hairstyle-grid` — Saç Stili Deneme Grid'i

## Türkçe

> Kaynak yüz kimliğini koruyarak dokuz hairstyle varyantı göster.
>
> Yüz, ten tonu, makyaj ve kıyafet mümkün olduğunca sabit kalsın.
>
> Saç modeli değişirken:
>
> - alın,
> - kulak,
> - yüz şekli
>
> yeniden tasarlanmasın.

## English

> Show nine hairstyle variations while preserving the source facial identity.
>
> Keep face, skin tone, makeup, and clothing as consistent as possible.
>
> Do not redesign forehead, ears, or facial shape when changing hair.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin ([§1971](#sec-1971)); aynı kişi bütün hücrelerde aynı kalsın, sapan hücre tek başına üretilsin.

---
# 1968. `/look-grid` — Dokuz Farklı Look

## Ayrım

`/outfit-grid`:

> yalnız kıyafet.

`/look-grid`:

> outfit + styling + kontrollü mood.

## Türkçe

> Aynı kişiyi dokuz farklı styling look içinde göster.
>
> Kimlik sabit kalsın.
>
> Her look için en fazla:
>
> - outfit,
> - hairstyle,
> - tek aksesuar,
> - sınırlı background cue
>
> değişsin.
>
> Dokuz farklı kişiye dönüşmesin.

## English

> Show the same person across nine styling looks while preserving identity.
>
> Limit each look to outfit, hairstyle, one accessory, and a restrained background cue.
>
> Do not let the grid become nine different people.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin ([§1971](#sec-1971)); aynı kişi bütün hücrelerde aynı kalsın, sapan hücre tek başına üretilsin.

---
# 1969. `/character-sheet-grid` — Karakter Tutarlılığı Grid'i

## Türkçe

> [KARAKTER]'i 3×3 grid içinde:
>
> front,
> three-quarter,
> profile,
> smiling,
> neutral,
> action pose,
> seated,
> close-up,
> full-body
>
> varyantlarında göster.
>
> Aynı karakter tasarımı tüm hücrelerde korunmalı.
>
> Bu çıktı yeni tasarımlar üretmek değil continuity kontrolü içindir.

## English

> Show [CHARACTER] in a 3×3 grid containing front, three-quarter, profile, smiling, neutral, action pose, seated, close-up, and full-body views.
>
> Preserve one character design throughout.
>
> Use the sheet for continuity rather than generating nine redesigns.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin ([§1971](#sec-1971)); aynı kişi bütün hücrelerde aynı kalsın, sapan hücre tek başına üretilsin.

---
# 1970. `/grid-variable-lock` — Grid'de Tek Değişken Kuralı

## Master kontrol

Karşılaştırma grid'inde:

> **bir seferde mümkün olduğunca tek ana değişken.**

Örnek:

### İfade testi

Sabit:

- outfit,
- light,
- camera,
- background.

Değişken:

- expression.

### Outfit testi

Sabit:

- face,
- pose,
- light,
- camera.

Değişken:

- clothing.

Bu yöntem “neden farklı görünüyor?” sorusunu azaltır.

---

<a id="sec-1971"></a>
# 1971. `/grid-cell-count-lock` — Hücre Sayısı Kilidi

## Türkçe

> Tam olarak 3 sütun × 3 satır = 9 hücre üret.
>
> Hücreleri birleştirme.
>
> Eksik veya fazladan panel üretme.
>
> Her hücrenin sınırı açık ve tutarlı olsun.

## English

> Produce exactly 3 columns × 3 rows = 9 cells.
>
> Do not merge cells or add extra panels.
>
> Keep every cell boundary clear and consistent.

## Neye dikkat edilmeli?

Hücre sayısı sabitlensin ([§1971](#sec-1971)); aynı kişi bütün hücrelerde aynı kalsın, sapan hücre tek başına üretilsin.

---
# 1972. `/grid-slop-filter` — 3×3 Grid AI Slop Filtresi

Kaçınılması gerekenler:

- 8 veya 10 hücre,
- birleşmiş yüzler,
- aynı ifadenin tekrarı,
- her hücrede farklı yüz,
- outfit testinde background değiştirmek,
- expression testinde saç/kıyafet değiştirmek,
- hücreler arasında farklı yaş,
- sahte “100% exact face match” teknik parametresi iddia etmek.

---

<a id="aile-038"></a>
# Sticker Sheet — 2026’nın En Kullanışlı Viral Formatlarından Biri

Ağustos 2026’da yayımlanan güncel prompt arşivlerinde:

> selfie → 12/16 expression sticker pack

formatı ayrı viral trend olarak geçiyor.

Bu trendin güçlü yanı:

> tek görsel değil, **kullanılabilir reaction asset seti** üretmesidir.

---

<a id="sec-1973"></a>
# 1973. `/sticker-sheet` — Genel Sticker Sheet

## Türkçe prompt

> [KONU/KARAKTER]'den 12 ayrı sticker oluşan düzenli sticker sheet oluştur.
>
> Tüm sticker'larda:
>
> - aynı karakter kimliği,
> - aynı line/render sistemi,
> - aynı outline/cutline mantığı
>
> korunsun.
>
> Sticker'lar birbirine temas etmesin.
>
> Her sticker ayrı kesilebilir kadar whitespace taşısın.

## English

> Create a sheet of 12 separate stickers based on [SUBJECT/CHARACTER].
>
> Preserve the same identity, line or rendering system, and outline or cutline logic across the set.
>
> Keep stickers separated with enough whitespace to cut individually.

## Neye dikkat edilmeli?

Karakter bütün çıkartmalarda aynı kalsın (yüz, giysi, renk); sapan çıkartma tek değişiklikle yeniden üretilir.

---
# 1974. `/face-sticker-16` — 16 İfadeli Yüz Sticker Seti

## Trend

**T1/T2 — Ağustos 2026 viral selfie sticker-sheet formatı.**

## Türkçe

> Kaynak kişiyi 4×4 grid içinde 16 ayrı reaction sticker'a dönüştür.
>
> Aynı yüz kimliği tüm sticker'larda korunmalı.
>
> İfadeler tekrar etmesin:
>
> happy,
> laugh,
> shocked,
> confused,
> sleepy,
> annoyed,
> proud,
> thinking,
> excited,
> embarrassed,
> skeptical,
> cheering,
> sad,
> focused,
> playful,
> calm.
>
> Yalnız ifade ve küçük pose değişsin.

## English

> Transform the source person into 16 separate reaction stickers arranged in a 4×4 grid.
>
> Preserve the same facial identity throughout.
>
> Use distinct expressions such as happy, laughing, shocked, confused, sleepy, annoyed, proud, thinking, excited, embarrassed, skeptical, cheering, sad, focused, playful, and calm.
>
> Change only expression and small pose cues.

---

# 1975. `/reaction-stickers` — Mesajlaşma Tepki Sticker'ları

## Türkçe

> [KARAKTER/KİŞİ]'den günlük mesajlaşmada kullanılabilecek 10 reaction sticker üret.
>
> Her sticker tek net duyguyu iletsin.
>
> Uzun text kullanma.
>
> Gerekirse yalnız:
>
> “tamam”
> “hadi”
> “eyvah”
> “teşekkür”
>
> gibi çok kısa copy kullanılabilir ve exact text olarak verilmelidir.

## English

> Create ten reaction stickers from [CHARACTER/PERSON] for everyday messaging.
>
> Make each sticker communicate one clear reaction.
>
> Avoid long text.
>
> If words are used, keep them very short and preserve the supplied copy exactly.

## Neye dikkat edilmeli?

Karakter bütün çıkartmalarda aynı kalsın (yüz, giysi, renk); sapan çıkartma tek değişiklikle yeniden üretilir.

---
# 1976. `/messaging-sticker-pack` — Mesajlaşma Uygulaması Paket Sistemi

## Türkçe

> Aynı sticker karakterini 24 parçalık messaging pack olarak planla.
>
> Aile:
>
> - greeting,
> - thanks,
> - yes/no,
> - celebration,
> - confusion,
> - apology,
> - waiting,
> - sleep,
> - food,
> - work/study
>
> gibi gerçek kullanım durumlarını kapsasın.
>
> 24 farklı rastgele mimik üretme.

## English

> Plan a 24-sticker messaging pack around real communication use cases such as greeting, thanks, yes or no, celebration, confusion, apology, waiting, sleep, food, and work or study.
>
> Do not generate 24 random expressions without communication purpose.

## Neye dikkat edilmeli?

Karakter bütün çıkartmalarda aynı kalsın (yüz, giysi, renk); sapan çıkartma tek değişiklikle yeniden üretilir.

---
# 1977. `/sticker-cutline` — Kesim Konturu

## Türkçe

> Her sticker çevresinde tutarlı beyaz veya şeffaflık sınırına uygun cutline bırak.
>
> Cutline saç, el ve ince detaylarda aşırı girintili çıkıntılı olmasın.
>
> Baskı için gerçek contour-cut dosyası gerekiyorsa vektör tasarım aracında ayrıca hazırlanmalı.

## English

> Give every sticker a consistent cutline with practical spacing around hair, hands, and small details.
>
> Avoid excessively complex contours.
>
> Prepare actual production contour-cut paths separately in vector software when needed.

## Neye dikkat edilmeli?

Karakter bütün çıkartmalarda aynı kalsın (yüz, giysi, renk); sapan çıkartma tek değişiklikle yeniden üretilir.

---
# 1978. `/sticker-isolated-assets` — Sticker'ları Ayrı Asset Olarak Planla

## Türkçe

> Sticker sheet'in yanında her sticker'ın ayrı transparent-background asset olarak çıkarılabileceği kompozisyon kur.
>
> Sticker'ların birbirine gölge veya obje taşması yapmamasını sağla.

## English

> Structure the sticker sheet so every sticker can also be isolated as a separate transparent-background asset.
>
> Prevent shadows or objects from crossing into neighboring stickers.

## Neye dikkat edilmeli?

Karakter bütün çıkartmalarda aynı kalsın (yüz, giysi, renk); sapan çıkartma tek değişiklikle yeniden üretilir.

---
# 1979. `/sports-card-sticker` — Sporcu Sticker Kartı

## 2026 World Cup bağlantılı sosyal kullanım

## Türkçe

> Kaynak kişiyi kurmaca spor sticker-card formatında göster.
>
> Kullanıcı tarafından verilmiş:
>
> isim,
> numara,
> takım/ülke bilgisi
>
> kullanılabilir.
>
> Gerçek lisanslı sticker markasının logo ve trade dress'ini bire bir kopyalama.
>
> Uydurma istatistik ekleme.

## English

> Present the source person as a fictional sports sticker card using supplied name, number, and team or country information.
>
> Do not reproduce a real licensed sticker brand’s logo or trade dress.
>
> Do not invent statistics.

## Neye dikkat edilmeli?

Karakter bütün çıkartmalarda aynı kalsın (yüz, giysi, renk); sapan çıkartma tek değişiklikle yeniden üretilir.

---
# 1980. `/sticker-slop-filter` — Sticker Sheet AI Slop Filtresi

Kaçınılması gerekenler:

- her sticker farklı karakter,
- 16 hücrede 11 gerçek sticker,
- yüz kimliği kayması,
- her sticker'a speech bubble,
- unreadable text,
- kesim sınırlarının birbirine girmesi,
- gereksiz chibi zorunluluğu,
- source adult'ı çocuk yüzüne dönüştürmek,
- gerçek messaging-app markasını kopyalamak.

---

<a id="aile-039"></a>
# Adult Self + Childhood Self — Viral “Impossible Memory” Formatı

Google’ın kendi Gemini örneklerinde:

> yetişkin fotoğrafı → yetişkin kişinin çocuk hâliyle aynı odada çay partisi yapması

doğrudan örnek kullanım olarak gösterildi.

2026’da bu fikir:

- adult meets child,
- adult hugs younger self,
- then vs now,
- childhood recreation

gibi varyantlarla sosyal medyada büyüdü.

Ana etik kural:

> **Bu bir geri kazanılmış anı veya gerçek tarihsel fotoğraf değildir.**
>
> AI-generated composite / imagined scene'dir.

---

# 1981. `/childhood-meets-adult` — Yetişkin Hâlin Çocuk Hâlinle Buluşması

## Türkçe prompt

> Reference A'daki yetişkin kişi ile Reference B'deki çocukluk fotoğrafındaki aynı kişiyi tek gerçekçi sahnede birlikte göster.
>
> Her iki yaş döneminin yüz özellikleri kendi referansına bağlı kalsın.
>
> Ortam kullanıcı tarafından belirtilen sade ve gündelik [MEKÂN] olsun.
>
> İki kişi doğal biçimde birbirine bakabilir veya yan yana oturabilir.
>
> Görseli gerçek geçmiş fotoğrafı gibi sunma.

## English

> Show the adult person from Reference A together with the same person as a child from Reference B in one believable scene.
>
> Preserve the age-appropriate identity cues from each reference separately.
>
> Place them in the user-specified ordinary [SETTING].
>
> They may look at each other or sit together naturally.
>
> Do not present the result as an authentic historical photograph.

## Neye dikkat edilmeli?

Kimlik bütün yaşlarda ve kişilerde karışmasın; hangi yüzün kime ait olduğu promptta adıyla belirtilsin ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623) kimlik kuralı).

---
# 1982. `/adult-child-tea-party` — Çocukluk Hâliyle Çay Partisi

## Google örnek promptuna dayalı varyant

## Türkçe

> Yetişkin kişi ile çocukluk hâlini sade bir oyun/çocuk odasında küçük çay partisi yaparken göster.
>
> Yetişkin ve çocuk aynı kişinin farklı yaşları olarak tanınabilir olsun.
>
> Sahne duygusal olabilir ama aşırı dramatik ışık, glow veya “healing aura” kullanma.

## English

> Show the adult person having a small tea party with their childhood self in a simple playroom.
>
> Make the two figures recognizable as different ages of the same person.
>
> Keep the scene emotionally warm without dramatic glow or healing-aura effects.

## Neye dikkat edilmeli?

Kimlik bütün yaşlarda karışmasın; hangi yüzün kime ait olduğu promptta adıyla belirtilsin ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623) kimlik kuralı).

---
# 1983. `/then-now-split` — Çocukluk / Bugün Yan Yana

## Türkçe

> Çocukluk reference ve güncel reference'ı iki eşit panelde göster.
>
> Yüzleri aynı frame hizasında mümkün olduğunca benzer head position ile yerleştir.
>
> Her panel kendi gerçek dönem/yaş kimliğini korusun.
>
> Yıllar kullanıcı tarafından verilmişse yazılabilir.
>
> Tarih uydurma.

## English

> Place the childhood reference and present-day reference in two matched panels with similar head position and framing where possible.
>
> Preserve the authentic age identity of each.
>
> Add years only when supplied.
>
> Do not invent dates.

## Neye dikkat edilmeli?

Kimlik bütün yaşlarda karışmasın; hangi yüzün kime ait olduğu promptta adıyla belirtilsin ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623) kimlik kuralı).

---
# 1984. `/then-now-aligned-face` — Yüz Hizalamalı Önce / Şimdi

## Türkçe

> Çocukluk ve bugünkü portreyi göz çizgileri ve yüz merkezi mümkün olduğunca hizalı olacak şekilde karşılaştır.
>
> Bu dönüşüm-aging efekti değil; iki ayrı gerçek reference'ın karşılaştırması olsun.
>
> Yüzlerden birini diğerine morph etme.

## English

> Align childhood and present-day portraits by eye line and facial center for comparison.
>
> Treat them as two separate source identities at different ages rather than morphing one face into the other.

## Neye dikkat edilmeli?

Kimlik bütün yaşlarda karışmasın; hangi yüzün kime ait olduğu promptta adıyla belirtilsin ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623) kimlik kuralı).

---
# 1985. `/childhood-recreation` — Eski Fotoğrafı Bugün Yeniden Canlandırma

## Türkçe

> Kaynak çocukluk fotoğrafındaki:
>
> - pose,
> - kişi yerleşimi,
> - framing,
> - önemli props
>
> bugünkü hâllerle yeniden kurulmuş recreation photo olarak göster.
>
> Yeni fotoğrafı eski fotoğrafın restore edilmiş sürümü gibi gösterme.
>
> İki tarihsel anı açıkça ayır.

## English

> Recreate the pose, subject placement, framing, and important props of the childhood photograph using the present-day subjects.
>
> Present it as a modern recreation rather than a restored version of the original.
>
> Keep the two time periods clearly distinct.

## Neye dikkat edilmeli?

Kimlik bütün yaşlarda karışmasın; hangi yüzün kime ait olduğu promptta adıyla belirtilsin ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623) kimlik kuralı).

---
# 1986. `/younger-self-scene-lock` — Yaş Dönemi Kilidi

## Türkçe

> Yetişkin reference'taki yüzü çocuk bedenine yapıştırma.
>
> Çocukluk figure'ı mümkün olduğunca gerçek childhood reference'a dayansın.
>
> Adult figure ise yalnız current reference'a dayansın.
>
> İki yaş kimliği ayrı referans rolü taşısın.

## English

> Do not paste the adult face onto a child body.
>
> Base the child figure on the real childhood reference and the adult figure on the current reference.
>
> Treat each age identity as a separate reference role.

## Neye dikkat edilmeli?

Kimlik bütün yaşlarda karışmasın; hangi yüzün kime ait olduğu promptta adıyla belirtilsin ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623) kimlik kuralı).

---
# 1987. `/imagined-memory-label` — Yapay Anı Etiketi

## Rehber kuralı

Bu tür görseller paylaşılırken yanlış anlaşılma riski varsa:

> AI-generated imagined scene
>
> veya
>
> AI composite

gibi açık tanım kullanılabilir.

Özellikle:

- tarihsel,
- ailevi,
- haber değeri taşıyan,
- belgesel bağlamlı

kullanımlarda önemlidir.

---

# 1988. `/younger-self-slop-filter` — Younger-self AI Slop Filtresi

Kaçınılması gerekenler:

- yetişkin yüzünü çocuk bedenine koymak,
- “healing light” klişesi,
- gerçek olmayan anıyı gerçek fotoğraf gibi sunmak,
- çocukluk tarihini uydurmak,
- childhood reference yokken kesin çocuk yüzü iddia etmek,
- her sahneyi sarılma/terapi metaforuna çevirmek.

---

<a id="aile-040"></a>
# Professional Headshot — Viral ama İşlevsel Prompt Ailesi

2026’da Gemini/Nano Banana prompt kütüphanelerinde:

> professional headshot,
> LinkedIn headshot,
> corporate studio portrait

en sık tekrarlanan pratik dönüşümlerden biri.

Ancak bu formatta sık hata:

> modelin kişiyi “daha profesyonel” yapmak adına yüzü güzelleştirmesi veya kimliği değiştirmesi.

Bu yüzden ana kontrol:

> **professionalize the presentation, not the face.**

---

# 1989. `/professional-headshot` — Profesyonel Profil Portresi

## Türkçe prompt

> Kaynak kişinin yüz kimliğini koruyarak temiz professional headshot oluştur.
>
> Framing:
>
> baş + omuzlar / üst göğüs.
>
> Kamera:
>
> eye-level.
>
> Işık:
>
> yumuşak kontrollü studio light.
>
> Background:
>
> sade neutral.
>
> Yüzü güzelleştirme, jaw/nose/eye shape değiştirme veya cildi plastikleştirme.
>
> Profesyonellik ışık, kıyafet ve kompozisyondan gelsin.

## English

> Create a clean professional headshot while preserving the source person’s facial identity.
>
> Use head-and-shoulders or upper-chest framing, eye-level camera, controlled soft studio lighting, and a restrained neutral background.
>
> Do not beautify, reshape the jaw, nose, or eyes, or create plastic skin.
>
> Let professionalism come from lighting, wardrobe, and composition.

## Neye dikkat edilmeli?

Cilt dokusu ve oranlar doğal kalsın; aşırı rötuş resmî başvurularda sorun çıkarır. Kimlik fotoğrafı estetiği resmî belge garantisi vermez (aile-048).

---
# 1990. `/corporate-headshot` — Kurumsal Headshot

## Türkçe

> Aynı yüz kimliğiyle sade kurumsal portre üret.
>
> Outfit:
>
> kullanıcının belirttiği formal/business attire.
>
> Background:
>
> neutral gray, off-white veya gerçek ofis bağlamı.
>
> “CEO look” diye kişiye daha sert çene, daha yaşlı görünüm veya lüks saat ekleme.

## English

> Create a restrained corporate portrait using the supplied business attire and a neutral gray, off-white, or real office background.
>
> Preserve identity.
>
> Do not invent a stronger jaw, older appearance, luxury watch, or status cues to signal “executive.”

## Neye dikkat edilmeli?

Cilt dokusu ve oranlar doğal kalsın; aşırı rötuş resmî başvurularda sorun çıkarır. Kimlik fotoğrafı estetiği resmî belge garantisi vermez (aile-048).

---
# 1991. `/creative-headshot` — Yaratıcı Meslek Portresi

## Türkçe

> Kaynak kişiyi yaratıcı-profesyonel headshot olarak göster.
>
> Neutral fakat daha sıcak/karakterli:
>
> - studio color,
> - soft window light,
> - subtle environmental cue
>
> kullanılabilir.
>
> Mesleği bilinmiyorsa kamera, fırça, laptop gibi “creative person props” uydurma.

## English

> Create a creative-professional headshot with the same identity using restrained studio color, soft window light, or one subtle environmental cue.
>
> Do not invent cameras, brushes, laptops, or other “creative professional” props unless relevant information is supplied.

## Neye dikkat edilmeli?

Cilt dokusu ve oranlar doğal kalsın; aşırı rötuş resmî başvurularda sorun çıkarır. Kimlik fotoğrafı estetiği resmî belge garantisi vermez (aile-048).

---
# 1992. `/outdoor-headshot` — Doğal Işık Profil Portresi

## Türkçe

> Aynı yüz kimliğiyle dış mekânda soft natural-light headshot oluştur.
>
> Background dikkat dağıtmayan gerçek çevre olsun.
>
> Shallow depth of field kontrollü kullanılabilir.
>
> Arka planı lüks şehir/iş merkezi yaparak sosyal statü ekleme.

## English

> Create an outdoor headshot using soft natural light while preserving facial identity.
>
> Keep the real environment understated and non-distracting.
>
> Use controlled shallow depth of field where useful.
>
> Do not invent luxury city or corporate settings to imply social status.

## Neye dikkat edilmeli?

Cilt dokusu ve oranlar doğal kalsın; aşırı rötuş resmî başvurularda sorun çıkarır. Kimlik fotoğrafı estetiği resmî belge garantisi vermez (aile-048).

---
# 1993. `/profile-photo-crop` — Profil Fotoğrafı Kadrajı

## Türkçe

> Portreyi küçük circular/square profile kullanımını düşünerek crop et.
>
> Yüz merkezi güvenli alanda kalsın.
>
> Saçın üstünü veya çeneyi gereksiz kesme.
>
> 1:1 thumbnail'da gözler net okunabilsin.

## English

> Crop the portrait for small circular or square profile use.
>
> Keep the face within a safe central area without unnecessarily cutting the top of the hair or chin.
>
> Make the eyes readable at thumbnail size.

## Neye dikkat edilmeli?

Cilt dokusu ve oranlar doğal kalsın; aşırı rötuş resmî başvurularda sorun çıkarır. Kimlik fotoğrafı estetiği resmî belge garantisi vermez (aile-048).

---
# 1994. `/headshot-identity-lock` — Headshot Kimlik Kilidi

## Türkçe

> Değiştirilebilecek:
>
> - background,
> - light,
> - crop,
> - user-specified clothing.
>
> Korunacak:
>
> - facial geometry,
> - skin tone,
> - age,
> - hairline,
> - defining marks.
>
> “100% exact” gibi gerçek olmayan teknik garanti yazma; hedefi açık doğal dille belirt.

## English

> Allow changes to background, lighting, crop, and user-specified clothing while preserving facial geometry, skin tone, age, hairline, and defining marks.
>
> State the preservation goal clearly without pretending “100% exact match” is a real guaranteed parameter.

## Neye dikkat edilmeli?

Cilt dokusu ve oranlar doğal kalsın; aşırı rötuş resmî başvurularda sorun çıkarır. Kimlik fotoğrafı estetiği resmî belge garantisi vermez (aile-048).

---
# 1995. `/headshot-slop-filter` — Headshot AI Slop Filtresi

Kaçınılması gerekenler:

- plastic skin,
- whitened teeth zorunluluğu,
- jaw enhancement,
- symmetry correction,
- generic navy suit,
- luxury office background,
- aşırı rim light,
- göz rengini değiştirmek,
- yaş küçültme,
- “professional” = sosyal statü sembolü.

---

<a id="aile-041"></a>
# Photo → Sketch — Basit ama Hâlâ Çok Kullanılan Dönüşüm

Google’ın kendi Nano Banana örneklerinde doğrudan:

> “Turn this photo into a pencil drawing.”

kullanımı yer alıyor.

Midjourney’nin resmî prompting rehberi de:

- ballpoint pen sketch,
- pencil sketch,
- block print,
- paint-by-numbers,
- risograph,
- cyanotype

gibi yerleşik medium adlarını açık örnek olarak listeliyor.

Bu aile rehberin ana amacına çok uygundur çünkü:

> **tek bir teknik terim, görsel sonucu güçlü biçimde değiştirir.**

---

# 1996. `/pencil-sketch` — Kurşun Kalem Eskizi

## Türkçe prompt

> Kaynak [FOTOĞRAF/NESNE]'yi graphite pencil sketch'e dönüştür.
>
> Kullan:
>
> - gerçek kalem çizgi yönü,
> - kontrollü hatching,
> - farklı pressure/value,
> - kâğıt beyazını highlight olarak bırakma.
>
> Kaynak form ve oranı koru.
>
> Fotoğrafın üzerine gri “sketch filter” uygulama.

## English

> Transform [PHOTO/OBJECT] into a graphite pencil sketch using real directional pencil strokes, controlled hatching, varied pressure and value, and the paper white as highlight.
>
> Preserve source form and proportions.
>
> Do not merely apply a gray sketch filter.

## Neye dikkat edilmeli?

Mediumun fiziksel mantığı (kurşun izi, boya akışı, kurşun came, poligon bütçesi) görünsün; yüze yalnızca doku kaplanmışsa baştan üretin.

---
# 1997. `/ballpoint-sketch` — Tükenmez Kalem Eskizi

## Midjourney resmî medium örneklerinden

## Türkçe

> [KONU]'yu ballpoint pen sketch olarak göster.
>
> Çizgi:
>
> - ince,
> - tekrar taramalı,
> - pressure değişimi sınırlı,
> - ink buildup görülebilir
>
> olsun.
>
> Marker veya brush pen gibi geniş stroke kullanma.

## English

> Render [SUBJECT] as a ballpoint pen sketch using fine repeated hatching, restrained pressure variation, and visible ink buildup.
>
> Avoid broad marker or brush-pen strokes.

## Neye dikkat edilmeli?

Mediumun fiziksel mantığı (kurşun izi, mürekkep akışı, baskı basıncı) görünsün; yüze yalnızca doku kaplanmışsa baştan üretin.

---
# 1998. `/pen-line-portrait` — Kalem Çizgi Portre

## Viral social varyant

## Türkçe

> Kaynak portreyi temiz black-ink line portrait'e dönüştür.
>
> Ana:
>
> - face contour,
> - eyes,
> - nose,
> - lips,
> - hair mass
>
> korunmalı.
>
> Gölgelendirmeyi sınırlı cross-hatching ile yap.
>
> Yüz kimliğini idealize etme.

## English

> Transform the source portrait into a clean black-ink line portrait preserving face contour, eyes, nose, lips, and hair mass.
>
> Use restrained cross-hatching for shading.
>
> Do not idealize facial identity.

## Neye dikkat edilmeli?

Mediumun fiziksel mantığı (kurşun izi, mürekkep akışı, baskı basıncı) görünsün; yüze yalnızca doku kaplanmışsa baştan üretin.

---
# 1999. `/block-print` — Block Print

## Midjourney resmî medium örneği

## Türkçe

> [KONU]'yu fiziksel block-print dilinde göster.
>
> Kullan:
>
> - sınırlı renk,
> - oyulmuş negatif alan,
> - düzensiz ink transfer,
> - kalın grafik form.
>
> Dijital vector silhouette üzerine grain eklemekle yetinme.

## English

> Render [SUBJECT] using a physical block-print language with limited color, carved negative space, irregular ink transfer, and bold graphic shapes.
>
> Do not simply add grain to a vector silhouette.

## Neye dikkat edilmeli?

Mediumun fiziksel mantığı (kurşun izi, mürekkep akışı, baskı basıncı) görünsün; yüze yalnızca doku kaplanmışsa baştan üretin.

---
# 2000. `/paint-by-numbers` — Numaralı Boyama

## Midjourney resmî medium örneği

## Türkçe

> [SAHNE]'yi paint-by-numbers template olarak göster.
>
> Görsel:
>
> - kapalı boya alanları,
> - sınırlı palette,
> - her alan içinde küçük paint number
>
> taşısın.
>
> Aynı numara aynı rengi temsil etsin.
>
> Gerçek kullanılabilir kit gerekiyorsa renk/numara eşleşmesi ayrıca vektör/şablon aracıyla doğrulanmalı.

## English

> Turn [SCENE] into a paint-by-numbers template using closed paint regions, a limited palette, and small paint numbers inside each region.
>
> Keep number-to-color mapping consistent.
>
> For a production-ready kit, verify the actual regions and palette in a dedicated design workflow.

## Neye dikkat edilmeli?

Mediumun fiziksel mantığı (kurşun izi, mürekkep akışı, baskı basıncı) görünsün; yüze yalnızca doku kaplanmışsa baştan üretin.

---
# 2001. `/photo-to-line-art` — Fotoğraftan Temiz Line Art

## Türkçe

> Kaynak nesnenin yalnız yapısal dış ve önemli iç contour çizgilerini çıkar.
>
> Gölge ve renk kaldırılabilir.
>
> Her texture ayrıntısını çizgiye dönüştürme.
>
> Nesne tanınabilirliği korunmalı.

## English

> Convert the source object into clean line art using only structural outer contours and important internal edges.
>
> Remove color and shading where appropriate.
>
> Do not convert every texture detail into a line.
>
> Preserve recognizability.

## Neye dikkat edilmeli?

Mediumun fiziksel mantığı (kurşun izi, mürekkep akışı, baskı basıncı) görünsün; yüze yalnızca doku kaplanmışsa baştan üretin.

---
# 2002. `/sketchbook-page` — Sketchbook Sayfası

## Türkçe

> [KONU]'yu tek sketchbook sayfasında 3–6 çalışma eskizi olarak göster.
>
> Aynı tasarımın:
>
> - quick thumbnail,
> - contour study,
> - detail,
> - final sketch
>
> gibi gerçek çalışma aşamaları olabilir.
>
> Sayfayı hazır final çizime dekoratif el yazısı eklenmiş moodboard'a dönüştürme.

## English

> Show [SUBJECT] as 3–6 genuine studies on one sketchbook page, such as quick thumbnail, contour study, detail, and final sketch.
>
> Avoid turning a finished illustration into a moodboard with decorative handwriting.

## Neye dikkat edilmeli?

Mediumun fiziksel mantığı (kurşun izi, mürekkep akışı, baskı basıncı) görünsün; yüze yalnızca doku kaplanmışsa baştan üretin.

---
# 2003. `/sketch-slop-filter` — Sketch AI Slop Filtresi

Kaçınılması gerekenler:

- sketch = grayscale filter,
- her yerde construction circle,
- sahte silgi izi,
- okunmayan random notes,
- her çizime spiral notebook,
- line art'ta gereksiz texture,
- kaynak yüzü “daha güzel” çizmek,
- bütün çizgilerin dijital olarak aynı kalınlıkta olması.

---

<a id="aile-042"></a>
# Photo Restoration — Viral “Before → Recovered” Ailesi

2026 Gemini prompt kütüphanelerinde photo restoration hâlâ çok sık kullanılan ana kategorilerden biridir.

Restoration'ın amacı:

> tarihi yeniden tasarlamak değil,
>
> **kaynak görüntüde zaten mevcut bilgiyi mümkün olduğunca geri kazanmak.**

---

# 2004. `/photo-restoration` — Eski Fotoğraf Restorasyonu

## Türkçe prompt

> Kaynak eski fotoğrafı restore et.
>
> Öncelik:
>
> - dust/scratch reduction,
> - torn/creased area repair,
> - faded tonal recovery,
> - face/detail clarity
>
> olsun.
>
> Kişilerin:
>
> - yüz yapısını,
> - kıyafetini,
> - saçını,
> - background nesnelerini
>
> yeniden tasarlama.
>
> Kaynakta görünmeyen ayrıntıları kesin bilgi gibi icat etme.

## English

> Restore the source old photograph with priority on dust and scratch reduction, repair of tears or creases, tonal recovery, and improved face or detail clarity.
>
> Do not redesign facial structure, clothing, hair, or background objects.
>
> Do not invent unseen details as factual.

## Neye dikkat edilmeli?

Orijinal kimlik ve dönem korunsun; model eksik kalan yüz, el ve yazı gibi yerleri uydurur. Uydurulan her ayrıntı kaynak fotoğrafla karşılaştırılır; emin olunamayan yer boş bırakılır.

---
# 2005. `/scratch-repair` — Çizik / Yırtık Onarımı

## Türkçe

> Yalnız fiziksel damage alanlarını düzelt.
>
> Hasarsız yüz ve background bölgelerini değiştirme.
>
> Büyük eksik bölgelerde reconstruction belirsizliği varsa bunu “best-effort reconstruction” olarak ele al.

## English

> Repair only physically damaged regions.
>
> Do not alter undamaged faces or background areas.
>
> Treat large missing regions as best-effort reconstruction rather than certain recovery.

## Neye dikkat edilmeli?

Orijinal kimlik ve dönem korunsun; model eksik kalan yüz, el ve yazı gibi yerleri uydurur. Uydurulan her ayrıntı kaynak fotoğrafla karşılaştırılır.

---
# 2006. `/fade-recovery` — Solmuş Tonları Geri Getirme

## Türkçe

> Solmuş fotoğrafın tonal range'ini kontrollü biçimde geri getir.
>
> Highlight ve shadow detail'i iyileştir.
>
> Modern HDR contrast üretme.
>
> Dönemin baskı karakterini tamamen silme.

## English

> Recover tonal range in the faded photograph while improving highlight and shadow detail.
>
> Avoid modern HDR contrast.
>
> Preserve the original photographic print character.

## Neye dikkat edilmeli?

Orijinal kimlik ve dönem korunsun; model eksik kalan yüz, el ve yazı gibi yerleri uydurur. Uydurulan her ayrıntı kaynak fotoğrafla karşılaştırılır.

---
# 2007. `/old-photo-colorize` — Eski Fotoğrafı Renklendirme

## Kritik doğruluk notu

Renklendirme:

> gerçek tarihsel renk kanıtı olmayabilir.

## Türkçe

> Siyah-beyaz [FOTOĞRAF]'ı colorize et.
>
> Bilinen:
>
> - uniform,
> - object,
> - architecture,
> - skin/hair
>
> renkleri kaynak varsa ona göre kullan.
>
> Bilinmeyen renkleri “plausible interpretation” olarak ele al.
>
> Renklendirilmiş sürümü orijinal belge gibi sunma.

## English

> Colorize [BLACK-AND-WHITE PHOTO].
>
> Use sourced colors for uniforms, objects, architecture, skin, or hair where known.
>
> Treat unknown colors as plausible interpretation.
>
> Do not present the colorized version as the original historical record.

## Neye dikkat edilmeli?

Orijinal kimlik ve dönem korunsun; model eksik kalan yüz, el ve yazı gibi yerleri uydurur. Uydurulan her ayrıntı kaynak fotoğrafla karşılaştırılır.

---
# 2008. `/face-restoration-lock` — Yüz Restorasyon Kilidi

## Türkçe

> Yüzde:
>
> - göz şekli,
> - burun,
> - ağız,
> - çene,
> - yaş
>
> kaynakta görülebildiği ölçüde korunmalı.
>
> Restoration sırasında modern beauty retouch yapma.
>
> Eksik ayrıntıda daha “yakışıklı/güzel” yüz uydurma.

## English

> Preserve visible eye shape, nose, mouth, jaw, and age cues during face restoration.
>
> Do not apply modern beauty retouching or invent a more attractive face when detail is missing.

## Neye dikkat edilmeli?

Orijinal kimlik ve dönem korunsun; model eksik kalan yüz, el ve yazı gibi yerleri uydurur. Uydurulan her ayrıntı kaynak fotoğrafla karşılaştırılır.

---
# 2009. `/restoration-pair` — Orijinal / Restore Eşleşmesi

## Türkçe

> Aynı fotoğrafı iki matched panelde göster:
>
> A — untouched source.
>
> B — restored version.
>
> Crop ve scale aynı kalsın.
>
> Restorasyonun etkisini dramatikleştirmek için B'de farklı contrast/crop kullanma.

## English

> Show the same photograph in matched panels:
>
> A — untouched source,
> B — restored version.
>
> Keep crop and scale identical.
>
> Do not exaggerate restoration through different framing or unrelated contrast.

## Neye dikkat edilmeli?

Orijinal kimlik ve dönem korunsun; model eksik kalan yüz, el ve yazı gibi yerleri uydurur. Uydurulan her ayrıntı kaynak fotoğrafla karşılaştırılır.

---
# 2010. `/restoration-slop-filter` — Restoration AI Slop Filtresi

Kaçınılması gerekenler:

- yaş küçültmek,
- yeni saç üretmek,
- kıyafet stilini değiştirmek,
- modern makyaj,
- plastik skin,
- olmayan diş/gülümseme,
- tarihi background'u modernleştirmek,
- colorized version'ı source diye göstermek,
- “restore” adı altında yeniden üretim.

---

<a id="aile-043"></a>
# Gerçek Model Sözdizimi vs Rehber Kısayolu

Bu rehberde `/...` biçiminin iki farklı şeyle karışmaması gerekir.

## 1. Rehber shorthand

Örneğin:

> `/pencil-sketch`
>
> `/expression-grid`
>
> `/figurine`

Bunlar:

> **bizim mnemonic etiketlerimizdir.**

ChatGPT/Gemini’nin evrensel resmî komutları değildir.

## 2. Modelin gerçekten belgelediği parametre

Örneğin Midjourney:

> `--sref`
>
> `--sw`

Bunlar ürünün resmî prompting sistemi içinde belgelenmiştir.

---

<a id="sec-2011"></a>
# 2011. `--sref` — Midjourney Style Reference

## Resmî Midjourney parametresi

Midjourney dokümantasyonuna göre `--sref`:

> başka bir image'ın veya style code'un genel görsel “look and feel” özelliklerini referans olarak kullanmak

içindir.

Amaç:

- renk,
- medium,
- texture,
- lighting

gibi stil özelliklerini taşımaktır.

Nesne/kişiyi kopyalamak için değildir.

## Örnek

> `portrait of a botanist in a greenhouse --sref [STYLE_REFERENCE]`

Bu:

> rehber içi `/style-reference` shorthand'ından farklı olarak gerçek Midjourney syntax'ıdır.

---

# 2012. `--sw` — Midjourney Style Weight

## Resmî parametre

Midjourney dokümantasyonunda `--sw`:

> style reference etkisinin ağırlığını

kontrol eder.

Dokümantasyonda:

> 0–1000

aralığı belirtilir ve varsayılan:

> 100

olarak verilir.

## Örnek

> `editorial portrait --sref [REF] --sw 200`

Not:

> bu sayı başka modeller için genel “style strength” parametresi değildir.

Yalnız ilgili Midjourney kullanım bağlamında değerlendirilmelidir.

---

# 2013. `/style-reference` — Modelden Bağımsız Stil Referansı Kavramı

## Türkçe

> Reference A'yı yalnız:
>
> - color,
> - texture,
> - medium,
> - lighting,
> - composition rhythm
>
> için style reference olarak kullan.
>
> A'daki kişi, nesne, logo ve metni yeni görsele taşıma.
>
> Yeni subject [B] olsun.

## English

> Use Reference A only for color, texture, medium, lighting, and compositional rhythm as a style reference.
>
> Do not transfer its subject, objects, logos, or text.
>
> Keep [B] as the new subject.

## Neye dikkat edilmeli?

Referansın görevi (kimlik, stil, nesne) promptta adıyla yazılsın; stil referansındaki kişi kimliğe karışmasın ([§2014](#sec-2014)).

---
<a id="sec-2014"></a>
# 2014. `/identity-reference` — Stil Değil Kimlik Referansı

## Türkçe

> Reference A yalnız kişinin/karakterin identity source'u olsun.
>
> Reference A'nın:
>
> - background,
> - light,
> - outfit,
> - pose,
> - visual style
>
> özelliklerini taşıma.
>
> Sadece kimliği koru.

## English

> Use Reference A only as the identity source.
>
> Do not inherit its background, lighting, outfit, pose, or visual style.
>
> Preserve identity only.

## Neye dikkat edilmeli?

Referansın görevi (kimlik, stil, nesne) promptta adıyla yazılsın; stil referansındaki kişi kimliğe karışmasın ([§2014](#sec-2014)).

---
# 2015. `/object-reference` — Nesne Geometrisi Referansı

## Türkçe

> Reference A'daki [ÜRÜN/NESNE]'nin form, oran, parça ve ayırt edici geometry'sini koru.
>
> Background ve visual style değişebilir.
>
> Ürünü “iyileştirmek” için sessizce yeniden tasarlama.

## English

> Preserve the form, proportions, parts, and distinctive geometry of [PRODUCT/OBJECT] from Reference A.
>
> Background and visual style may change.
>
> Do not silently redesign the product.

## Neye dikkat edilmeli?

Referansın görevi (kimlik, stil, nesne) promptta adıyla yazılsın; stil referansındaki kişi kimliğe karışmasın ([§2014](#sec-2014)).

---
<a id="sec-2016"></a>
# 2016. `/reference-role-map` — Referansların Görevini Açık Yaz

## Örnek

> Reference A → face identity  
> Reference B → outfit  
> Reference C → pose  
> Reference D → visual style

Böylece modelin:

> her referanstan her şeyi karıştırması

azaltılabilir.

*Benzer: [§1006](30-katalog-aile-009-016.md#sec-1006) — kullanım alanlarıyla geniş sürüm.*

---

# 2017. `/preserve-change` — “Neyi Koru / Neyi Değiştir?” Prompt Kalıbı

2026 Nano Banana prompt rehberlerinde güçlü ortak tekniklerden biri:

> **değişecek alanı ve korunacak alanı ayrı yazmak.**

## Türkçe

> KORU:
>
> - [kimlik/form/ürün/geometri]
>
> DEĞİŞTİR:
>
> - [background/outfit/material/style]
>
> DOKUNMA:
>
> - [logo/text/facial feature]
>
> ÇIKTI:
>
> - [format/aspect/composition]

## English

> PRESERVE:
>
> - [identity/form/product/geometry]
>
> CHANGE:
>
> - [background/outfit/material/style]
>
> DO NOT ALTER:
>
> - [logo/text/facial feature]
>
> OUTPUT:
>
> - [format/aspect/composition]

## Neye dikkat edilmeli?

Referansın görevi (kimlik, stil, nesne) promptta adıyla yazılsın; stil referansındaki kişi kimliğe karışmasın ([§2014](#sec-2014)).

---
<a id="sec-2018"></a>
# 2018. `/one-change-at-a-time` — Tek Değişiklikle İterasyon

## Türkçe

> Kaynak görselde yalnız [TEK DEĞİŞİKLİK] yap.
>
> Başka hiçbir öğeyi değiştirme.
>
> Sonuç onaylandıktan sonra ikinci edit ayrı promptla yapılır.

## English

> Make only [ONE SPECIFIC CHANGE] to the source image.
>
> Do not alter anything else.
>
> Apply any second edit in a separate iteration after the first is approved.

## Neye dikkat edilmeli?

Referansın görevi (kimlik, stil, nesne) promptta adıyla yazılsın; stil referansındaki kişi kimliğe karışmasın ([§2014](#sec-2014)).

---
# 2019. `/change-only-background` — Yalnız Arka Plan

## Türkçe

> Kaynak kişi/ürün tamamen aynı kalsın.
>
> Yalnız background'u [YENİ BACKGROUND] ile değiştir.
>
> Subject'ta:
>
> - face,
> - hair,
> - clothing,
> - pose,
> - proportions
>
> değişmesin.
>
> Yeni background light'ıyla fiziksel uyum için yalnız gerekli doğal ışık entegrasyonu yapılabilir.

## English

> Keep the source person or product unchanged and replace only the background with [NEW BACKGROUND].
>
> Do not change face, hair, clothing, pose, or proportions.
>
> Allow only the minimal natural lighting integration necessary for physical coherence.

## Neye dikkat edilmeli?

Referansın görevi (kimlik, stil, nesne) promptta adıyla yazılsın; stil referansındaki kişi kimliğe karışmasın ([§2014](#sec-2014)).

---
# 2020. `/change-only-outfit` — Yalnız Kıyafet

## Türkçe

> Aynı kişi, yüz, saç, poz, background ve light korunsun.
>
> Yalnız outfit [YENİ KIYAFET] ile değişsin.
>
> Beden oranını kıyafete göre yeniden şekillendirme.

## English

> Preserve the same person, face, hair, pose, background, and lighting.
>
> Change only the outfit to [NEW OUTFIT].
>
> Do not reshape the body to suit the clothing.

## Neye dikkat edilmeli?

Referansın görevi (kimlik, stil, nesne) promptta adıyla yazılsın; stil referansındaki kişi kimliğe karışmasın ([§2014](#sec-2014)).

---
# 2021. `/change-only-material` — Yalnız Malzeme

## Türkçe

> Kaynak nesnenin geometry, scale ve bütün parça sınırlarını koru.
>
> Yalnız surface/material'ı [YENİ MALZEME] yap.
>
> Malzemenin:
>
> - roughness,
> - reflectivity,
> - thickness,
> - edge behavior
>
> fiziksel olarak yeni materyale uysun.
>
> Formu değiştirme.

## English

> Preserve the source object’s geometry, scale, and all component boundaries.
>
> Change only the surface material to [NEW MATERIAL].
>
> Make roughness, reflectivity, thickness, and edge behavior physically consistent with the new material.
>
> Do not alter form.

## Neye dikkat edilmeli?

Referansın görevi (kimlik, stil, nesne) promptta adıyla yazılsın; stil referansındaki kişi kimliğe karışmasın ([§2014](#sec-2014)).

---
# 2022. `/reference-slop-filter` — Reference Prompt AI Slop Filtresi

Kaçınılması gerekenler:

- identity ref'ten outfit kopyalamak,
- style ref'ten subject kopyalamak,
- “100% face match”i gerçek API parametresi sanmak,
- ağırlık sayılarını bütün modellere genellemek,
- aynı anda 8 referans kullanıp rol vermemek,
- source image'de istemeden background değiştirmek,
- “style” derken logo/metin de taşımak.

---

# 2023. Gerçek Sözdizimi / Topluluk Sözdizimi / Rehber Sözdizimi Tablosu

| Yazım | Tür | Örnek | Nasıl yorumlanmalı? |
|---|---|---|---|
| `/lego` | topluluk / rehber shorthand | `/lego` | resmî evrensel komut değil |
| `/figurine` | rehber shorthand | `/figurine` | uzun promptun kısa etiketi |
| `/expression-grid` | rehber shorthand | `/expression-grid` | preset mantığı |
| `--sref` | resmî Midjourney parametresi | `--sref URL` | gerçek ürün syntax'ı |
| `--sw` | resmî Midjourney parametresi | `--sw 200` | gerçek style-weight parametresi |
| doğal dil | ChatGPT/Gemini ana kullanım | `turn this photo into a pencil drawing` | belgelenmiş doğal dil yaklaşımı |

Bu tablo rehberin merkezinde tekrar tekrar hatırlatılmalıdır.

---

# 2024. Yeni üst aile: `Viral Grid Visual`

Aile:

- `/3x3-grid`
- `/expression-grid`
- `/outfit-grid`
- `/pose-grid`
- `/camera-angle-grid`
- `/hairstyle-grid`
- `/look-grid`
- `/character-sheet-grid`

Ana kural:

> **grid karşılaştırma aracıdır; her hücrede her şeyi değiştirme.**

---

# 2025. Yeni üst aile: `Viral Asset Pack`

Aile:

- `/sticker-sheet`
- `/face-sticker-16`
- `/reaction-stickers`
- `/messaging-sticker-pack`
- `/bag-catch-item-stickers`
- `/custom-cursor-sheet`
- `/pixel-sheet`

Ana fikir:

> tek “güzel görsel” yerine **tekrar kullanılabilir asset seti**.

---

# 2026. Yeni üst aile: `Impossible Personal Photo`

Aile:

- `/childhood-meets-adult`
- `/adult-child-tea-party`
- `/then-now-split`
- `/childhood-recreation`

Ana etik kural:

> **imagined composite ≠ recovered memory.**

---

# 2027. Yeni üst aile: `Professional Portrait Transformation`

Aile:

- `/professional-headshot`
- `/corporate-headshot`
- `/creative-headshot`
- `/outdoor-headshot`
- `/profile-photo-crop`

Ana kural:

> **presentation changes; identity does not.**

---

# 2028. Yeni üst aile: `Medium-name Prompting`

Aile:

- `/pencil-sketch`
- `/ballpoint-sketch`
- `/block-print`
- `/paint-by-numbers`
- `/risograph`
- `/cyanotype`
- `/screenprint-two-color`
- `/letterpress`

Ana fikir:

> Yerleşik medium adı, “artistic / beautiful / creative” gibi genel sıfatlardan çok daha belirgin sonuç üretebilir.

---

# 2029. `/core-trend-test` — Yeni Terim Ana Rehbere Girmeli mi?

Bundan sonraki genişletmeler için hızlı test:

Bir terim şu dört koşuldan en az üçünü karşılamalı:

1. **Doğrudan belirgin bir görsel sonuç üretiyor mu?**
2. **İnternette prompt/preset/trend olarak gerçekten kullanılıyor mu?**
3. **Kullanıcı tek satırda anlayıp yeniden kullanabilir mi?**
4. **Türkçe + İngilizce genişletilmiş prompta dönüştürülebiliyor mu?**

Karşılamıyorsa:

> ana rehber yerine ileri/uzmanlık eki.

Bu kontrol, rehberin yeniden görsel prompt rehberi ekseninde kalmasını sağlar.

---

# 2030. Bu turdaki çekirdek slash-style indeks (aile-043)

| Kısayol / Parametre | Sonuç |
|---|---|
| `/3x3-grid` | nine-panel consistent subject grid |
| `/expression-grid` | same face, different expressions |
| `/outfit-grid` | same subject, outfit comparison |
| `/pose-grid` | same subject, pose comparison |
| `/camera-angle-grid` | viewpoint comparison |
| `/hairstyle-grid` | hairstyle variations |
| `/look-grid` | complete styling variations |
| `/character-sheet-grid` | character consistency board |
| `/grid-variable-lock` | one main variable at a time |
| `/sticker-sheet` | reusable sticker asset sheet |
| `/face-sticker-16` | 16-expression selfie sticker pack |
| `/reaction-stickers` | messaging reactions |
| `/messaging-sticker-pack` | use-case-based sticker system |
| `/sticker-cutline` | sticker production boundary |
| `/childhood-meets-adult` | adult + younger self composite |
| `/adult-child-tea-party` | Google-style younger-self scene |
| `/then-now-split` | childhood / present comparison |
| `/then-now-aligned-face` | aligned age comparison |
| `/childhood-recreation` | modern recreation of old photo |
| `/imagined-memory-label` | composite disclosure |
| `/professional-headshot` | clean professional portrait |
| `/corporate-headshot` | restrained corporate portrait |
| `/creative-headshot` | creative-professional portrait |
| `/outdoor-headshot` | natural-light profile portrait |
| `/profile-photo-crop` | thumbnail-safe crop |
| `/headshot-identity-lock` | preserve real facial identity |
| `/pencil-sketch` | graphite medium transformation |
| `/ballpoint-sketch` | ballpoint pen medium |
| `/pen-line-portrait` | black-ink portrait |
| `/block-print` | carved print language |
| `/paint-by-numbers` | numbered painting template |
| `/photo-to-line-art` | structural line extraction |
| `/sketchbook-page` | multiple real drawing studies |
| `/photo-restoration` | source-preserving repair |
| `/scratch-repair` | damage-only restoration |
| `/fade-recovery` | tonal recovery |
| `/old-photo-colorize` | interpreted colorization |
| `/face-restoration-lock` | preserve face during restoration |
| `/restoration-pair` | source vs restored |
| `--sref` | official Midjourney style-reference parameter |
| `--sw` | official Midjourney style-weight parameter |
| `/style-reference` | model-independent style-ref concept |
| `/identity-reference` | identity-only reference |
| `/object-reference` | product/object geometry reference |
| `/reference-role-map` | assign each reference one job |
| `/preserve-change` | preserve/change/do-not-alter structure |
| `/one-change-at-a-time` | controlled iterative editing |
| `/change-only-background` | background-only edit |
| `/change-only-outfit` | outfit-only edit |
| `/change-only-material` | material-only transformation |
| `/core-trend-test` | keep main guide on-scope |

## Bu turdaki ana kaynak sinyalleri

- Google Gemini — Nano Banana image-edit examples  
  https://blog.google/products-and-platforms/products/gemini/gemini-nano-banana-examples/
- Google — personalized image creation with Nano Banana  
  https://blog.google/innovation-and-ai/products/gemini-app/personal-intelligence-nano-banana/
- Midjourney — Style Reference (`--sref`, `--sw`)  
  https://docs.midjourney.com/hc/en-us/articles/32180011136653-Style-Reference
- Midjourney — Art of Prompting / medium names  
  https://docs.midjourney.com/hc/en-us/articles/32835253061645-Art-of-Prompting
- Miraflow — 2026 face sticker-sheet prompt trend  
  https://miraflow.ai/blog/ai-face-sticker-sheet-prompts-2026
- Sweet Prompt — 2026 3×3 identity/editorial grids  
  https://sweetprompt.com/nano-banana-pro-prompt-photorealistic-3x3-editorial-dance-grid
- AI Academy — August 2026 Gemini prompt library  
  https://academy.techpresso.co/prompts/gemini-image-prompts
- GetVivix — 2026 Nano Banana editing prompt patterns  
  https://getvivix.com/blog/nano-banana-prompts
- TechRepublic — 2026 viral AI photo-edit trends  
  https://www.techrepublic.com/article/news-ai-photo-editing-trends-2026/

---
