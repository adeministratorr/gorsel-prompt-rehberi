> [← Genel İçindekiler](gorsel-prompt-rehberi.md) · [Süleyman’a Umut Ol — Dayanışma Çağrısı](gorsel-prompt-rehberi.md#suleymana-umut-ol)

<a id="sec-891"></a>
# 891. Bu tur için slash-style kısa adlar

Bunlar yine rehber içi takma adlardır; resmî ChatGPT slash komutları değildir.

Kısayollar üç biçimde karşınıza çıkar: **tam preset** (kendi numaralı bölümü ve TR+EN açılımı olan, örn. `/lego` [§892](#sec-892)), **aile öneki** (sonek varyantlarla veya ölçüyle birlikte kullanılan, örn. `/editorial-split-paper-cut` [§900](#sec-900)–907 ya da `/editorial-split 60/40`), ve **indeks kelimesi** (tur indeks tablolarındaki varyant adları; bağımsız bölümü yoksa ailenin genel formülü ve kısıt cümleleriyle doğrudan kullanılır).

| Kısayol | Prompt ailesi |
|---|---|
| `/direct-flash` | direct-flash snapshot portrait |
| `/party-snapshot` | casual party snapshot |
| `/connection` | genuine interaction portrait |
| `/motion-portrait` | motion-blur portrait |
| `/fisheye` | fisheye casual portrait |
| `/mirror` | mirror portrait |
| `/reflection` | glass reflection portrait |
| `/scanography` | scanner portrait |
| `/xerox-portrait` | photocopied portrait |
| `/contact-sheet` | portrait contact sheet |
| `/real-skin` | natural-skin beauty portrait |
| `/sensory-closeup` | sensory extreme close-up |
| `/editorial-crop` | editorial portrait crop |
| `/street-style` | street-style candid |
| `/outfit-formula` | outfit formula |
| `/capsule-wardrobe` | capsule wardrobe board |
| `/exploded-outfit` | outfit component breakdown |
| `/fabric-swatches` | fabric swatch board |
| `/garment-breakdown` | garment construction breakdown |
| `/reading-nook` | personalized reading nook |
| `/closet-nook` | closet reading nook |
| `/micro-makeover` | same-camera before/after interior |
| `/moody-blue` | moody-blue interior |
| `/vintage-pink` | vintage-pink kitchen |
| `/grandma-kitchen` | collected vintage kitchen |
| `/dark-cottage` | dark cottage kitchen |
| `/warm-wood` | warm wood interior |
| `/material-board` | interior material board |
| `/lived-in-shelf` | naturally collected shelf |
| `/product-macro` | tactile product macro |
| `/used-product` | used-but-cared-for product |
| `/mono-material` | mono-material product world |
| `/pulp-pack` | molded pulp packaging |
| `/mono-pack` | mono-material packaging |
| `/second-life-pack` | reusable packaging |
| `/peel-reveal` | peel-to-reveal label |
| `/local-craft` | product × local craft |
| `/blindbox-pack` | blind-box packaging system |
| `/material-anatomy` | product material anatomy |
| `/type-cover` | type-led album cover |
| `/found-photo` | found-photo album cover |
| `/scan-cover` | scanography cover |
| `/cassette` | cassette J-card |
| `/cd-jewel` | CD jewel-case design |
| `/vinyl` | vinyl sleeve system |
| `/music-ephemera` | music ephemera set |
| `/map-graphic` | map as primary graphic |
| `/contour-art` | real topographic contour art |
| `/route-memory` | journey route memory print |
| `/year-routes` | year-in-routes map |
| `/data-object` | data represented by physical objects |
| `/object-count` | repeated-object data visual |
| `/matched-pair` | locked-camera before/after |
| `/identity-grid` | same-person style grid |
| `/material-grid` | same-object material comparison |

---

<a id="aile-009"></a>
# ChatGPT’te `/lego` Gibi Kullanımlar: Resmî Komut mu, Topluluk Kısayolu mu?

Bu noktayı rehberde kesinleştirmek gerekir.

ChatGPT’nin güncel resmî görsel kullanımında temel yöntem **doğal dille ne istediğini tarif etmektir**. Görsel yüklenir ve yapılması istenen değişiklik yazılır. ChatGPT’nin bazı uygulama sürümlerinde slash (`/`) menüsü veya slash ile çağrılan uygulama işlevleri bulunmuş olsa da:

> `/lego`, `/doodle`, `/cutaway`, `/figurine`, `/postcard`

gibi kelimeler ChatGPT’nin belgelenmiş evrensel, resmî görsel komut sözlüğü değildir.

İnternette bu biçimin kullanılmasının nedeni çoğunlukla üç şeydir:

1. **Kısayol gibi görünmesi:** Kullanıcı uzun prompt ailesini tek kelimeyle hatırlar.
2. **Prompt koleksiyonlarını düzenlemek:** `/lego`, `/clay`, `/editorial-split` gibi etiketler başlık görevi görür.
3. **Özel GPT / özel talimat sistemi:** Bir kişi kendi GPT’sinde `/lego` yazıldığında önceden tanımladığı uzun promptu çalıştırabilir.

Bu nedenle rehberde slash biçimini kullanabiliriz; fakat başında açıkça şu not bulunmalıdır:

> **Bu kısayollar ChatGPT’nin resmî komutları değildir. Rehber içi mnemonic/preset adlarıdır.**

---

<a id="sec-892"></a>
# 892. `/lego` — Brick-built Transformation

## Kısa kullanım

> `/lego`

## Rehberde açılımı

> Verilen özneyi birbirine geçen oyuncak yapı bloklarından fiziksel olarak kurulmuş bir modele dönüştür. Ana siluet, renk dağılımı ve tanınabilir özellikler korunsun. Yapı gerçek blok geometrisiyle kurulabilir görünsün; yalnızca yüzeye blok dokusu kaplama. İnsan varsa minifigure benzeri sadeleştirilmiş oranlar kullanılabilir ancak kimlik işaretleri korunmalı.

## English

> Transform the subject into a physically buildable model made from interlocking toy bricks. Preserve the main silhouette, color distribution, and recognizable features. Make the geometry look genuinely assembled from bricks rather than merely applying a brick texture to the surface.

## Not

Marka adı gerekmiyorsa daha genel ifade:

> `interlocking toy bricks`
>
> `brick-built miniature`
>
> `construction-brick model`

kullanılabilir.

---

<a id="sec-893"></a>
# 893. Slash-style preset kullanma biçimi

Slash kısayolu tek başına “sihirli kelime” olarak değil, rehberde bir **preset çağrısı** gibi düşünülebilir.

### Çok kısa

> `/lego`

### Kısa kontrollü

> `/lego — keep identity, original clothing colors, desk-scale collectible`

### Referanslı

> `/lego — use the uploaded photo as identity reference, preserve pose and clothing`

### Birleşik

> `/lego + /exploded-view`

### Dönüşüm + format

> `/clay + /contact-sheet`

### Şehir örneği

> `/pocket-city — Konya, monochrome architectural miniature`

Bu gösterim rehberi kullanmayı hızlandırır; gerçek uzun prompt ise ilgili maddede bulunur.

---

# 894. Viral “Fotoğraf + Minimal El Çizimi” Editoryal Poster — Editorial Split Poster

## Trend

**TREND — Eylül 2026’da hızla yayılan promptlardan biri.**

Bu prompt ailesi son günlerde Reddit’in `r/aiArt`, `r/PromptEngineering`, `r/promptingmagic`, X/Twitter prompt paylaşım hesapları, prompt arşivleri ve seyahat/blog içeriklerinde aynı veya çok benzer metinle dolaşıyor.

Temel fikir:

> **Üst yarı = kaynak fotoğraf**
>
> **Alt yarı = aynı fotoğrafın çok sade el yapımı editoryal yorumu**

Bu bir collage değildir. Aynı hikâyenin iki farklı görsel dili üst üste kullanılır.

## Rehber kısayolu

> `/editorial-split`

Alternatif:

> `/photo-paper-dual`

---

# 895. İnternette dolaşan tam Editorial Split master prompt

Aşağıdaki sürüm, kullanıcı tarafından paylaşılan viral promptun rehber kaydıdır.

```text
Create one independent high-end editorial poster for each uploaded photo. Do not combine multiple photos into a collage. Each photo must be processed and output as a separate poster.

OVERALL FORMAT

Strict 3:4 vertical composition.

Divide the canvas horizontally into two exactly equal sections, with a precise 1:1 height ratio.

The top half occupies exactly 50% of the canvas.

The bottom half occupies exactly 50% of the canvas.

The two sections should feel visually connected as one refined art publication cover.

TOP HALF — ORIGINAL PHOTOGRAPH

Preserve the original photograph as faithfully as possible.

Keep the main composition, subjects, identity, facial features, body proportions, poses, expressions, clothing, objects, and spatial relationships unchanged.

Preserve the realistic photographic texture, natural lighting, shadows, atmosphere, and original color mood.

Apply only subtle, sophisticated editorial color grading, creating the feeling of a premium magazine photograph, contemporary art book, or high-end independent publication.

The image should remain photorealistic and authentic, never overly retouched or artificially stylized.

If necessary to fit the 3:4 composition naturally, extend the sky, ground, walls, or surrounding environmental background.

Background extension must feel seamless and photographic.

Never stretch, distort, reshape, replace, or alter the main subject.

BOTTOM HALF — MINIMAL HAND-DRAWN PAPER ILLUSTRATION

Extract the most recognizable visual elements from the original photograph and reinterpret them as a minimalist hand-drawn paper-cover illustration.

Preserve:

The most recognizable subject

Essential silhouette and proportions

Key pose or gesture

Important objects

The core narrative relationship between people and objects

Highly simplify the image. Remove unnecessary details and retain only the visual information needed for immediate recognition.

Use:

Delicate, slightly imperfect hand-drawn lines

A small number of bold, clearly defined acrylic-style flat color shapes

Rough paper texture

Visible handmade brush marks

Slightly irregular, organic edges

Subtle imperfections that make it feel genuinely handmade

The main illustrated subject should be small, centered, and carefully composed, occupying approximately 10–20% of the bottom half.

Leave a large amount of negative space around the illustration.

The background should primarily resemble:

Rough white paper

Warm off-white paper

Pale natural paper

Minimal editorial book-cover stock

Use only a few lines or small color shapes to suggest the surrounding environment.

COLOR PALETTE

Extract the dominant colors directly from the original photograph.

Compress the palette into no more than 4 main colors.

Keep the colors restrained, sophisticated, and harmonious.

Use bold but controlled flat color blocks.

Avoid excessive color variation.

Preserve subtle paper grain and handmade brush texture.

The illustration should visually feel like a simplified color interpretation of the photograph.

TYPOGRAPHY

A small amount of simple typography may be included when appropriate.

Possible elements:

A short title

Keyword

Object name

Location

Year

Number

Short phrase

Text should be minimal, understated, and editorial.

Typography should naturally interact with the large areas of negative space and the small illustration, evoking:

Art book covers

Independent publishing

Contemporary editorial design

Thoughtful children's picture books

Do not force text into the composition if it does not naturally fit the photograph.

VISUAL LANGUAGE

The final poster should feel:

Quiet · Poetic · Refined · Minimal · Innocent · Relaxed · Artistic · Thoughtful · High-recognition · Premium

The visual concept should be:

“A small subject surrounded by a large amount of empty space.”

The result should resemble a carefully designed independent art publication cover, rather than a commercial advertisement.

AVOID

Do not use:

Colored-pencil aesthetics

Crayon textures

Bleeding watercolor

Pure line-art illustration

Complex realistic illustration

Heavy oil-painting effects

Smooth polished digital illustration

3D rendering

Glossy 3D textures

Commercial cartoon aesthetics

Cute commercial character design

E-commerce advertising aesthetics

Generic poster templates

Excessive decorative elements

Busy compositions

Excessive typography

FINAL ART DIRECTION

The top half should feel like a beautiful, authentic editorial photograph.

The bottom half should feel like a small, handmade visual poem derived from that photograph.

The two halves should clearly belong to the same visual story, while maintaining a strong contrast between photographic realism above and minimal handmade illustration below.

Prioritize recognition, restraint, negative space, material texture, subtle imperfection, editorial sophistication, and artistic storytelling over decorative complexity.
```

---

# 896. Editorial Split promptunun neden iyi çalıştığı

Bu promptu değerli yapan yalnızca uzun olması değildir. Birkaç doğru kontrolü aynı anda kurar:

### 1. Bilgi mimarisi açık

> `top 50% photo / bottom 50% illustration`

Modelin “poster” kelimesini rastgele yorumlamasını azaltır.

### 2. Kaynak koruma açık

Kimlik, poz, kıyafet, nesne ve mekânsal ilişki ayrı ayrı korunur.

### 3. Stil dönüşümü alt bölgeyle sınırlandırılır

Tüm fotoğrafın illüstrasyona dönüşmesi engellenmeye çalışılır.

### 4. “Minimal” ölçülebilir hâle gelir

> `subject occupies approximately 10–20%`
>
> `large amount of negative space`

### 5. Renk ilişkisi kurulmuştur

Alt bölümün paleti kaynak fotoğraftan türetilir.

### 6. Negatif prompt yalnız “kötü şeyler” listesi değildir

İstenen editoryal dilin karşıtı olan görsel aileler dışlanır.

---

# 897. Editorial Split promptunda gereksiz tekrarlar

Viral prompt güçlü olsa da bazı bölümleri sıkıştırılabilir.

Örneğin:

> `top half occupies exactly 50%`
>
> `bottom half occupies exactly 50%`
>
> `divide ... exactly equal`
>
> `precise 1:1 height ratio`

aynı kuralın farklı tekrarlarıdır.

Aynı şekilde “quiet / poetic / refined...” gibi uzun sıfat zincirleri tek başına görsel kontrol sağlamaz.

Daha kısa sürümde korunması gereken temel çekirdek:

> **layout + source preservation + lower-half transformation + subject scale + negative space + palette extraction + paper/paint behavior + avoid list**

---

# 898. Editorial Split — Kısa kontrollü sürüm

## Türkçe

> `/editorial-split`
>
> Yüklediğim her fotoğraf için ayrı bir 3:4 dikey editoryal poster oluştur; fotoğrafları kolajda birleştirme.
>
> Tuvali yatay olarak tam iki eşit bölüme ayır.
>
> **Üst %50:** Kaynak fotoğrafı mümkün olduğunca aynen koru. Kimlik, yüz, vücut oranı, poz, kıyafet, nesneler, ışık ve mekânsal ilişkileri değiştirme. Yalnızca çok hafif bağımsız sanat yayını düzeyinde color grading uygula. Kadraja uyum için gerekiyorsa yalnız çevresel arka planı doğal biçimde genişlet.
>
> **Alt %50:** Aynı sahnenin en tanınabilir öznesini çok sade el yapımı kâğıt illüstrasyonuna dönüştür. Hafif kusurlu ince çizgi, 3–4 düz akrilik renk şekli, görünür fırça izi ve kırık beyaz kaba kâğıt kullan. Ana illüstrasyon alt bölümün yaklaşık %10–20'sini kaplasın ve büyük negatif alan içinde küçük, merkezlenmiş kalsın.
>
> Alt bölümün 4 renkten fazla olmayan paletini üst fotoğraftan çıkar.
>
> Tipografi yalnız gerekliyse bir kısa başlık/yer/yıl ile sınırlı olsun.
>
> Crayon, colored pencil, watercolor bleed, glossy digital illustration, 3D, commercial cartoon, generic poster template, yoğun dekor ve fazla yazı kullanma.

## English compact version

> `/editorial-split`
>
> Create one separate 3:4 editorial poster for each uploaded photo; never combine photos into a collage.
>
> Split the canvas horizontally into equal 50/50 halves.
>
> **Top:** preserve the source photograph faithfully—identity, face, proportions, pose, clothing, objects, lighting, and spatial relationships unchanged. Apply only subtle independent-publication color grading. Extend environmental background only if needed for framing.
>
> **Bottom:** reinterpret the most recognizable subject as a very small handmade paper illustration using slightly imperfect fine lines, 3–4 flat acrylic color shapes, visible brush marks, and rough warm-white paper. Keep the illustration centered and only about 10–20% of the lower half, surrounded by generous negative space.
>
> Derive the lower palette from the source photograph. Use minimal typography only when useful.
>
> Avoid crayon, colored pencil, bleeding watercolor, polished digital illustration, 3D, commercial cartoon styling, generic poster templates, decorative clutter, and excessive text.

---

# 899. `/editorial-split-isometric` — Photo + Tiny Isometric Scene

## Trend

Viral master promptun ilk görülen remixlerinden biri.

## Türkçe prompt

> Üst %50 kaynak fotoğraf olarak kalsın. Alt %50'de aynı fotoğrafın ana sahnesini çok küçük izometrik paper-model / display-scene olarak yeniden kur. Alt sahne geniş manzara değil, küçük masaüstü sergi maketi gibi olsun. Fotoğraftan alınan 3–4 ana renk kullan ve çevresinde geniş negatif alan bırak.

## English

> Keep the top 50% as the source photograph. In the lower 50%, rebuild the main scene as a very small isometric paper-model or display scene. Treat it as a tiny desktop exhibit rather than a wide landscape. Use 3–4 main colors derived from the photograph and preserve generous negative space.

---

<a id="sec-900"></a>
# 900. `/editorial-split-paper-cut` — Photo + Paper-cut

## Türkçe prompt

> Üst yarıda kaynak fotoğrafı koru. Alt yarıda aynı özneyi 4–6 büyük kesilmiş kâğıt şekliyle çok sade paper-cut illüstrasyona dönüştür. Katmanlar arasında çok hafif gerçek temas gölgesi ve kâğıt kalınlığı görülsün. Ana figür küçük kalsın; paper-craft diorama kadar hacimli yapma.

## English

> Preserve the source photograph in the top half. In the lower half, reduce the same subject to a very small paper-cut illustration built from 4–6 large cut-paper shapes. Show subtle real paper thickness and contact shadows. Keep the figure small and avoid turning it into a full paper-craft diorama.

## Neye dikkat edilmeli?

Alt yarıdaki yorum, üstteki kişinin kimliğini ve giysisini değiştirmesin; iki yarıyı ayıran çizginin tam ortada ve düz olduğunu kontrol edin. Alt bölümdeki medium dokusu (kâğıt kalınlığı, toner, registration kayması) abartılırsa portre karikatüre kayar.

---
# 901. `/editorial-split-riso` — Photo + Risograph Interpretation

## Türkçe prompt

> Üst yarı gerçek fotoğraf, alt yarı aynı öznenin iki spot renkli risograph yorumu olsun. Alt görsel küçük, sade ve geniş negatif alan içinde kalsın. Hafif registration kayması yalnız alt illüstrasyonda kullanılsın.

## English

> Keep the top half photographic and reinterpret the same subject in the lower half as a small two-spot-color risograph illustration. Preserve generous negative space and use slight registration misalignment only in the lower artwork.

## Neye dikkat edilmeli?

Alt yarıdaki yorum, üstteki kişinin kimliğini ve giysisini değiştirmesin; iki yarıyı ayıran çizginin tam ortada ve düz olduğunu kontrol edin. Alt bölümdeki medium dokusu (kâğıt kalınlığı, toner, registration kayması) abartılırsa portre karikatüre kayar.

---
# 902. `/editorial-split-xerox` — Photo + Xerox Zine

## Türkçe prompt

> Üst yarıda doğal fotoğrafı koru. Alt yarıda aynı özneyi küçük siyah-beyaz xerox/fanzin görüntüsüne dönüştür. Yüksek kontrast ve toner dokusu kullan ancak alt kısmı sticker ve metin kolajına dönüştürme.

## English

> Preserve the natural photograph in the upper half. Turn the same subject into a small black-and-white Xerox/zine interpretation in the lower half. Use high contrast and toner texture while avoiding sticker and text clutter.

## Neye dikkat edilmeli?

Alt yarıdaki yorum, üstteki kişinin kimliğini ve giysisini değiştirmesin; iki yarıyı ayıran çizginin tam ortada ve düz olduğunu kontrol edin. Alt bölümdeki medium dokusu (kâğıt kalınlığı, toner, registration kayması) abartılırsa portre karikatüre kayar.

---
# 903. `/editorial-split-linocut` — Photo + Linocut

## Türkçe prompt

> Alt yarıdaki özneyi tek veya iki renkli küçük linocut baskıya dönüştür. Oyma izleri ve baskı basıncı hissi görülsün; detaylar güçlü silhouette için sadeleşsin.

## English

> Reinterpret the lower subject as a small one- or two-color linocut print. Show carving marks and physical print-pressure character while simplifying details into a strong recognizable silhouette.

## Neye dikkat edilmeli?

Alt yarıdaki yorum, üstteki kişinin kimliğini ve giysisini değiştirmesin; iki yarıyı ayıran çizginin tam ortada ve düz olduğunu kontrol edin. Alt bölümdeki medium dokusu (kâğıt kalınlığı, toner, registration kayması) abartılırsa portre karikatüre kayar.

---
<a id="sec-904"></a>
# 904. `/editorial-split-food` — Yemek Fotoğrafı İçin Koruma Sürümü

Yemek/ürün fotoğraflarında kaynak koruma cümlesi özellikle önemlidir.

## Türkçe ek

> Yemeğin türünü, porsiyon miktarını, malzeme sayısını, servis kabını, garnish'leri ve tabak içindeki konumlarını değiştirme. Alt illüstrasyonda da aynı temel yiyecek yapısını koru; malzeme icat etme veya eksiltme.

## English add-on

> Do not change the food type, portion size, number of ingredients, serving vessel, garnishes, or their arrangement. Preserve the same essential food structure in the lower illustration; do not invent or remove ingredients.

## Neye dikkat edilmeli?

Koruma eki ana split promptun önüne aynen eklensin; kısaltılmış koruma, korumasızlıktır. Alt illüstrasyondaki malzeme sayısı üstteki fotoğrafla tek tek karşılaştırılsın.

---

# 905. `/editorial-split-product` — Ürün Fotoğrafı Sürümü

## Türkçe ek

> Ürünün marka/ürün geometrisini, parça sayısını, malzeme bitişini ve ana işlevsel ayrıntılarını değiştirme. Alt illüstrasyonda yalnız görsel dil sadeleşsin; ürün tasarımı yeniden tasarlanmasın.

## English add-on

> Preserve the product geometry, part count, material finish, and primary functional details. Simplify only the visual language in the lower illustration; do not redesign the product.

## Neye dikkat edilmeli?

Koruma eki prompta aynen eklensin; alt illüstrasyonda sadeleşen yalnız görsel dil olsun, parça sayısı ve geometri denetlensin.

---

# 906. `/editorial-split-travel` — Seyahat Fotoğrafı Sürümü

## Türkçe ek

> Landmark, sokak veya doğal oluşumun gerçek kimliğini koru. Alt illüstrasyonda yapıyı jenerik şehir simgesine dönüştürme; belirgin siluet ve coğrafi ilişki devam etsin. Küçük bir yer adı ve yıl kullanılabilir.

## English add-on

> Preserve the real identity of the landmark, street, or natural formation. Do not reduce it to a generic city symbol in the lower illustration; retain the distinctive silhouette and geographic relationship. A small place name and year may be used.

## Neye dikkat edilmeli?

Koruma eki prompta aynen eklensin; silüet ve coğrafi ilişki üst-alt iki yarıda da aynı kalsın.

---

# 907. `/editorial-split-portrait` — Portre Sürümü

## Türkçe ek

> Alt illüstrasyonda kişiyi yalnız birkaç çizgiye indirirken saç biçimi, yüzün genel oranı, gözlük/sakal gibi ayırt edici öğe, kıyafet rengi ve ana pozu koru. Sevimli karaktere veya chibi figüre dönüştürme.

## English add-on

> When simplifying the person in the lower illustration, preserve hairstyle, overall facial proportion, distinctive elements such as glasses or beard, clothing color, and primary pose. Do not turn the person into a cute or chibi character.

## Neye dikkat edilmeli?

Koruma eki prompta aynen eklensin; ayırt edici öğeler (gözlük, sakal, renk) iki yarıda da korunsun.

---

# 908. Split-poster ailesinde kompozisyon varyasyonları

Viral sürüm 50/50 yatay bölünmeyi kullanıyor. Aynı fikir başka oranlarla da çalışabilir:

### 60/40

Fotoğrafın daha baskın olması isteniyorsa.

### 40/60

Alt illüstrasyon ve negatif alan yayın kapağının ana hissi olacaksa.

### 2/3 + 1/3

Daha klasik editorial sayfa oranı.

### İnce fotoğraf şeridi + geniş kâğıt alan

Fotoğraf referans, illüstrasyon ana anlatı olduğunda.

Bu varyasyonlarda kısayol:

> `/editorial-split 60/40`

gibi yazılabilir.

---

# 909. Kamera/film dili: “film look” yerine fiziksel davranış

2026 prompt topluluklarında hâlâ `Portra`, `Kodachrome`, `Ektachrome`, `disposable camera`, `35mm`, `point-and-shoot` gibi terimler yoğun kullanılıyor.

Ancak rehberde mümkün olduğunca yalnız marka/film adı değil, onun görsel davranışı tarif edilmelidir.

Örneğin:

> `slightly warm skin, restrained highlight roll-off, subtle organic grain, gentle black fade`

gibi.

---

# 910. `/disposable-35mm` — Ucuz Tek Kullanımlık Kamera

## Türkçe

> Fotoğrafı ucuz 35mm tek kullanımlık kamerayla anlık çekilmiş gibi göster. Sabit geniş açı lens, hafif yumuşaklık, sınırlı düşük ışık performansı, sert dahili flaş, organik film grenleri ve zaman zaman küçük pozlama hatası kullan. Kusurları bütün fotoğrafı boğacak kadar abartma.

## English

> Make the image feel like an accidental snapshot from a cheap 35mm disposable camera: fixed wide lens, slight softness, limited low-light performance, harsh built-in flash, organic film grain, and occasional minor exposure error. Keep the imperfections restrained.

## Neye dikkat edilmeli?

Dönem kameranın kusurları dozunda kalsın: gren, tarih damgası ve renk kayması tek ışık mantığına uysun; her kareye aynı kusuru basmak klişeye kayar.

---
# 911. `/point-and-shoot-2000s` — Erken Dijital Kompakt Kamera

## Türkçe

> Fotoğrafı 2000'lerin başı tüketici tipi dijital kompakt kamerayla çekilmiş gibi göster. Küçük sensör, sınırlı highlight latitude, hafif dijital noise, düşük ışıkta direkt flaş, biraz aşırı sharpening ve dönem tipi JPEG karakteri kullan.

## English

> Make the photo resemble an early-2000s consumer digital point-and-shoot image: small sensor, limited highlight latitude, mild digital noise, direct flash in low light, slightly aggressive sharpening, and period-appropriate JPEG character.

## Neye dikkat edilmeli?

Dönem kameranın kusurları dozunda kalsın: gren, tarih damgası ve renk kayması tek ışık mantığına uysun; her kareye aynı kusuru basmak klişeye kayar.

---
# 912. `/film-contact-sheet` — Film Contact Sheet

## Türkçe

> Aynı çekim serisini 35mm film contact sheet üzerinde göster. Karelerin arasında film bordürü, kare numarası ve küçük pozlama farklılıkları olsun. Bir veya iki kare grease-pencil ile seçilebilir.

## English

> Show the same shoot as a 35mm film contact sheet with film borders, frame numbers, and small exposure variations. One or two frames may be selected with grease-pencil marks.

## Neye dikkat edilmeli?

Dönem kameranın kusurları dozunda kalsın: gren, tarih damgası ve renk kayması tek ışık mantığına uysun; her kareye aynı kusuru basmak klişeye kayar.

---
# 913. `/film-border` — Film Kenarlı Baskı

## Türkçe

> Fotoğrafı film çerçevesi/negatif kenarı görünen taranmış baskı gibi göster. Kenar numaraları ve film perforasyonu yalnız fiziksel olarak uygun yönde bulunsun. Sahte film metnini ana görsel öğe yapma.

## English

> Present the photo like a scan with visible film or negative borders. Keep frame numbers and perforations only where physically plausible. Do not make fake film text the main graphic element.

## Neye dikkat edilmeli?

Dönem kameranın kusurları dozunda kalsın: gren, tarih damgası ve renk kayması tek ışık mantığına uysun; her kareye aynı kusuru basmak klişeye kayar.

---
# 914. `/halation` — Analog Işık Taşması

## Not

Halation, her parlak alanın neon aura kazanması değildir.

## Türkçe

> Çok parlak küçük ışık kaynaklarının çevresinde ince sıcak film halation kullan. Etki yalnız highlight kenarlarında görülmeli; bütün sahneye kırmızı glow kaplama.

## English

> Use subtle warm film halation around small very bright light sources. Restrict the effect to highlight edges rather than covering the entire scene with a red glow.

---

# 915. `/light-leak` — Film Light Leak

## Türkçe

> Fotoğrafın yalnız bir kenarında fiziksel film sızıntısını andıran hafif turuncu/kırmızı light leak kullan. Özneyi kapatmasın ve birden fazla kenardan simetrik gelmesin.

## English

> Add one restrained orange-red light leak along a single edge, resembling a real film-loading or camera-seal leak. Keep it away from the primary subject and avoid symmetrical leaks from multiple sides.

## Neye dikkat edilmeli?

Dönem kameranın kusurları dozunda kalsın: gren, tarih damgası ve renk kayması tek ışık mantığına uysun; her kareye aynı kusuru basmak klişeye kayar.

---
# 916. `/expired-film` — Son Kullanma Tarihi Geçmiş Film

## Türkçe

> Eski film stoğuna özgü hafif renk kayması, düzensiz gren ve düşük kontrast kullan. Renk bozulması öngörülemez ama sınırlı olsun. Her kanalı neon renge çevirme.

## English

> Use subtle color shifts, irregular grain, and reduced contrast characteristic of aged film stock. Let color instability feel unpredictable but restrained. Avoid turning every color channel neon.

## Neye dikkat edilmeli?

Dönem kameranın kusurları dozunda kalsın: gren, tarih damgası ve renk kayması tek ışık mantığına uysun; her kareye aynı kusuru basmak klişeye kayar.

---
# 917. `/toy-box` — Collectible Toy Packaging

## Trend

**TREND — 2025'ten 2026'ya taşınan en güçlü viral ailelerden.**

Rehberde mevcut action-figure/blister promptlarının yanına kısa preset olarak eklenebilir.

## Türkçe

> Fotoğraftaki kişiyi gerçek mağaza ürünü gibi koleksiyon figürüne dönüştür. Figür ve 3 kişisel aksesuar şeffaf blister içinde fiziksel olarak yerleşsin. Karton arka yüz sade olsun. Kimlik, kıyafet ve kişiye gerçekten ait aksesuarlar korunsun.

## English

> Turn the person into a believable retail collectible figure with three genuinely personal accessories arranged in a clear blister package. Keep the backing card restrained and preserve identity and clothing.

---

# 918. `/designer-toy` — Designer Vinyl Figure

## Türkçe

> Özneyi küçük üretim designer vinyl art toy'a dönüştür. Sade tek ana form, mat vinil, sınırlı renk ve fiziksel kalıp mantığı kullan. Büyük kafa gerekiyorsa oranı kontrollü tut. Sahte lüks marka veya hypebeast logo ekleme.

## English

> Transform the subject into a small-production designer vinyl art toy. Use one simple primary form, matte vinyl, limited color, and plausible molded construction. If using an enlarged head, keep proportions controlled. Avoid fake luxury branding and hype logos.

## Neye dikkat edilmeli?

Figür fiziksel olarak üretilebilir görünsün: eklem yerleri, boya sınırları ve kutu ölçüleri tutarlı olsun; lisanslı karaktere benzemesin.

---
# 919. `/blind-box` — Mystery Collectible

## Türkçe

> Aynı tema içinde 6 figürlük küçük blind-box serisi tasarla. Figürler ortak ölçü, taban ve malzeme dili kullansın; her biri farklı fikir taşısın. Nadir sürümü yalnız altın/glitter yaparak ayırma.

## English

> Design a six-figure blind-box collection around one theme. Keep scale, base, and material language consistent while giving each figure a distinct concept. Do not distinguish the rare figure merely with gold or glitter.

## Neye dikkat edilmeli?

Figür fiziksel olarak üretilebilir görünsün: eklem yerleri, boya sınırları ve kutu ölçüleri tutarlı olsun; lisanslı karaktere benzemesin.

---
# 920. `/miniature-box` — Boxed Diorama

## Türkçe

> [SAHNE]'yi ön yüzü açık küçük kutu içinde fiziksel minyatür diorama olarak göster. Kutu ölçeğini gerçek nesne ölçüsüyle belirt; 3–5 ana öğe yeterli olsun. Oyuncak mağazası ambalajına dönüştürme.

## English

> Show [SCENE] as a physical miniature diorama inside a small open-front box. Specify a believable physical box size and limit the scene to 3–5 primary elements. Avoid retail toy-package styling.

## Neye dikkat edilmeli?

Figür fiziksel olarak üretilebilir görünsün: eklem yerleri, boya sınırları ve kutu ölçüleri tutarlı olsun; lisanslı karaktere benzemesin.

---
# 921. `/phone-popout` — Smartphone Pop-out Illusion

## Trend

2026 prompt paylaşım topluluklarında görülen viral fotoğraf dönüşümlerinden.

## Türkçe

> Yüklenen fotoğraftaki kişiyi büyük bir akıllı telefon ekranından fiziksel olarak dışarı adım atıyormuş gibi göster. Ekranın içindeki sahne ile dışarı çıkan gövde aynı kişi ve aynı perspektif ilişkisini korusun. Bir bacak/kol ekran düzlemini aşarken diğer bölüm hâlâ ekran içinde olabilir. İkinci bir kişi veya kopya beden üretme.

## English

> Use the uploaded person as a strict identity reference and show them physically stepping out of a large smartphone screen. Keep the person inside and outside the screen as one continuous body with consistent perspective. One limb may cross the screen plane while the remaining body is still inside. Do not create a duplicate person.

---

# 922. `/open-head-concept` — Head-as-Container Editorial

## Trend

**TREND — playful editorial surrealism.**

## Türkçe

> Gerçekçi editoryal portrede kişinin başının üst bölümünü metaforik kapak gibi aç ve içinden yalnızca [KONU]'yu temsil eden 3–5 küçük nesne/figür çıkar. Yüz ve kimlik gerçekçi kalsın. Görsel komik veya kavramsal olsun; gore, anatomi ve biyolojik doku kullanma.

## English

> In a realistic editorial portrait, open the top of the person's head metaphorically like a lid and let only 3–5 small objects or figures representing [TOPIC] emerge. Keep the face and identity realistic. Make the concept playful rather than anatomical; avoid gore and biological tissue.

---

# 923. `/exploded-architecture` — Exploded Axonometric Building

## Trend

**EVERGREEN — 2026 mimari AI promptlarında çok görünür.**

## Türkçe

> Yapının katlarını ve ana sistemlerini düşey eksen boyunca kontrollü exploded axonometric olarak ayır. Zemin, taşıyıcı sistem, katlar, cephe ve çatı gerçek yapı mantığını korusun. Katmanlar rastgele havada yüzmesin; aynı aks ve footprint üzerinde hizalansın.

## English

> Separate the building's floors and primary systems vertically in a controlled exploded axonometric. Preserve the real logic of ground plane, structure, floors, facade, and roof. Keep every layer aligned to the same axes and footprint rather than floating randomly.

---

# 924. `/architecture-collage` — Architectural Competition Collage

## Trend

**EVERGREEN / competition-board language.**

## Türkçe

> [PROJE]'yi tek ana mimari perspektif, 1–2 kesilmiş insan/bitki ölçek öğesi ve sınırlı renk bloklarıyla competition collage olarak göster. Plan, diyagram, render ve 20 etiketin hepsini aynı görsele doldurma.

## English

> Present [PROJECT] as an architectural competition collage using one primary architectural perspective, 1–2 cut-out scale figures or plants, and restrained color fields. Do not crowd the image with plans, diagrams, renders, and excessive labels.

---

# 925. `/white-model` — White Card Architectural Model

## Türkçe

> Yapıyı beyaz karton/foamboard fiziksel mimari maket gibi göster. Gerçek kesilmiş kenar, katman ve temas gölgeleri olsun. Malzeme ve renk bilgisini kaldır; yalnız kütle, açıklık ve mekânsal ilişkiyi öne çıkar.

## English

> Show the building as a physical white-card or foam-board architectural model. Preserve cut edges, layers, and real contact shadows. Remove material and color information and emphasize only massing, openings, and spatial relationships.

## Neye dikkat edilmeli?

Model dili tutarlı olsun: beyaz kartonda renkli doku, kesitte ölçüsüz açıklık olmasın; pafta yazıları ayrıca denetlenir.

---
# 926. `/material-model` — Material Architecture Model

## Türkçe

> Mimari maketi gerçek model malzemeleriyle kur: basswood, gri karton, şeffaf asetat ve küçük bitki maketleri gibi. Malzemeler gerçek fiziksel ölçeğe uygun olsun. Tam ölçekli bina renderı gibi görünmesin.

## English

> Build the architectural model visually from real model-making materials such as basswood, gray board, clear acetate, and small model vegetation. Keep material behavior consistent with physical model scale. Avoid making it look like a full-scale building render.

## Neye dikkat edilmeli?

Model dili tutarlı olsun: beyaz kartonda renkli doku, kesitte ölçüsüz açıklık olmasın; pafta yazıları ayrıca denetlenir.

---
# 927. `/section-perspective` — Section Perspective

## Türkçe

> Yapının kesilen kısmını temiz düz kesit yüzeyiyle aç ve iç mekânsal derinliği perspektifle göster. Kesilen duvar/döşemeler diğer yüzeylerden grafik olarak ayrışsın. Dollhouse görünümü ile teknik kesit mantığını karıştırma.

## English

> Cut through the building with a clean section plane while showing interior spatial depth in perspective. Distinguish cut walls and slabs graphically from surfaces seen in elevation. Do not confuse a technical section perspective with a decorative dollhouse view.

## Neye dikkat edilmeli?

Model dili tutarlı olsun: beyaz kartonda renkli doku, kesitte ölçüsüz açıklık olmasın; pafta yazıları ayrıca denetlenir.

---
# 928. `/diagrammatic-render` — Render + Diagram Hybrid

## Türkçe

> Gerçekçi mimari görüntünün üzerine yalnızca gerekli 2–4 diyagram katmanı ekle: dolaşım, güneş, rüzgâr veya program gibi. Her bilgi için farklı ama sınırlı bir kod kullan. Renderı ok, ikon ve metinle kaplama.

## English

> Add only 2–4 necessary diagram layers over a realistic architectural view, such as circulation, sun, wind, or program. Use a restrained visual code for each information type. Do not cover the render with arrows, icons, and text.

## Neye dikkat edilmeli?

Model dili tutarlı olsun: beyaz kartonda renkli doku, kesitte ölçüsüz açıklık olmasın; pafta yazıları ayrıca denetlenir.

---
# 929. `/retro-airbrush` — 1980s Airbrush Illustration

## Trend

**TREND — Ağustos 2026’da yeniden görünür.**

## Türkçe

> [ÖZNE]'yi gerçek 1980'ler airbrush illüstrasyon sürecini çağrıştıracak biçimde oluştur. Önce yumuşak püskürtülmüş ton geçişleri, ana nesnede gerektiğinde maskelenmiş sert kenarlar, sınırlı krom yansıma ve en sonda küçük glow kullan. “80s” diye yalnız mor-mavi neon gradient ekleme.

## English

> Render [SUBJECT] using the logic of real 1980s airbrush illustration: soft sprayed tonal transitions first, masked hard edges where needed on the focal object, restrained chrome reflection, and only small final glow accents. Do not create “80s” style by adding only purple-blue neon gradients.

---

# 930. `/chrome-airbrush` — Chrome Airbrush Graphic

## Türkçe

> Tek ana [NESNE/KELİME]'yi airbrush ile resmedilmiş krom yüzey gibi göster. Kromda çevre yansımaları belirli ve geometrik olsun; kenarlar maskelenmiş keskin, geçişler püskürtülmüş yumuşak olsun. Her yüzeyi krom yapma.

## English

> Render one primary [OBJECT/WORD] as airbrushed chrome. Keep environmental reflections deliberate and geometric, with masked hard edges and soft sprayed transitions. Do not make every surface chrome.

## Neye dikkat edilmeli?

Harita ve grafik öğelerde yer adları ve sınırlar gerçek veriyle karşılaştırılır; süsleme bilgiyi gölgeliyorsa öğe çıkarılır.

---
# 931. `/y2k-product` — Y2K Consumer-tech Object

## Trend

**TREND — retro-futurism.**

## Türkçe

> [ÜRÜN]'ü 1998–2004 tüketici elektroniği tasarım dilinde yeniden yorumla: yarı saydam renkli plastik, yuvarlatılmış gövde, küçük LCD/LED ayrıntısı ve fiziksel düğmeler kullan. İnce modern smartphone minimalizmi veya cyberpunk neon ekleme.

## English

> Reinterpret [PRODUCT] through 1998–2004 consumer-electronics design language using translucent colored plastic, rounded casing, a small LCD or LED detail, and physical buttons. Avoid thin modern smartphone minimalism and cyberpunk neon.

---

# 932. `/cassette-futurism` — Analog Retro-futurist Object

## Türkçe

> Gelecekten gelen bir [CİHAZ]'ı 1980–1990'ların analog elektronik üretim mantığıyla tasarla: kaset/slider/düğme/segment display gibi fiziksel kontrol elemanları kullan. “Gelecek” hissini hologramla değil mekanik-elektronik tasarımla kur.

## English

> Design a futuristic [DEVICE] through 1980s–1990s analog-electronics logic using physical controls such as cassette slots, sliders, buttons, and segmented displays. Build futurism through mechanical-electronic design rather than holograms.

## Neye dikkat edilmeli?

Harita ve grafik öğelerde yer adları ve sınırlar gerçek veriyle karşılaştırılır; süsleme bilgiyi gölgeliyorsa öğe çıkarılır.

---
# 933. `/tattoo-flash` — Tattoo Flash Sheet

## Trend

**EVERGREEN / prompt kütüphanelerinde güçlü.**

## Türkçe

> [TEMA] için 9 parçalık cohesive tattoo flash sheet oluştur. Her motif ayrı, beyaz zeminde, benzer line weight ve shading tekniğinde olsun. Stil: [traditional / blackwork / fine line / engraving / botanical]. Motifleri birbirine değdirme. Anatomik yerleşim veya gerçek cilt üzerinde mockup istemiyorsam yalnız flash sheet göster.

## English

> Create a cohesive nine-piece tattoo flash sheet around [THEME]. Keep every motif separate on a white background with consistent line weight and shading technique. Style: [traditional / blackwork / fine line / engraving / botanical]. Do not overlap motifs. Show only the flash sheet unless skin-placement mockups are explicitly requested.

---

# 934. `/patch-sheet` — Embroidered Patch Sheet

## Türkçe

> [TEMA] için 6 farklı işlemeli patch'i tek collection sheet üzerinde göster. Her patch fiziksel kumaş kenarı, iplik yönü ve gerçek nakış yoğunluğu taşısın. Tasarımlar ortak ailede olsun ancak aynı dış şekli tekrar etmesin.

## English

> Show six different embroidered patches around [THEME] on one collection sheet. Give each patch physical fabric edging, visible thread direction, and believable stitch density. Keep the designs cohesive without repeating one outer shape.

## Neye dikkat edilmeli?

Harita ve grafik öğelerde yer adları ve sınırlar gerçek veriyle karşılaştırılır; süsleme bilgiyi gölgeliyorsa öğe çıkarılır.

---
# 935. `/crest` — Modern Emblem / Crest

## Türkçe

> [KONU/KURUM] için sade modern emblem/crest tasarla. En fazla 3–4 ana sembol kullan ve bunları net hiyerarşiyle bir araya getir. Küçük ölçekte okunabilir silhouette üret. Sahte tarihî arma, gereksiz taç, kartal, defne ve Latin motto ekleme.

## English

> Design a restrained modern emblem or crest for [SUBJECT/ORGANIZATION]. Use no more than 3–4 primary symbols and combine them with clear hierarchy. Keep the silhouette readable at small scale. Avoid fake heraldry, unnecessary crowns, eagles, laurels, and Latin mottos.

## Neye dikkat edilmeli?

Harita ve grafik öğelerde yer adları ve sınırlar gerçek veriyle karşılaştırılır; süsleme bilgiyi gölgeliyorsa öğe çıkarılır.

---
# 936. `/topographic-relief` — Physical Topographic Relief

## Türkçe

> [BÖLGE]'yi fiziksel topoğrafik kabartma levha olarak göster. Yükselti gerçek veya doğrulanmış veri mantığıyla şekillensin; su düz ve alçak, kara kademeli relief olsun. Rastgele dağ ekleme.

## English

> Show [REGION] as a physical topographic relief panel. Shape elevation according to real or verified terrain logic, keeping water flat and low and land as graduated relief. Do not invent random mountains.

## Neye dikkat edilmeli?

Harita ve grafik öğelerde yer adları ve sınırlar gerçek veriyle karşılaştırılır; süsleme bilgiyi gölgeliyorsa öğe çıkarılır.

---
# 937. `/map-emboss` — Embossed Map Print

## Türkçe

> [ŞEHİR/BÖLGE] haritasını kalın sanat kâğıdına kör gofre/emboss uygulanmış minimal baskı olarak göster. Ana kıyı/yol/topoğrafi çizgileri yüzeyden hafif yükselsin. Mürekkep gerekiyorsa yalnız tek küçük vurgu kullan.

## English

> Show the map of [CITY/REGION] as a minimal blind-emboss print on thick art paper. Raise only the primary coastline, road, or topographic lines slightly from the surface. If ink is used, keep it to one restrained accent.

## Neye dikkat edilmeli?

Harita ve grafik öğelerde yer adları ve sınırlar gerçek veriyle karşılaştırılır; süsleme bilgiyi gölgeliyorsa öğe çıkarılır.

---
# 938. `/map-thread` — Thread-map Artwork

## Türkçe

> [ROTA/ŞEHİR] haritasını fiziksel iğne-iplik çalışması olarak göster. Harita tabanında yalnız ana noktalar, aralarında gerçek rotayı izleyen iplik çizgileri bulunsun. Her yol için farklı renk kullanma; 1–3 iplik rengiyle sınırla.

## English

> Render [ROUTE/CITY] as physical pin-and-thread map artwork. Keep only the primary locations on the base and connect them with thread following the real route. Limit the work to 1–3 thread colors rather than coloring every road differently.

## Neye dikkat edilmeli?

Harita ve grafik öğelerde yer adları ve sınırlar gerçek veriyle karşılaştırılır; süsleme bilgiyi gölgeliyorsa öğe çıkarılır.

---
# 939. `/map-cutout` — Laser-cut Map

## Türkçe

> [ŞEHİR]'in sokak ağını lazer kesilmiş tek bağlı ahşap/metal harita olarak tasarla. Yol boşlukları ve ada parçaları üretilebilir bağlantı mantığı taşısın. Haritada fiziksel olarak havada kalacak bağımsız küçük parçalar bırakma.

## English

> Design the street network of [CITY] as one connected laser-cut wood or metal map. Make street openings and block islands physically manufacturable. Do not leave tiny unsupported pieces floating inside the map.

## Neye dikkat edilmeli?

Harita ve grafik öğelerde yer adları ve sınırlar gerçek veriyle karşılaştırılır; süsleme bilgiyi gölgeliyorsa öğe çıkarılır.

---
# 940. Viral prompt taramasında yeni kural: promptun kendisi de “trend nesnesi” olabilir

İnternette artık yalnız görsel stil değil, **aynı uzun prompt metninin kendisi** viral olarak kopyalanıyor.

Editorial Split bunun açık örneğidir.

Bu nedenle rehberde trendleri ikiye ayırmak yararlı olabilir:

### A. Görsel trend

Örneğin:

- action figure,
- crayon doodle,
- disposable camera,
- pocket city,
- paper cut.

### B. Viral master prompt

Belirli, uzun ve tekrar tekrar kopyalanan komut reçetesi:

- Editorial Split Poster,
- identity-preserving figure packaging,
- same-person style grid,
- smartphone pop-out,
- structured product photography prompt.

Bu ayrım güncel internet kültürünü daha doğru yakalar.

---

# 941. Viral master promptları değerlendirme rubriği

İnternette dolaşan uzun bir prompt rehbere alınmadan önce şu sorularla değerlendirilmeli:

1. **Gerçekten tekrarlı kullanılıyor mu?**
2. **Sonucu belirleyen açık bir görsel mekanizma var mı?**
3. **Yalnız sıfat zinciri mi, yoksa ölçülebilir kompozisyon talimatı mı içeriyor?**
4. **Referans fotoğraf/kimlik korunması açık mı?**
5. **Malzeme veya baskı süreci tarif ediliyor mu?**
6. **Negatif talimatlar amaca hizmet ediyor mu?**
7. **Kısaltılabilir gereksiz tekrar var mı?**
8. **Farklı konuya uyarlanabilir mi?**
9. **Modelin en sık yaptığı hatalara karşı çözüm içeriyor mu?**
10. **Bir ay sonra unutulacak meme mi, yoksa yeniden kullanılabilir görsel sistem mi?**

Bu rubrik, rehberi rastgele “1000 viral prompt” deposuna dönüşmekten korur.

---

# 942. Yeni tarama için geniş slash-style indeks

Aşağıdaki ifadeler resmî ChatGPT komutları değildir. Rehberde hızlı erişim/preset adı olarak düşünülebilir:

| Kısayol | Aile |
|---|---|
| `/lego` | brick-built transformation |
| `/editorial-split` | photo + minimal handmade illustration |
| `/editorial-split-isometric` | photo + tiny isometric model |
| `/editorial-split-paper-cut` | photo + paper-cut |
| `/editorial-split-riso` | photo + risograph |
| `/editorial-split-xerox` | photo + Xerox |
| `/editorial-split-food` | food-preserving split poster |
| `/disposable-35mm` | cheap 35mm snapshot |
| `/point-and-shoot-2000s` | early digital compact |
| `/film-contact-sheet` | film contact sheet |
| `/halation` | real highlight halation |
| `/light-leak` | controlled film leak |
| `/expired-film` | restrained expired-film behavior |
| `/toy-box` | collectible blister packaging |
| `/designer-toy` | designer vinyl figure |
| `/blind-box` | mystery collectible series |
| `/miniature-box` | boxed physical diorama |
| `/phone-popout` | subject stepping out of smartphone |
| `/open-head-concept` | metaphorical editorial portrait |
| `/exploded-architecture` | exploded architectural axonometric |
| `/architecture-collage` | competition collage |
| `/white-model` | white-card architectural model |
| `/material-model` | physical material architecture model |
| `/section-perspective` | technical section perspective |
| `/diagrammatic-render` | render + diagram hybrid |
| `/retro-airbrush` | real airbrush-process aesthetic |
| `/chrome-airbrush` | chrome airbrush |
| `/y2k-product` | Y2K consumer-tech design |
| `/cassette-futurism` | analog retro-futurism |
| `/tattoo-flash` | tattoo flash sheet |
| `/patch-sheet` | embroidered patch collection |
| `/crest` | restrained emblem/crest |
| `/topographic-relief` | physical terrain relief |
| `/map-emboss` | blind-emboss map |
| `/map-thread` | thread route map |
| `/map-cutout` | laser-cut street map |

---

<a id="aile-010"></a>
# Viral Fotoğraf Düzenleme Master Promptları — Eylül 2026 Ek Taraması

Son taramada kısa stil etiketlerinden farklı bir ikinci internet davranışı daha netleşti:

> Kullanıcılar yalnızca `/polaroid`, `/toy-box` gibi bir estetik adı paylaşmıyor; **kimliği koruma + kamera davranışı + kompozisyon + değiştirilecek alan + korunacak alan** içeren uzun “master prompt” reçetelerini de kopyalayıp birbirine aktarıyor.

2026 boyunca özellikle şu kümeler yoğunlaşıyor:

- iPhone / smartphone “imperfect photo dump” görünümü,
- erken dijital CCD gece flaşı,
- Polaroid setleri ve aynı kişinin çok karede korunması,
- çok panelli günlük hayat / “Prompt Seen” türü portreler,
- eski fotoğraf restorasyonu için aşırı ayrıntılı JSON-benzeri promptlar,
- kimliği kilitleyip yalnız arka plan, dönem, kamera veya ışığı değiştirme,
- “same person / same outfit / same camera” tutarlılık reçeteleri.

Bunların içinde önemli bir ayrım vardır:

> Promptta `"identity_lock": true` veya `"reference_weight": 0.95` yazılması, ChatGPT veya Gemini’de gerçekten böyle bir teknik parametre bulunduğu anlamına gelmez.

Doğal dil arayüzünde bu ifadeler çoğunlukla **metinsel talimat** olarak yorumlanır. Rehber bu nedenle viral promptu arşivlerken bir de **gerçekte ne işe yaradığını** açıklar.

---

# 943. `/iphone-blur` — Smartphone Photo Dump Aesthetic

## Trend

**TREND — çok güçlü.**

2026 viral photo-editing listelerinde “iPhone blurry”, “imperfect handheld”, “Instagram dump” gibi adlarla tekrar tekrar görülüyor.

## Türkçe prompt

> Yüklenen fotoğrafı gündelik smartphone photo-dump estetiğine dönüştür. Kişinin yüzünü, kimliğini, pozunu, kıyafetini ve kadrajını değiştirme.
>
> Hafif elde çekim hareket bulanıklığı, küçük odak kusuru, düşük ışıkta doğal telefon noise'u, bazı parlak kaynaklarda hafif taşma ve gerçek cilt dokusu kullan. Fotoğraf, planlanmış profesyonel çekim değil arkadaşın telefonuyla anlık çekilmiş iyi bir kare gibi görünsün.
>
> Yapay lens flare, sinematik sis, profesyonel bokeh, aşırı HDR ve beauty filter kullanma.

## English

> Transform the uploaded photo into a casual smartphone photo-dump image while preserving the person's exact identity, pose, clothing, and framing.
>
> Use subtle handheld motion blur, minor focus imperfection, believable low-light phone noise, slight clipping around bright practical lights, and natural skin texture. Make it feel like a good accidental phone photograph taken by a friend rather than a planned professional shoot.
>
> Avoid artificial lens flare, cinematic haze, professional bokeh, excessive HDR, and beauty filtering.

---

# 944. `/ccd-night` — Early-2000s CCD Night Flash

## Trend

**TREND — çok güçlü.**

## Türkçe prompt

> Fotoğrafı 2000'lerin başındaki küçük CCD sensörlü kompakt dijital kamerayla gece çekilmiş gibi göster. Yüz ve kimliği değiştirme.
>
> Dahili doğrudan flaş, özne üzerinde hafif fazla pozlanmış highlight, hızlıca kararan arka plan, küçük CCD noise'u, düşük ışık renk sapmaları, az miktarda motion blur ve biraz sert dijital sharpening kullan.
>
> Modern telefon night-mode HDR, büyük sensör bokeh'i veya analog film grain'i taklit etme.

## English

> Make the image look like a nighttime photograph from an early-2000s compact digital camera with a small CCD sensor. Preserve identity exactly.
>
> Use direct built-in flash, slightly overexposed highlights on the subject, rapid falloff into a dark background, mild CCD noise, low-light color artifacts, a little motion blur, and slightly harsh digital sharpening.
>
> Avoid modern smartphone night-mode HDR, large-sensor bokeh, and analog-film grain.

---

# 945. `/ccd-party` — CCD Party Snapshot

## Türkçe prompt

> 2–4 kişilik sahneyi küçük CCD kamera ile doğrudan flaş kullanılarak çekilmiş 2000'ler parti fotoğrafı gibi göster. İnsanların yüzleri ve kimlikleri korunmalı. Bir kişi kameraya tam bakmayabilir; pozlar hafif hazırlıksız olabilir. Flaş ön planı aydınlatsın, arka plan hızlıca kararsın.
>
> Profesyonel gece kulübü reklam fotoğrafı gibi renkli rim light ve sis kullanma.

## English

> Render the 2–4 person scene as an early-2000s party snapshot taken with a compact CCD camera and direct flash. Preserve every person's identity. Allow slightly unprepared poses and imperfect eye contact. Let the flash illuminate the foreground while the background falls off quickly.
>
> Avoid nightclub-advertising rim lights and haze.

## Neye dikkat edilmeli?

Ortam ışığı ve kişi kimliği kareler arasında sabit kalsın; model arka planı ve yüzdeki küçük izleri her karede yeniden uydurmaya eğilimlidir. Flaş parlaması ve gren dozunda kalsın, sahne stüdyo parlaklığına çekilmemiş olsun.

---
# 946. `/photo-dump` — Casual Multi-photo Dump

## Trend

**TREND — sosyal medya anlatı formatı.**

## Türkçe prompt

> Aynı gün veya aynı etkinlikten 6 fotoğraflık doğal photo-dump serisi oluştur. Fotoğrafların hepsi aynı kamera/telefon ve aynı zaman aralığından gelmiş gibi görünmeli.
>
> Seri:
>
> 1. ana insan/olay karesi,
> 2. küçük detay,
> 3. yemek/nesne,
> 4. hareketli veya hafif bulanık an,
> 5. ortam/şehir karesi,
> 6. beklenmedik sıradan kapanış karesi
>
> içersin.
>
> Her kareyi “mükemmel Instagram fotoğrafı” yapma. Aynı filtreyi ağır biçimde uygulama.

## English

> Create a natural six-image photo dump from the same day or event. Every image should feel captured with the same phone or camera during the same time period.
>
> Include:
>
> 1. one main people/event image,
> 2. one small detail,
> 3. one food/object image,
> 4. one moving or slightly blurry moment,
> 5. one environment/city frame,
> 6. one unexpectedly ordinary closing image.
>
> Do not make every frame a perfect Instagram hero shot or apply one heavy filter to all of them.

---

# 947. `/three-polaroids` — Same-person Polaroid Set

## Trend

**TREND — identity consistency testi olarak da kullanılıyor.**

## Türkçe prompt

> Aynı kişinin üç ayrı Polaroid portresini yan yana veya masa üzerinde göster.
>
> Tüm karelerde:
>
> - aynı yüz,
> - aynı saç,
> - aynı kıyafet,
> - aynı yaş,
> - aynı genel ışık kaynağı
>
> korunmalı.
>
> Yalnız baş açısı, küçük ifade değişimi ve el pozu farklı olabilir. Üç fotoğrafın her birinde yeni aksesuar veya yeni kıyafet üretme.

## English

> Show three Polaroid portraits of the same person side-by-side or placed on a tabletop.
>
> Preserve the same face, hair, outfit, age, and overall lighting source in every frame. Vary only head angle, small expression changes, and hand pose. Do not invent new accessories or clothing between the photographs.

---

# 948. `/polaroid-sequence` — Instant-photo Mini Narrative

## Türkçe prompt

> Aynı kişiyi dört instant-photo karesinde küçük bir doğal eylem dizisi içinde göster: hazırlanıyor, eylemi yapıyor, tepki veriyor, son karede rahatlıyor. Tüm karelerde kimlik ve kıyafet aynı olsun. Her fotoğraf bağımsız poz değil, aynı birkaç dakikanın devamı gibi hissettirsin.

## English

> Show the same person across four instant-photo frames in one small natural action sequence: preparing, doing the action, reacting, and relaxing afterward. Keep identity and clothing identical. Make the images feel like consecutive moments from the same few minutes rather than four unrelated poses.

## Neye dikkat edilmeli?

Ortam ışığı ve kişi kimliği kareler arasında sabit kalsın; model arka planı ve yüzdeki küçük izleri her karede yeniden uydurmaya eğilimlidir. Flaş parlaması ve gren dozunda kalsın, sahne stüdyo parlaklığına çekilmemiş olsun.

---
# 949. `/seen-portrait` — Identity-preserved Lifestyle Portrait

## Trend

**TREND — “Prompt Seen” adı altında dolaşan geniş aile.**

Bu ad tek bir stil tanımlamaz. Ortak mekanizma:

> **yüklenen yüzü koru + kişiyi yeni ama gündelik/estetik bir yaşam sahnesine taşı + gerekirse 2–3 panel kullan**

olarak özetlenebilir.

## Türkçe prompt

> Yüklenen yüzü tek kimlik referansı olarak kullan. Yüzü güzelleştirme, yeniden şekillendirme veya yaş değiştirme.
>
> Kişiyi [MEKÂN] içinde doğal bir gündelik anın parçası olarak göster. Kıyafet ve ortamı belirtilen bağlama uygun tut. Kişi kameraya poz vermek zorunda değil.
>
> Sonuç lifestyle reklamı değil, kişisel editoryal fotoğraf hissi taşısın.

## English

> Use the uploaded face as the only identity reference. Do not beautify, reshape, or change age.
>
> Place the person naturally inside [SETTING] as part of an everyday moment. Keep clothing and environment appropriate to the context. The person does not need to pose for the camera.
>
> Make the result feel like a personal editorial photograph rather than lifestyle advertising.

---

# 950. `/rain-window` — Rainy Window Portrait

## Trend

**TREND — “seen portrait” ailesinde sık kullanılan varyasyon.**

## Türkçe prompt

> Kişiyi yağmur damlaları bulunan pencerenin yanında otururken göster. Yüz kimliği aynı kalsın. Dışarıdaki ışık soğuk mavi-gri, içerideki ışık daha nötr/yumuşak olabilir. Camdaki damlalar ve arka şehir ışıkları doğal alan derinliği oluştursun.
>
> Pencereye teatral sağanak, yoğun sis ve dramatik neon ekleme.

## English

> Show the person sitting beside a rain-streaked window while preserving facial identity exactly. Use cool blue-gray exterior light with restrained neutral interior light. Let water droplets and distant city lights create natural depth.
>
> Avoid theatrical downpour, heavy fog, and dramatic neon.

---

# 951. `/library-triptych` — Lifestyle Editorial Triptych

## Türkçe prompt

> Aynı kişinin kütüphanede üç panelli dikey editoryal serisini oluştur:
>
> 1. ortamı gösteren geniş kare,
> 2. kitap/eller ayrıntısı,
> 3. yan profil veya doğal orta plan.
>
> Kimlik, kıyafet, günün saati ve ışık tüm panellerde aynı olsun. Üç paneli üç ayrı fotoğraf çekimi gibi gösterme.

## English

> Create a three-panel vertical editorial series of the same person in a library:
>
> 1. one wide environmental frame,
> 2. one close detail of book or hands,
> 3. one side profile or natural medium shot.
>
> Keep identity, clothing, time of day, and lighting consistent across all panels. Do not make them look like three unrelated shoots.

## Neye dikkat edilmeli?

Ortam ışığı ve kişi kimliği kareler arasında sabit kalsın; model arka planı ve yüzdeki küçük izleri her karede yeniden uydurmaya eğilimlidir. Flaş parlaması ve gren dozunda kalsın, sahne stüdyo parlaklığına çekilmemiş olsun.

---
# 952. `/train-window` — Travel-documentary Portrait

## Türkçe prompt

> Kişiyi hareket hâlindeki trenin pencere yanında doğal portre olarak göster. Yüz aynı kalsın. Pencere dışındaki manzara hareket yönünde bulanık, kişinin yüzü ise okunabilir olsun. Işık gerçek pencere yönünden gelsin.
>
> Sahneyi lüks tren reklamı veya moda çekimine dönüştürme.

## English

> Show the person naturally seated beside the window of a moving train while preserving identity. Blur the passing landscape directionally while keeping the face readable. Let the light originate from the actual window.
>
> Avoid luxury-train advertising and fashion-shoot styling.

## Neye dikkat edilmeli?

Ortam ışığı ve kişi kimliği kareler arasında sabit kalsın; model arka planı ve yüzdeki küçük izleri her karede yeniden uydurmaya eğilimlidir. Flaş parlaması ve gren dozunda kalsın, sahne stüdyo parlaklığına çekilmemiş olsun.

---
# 953. `/night-market-candid` — Night Market Candid

## Türkçe prompt

> Kişiyi gece pazarında yürürken doğal candid olarak göster. Yüz aynı kalsın. Tezgâh ışıkları ve gerçek tabelalar ciltte küçük karışık renk yansımaları oluşturabilir. Arka plan hafif hareketli ve canlı, kişi ise yeterince okunabilir olsun.
>
> Tüm sahneyi mavi-mor cyberpunk neonla kaplama.

## English

> Show the person walking naturally through a night market while preserving identity. Allow practical stall lighting and real signs to create small mixed-color reflections on skin. Keep the background lively with slight motion while the subject remains readable.
>
> Do not flood the scene with blue-purple cyberpunk neon.

## Neye dikkat edilmeli?

Ortam ışığı ve kişi kimliği kareler arasında sabit kalsın; model arka planı ve yüzdeki küçük izleri her karede yeniden uydurmaya eğilimlidir. Flaş parlaması ve gren dozunda kalsın, sahne stüdyo parlaklığına çekilmemiş olsun.

---
# 954. `/old-cafe` — Quiet Café Editorial

## Türkçe prompt

> Kişiyi eski ama gerçekçi bir kafenin pencere yanında doğal otururken göster. Masada yalnız bir kitap/defter ve içecek olsun. İç sıcak ışık ile dış daha soğuk gün ışığı doğal biçimde karışsın. Kişi kameraya bakmak zorunda değil.
>
> Kahve, kurutulmuş çiçek, gazete, gözlük ve 15 dekor objesiyle “cozy aesthetic” klişesi üretme.

## English

> Show the person seated naturally beside the window of an older believable café. Keep only one book or notebook and one drink on the table. Let warm interior light mix naturally with cooler exterior daylight. The subject does not need to look at the camera.
>
> Avoid the “cozy aesthetic” pile of coffee, dried flowers, newspapers, glasses, and excessive props.

## Neye dikkat edilmeli?

Ortam ışığı ve kişi kimliği kareler arasında sabit kalsın; model arka planı ve yüzdeki küçük izleri her karede yeniden uydurmaya eğilimlidir. Flaş parlaması ve gren dozunda kalsın, sahne stüdyo parlaklığına çekilmemiş olsun.

---
# 955. `/restore-photo` — Kimlik Korumalı Fotoğraf Restorasyonu

## Trend

**VIRAL MASTER PROMPT — güçlü ve pratik.**

2026'da özellikle Gemini topluluklarında çok uzun JSON-benzeri restorasyon promptları paylaşılmıştır.

## Türkçe kısa sürüm

> Eski veya düşük kaliteli bu fotoğrafı dikkatle restore et.
>
> Öncelik sırası:
>
> 1. kişinin kimliğini ve yüz geometrisini koru,
> 2. ifadeyi ve pozu değiştirme,
> 3. kıyafet, ayakkabı, takı ve mevcut nesneleri koru,
> 4. çizik, toz, solma ve sıkıştırma artefaktlarını onar,
> 5. yalnız gerçekten desteklenen ayrıntıyı geri kazan,
> 6. doğal ton ve cilt dokusunu koru.
>
> Yüzü güzelleştirme, simetrikleştirme, gençleştirme veya modernleştirme. Eksik ayrıntıları özgürce icat etme.

## English

> Carefully restore this old or low-quality photograph.
>
> Priority:
>
> 1. preserve identity and facial geometry,
> 2. preserve expression and pose,
> 3. preserve clothing, footwear, accessories, and existing objects,
> 4. repair scratches, dust, fading, and compression artifacts,
> 5. recover only details reasonably supported by the source,
> 6. preserve natural tones and skin texture.
>
> Do not beautify, symmetrize, de-age, or modernize the person. Do not freely invent missing details.

---

# 956. Viral JSON promptları hakkında kritik not

İnternette şöyle yapılar dolaşıyor:

```json
{
  "identity_lock": true,
  "facial_geometry_lock": true,
  "reference_weight": 0.95,
  "variation_limit": "extremely_low",
  "face_mutation_prevention": true
}
```

Bunlar **doğal dil ile çalışan ChatGPT/Gemini arayüzlerinde belgelenmiş teknik API parametreleri değildir**.

Model bunları:

> “Kullanıcı kimliği çok sıkı korumamı istiyor.”

şeklinde anlayabilir.

Ama:

> `"reference_weight": 0.95`

yazmak, sistem içinde gerçekten 0.95 ağırlıklı bir kontrol slider'ı ayarladığınız anlamına gelmez.

Bu nedenle rehberde:

### Viral biçim

arşivlenebilir.

Ancak yanında:

### Gerçek anlam

> `Keep the person's facial geometry, expression, age, pose and clothing unchanged.`

şeklinde sade doğal dil karşılığı verilmelidir.

---

# 957. `/restore-structure` — Structure-first Restoration

## Türkçe prompt

> Bu fotoğrafı restore ederken önce yapısal doğruluğu koru. Yüz hatları, gözler arası mesafe, burun formu, ağız, çene, saç çizgisi, beden oranı ve perspektif kaynak görüntüden sapmasın.
>
> Keskinlik artırımı yalnız mevcut bilgiyi daha okunur hâle getirsin; yeni yüz ayrıntısı icat etmesin.

## English

> Restore this photograph with structural fidelity as the first priority. Keep facial proportions, eye spacing, nose structure, mouth, jawline, hairline, body proportions, and perspective consistent with the source.
>
> Sharpening should make existing information clearer rather than inventing new facial detail.

## Neye dikkat edilmeli?

Orijinal kimlik ve dönem korunsun; model eksik kalan yüz, el ve yazı gibi yerleri uydurur. Uydurulan her ayrıntı kaynak fotoğrafla karşılaştırılır; emin olunamayan yer boş bırakılır.

---
# 958. `/historical-colorize` — Tarihsel Olarak Kontrollü Renklendirme

## Türkçe prompt

> Siyah-beyaz fotoğrafı renklendir ancak renkleri tarihsel bağlamdan türet. Cilt, kumaş, ahşap, taş, bitki ve gökyüzü doğal doygunlukta olsun. Emin olunmayan kıyafet veya nesne rengini aşırı iddialı seçme.
>
> Fotoğrafın ışık yönü ve ton ilişkisi korunmalı.

## English

> Colorize the black-and-white photograph using colors grounded in the historical context. Keep skin, fabric, wood, stone, vegetation, and sky naturally saturated. Avoid overconfident color choices for uncertain clothing or objects.
>
> Preserve the original lighting direction and tonal relationships.

## Neye dikkat edilmeli?

Orijinal kimlik ve dönem korunsun; model eksik kalan yüz, el ve yazı gibi yerleri uydurur. Uydurulan her ayrıntı kaynak fotoğrafla karşılaştırılır; emin olunamayan yer boş bırakılır.

---
# 959. `/restore-not-reshoot` — Restorasyon ve “Yeniden Çekim” Ayrımı

Bazı viral promptlar eski fotoğrafı:

> `high-end medium-format reshoot`

gibi tarif eder.

Bu, sonuç daha etkileyici görünse bile tarihî görüntünün:

- lens karakterini,
- ışığını,
- kontrastını,
- dönemin kamera davranışını

modernleştirebilir.

Gerçek restorasyon isteniyorsa:

> `/restore-not-reshoot`

kullanılabilir.

## Türkçe

> Fotoğrafı modern kamerayla yeniden çekilmiş gibi değiştirme. Orijinal kamera perspektifi, alan derinliği, ışık ve dönemsel fotoğraf karakteri mümkün olduğunca korunsun. Yalnız hasarı onar ve okunabilirliği iyileştir.

## English

> Do not reinterpret the photograph as if reshot on a modern camera. Preserve the original camera perspective, depth of field, lighting, and period photographic character as much as possible. Repair damage and improve readability only.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 960. `/modern-reshoot` — Bilinçli Modern Yeniden Çekim

Restorasyondan farklı bir amaçtır.

## Türkçe prompt

> Kaynak fotoğraftaki kişi, kimlik, ifade, poz ve ana kompozisyonu koruyarak aynı anın bugün yüksek kaliteli modern kamera ile yeniden çekilmiş hâlini oluştur. Modern lens/renk/dinamik aralık kullanabilirsin; ancak kıyafet, yaş, beden, çevresel objeler ve tarihsel içerik değişmesin.

## English

> Recreate the same moment as if photographed today with a high-quality modern camera while preserving the source person's identity, expression, pose, and primary composition. Modern lens rendering, color, and dynamic range may change, but clothing, age, body, environmental objects, and historical content must remain unchanged.

## Neye dikkat edilmeli?

Orijinal kimlik ve dönem korunsun; model eksik kalan yüz, el ve yazı gibi yerleri uydurur. Uydurulan her ayrıntı kaynak fotoğrafla karşılaştırılır; emin olunamayan yer boş bırakılır.

---
<a id="sec-961"></a>
# 961. `/identity-lock` — Evrensel Kimlik Koruma Bloğu

## Rehber içi preset

> `/identity-lock`

## Türkçe açılım

> Yüklenen fotoğraftaki kişiyi tek kimlik referansı olarak kullan. Yüz geometrisini, gözler arası mesafeyi, burun/ağız/çene yapısını, saç çizgisini, yaşını ve ayırt edici özelliklerini değiştirme. Yüz güzelleştirmesi, simetri düzeltmesi veya yeni yüz üretme yapma.

## English

> Use the uploaded person as the sole identity reference. Preserve facial geometry, eye spacing, nose, mouth, jaw structure, hairline, age, and distinctive features. Do not beautify, symmetrize, or generate a replacement face.

## Neye dikkat edilmeli?

Kilit cümlesi her prompta aynen kopyalanır; mealen yazılmış kilit çalışmaz. Güzelleştirme yasağı portre presetleriyle birlikte kullanıldığında ayrıca denetlenir.

---

# 962. `/pose-lock` — Poz Koruma Bloğu

## Türkçe

> Baş açısı, omuz yönü, el/kol konumu, beden duruşu ve ağırlık dağılımını kaynak fotoğraftaki gibi koru. Yalnız istenen stil, malzeme veya çevre değişsin.

## English

> Preserve head angle, shoulder direction, hand and arm positions, body posture, and weight distribution from the source. Change only the requested style, material, or environment.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 963. `/outfit-lock` — Kıyafet Koruma Bloğu

## Türkçe

> Kıyafet türü, kesimi, katmanları, ana renkleri, ayakkabı ve görünür aksesuarları değiştirme. Stil dönüşümü kıyafeti yeniden tasarlamasın.

## English

> Preserve garment types, cuts, layers, primary colors, footwear, and visible accessories. The style transformation must not redesign the outfit.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 964. `/composition-lock` — Kadraj ve Mekânsal İlişki Koruma

## Türkçe

> Kamera yüksekliği, kamera yönü, crop, ana öznenin kadrajdaki yeri, nesneler arası mesafe ve perspektifi kaynakla aynı tut. Yalnız açıkça belirtilen değişkeni değiştir.

## English

> Preserve camera height, camera direction, crop, main-subject placement, distances between objects, and perspective. Change only the explicitly requested variable.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
<a id="sec-965"></a>
# 965. `/background-swap` — Kontrollü Arka Plan Değişimi

## Türkçe

> Kişiyi ve ön planı aynen koru; yalnız arka planı [YENİ MEKÂN] ile değiştir. Yeni arka planın perspektifi, ufuk çizgisi, ışık yönü, gölge ve renk sıcaklığı mevcut özneyle eşleşsin. Kişiyi yeniden üretme.

## English

> Preserve the person and foreground exactly; replace only the background with [NEW SETTING]. Match perspective, horizon, light direction, shadows, and color temperature to the existing subject. Do not regenerate the person.

*Benzer: [§2071](33-katalog-aile-044-076.md#sec-2071) — aynı işlemin kaynak-özne (capture-source) ağzıyla sürümü.*

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 966. `/wardrobe-swap` — Kontrollü Kıyafet Değişimi

## Türkçe

> Yüz, saç, beden oranı, poz, eller, kamera ve arka planı değiştirmeden yalnız kıyafeti [YENİ KIYAFET] ile değiştir. Yeni kumaş mevcut ışık ve beden geometrisine doğal biçimde otursun.

## English

> Change only the clothing to [NEW OUTFIT] while preserving face, hair, body proportions, pose, hands, camera, and background. Make the new fabric fit the existing body geometry and lighting naturally.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 967. `/era-transfer` — Tarihsel Döneme Taşıma

## Trend

**TREND — identity-preserving time travel.**

## Türkçe

> Kişinin kimliğini ve temel yüz yapısını koruyarak sahneyi [DÖNEM]'e taşı. Kıyafet, saç düzenleme, mimari, ulaşım, aydınlatma ve gündelik nesneler dönemle uyumlu olsun.
>
> Kişiyi tarihî bir ünlüye dönüştürme. Modern nesneleri yanlışlıkla sahnede bırakma.

## English

> Move the scene into [ERA] while preserving the person's identity and core facial structure. Make clothing, grooming, architecture, transport, lighting, and everyday objects period-appropriate.
>
> Do not turn the person into a historical celebrity or leave accidental modern objects in the scene.

---

# 968. `/same-person-grid` — Çok Karede Kimlik Tutarlılığı

## Türkçe

> Aynı kişiyi [N] karelik grid içinde göster. Tüm karelerde aynı yüz geometrisi, yaş, saç çizgisi ve ayırt edici özellikleri koru. Değişecek tek öğe: [POZ / STİL / IŞIK / MALZEME].
>
> Kareler arasında kişiyi yeniden yorumlama.

## English

> Show the same person in an [N]-frame grid. Preserve the same facial geometry, age, hairline, and distinctive features across every frame. Change only [POSE / STYLE / LIGHTING / MATERIAL].
>
> Do not reinterpret the person's identity between frames.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 969. `/same-outfit-grid` — Aynı Kıyafet, Farklı Kare

## Türkçe

> Çok kareli seride kıyafetin türü, renkleri, desenleri, ayakkabısı ve takıları tüm karelerde bire bir aynı kalsın. Yalnız poz ve ifade değişebilir.

## English

> Across the multi-frame series, keep garment type, colors, patterns, footwear, and jewelry identical. Only pose and expression may change.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 970. `/detail-diptych` — Ana Kare + Ayrıntı

## Trend

**TREND — lifestyle editlerinde yaygın.**

## Türkçe prompt

> İki panelli editoryal kompozisyon oluştur. İlk panel ana sahneyi orta/geniş kadrajda, ikinci panel aynı anın tek anlamlı ayrıntısını yakın planda göstersin. İkinci panelde yeni bir sahne icat etme.
>
> Örnek ayrıntı: eller, kitap, kumaş, bilet, yemek, nesne.

## English

> Create a two-panel editorial composition. Show the primary scene in a medium or wide frame in the first panel, then one meaningful detail from the same moment in close-up in the second. Do not invent a new scene for the detail panel.
>
> Possible details: hands, book, fabric, ticket, food, object.

---

# 971. `/wide-detail-profile` — Üçlü Editoryal Hikâye

## Türkçe prompt

> Aynı sahneden üç kare oluştur:
>
> - geniş ortam,
> - yakın ayrıntı,
> - profil/orta plan insan karesi.
>
> Işık, kıyafet, saat, hava ve nesneler arasında süreklilik koru.

## English

> Create three frames from the same scene:
>
> - wide environment,
> - close detail,
> - profile or medium human frame.
>
> Preserve continuity in light, clothing, time, weather, and objects.

## Neye dikkat edilmeli?

Ortam ışığı ve kişi kimliği kareler arasında sabit kalsın; model arka planı ve yüzdeki küçük izleri her karede yeniden uydurmaya eğilimlidir. Flaş parlaması ve gren dozunda kalsın, sahne stüdyo parlaklığına çekilmemiş olsun.

---
# 972. `/thermal-cam` — Thermal Imaging

## Trend

**TREND — filtre/prompts listelerinde sık görülüyor, ancak bilimsel doğrulukla karıştırılmamalı.**

## Türkçe prompt

> Görseli thermal-camera estetiğinde yorumla. Sıcak bölgelerde açık sarı/beyaz, orta sıcaklıkta kırmızı/turuncu, daha soğuk bölgelerde mor/mavi renk haritası kullan.
>
> Bu görselin gerçek sıcaklık ölçümü veya bilimsel termografi olmadığı açıkça bilinmeli. Tıbbi veya teknik teşhis için kullanma.

## English

> Reinterpret the image using a thermal-camera visualization with pale yellow/white for hotter areas, red/orange for medium temperatures, and purple/blue for cooler areas.
>
> Treat this as a visual simulation rather than real temperature measurement or scientific thermography. Do not use it for medical or technical diagnosis.

---

# 973. `/uncanny-snapshot` — Familiar-but-Wrong Snapshot

## Trend

**TREND — Eylül 2026’da Reddit/medyada görülen yeni deneysel dalga.**

Bu stil korkuyu:

- canavar,
- kan,
- saldırı

yerine **normal görünen fakat küçük ayrıntıları yanlış olan tanıdık fotoğraf** üzerinden kurar.

## Türkçe prompt

> 1980–1990'lar aile/arkadaş snapshot'ına benzeyen sıradan bir fotoğraf oluştur. İlk bakışta sahne normal ve gündelik olsun.
>
> Yalnız 2–3 ince rahatsızlık kullan:
>
> - bir kişinin ifadesinin sahneyle hafif uyumsuz olması,
> - aynadaki küçük tutarsızlık,
> - arka planda açıklanamayan ama belirgin olmayan şekil,
> - insanların bakış yönlerinde küçük uyumsuzluk.
>
> Gore, canavar, kırmızı göz, korku filmi sis efekti veya jumpscare kullanma.

## English

> Create an ordinary-looking 1980s–1990s family or friends snapshot that appears normal at first glance.
>
> Introduce only 2–3 subtle inconsistencies, such as a slightly context-inappropriate expression, a small reflection mismatch, an unexplained but inconspicuous background shape, or subtly inconsistent gaze directions.
>
> Avoid gore, monsters, red eyes, horror fog, and jumpscare imagery.

---

# 974. `/neo-noir-car` — Neo-noir Car Portrait

## Trend

**TREND — 2026 prompt listelerinde yüksek görünürlük.**

## Türkçe

> [ARAÇ] ve kişiyi gece şehir ortamında neo-noir fotoğraf olarak göster. Işık yalnız gerçek kaynaklardan gelsin: sokak lambası, tabela, far, dükkân ışığı. Islak zemin varsa yansımalar bu kaynaklarla eşleşsin. Her kenara cyan/magenta rim light ekleme.

## English

> Show [VEHICLE] and the person as a neo-noir nighttime city photograph. Let light come only from plausible sources such as street lamps, signs, headlights, and shop windows. If the pavement is wet, reflections must correspond to those sources. Avoid cyan-magenta rim light on every edge.

---

# 975. `/fake-film-poster` — Fictional Movie Poster Master

## Trend

**TREND — sürdürülebilir viral format.**

## Türkçe prompt

> Yüklenen kişiyi kurmaca [TÜR] film afişinin ana karakteri olarak kullan. Kimliği koru. Tek ana görsel metafor, kısa özgün film adı ve en fazla bir alt satır kullan. Türün görsel dilini ışık, kadraj ve tipografi üzerinden kur.
>
> Sahte oyuncu listesi, 20 festival laureli, anlamsız küçük metin ve mevcut film franchise'larını kopyalama.

## English

> Use the uploaded person as the main character of a fictional [GENRE] movie poster while preserving identity. Build the poster around one primary visual metaphor, one concise original title, and at most one secondary line. Express the genre through lighting, framing, and typography.
>
> Avoid fake cast lists, excessive festival laurels, meaningless fine print, and copying existing film franchises.

---

# 976. `/book-cover-editorial` — Independent Book Cover

## Trend

**TREND — yüksek.**

## Türkçe prompt

> [KONU/HİKÂYE] için bağımsız yayıncılık hissinde kitap kapağı oluştur. Tek görsel fikir, büyük negatif alan ve kontrollü tipografi kullan. Kapak “premium” görünmek için altın folyo, mockup gölge, 3B nesne ve gradient kullanmak zorunda değil.
>
> Ön kapakta yalnız başlık, gerekliyse alt başlık ve yazar adı yer alsın.

## English

> Create an independent-publishing book cover for [TOPIC/STORY] using one visual idea, generous negative space, and restrained typography. Do not rely on gold foil, mockup shadows, 3D objects, or gradients to signal “premium.”
>
> Keep the front cover limited to title, optional subtitle, and author name.

---

# 977. `/scrapbook-story` — Controlled Scrapbook Narrative

## Trend

**TREND — yüksek ancak slop riski yüksek.**

## Türkçe prompt

> [ANI/SEYAHAT] için tek ana fotoğraf ve yalnız 4 destek öğesiyle scrapbook sayfası oluştur:
>
> - küçük tarih etiketi,
> - tek bilet/efemera,
> - bir kısa el yazısı not,
> - bir küçük ikinci fotoğraf veya nesne.
>
> Yırtık kâğıt ve bant yalnız fiziksel olarak gerekli yerde olsun. Kahve lekesi, kurutulmuş çiçek, yıldız, kalp ve 20 sticker ekleme.

## English

> Create a scrapbook page for [MEMORY/TRIP] using one primary photograph and only four supporting elements:
>
> - small date label,
> - one ticket or ephemera item,
> - one short handwritten note,
> - one small secondary photo or object.
>
> Use torn paper and tape only where physically plausible. Avoid coffee stains, dried flowers, stars, hearts, and sticker overload.

---

# 978. `/clay-avatar` — Handmade Clay Portrait

## Trend

**TREND — yükselen.**

## Türkçe

> Yüklenen kişiyi el yapımı küçük kil figüre dönüştür. Kimliği saç, yüz oranı, gözlük/sakal ve kıyafet ana renkleriyle koru. Kil üzerinde küçük parmak/alet izleri ve mat yüzey olsun. Kusursuz CGI, parlak plastik ve aşırı chibi oranlardan kaçın.

## English

> Transform the uploaded person into a small handmade clay figure. Preserve identity through hairstyle, facial proportions, glasses or beard, and primary clothing colors. Show small finger or tool marks and a matte clay surface. Avoid perfect CGI, glossy plastic, and extreme chibi proportions.

---

# 979. `/pet-sticker-sheet` — Same-pet Expression Sheet

## Trend

**TREND — sticker/chibi ailelerinin dayanıklı varyantı.**

## Türkçe

> Aynı evcil hayvanı altı sticker'da göster: oturuyor, meraklı, uyuyor, oyun oynuyor, şaşkın, selam/etkileşim. Tüy rengi, desen, kulak biçimi, göz rengi ve ayırt edici işaretler tüm sticker'larda aynı kalsın. Her sticker'da farklı hayvan üretme.

## English

> Show the same pet across six stickers: sitting, curious, sleeping, playing, surprised, and interacting. Keep fur color, markings, ear shape, eye color, and distinctive features identical in every sticker. Do not generate a different animal in each frame.

---

# 980. `/identity-preservation-line` — Viral Promptların Ortak Koruma Satırı

2026 photo-editing promptlarının çoğunda aynı fikir tekrar ediyor.

## Türkçe

> Kaynak kişinin yüzünü ve kimliğini tanınabilir ve değişmeden koru. Yüz özelliklerini, saç biçimini, beden oranlarını, kıyafeti, pozu ve kamera açısını yalnız açıkça istenmedikçe değiştirme. Yalnız talep edilen görsel dönüşümü uygula.

## English

> Keep the source person's face and identity recognizable and unchanged. Do not alter facial features, hairstyle, body proportions, clothing, pose, or camera angle unless explicitly requested. Apply only the requested visual transformation.

Bu blok:

- restorasyon,
- kamera estetiği,
- arka plan değişimi,
- dönem transferi,
- çok panelli editoryal,
- toyification

gibi birçok prompta eklenebilir.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 981. Viral master promptlarda “sözde kontrol parametresi” filtresi

Aşağıdaki tür ifadeler internette sık görülür:

```text
identity_lock = true
reference_weight = 0.95
preservation_strength = maximum
variation_limit = extremely_low
face_mutation_prevention = true
8K feel
32K
RAW mode
Hasselblad color engine
```

Bunları üç gruba ayırmak gerekir.

## A. Yararlı doğal dil niyeti

> `preserve identity`
>
> `do not change expression`
>
> `match original light direction`

Gerçekten prompt anlamını netleştirir.

## B. Estetik referans

> `medium-format depth`
>
> `soft highlight roll-off`

Görsel davranış anlatmak için yararlı olabilir.

## C. Sözde teknik parametre

> `reference_weight = 0.95`
>
> `identity_lock = true`
>
> `32K`

Arayüz böyle bir parametre sunmuyorsa teknik kontrol değildir.

### Rehber ilkesi

> **Parametre gibi görünen sözcüğü, gözlemlenebilir talimata çevir.**

Örneğin:

### Yerine

> `"variation_limit": "extremely_low"`

### Yaz

> `Change only the damaged areas; preserve all undamaged parts.`

---

# 982. Viral promptları kısaltma algoritması

Uzun bir internet promptu bulunduğunda şu sırayla sıkıştırılabilir:

1. **Görev:** ne yapılacak?
2. **Kaynak:** hangi yüklenen görsel referans?
3. **Kilit:** ne değişmeyecek?
4. **Dönüşüm:** ne değişecek?
5. **Kompozisyon:** yerleşim/oran.
6. **Fizik/kamera/malzeme:** sonucu gerçekten belirleyen davranış.
7. **Negatifler:** yalnız sık yapılan 3–6 hata.
8. **Çıktı:** ayrı görsel mi, seri mi, grid mi?

### Çıkarılabilecekler

- aynı kuralın dört farklı tekrarı,
- `masterpiece`,
- `stunning`,
- `premium`,
- `8K/16K/32K`
- modele gerçek teknik kontrol sağlamayan sahte parametreler.

---

# 983. Viral trendlerin güvenilirlik sınıfı

Rehberde bundan sonra trendlere yalnız `TREND` etiketi değil, kanıt seviyesi de verilebilir:

### T1 — geniş ve kalıcı

Birden fazla platformda aylardır görülüyor.

Örnek:

- action figure,
- Polaroid,
- disposable camera,
- scrapbook,
- clay toy.

### T2 — hızlı yükselen

Son haftalarda birden fazla prompt topluluğunda görülüyor.

Örnek:

- Editorial Split,
- smartphone pop-out,
- CCD night,
- structured restoration JSON.

### T3 — mikrotrend

Tek platform/ülke/toplulukta görünür ama genelleşmesi belirsiz.

### T4 — yalnız prompt sitesi iddiası

“Viral” deniyor ama bağımsız sosyal kanıt zayıf.

Bu sınıf, rehberin internetteki her “viral prompt” iddiasını gerçek trend gibi sunmasını önler.

---

# 984. `/` kısayolları için nihai kullanım kuralı

Rehberde bundan sonra üç seviyeli gösterim kullanılabilir:

### 1. Slash adı

> `/editorial-split`

Hızlı hatırlatma.

### 2. Tek satır açılım

> `photo top + handmade minimal illustration bottom + identity lock + negative space`

Hangi görsel mekanizmanın çağrıldığını gösterir.

### 3. Tam prompt

Türkçe ve İngilizce kontrollü prompt.

Bu sistemle:

> `/lego`

“ChatGPT’de gizli komut” anlamına gelmez.

Şu anlama gelir:

> **Rehberde LEGO/brick-built dönüşüm reçetesinin kısa adı.**

---

# 985. Bu turdaki yeni slash-style indeks (aile-010)

| Kısayol | Aile |
|---|---|
| `/iphone-blur` | imperfect smartphone photo-dump look |
| `/ccd-night` | early-2000s CCD night flash |
| `/ccd-party` | compact-digital party snapshot |
| `/photo-dump` | casual six-image narrative set |
| `/three-polaroids` | same-person Polaroid set |
| `/polaroid-sequence` | instant-photo mini narrative |
| `/seen-portrait` | identity-preserved lifestyle portrait |
| `/rain-window` | rainy-window portrait |
| `/library-triptych` | wide/detail/profile editorial series |
| `/train-window` | travel-documentary portrait |
| `/night-market-candid` | night-market candid |
| `/old-cafe` | quiet café editorial |
| `/restore-photo` | identity-preserving restoration |
| `/restore-structure` | structure-first restoration |
| `/historical-colorize` | historical colorization |
| `/restore-not-reshoot` | conservative restoration |
| `/modern-reshoot` | intentional modern-camera reinterpretation |
| `/identity-lock` | identity preservation block |
| `/pose-lock` | pose preservation |
| `/outfit-lock` | clothing preservation |
| `/composition-lock` | camera/composition preservation |
| `/background-swap` | controlled background replacement |
| `/wardrobe-swap` | clothing-only edit |
| `/era-transfer` | identity-preserving time transfer |
| `/same-person-grid` | multi-panel identity consistency |
| `/same-outfit-grid` | outfit consistency |
| `/detail-diptych` | scene + meaningful detail |
| `/wide-detail-profile` | three-frame editorial narrative |
| `/thermal-cam` | thermal-style visualization |
| `/uncanny-snapshot` | familiar-but subtly wrong snapshot |
| `/neo-noir-car` | realistic-source neo-noir vehicle portrait |
| `/fake-film-poster` | fictional movie poster |
| `/book-cover-editorial` | independent book cover |
| `/scrapbook-story` | controlled scrapbook narrative |
| `/clay-avatar` | handmade clay identity transformation |
| `/pet-sticker-sheet` | same-pet expression stickers |
| `/identity-preservation-line` | reusable preservation block |

---

<a id="aile-011"></a>
# Yeni Viral Master Prompt Aileleri — Sosyal Medya Fotoğraf Serileri, Jumbotron, Dergi Kapağı ve Örgü Dünyalar

Eylül 2026 taramasında birkaç trend, önceki bölümlerdeki kısa estetik adlarından ayrılarak **belirli kompozisyon reçeteleri** hâlinde tekrar ediyor.

Özellikle şu kalıplar dikkat çekiyor:

- aynı kişinin saniyeler arayla çekilmiş gibi görünen 3 karelik smartphone collage,
- laptop/webcam ekranını yeniden fotoğraflama,
- konser jumbotron'unda kişinin dev LED ekranda görünmesi,
- kaynak yüzü koruyarak magazine-cover oluşturma,
- bütün dünyayı iplik/örgü malzemesine dönüştürme,
- “character intro” posterleri,
- kişisel gelecek/özgeçmiş temasını posterleştirme.

Burada yine aynı ayrım korunmalıdır:

> **Trend olan promptu arşivle; ama içindeki AI slop ve sahte teknik kontrol ifadelerini düzelt.**

---

# 986. `/iphone-3frame` — Candid Smartphone 3-frame Collage

## Trend

**T2 — hızlı yükselen.**

2026 Instagram prompt derlemelerinde doğrudan “Candid iPhone 3-Frame Collage” adıyla dolaşan formatlardan biridir.

Temel mekanizma:

> **aynı kişi + aynı kıyafet + aynı yer + birkaç saniye arayla çekilmiş üç farklı doğal kadraj**

## Türkçe prompt

> Yüklediğim kişiyi tek kimlik referansı olarak kullan ve 9:16 dikey, üç karelik smartphone collage oluştur.
>
> Tüm karelerde:
>
> - aynı yüz,
> - aynı saç,
> - aynı kıyafet,
> - aynı aksesuarlar,
> - aynı konum,
> - aynı gün ve ışık
>
> korunmalı.
>
> **Üst kare:** doğal orta plan; kişi hafif yana dönmüş veya başı aşağı bakıyor.
>
> **Orta kare:** aynı anın yüz göstermeyen anlamlı yakın ayrıntısı; örneğin eller, saat, gömlek kıvrımı veya tutulan nesne.
>
> **Alt kare:** aynı ortamda arkadan veya yarım profil, rahat ve hazırlıksız poz.
>
> Hafif elde çekim eğriliği, kusursuz olmayan crop, doğal telefon keskinliği ve küçük pozlama farklılıkları olabilir.
>
> Üç kareyi ayrı moda çekimlerine dönüştürme. Aynı kişinin birkaç saniye içindeki gerçek fotoğrafları gibi hissettir.

## English

> Use the uploaded person as the sole identity reference and create a vertical 9:16 three-frame smartphone collage.
>
> Preserve the same face, hair, outfit, accessories, location, time of day, and lighting across all frames.
>
> **Top:** natural medium shot with a slight turn or downward glance.
>
> **Middle:** one meaningful close detail from the same moment, such as hands, watch, shirt folds, or a held object, without showing the full face.
>
> **Bottom:** relaxed back or partial-profile view in the same setting.
>
> Allow slight handheld tilt, imperfect crop, natural smartphone sharpness, and tiny exposure variation.
>
> Make the frames feel captured seconds apart rather than like three separate fashion shoots.

---

# 987. `/laptop-photobooth` — Late-night Laptop Photo Booth

## Trend

**T2 — sosyal medyada belirgin.**

Bu promptta asıl fikir portre değil, **fotoğrafın ikinci bir ekranın içinden görüntülenmesi**dir.

## Türkçe prompt

> Sahneyi gece masa başında bir laptop ekranına bakıyormuşuz gibi birinci şahıs fotoğraf olarak oluştur.
>
> Laptop ekranında eski/klasik webcam Photo Booth benzeri uygulama açık olsun ve ana kişinin büyük webcam görüntüsü görünsün. Aynı ekranda yan tarafta küçük bir müzik oynatıcı veya playlist penceresi olabilir.
>
> Fiziksel laptop klavyesinin üst kenarı görüntünün en altında hafif odak dışı görünsün.
>
> Ekran parlaklığı yüzü doğal biçimde aydınlatsın. Küçük sensör/webcam görüntüsünde hafif noise ve düşük ışık karakteri olabilir.
>
> Modern glassmorphism, hologram veya sahte 3B arayüz ekleme.

## English

> Create a first-person late-night photograph looking toward a laptop screen.
>
> On the laptop, show a classic webcam Photo Booth-like application containing a large webcam image of the same person. A small music-player or playlist window may sit beside it.
>
> Let the top edge of the physical laptop keyboard appear softly out of focus at the bottom of the photograph.
>
> Use believable screen light on the face, with mild low-light webcam noise.
>
> Avoid glassmorphism, holograms, and futuristic 3D interfaces.

---

# 988. `/jumbotron` — Concert Jumbotron Portrait

## Trend

**T2 — güçlü sosyal medya formatı.**

Viral promptlarda kritik ayrıntı şudur:

> **Kişi sahnede görünmez; yalnız dev konser ekranında görünür.**

Bu ayrıntı, görüntünün “seyircinin telefonuyla çekilmiş gerçek konser anı” gibi görünmesini sağlar.

## Türkçe prompt

> Yüklediğim kişinin yüzünü tek kimlik referansı olarak kullan.
>
> Büyük kapalı konser salonunda seyirci bölümünden telefonla çekilmiş gerçekçi bir an oluştur. Görüntünün büyük kısmını dev LED jumbotron ekranı kaplasın.
>
> Kişi yalnızca LED ekranda yakın plan performans görüntüsü olarak görünsün. Gerçek sahnedeki bedenini ayrıca gösterme.
>
> Alt bölümde az miktarda seyirci silhouette'ı, birkaç telefon ekranı ve sahne ışığı olabilir.
>
> LED ekran üzerinde gerçek piksel yapısı, küçük moiré ve ekran parlaklığı hissi olsun.
>
> Yüzü yeniden tasarlama. Kimliği, saç çizgisini ve ana yüz oranlarını koru.
>
> Konser ışığını tek bir gerçek paletle sınırla. Her kenara rastgele pembe-mor-mavi glow ekleme.

## English

> Use the uploaded person as the sole facial identity reference.
>
> Create a believable audience-perspective smartphone photograph inside a large concert arena, with a giant LED jumbotron occupying most of the frame.
>
> Show the person only as a close-up performance image on the LED screen. Do not also show a duplicate full-body performer on the stage.
>
> Include only a limited amount of audience silhouettes, a few raised phones, and plausible stage light near the bottom.
>
> Give the LED display subtle pixel structure, mild moiré, and believable screen brightness.
>
> Preserve facial identity and hairline. Use one coherent concert-lighting palette rather than random pink-purple-blue glow on every edge.

---

# 989. `/jumbotron-fanphoto` — Fan-shot Jumbotron Variant

## Ne zaman kullanılır?

Daha “gerçek kullanıcı fotoğrafı” hissi istendiğinde.

## Türkçe prompt

> `/jumbotron` kuralını kullan ancak görüntüyü biraz uzaktan, telefon zoom'u ile çekilmiş fan fotoğrafı gibi yap. Hafif dijital zoom yumuşaklığı, küçük elde çekim eğriliği ve ekran çevresinde karanlık arena alanı bulunsun. Kusurlar kontrollü kalsın.

## English

> Use the `/jumbotron` structure but make the image feel captured from farther away using phone zoom. Add slight digital-zoom softness, small handheld tilt, and dark arena space around the screen. Keep imperfections restrained.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 990. `/character-intro` — Cinematic Character Intro Poster

## Trend

**T2 — 2026 prompt sitelerinde yüksek görünürlük.**

İnternette bu trend çoğunlukla:

> cinematic smoke + orange rim light + bold name + 4:5

şeklinde dolaşıyor.

Bu formül çok kolay **AI slop** üretir.

## Rehber sürümü

> Yüklediğim kişiyi tek kimlik referansı olarak kullan ve 4:5 dikey character-intro poster oluştur.
>
> Kişiyi tek güçlü pozda göster. Arka planda yalnız hikâyeye hizmet eden tek çevresel unsur veya basit tonal alan olsun.
>
> İsim gerekiyorsa bir kez büyük veya orta boy kullan. “CHARACTER INTRO” gibi açıklayıcı meta yazıyı yalnız gerçekten isteniyorsa ekle.
>
> Işık sahnede bulunan gerçek kaynaklardan gelsin.
>
> Duman, turuncu rim light, sparks, volumetric rays, dev 3B isim ve lens flare'i otomatik varsayma.
>
> Sonuç film fragmanı klişesi değil, karakterin kimliğini anlatan tek kare olsun.

## English

> Use the uploaded person as the sole identity reference and create a vertical 4:5 character-introduction poster.
>
> Use one strong pose and only one environmental or tonal background element that supports the character story.
>
> If a name is needed, use it once at large or medium scale. Add meta text such as “CHARACTER INTRO” only when explicitly desired.
>
> Make lighting originate from plausible sources in the scene.
>
> Do not automatically add smoke, orange rim light, sparks, volumetric rays, giant 3D names, and lens flare.
>
> Make it feel like one defining character image rather than a generic movie-trailer cliché.

---

<a id="sec-991"></a>
# 991. `/character-card` — Minimal Character Profile Card

## Alternatif

AI slop'u azaltmak için character intro'nun daha sakin sürümü.

*Benzer: [§2253](33-katalog-aile-044-076.md#sec-2253) — koleksiyon (collectible) kart sürümü.*

## Türkçe prompt

> Aynı kişiyi sade karakter profil kartı olarak göster. Tek portre, kısa isim, bir satır rol/tema ve 3 küçük anahtar özellik yeterli olsun. Arka planı sade tut. Oyun arayüzü, HP bar, rank yıldızları veya sahte istatistik ekleme.

## English

> Present the same person as a restrained character-profile card using one portrait, one concise name, one role/theme line, and three small key traits. Keep the background simple. Avoid game UI, HP bars, ranking stars, and fake stats.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 992. `/future-self` — Future-self Concept Poster

## Trend

**T2 — “AI Future Prediction Poster” adıyla dolaşıyor.**

### Kritik düzeltme

Viral sürümlerde AI'dan:

- yüz üzerinden kariyer tahmini,
- kişilik çıkarımı,
- “confidence score”,
- “social status”,
- gelecek yaşam tarzı

gibi temelsiz sonuçlar üretmesi istenebiliyor.

Bunları gerçek “tahmin” gibi sunmak doğru değildir.

## Güvenli ve daha iyi sürüm

> Kullanıcının belirttiği gelecek hedeflerinden yola çıkarak kurmaca **future-self concept poster** oluştur.

## Türkçe prompt

> Yüklediğim kişinin kimliğini koruyarak [5/10] yıl sonraki hedeflenen yaşamını anlatan kurmaca future-self concept poster oluştur.
>
> Kullanılacak gelecek unsurları yalnız verdiğim hedeflerden türet:
>
> - [MESLEK/PROJE],
> - [YAŞAM ALANI],
> - [BECERİ],
> - [ALIŞKANLIK],
> - [KİŞİSEL HEDEF].
>
> AI yüzünden kişilik, zekâ, kariyer veya sosyal statü tahmini yapma.
>
> Poster üzerinde en fazla 3 kısa hedef satırı ve bir kısa “future note” kullan.

## English

> Create a fictional future-self concept poster for the uploaded person while preserving identity.
>
> Derive all future elements only from goals explicitly supplied by the user:
>
> - [CAREER/PROJECT],
> - [PLACE/LIFESTYLE],
> - [SKILL],
> - [HABIT],
> - [PERSONAL GOAL].
>
> Do not infer personality, intelligence, career outcome, or social status from facial appearance.
>
> Use no more than three short goal lines and one concise future-note line.

---

# 993. `/sky-editorial` — Big-sky Editorial Portrait

## Trend

**T2 — “Korean Editorial Sky” gibi adlarla dolaşıyor.**

## Türkçe prompt

> Yüklenen kişiyi geniş açık gökyüzü altında düşük açıdan çekilmiş editoryal portreye dönüştür. Gökyüzü kadrajın yaklaşık %60–75'ini kaplasın. Kişi alt bölümde küçük/orta ölçekte kalsın. Doğal yaz gün ışığı, gerçek bulut hacmi ve hafif rüzgâr kullan.
>
> “Korean aesthetic” gibi belirsiz etiket yerine kompozisyonu ve ışığı açıkça tarif et.
>
> Aşırı dreamy haze, lens glow ve yapay bulut dramatizasyonu kullanma.

## English

> Transform the uploaded person into a low-angle editorial portrait beneath a large open sky. Let the sky occupy roughly 60–75% of the frame while the person remains small to medium in the lower area. Use natural summer daylight, believable cloud volume, and a light breeze.
>
> Describe composition and lighting directly rather than relying on vague labels such as “Korean aesthetic.”
>
> Avoid excessive dreamy haze, lens glow, and over-dramatized clouds.

---

# 994. `/magazine-cover` — Identity-preserving Magazine Cover

## Trend

**T1/T2 — geniş ve kalıcı.**

Eylül 2026'da da özellikle selfie → magazine-cover promptları aktif biçimde paylaşılıyor.

## Türkçe prompt

> Yüklediğim kişiyi 4:5 dikey kurmaca editoryal dergi kapağı için fotoğraflanmış gibi göster.
>
> Yüz ve kimliği koru. Head-and-shoulders veya belirtilen crop'u kullan. Masthead için üstte, 1–2 kısa cover line için yanlarda kontrollü negatif alan bırak.
>
> Kapakta yalnız:
>
> - kurmaca dergi adı,
> - tek ana başlık,
> - en fazla iki küçük cover line
>
> olsun.
>
> Portre ana odak kalsın.
>
> Sahte barkod, fiyat, 12 ayrı başlık, ödül rozeti ve okunmayan filler text üretme.
>
> Belirli gerçek derginin kapağını bire bir kopyalama; bağımsız yayın tasarımı oluştur.

## English

> Present the uploaded person as a portrait photographed for a fictional vertical 4:5 editorial magazine cover.
>
> Preserve facial identity. Use a head-and-shoulders or otherwise specified crop, leaving controlled negative space at the top for a masthead and along the sides for 1–2 concise cover lines.
>
> Include only:
>
> - one fictional magazine name,
> - one main headline,
> - no more than two small cover lines.
>
> Keep the portrait dominant.
>
> Avoid fake barcodes, prices, excessive headlines, award badges, and unreadable filler text.
>
> Do not copy the layout of a specific real magazine; create an independent editorial design.

---

<a id="sec-995"></a>
# 995. `/bw-magazine` — Black-and-white Editorial Cover

## Türkçe prompt

> `/magazine-cover` yapısını kullan, ancak portreyi kontrollü siyah-beyaz editoryal fotoğraf olarak yorumla. Gerçek cilt dokusu, derin ama bilgi kaybetmeyen siyahlar, doğal highlight ve hafif baskı/film tanesi kullan.
>
> “Luxury” hissini parlak cilt, dev serif logo veya sahte folyo ile kurma.

## English

> Use the `/magazine-cover` structure but render the portrait as restrained black-and-white editorial photography. Preserve real skin texture, deep but informative blacks, natural highlights, and subtle print or film grain.
>
> Do not signal “luxury” through glossy skin, oversized serif logos, or fake foil.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 996. `/cover-negative-space` — Cover-ready Portrait Without Text

## Ne zaman kullanılır?

Tipografiyi sonradan gerçek tasarım aracında eklemek daha güvenli olduğunda.

## Türkçe prompt

> Dergi kapağına uygun portre oluştur ancak görselin içinde hiçbir yazı üretme. Masthead ve cover lines için bilinçli negatif alan bırak. Kişiyi, önemli yüz ve saç ayrıntıları sonradan gelecek tipografiyle çakışmayacak biçimde konumlandır.

## English

> Create a cover-ready portrait without generating any text inside the image. Leave deliberate negative space for a masthead and cover lines. Position the person so important facial and hair details will not conflict with later typography.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 997. Dergi kapağında metin için üretim ilkesi

AI görüntü modeli metni iyi üretebilse bile gerçek yayın üretiminde daha güvenilir iş akışı:

1. **kapak-ready görseli üret,**
2. **tipografiyi Canva/Figma/InDesign/Affinity/Photoshop gibi araçta ekle.**

Özellikle:

- issue number,
- fiyat,
- barkod,
- uzun cover lines,
- URL,
- doğru özel isimler

görüntü üretim modeline bırakılmamalıdır.

---

# 998. `/knitted-world` — AI Knitted World

## Trend

**T1/T2 — 2026 boyunca devam eden güçlü tactile dönüşüm.**

Ağustos 2026 kaynaklarında yüzleri, evcil hayvanları ve landmarkları tamamen iplik/yün dünyaya dönüştüren “AI Knitted World” trendinin TikTok ve Instagram'da yılın ilk yarısı boyunca devam ettiği bildiriliyor.

## Türkçe prompt

> Yüklenen fotoğrafın tüm sahnesini gerçekten örülmüş fiziksel yün/örgü dünyasına dönüştür.
>
> Yalnız öznenin üzerine “fuzzy texture” kaplama.
>
> Her nesnenin yapısı:
>
> - örgü ilmekleri,
> - iplik yönü,
> - dikiş/birleşim noktası,
> - dolgu veya kumaş gerilimi,
> - malzemeye uygun yuvarlanan kenarlar
>
> üzerinden oluşsun.
>
> Kişi varsa yüz kimliğini saç formu, genel yüz oranı, gözlük/sakal ve kıyafet renkleriyle koru.
>
> Sert metal/cam nesneler bile “örgüden yapılmış karşılıkları” olarak yeniden kurulmalı.
>
> Plastik CGI fuzz veya bulanık yapay tüy efekti kullanma.

## English

> Transform the entire uploaded scene into a physically knitted yarn-and-wool world.
>
> Do not merely apply fuzzy texture to the existing objects.
>
> Reconstruct every object through believable knitted structure:
>
> - visible stitches,
> - yarn direction,
> - seams and joins,
> - stuffing or fabric tension,
> - softened edges appropriate to the material.
>
> If a person is present, preserve identity through hairstyle, overall facial proportion, glasses or beard, and clothing colors.
>
> Even hard objects such as metal or glass should be rebuilt as knitted equivalents.
>
> Avoid generic CGI fuzz and blurred synthetic fur.

---

# 999. `/knitted-portrait` — Knitted Portrait

## Türkçe prompt

> Yüklenen kişiyi fiziksel el işi örgü portre/figüre dönüştür. Saç tek tek plastik iplik teli değil, örülmüş veya işlenmiş yün kütlesi olarak davranmalı. Yüzde ilmek yapısı görülsün ancak temel yüz oranları tanınabilir kalsın.

## English

> Transform the uploaded person into a physical handmade knitted portrait or figure. Treat hair as knitted or stitched wool mass rather than plastic strands. Keep stitch structure visible on the face while preserving recognizable facial proportions.

## Neye dikkat edilmeli?

Sonuç gerçek örgüyle kurulabilir görünsün; binaya ya da bedene yalnızca yün dokusu kaplanmışsa prompta tek tek ilmek ve dikiş kısıtını ekleyip yeniden üretin.

---
# 1000. `/knitted-landmark` — Knitted Landmark

## Türkçe prompt

> [LANDMARK]'ı tamamen iplik/yün ile kurulmuş küçük fiziksel maket gibi göster. Yapının ana silueti ve mimari oranı korunmalı; taşıyıcı ve cephe ayrıntıları örgü tekniklerine göre sadeleşsin. Yalnız binaya yün dokusu kaplama.

## English

> Show [LANDMARK] as a small physical model constructed entirely from yarn and wool. Preserve the primary architectural silhouette and proportions while simplifying structural and facade details according to knitting or textile construction. Do not simply cover the building in wool texture.

## Neye dikkat edilmeli?

Sonuç gerçek örgüyle kurulabilir görünsün; binaya ya da bedene yalnızca yün dokusu kaplanmışsa prompta tek tek ilmek ve dikiş kısıtını ekleyip yeniden üretin.

---
# 1001. `/knitted-city` — Knitted City Scene

## Türkçe prompt

> Küçük [ŞEHİR] sokak sahnesini bütünüyle örgü dünyasına dönüştür. Yol, bina, tabela, ağaç ve araçlar aynı tekstil evreninde olsun. Her malzeme farklı iplik/örgü tekniğiyle ayrışabilir, ancak aynı fiziksel el işi setinde yapılmış görünmeli.

## English

> Transform a small [CITY] street scene completely into a knitted world. Rebuild roads, buildings, signs, trees, and vehicles within the same textile universe. Different surfaces may use different yarn or stitch techniques, but everything should feel handmade within one physical set.

## Neye dikkat edilmeli?

Sonuç gerçek örgüyle kurulabilir görünsün; binaya ya da bedene yalnızca yün dokusu kaplanmışsa prompta tek tek ilmek ve dikiş kısıtını ekleyip yeniden üretin.

---
# 1002. `/felt-world` — Felted World

## Trend

**Knitted World'ün yakın ama farklı fiziksel alt türü.**

## Türkçe prompt

> Sahneyi örgü ilmekleri yerine sıkıştırılmış keçe/yün liflerinden yapılmış fiziksel dünyaya dönüştür. Yüzeylerde lifli, hafif düzensiz needle-felt karakteri kullan. Dikiş ilmekleri yalnız gerektiğinde görünsün.

## English

> Rebuild the scene as a physical world made from compressed felt and wool fibers rather than knitted stitches. Use visible fibrous, slightly irregular needle-felt character. Show seams only where structurally necessary.

---

# 1003. `/doodle-ui` — Doodle-over-Interface

## Trend

**T2/T3 — profil ekranı ve sosyal medya screenshot'ları üzerinde dolaşan varyasyon.**

## Türkçe prompt

> Kaynak sosyal medya/profil ekranının temel yerleşimini koru ve üzerine yalnız birkaç el çizimi doodle vurgu ekle.
>
> Doodle:
>
> - profil fotoğrafını daire içine alma,
> - 1–2 kısa ok,
> - küçük el yazısı not,
> - birkaç kaba çizgi
>
> ile sınırlı olsun.
>
> Uygulama arayüzünü yeniden tasarlama, ikonları karikatüre dönüştürme veya bütün ekranı sticker'la doldurma.

## English

> Preserve the basic layout of the source social-media or profile screen and add only a few hand-drawn doodle accents.
>
> Limit them to a profile-photo circle, 1–2 short arrows, one small handwritten note, and a few rough lines.
>
> Do not redesign the interface, cartoonify every icon, or cover the whole screen in stickers.

---

# 1004. `/future-ui-poster` — Fictional Future Interface Poster

## Trend

**T2 — “future prediction” trendinin daha güvenilir grafik karşılığı.**

## Türkçe prompt

> Kişinin geleceğini “tahmin ediyor” gibi davranmak yerine, kullanıcının verdiği hedefleri kurmaca future-interface poster içinde görselleştir.
>
> Arayüzde yalnız:
>
> - hedef yıl,
> - hedef proje,
> - öğrenilecek beceri,
> - tek kısa milestone
>
> bulunsun.
>
> Yüz analizi, kişilik puanı, sosyal statü veya başarı olasılığı üretme.

## English

> Instead of pretending to predict the person's future, visualize user-supplied goals inside a fictional future-interface poster.
>
> Include only:
>
> - target year,
> - target project,
> - skill to learn,
> - one concise milestone.
>
> Do not generate facial analysis, personality scores, social status, or probability of success.

---

# 1005. `/style-reference-identity-reference` — İki Referanslı Edit

## Trend

**EVERGREEN / 2026 araçlarında daha önemli hâle geldi.**

## Mantık

Bir görsel:

> **kimliği**

diğeri:

> **stil/kompozisyonu**

belirler.

## Türkçe prompt

> Görsel 1'i yalnız kimlik referansı olarak kullan: yüz, saç, yaş ve ayırt edici özellikleri buradan koru.
>
> Görsel 2'yi yalnız görsel stil/kompozisyon referansı olarak kullan: ışık, crop, renk davranışı ve grafik yerleşimi buradan al.
>
> Görsel 2'deki kişinin yüzünü veya beden özelliklerini Görsel 1'e aktarma.

## English

> Use Image 1 only as the identity reference, preserving face, hair, age, and distinctive features.
>
> Use Image 2 only as the visual-style and composition reference, borrowing lighting, crop, color behavior, and graphic layout.
>
> Do not transfer the person or body characteristics from Image 2 onto the identity from Image 1.

---

<a id="sec-1006"></a>
# 1006. `/reference-role-map` — Çoklu Referansların Görevini Tanımlama

Birden fazla görsel yüklendiğinde:

> “bunları kullan”

demek yerine her görselin rolü belirlenmelidir.

### Örnek

> Image 1 = face identity  
> Image 2 = clothing reference  
> Image 3 = environment reference  
> Image 4 = color/print reference

Bu özellikle:

- editorial cover,
- historical transformation,
- product composite,
- fashion styling,
- city scene

promptlarında tutarlılığı artırır.

*Benzer: [§2016](32-katalog-aile-024-043.md#sec-2016) — referans karışmasını azaltma gerekçesiyle kısa sürüm.*

---

# 1007. `/one-change-only` — Tek Değişkenli Edit

## Evrensel kısa komut

> `/one-change-only`

## Türkçe

> Kaynak görüntüde yalnız [DEĞİŞKEN]'i değiştir. Yüz, beden, poz, kamera, ışık, arka plan, nesne konumu ve diğer tüm ayrıntıları kaynakla aynı bırak.

## English

> Change only [VARIABLE] in the source image. Preserve face, body, pose, camera, lighting, background, object placement, and every other detail.

Bu blok küçük düzenlemelerde uzun master prompttan daha değerlidir.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 1008. `/edit-stack` — Aşamalı Düzenleme

## Yeni rehber ilkesi

Tek promptta:

- kıyafet,
- saç,
- dönem,
- arka plan,
- ışık,
- poster,
- yazı,
- materyal

değiştirmek yerine işlem aşamalara ayrılabilir.

### Örnek

1. `/background-swap`
2. kontrol
3. `/wardrobe-swap`
4. kontrol
5. color grade
6. typography

Bu yöntem özellikle referans kimliğin korunmasında daha güvenilirdir.

---

# 1009. Viral promptlarda “100% face match” ifadesi

İnternette çok yaygın:

> `100% face match`
>
> `exact identity`
>
> `absolute face lock`

Bunların hiçbiri teknik garanti değildir.

Daha yararlı ifade:

> `Preserve the source facial geometry, hairline, age and distinctive features. Do not beautify or replace the face.`

Rehberde yine kısa kısayol:

> `/identity-lock`

yeterlidir.

---

# 1010. Bu turdaki slash-style indeks (aile-011)

| Kısayol | Aile |
|---|---|
| `/iphone-3frame` | same-person candid smartphone collage |
| `/laptop-photobooth` | late-night webcam/laptop scene |
| `/jumbotron` | identity-preserved concert LED screen |
| `/jumbotron-fanphoto` | zoomed audience snapshot |
| `/character-intro` | cinematic character intro |
| `/character-card` | restrained profile card |
| `/future-self` | user-goal future concept poster |
| `/sky-editorial` | large-sky editorial portrait |
| `/magazine-cover` | identity-preserved fictional magazine |
| `/bw-magazine` | monochrome magazine cover |
| `/cover-negative-space` | text-free cover-ready portrait |
| `/knitted-world` | entire scene knitted from yarn |
| `/knitted-portrait` | knitted identity portrait |
| `/knitted-landmark` | knitted architecture |
| `/knitted-city` | knitted urban scene |
| `/felt-world` | needle-felt material world |
| `/doodle-ui` | restrained doodle overlay on UI |
| `/future-ui-poster` | goal-based future interface |
| `/style-reference-identity-reference` | separate identity and style references |
| `/reference-role-map` | define each reference image role |
| `/one-change-only` | edit one variable only |
| `/edit-stack` | sequential image-edit workflow |

---

# 1011. Trend taramasından çıkan önemli sonuç

2026 viral promptlarının büyük kısmı aslında birkaç tekrar eden teknik fikrin remixidir:

### 1. Kimlik kilidi

> aynı kişi kalsın.

### 2. Zaman sürekliliği

> aynı birkaç saniye / aynı gün / aynı çekim.

### 3. İkinci yüzey

> fotoğraf ekran, Polaroid, jumbotron, laptop, dergi veya kart içine taşınır.

### 4. Malzeme dönüşümü

> örgü, kil, kâğıt, Lego-benzeri blok, seramik.

### 5. Boyut/ölçek değişimi

> minyatür, dev, kutu içinde, ekran dışına çıkan.

### 6. Editoryal çerçeveleme

> magazine, split poster, triptych, contact sheet.

### 7. Kontrollü kusur

> direct flash, CCD noise, motion blur, crayon, registration error.

Bundan sonra yeni viral promptları bu **mekanizmalardan hangisini gerçekten yeni biçimde kullandığına** göre değerlendirmek, yalnız “adı yeni” diye rehbere eklemekten daha doğru olacaktır.

---

<a id="aile-012"></a>
# Paketleme, Ürün Fotoğrafçılığı, Albüm Kapağı ve Evcil Hayvan Master Promptları — Eylül 2026 Ek Taraması

Bu turda dört alan öne çıktı:

1. **Kaynak fotoğraftan tam bir ambalaj/marka sistemi üretme**
2. **Ürün fotoğrafında ürün geometrisini kilitleyip yalnız sahne/ışık değiştirme**
3. **Albüm/single kapağını “genre cliché” yerine tek görsel fikirle kurma**
4. **Evcil hayvan kimliğini koruyarak oyuncak, kil, sticker ve editoryal dönüşümler yapma**

Önemli not:

> Bu alanlarda “iyi görünmesi” kadar **ürünün, yüzün, hayvanın veya markanın değişmemesi** önemlidir.

---

# 1012. `/packaging-board` — Photo-to-Packaging Identity Board

## Trend

**T2 — Ağustos sonu 2026’da Reddit prompt topluluklarında yayılan yeni master prompt ailesi.**

Temel mekanizma:

> **üst yarı kaynak fotoğraf**
>
> **alt yarı fotoğraftan türetilen ambalaj/marka sistemi**

Bu, daha önceki `/editorial-split` formülünün doğrudan marka tasarımına uyarlanmış hâlidir.

## Türkçe prompt

> Yüklediğim her fotoğraf için ayrı bir 3:4 dikey packaging identity poster oluştur; birden fazla fotoğrafı tek kolajda birleştirme.
>
> **Üst %50:** kaynak fotoğrafı kimlik, yapı, poz, gerçek doku, doğal ışık ve renk atmosferiyle mümkün olduğunca aynen koru.
>
> **Alt %50:** fotoğrafı ambalaj üzerine doğrudan basmak yerine, fotoğraftaki:
>
> - ana siluet,
> - karakteristik biçimler,
> - renk ilişkileri,
> - ritim/pattern potansiyeli,
> - tema,
> - yerel veya sembolik ayrıntılar
>
> üzerinden özgün bir marka/ambalaj görsel sistemi türet.
>
> Konuya uygun yalnız 5–7 taşıyıcı seç:
>
> - kutu,
> - sleeve,
> - etiket,
> - tag,
> - kart,
> - küçük kâğıt çanta,
> - sticker,
> - wrapping paper
>
> gibi.
>
> 1–2 hero package büyük; diğerleri ikincil olsun. Grid, kenar hizası, ölçü kontrastı ve negatif alanla gerçek tasarım stüdyosu sunum panosu oluştur.
>
> Ambalajlar aynı görsel aileye ait olsun ancak aynı logoyu aynı yerde tekrar eden mockup seti gibi görünmesin.
>
> Mat kâğıt, kalın karton, translucent paper, emboss, die-cut veya fold gibi gerçek üretim yöntemlerinden yalnız konuya uygun olanları kullan.
>
> Plastik 3B mockup parıltısı, sahte lüks folyo, aşırı pastel, yoğun dekor ve e-ticaret ürün dizilimi kullanma.

## English

> Create one separate 3:4 packaging-identity poster for each uploaded photo; never merge multiple source images into one collage.
>
> **Top 50%:** preserve the source photograph as faithfully as possible in identity, structure, pose, real texture, natural light, and color atmosphere.
>
> **Bottom 50%:** do not simply print the photo onto packaging. Extract a brand language from its recognizable silhouette, shapes, color relationships, rhythm/pattern potential, theme, and meaningful local or symbolic details.
>
> Select only 5–7 packaging carriers appropriate to the subject, such as boxes, sleeves, labels, tags, cards, small paper bags, stickers, or wrapping paper.
>
> Use 1–2 hero packages as the main focus and organize supporting pieces through grid alignment, scale contrast, and generous negative space like a real design-studio presentation board.
>
> Keep all pieces within one visual family without repeating the same logo placement across identical mockups.
>
> Use physically plausible materials and techniques such as matte paper, thick cardstock, translucent paper, embossing, die-cuts, and folds only when appropriate.
>
> Avoid glossy 3D mockup sheen, fake luxury foil, excessive pastel styling, decorative clutter, and e-commerce product-grid presentation.

---

# 1013. `/brand-from-photo` — Fotoğraftan Görsel Kimlik Çıkarma

## Ne zaman kullanılır?

Tam packaging board gerekmiyorsa, yalnız marka dili çıkarmak için.

## Türkçe prompt

> Yüklenen fotoğrafı marka logosu olarak kopyalama.
>
> Bunun yerine fotoğraftan şu beş tasarım bileşenini çıkar:
>
> 1. 3–4 ana renk,
> 2. tek basitleştirilmiş sembol,
> 3. bir pattern veya tekrar mantığı,
> 4. tipografi karakteri,
> 5. bir malzeme/yüzey davranışı.
>
> Bu bileşenleri tek görsel identity board üzerinde göster.

## English

> Do not copy the uploaded photograph as a logo.
>
> Instead extract five reusable design components:
>
> 1. 3–4 primary colors,
> 2. one simplified symbol,
> 3. one repeat or pattern logic,
> 4. one typography character,
> 5. one material or surface behavior.
>
> Present them on one restrained visual-identity board.

## Neye dikkat edilmeli?

Logo, renk ve ambalaj dili bütün varyantlarda aynı kalsın; etiketteki yazıyı [§995](#sec-995)'teki kapak notundaki gibi harf harf doğrulayın. Model “ilgili görünsün” diye aileye ait olmayan öğeler ekler.

---
# 1014. `/carrier-select` — Konuya Göre Ambalaj Taşıyıcısı Seçme

## Yeni kural

Viral packaging promptlarındaki en yararlı fikirlerden biri:

> **Her marka için aynı “box + bag + cup + card + tape” setini zorunlu kullanma.**

## Prompt

> Choose only packaging formats that make functional sense for [PRODUCT/CATEGORY]. Do not include cups, bottles, boxes, bags, or tags unless the product would realistically use them.

Bu, AI packaging slop'unu ciddi biçimde azaltır.

---

# 1015. `/packaging-family` — Farklı Form, Aynı Kimlik

## Türkçe prompt

> [MARKA/ÜRÜN] için 5 parçalık packaging family oluştur. Her format farklı fiziksel işleve sahip olsun ancak tipografi, renk, grafik oranı ve malzeme davranışı aynı kimlik sistemini taşısın. Aynı yüzey tasarımını yalnız kutu şekline göre yeniden boyutlandırma.

## English

> Create a five-piece packaging family for [BRAND/PRODUCT]. Give every format a different physical function while maintaining one typography, color, graphic-proportion, and material system. Do not simply resize the same surface artwork onto different box shapes.

## Neye dikkat edilmeli?

Logo, renk ve ambalaj dili bütün varyantlarda aynı kalsın; etiketteki yazıyı [§995](#sec-995)'teki kapak notundaki gibi harf harf doğrulayın. Model “ilgili görünsün” diye aileye ait olmayan öğeler ekler.

---
# 1016. `/packaging-material-study` — Packaging Material Study

## Türkçe prompt

> Aynı ambalaj tasarımını üç gerçek malzeme seçeneğiyle karşılaştır:
>
> - uncoated paper/card,
> - molded pulp,
> - translucent paper + card.
>
> Kamera, boyut, grafik ve ürün aynı kalsın. Yalnız malzeme kalınlığı, yüzey dokusu, kıvrım ve baskı davranışı değişsin.

## English

> Compare the same package design across three real material systems:
>
> - uncoated paper/card,
> - molded pulp,
> - translucent paper with card.
>
> Keep camera, dimensions, graphics, and product identical. Change only thickness, surface texture, folds, and print behavior.

## Neye dikkat edilmeli?

Logo, renk ve ambalaj dili bütün varyantlarda aynı kalsın; etiketteki yazıyı [§995](#sec-995)'teki kapak notundaki gibi harf harf doğrulayın. Model “ilgili görünsün” diye aileye ait olmayan öğeler ekler.

---
# 1017. `/product-hero-lock` — Ürün Geometrisi Kilidi

## Evrensel ürün bloğu

> `/product-hero-lock`

## Türkçe

> Yüklenen ürünü tek ürün referansı olarak kullan. Şişe/kutu/gövde geometrisini, kapak biçimini, oranları, logo/etiket konumunu, malzeme bitişini ve görünür parçaları değiştirme. Yalnız arka plan, yüzey, kamera veya ışığı belirtilen şekilde değiştir.

## English

> Use the uploaded product as the sole product reference. Preserve bottle/box/body geometry, closure shape, proportions, logo and label placement, material finish, and visible components. Change only the specified background, surface, camera, or lighting.

## Neye dikkat edilmeli?

Ürün geometrisi ve etiket bütün karelerde sabit kalsın; seride zemin ve ışık değişiyorsa önce hero kare onaylanır.

---
# 1018. `/label-lock` — Etiket ve Yazı Koruma

## Türkçe

> Ürün üzerindeki mevcut logo, ürün adı, tipografi, etiket boyutu, etiket konumu ve okunabilir metni değiştirme veya yeniden yazma. Ambalajın yalnız çevresel sahnesini değiştir.

## English

> Preserve the existing logo, product name, typography, label size, label position, and readable package text. Change only the environmental scene around the product.

## Neye dikkat edilmeli?

Ürün geometrisi ve etiket bütün karelerde sabit kalsın; seride zemin ve ışık değişiyorsa önce hero kare onaylanır.

---
# 1019. `/white-product` — Temiz Beyaz Fon Ürün Fotoğrafı

## Türkçe prompt

> [ÜRÜN]'ü saf beyaz arka plan üzerinde katalog/ürün veri sayfasına uygun fotoğraf olarak göster. Ürün tam görünür, merkezde veya hafif optik merkezde, doğal çok hafif temas gölgesiyle zemine otursun.
>
> Yumuşak geniş softbox benzeri aydınlatma kullan. Kenarlar net ama aşırı HDR keskinliğinde olmasın.
>
> Dekoratif props, gradient, yansımalı platform ve dramatik spotlight kullanma.

## English

> Show [PRODUCT] on a pure white background as clean catalog/product-detail photography. Keep the entire product visible, centered or optically centered, with one restrained natural contact shadow.
>
> Use broad softbox-like illumination. Keep edges clear without hyper-HDR sharpness.
>
> Avoid decorative props, gradients, reflective platforms, and dramatic spotlights.

## Neye dikkat edilmeli?

Ürünün gerçek oranı ve malzemesi korunsun; “premium” parlaklık adı altında eklenen sahte yansıma ve gölgeleri [§163](10-temeller-001-222.md#sec-163) filtresinden geçirin.

---
# 1020. `/gray-product` — Nötr Gri Hero Shot

## Türkçe prompt

> [ÜRÜN]'ü açık/nötr gri seamless fonda sade hero product photo olarak göster. Ürünün gerçek malzemesini doğru anlatacak yumuşak directional light ve çok hafif gradient kullan. Fon “premium” görünmek için siyah-gold lüks stüdyo setine dönüşmesin.

## English

> Show [PRODUCT] as a restrained hero product photograph on a light neutral-gray seamless background. Use soft directional light and only a slight tonal gradient to reveal the real material. Do not turn the background into a black-and-gold luxury set.

## Neye dikkat edilmeli?

Ürünün gerçek oranı ve malzemesi korunsun; “premium” parlaklık adı altında eklenen sahte yansıma ve gölgeleri [§163](10-temeller-001-222.md#sec-163) filtresinden geçirin.

---
# 1021. `/product-in-hand` — Ürünün Elde Kullanımı

## Türkçe

> Ürünü gerçek ölçekte tek elde doğal biçimde tutulurken göster. Parmakların ürünle temas noktaları, kavrama geometrisi ve gölgeler fiziksel olarak doğru olsun. Ürünün etiketi mümkün olduğunca görünür kalsın.
>
> Elin parmak sayısını veya ürünü tutma fiziğini bozma.

## English

> Show the product held naturally in one hand at its real scale. Keep finger contact points, grip geometry, and shadows physically plausible. Preserve label visibility where possible.
>
> Do not distort finger count or product-holding physics.

## Neye dikkat edilmeli?

Ürün geometrisi ve etiket bütün karelerde sabit kalsın; seride zemin ve ışık değişiyorsa önce hero kare onaylanır.

---
# 1022. `/product-use` — Gerçek Kullanım Anı

## Türkçe prompt

> [ÜRÜN]'ü kullanıcı tarafından gerçek işlevi sırasında göster. Poz, el yerleşimi, miktar/ölçek ve ürün yönü kullanım biçimine uygun olsun.
>
> Ürünü yalnız “elde tutulan reklam objesi” gibi göstermeyin; kullanımın fiziksel sonucu görünür olsun.

## English

> Show [PRODUCT] during its actual use by a person. Keep pose, hand placement, amount or scale, and product orientation appropriate to the function.
>
> Do not show it merely as an advertising prop being held; make the physical result of use visible.

## Neye dikkat edilmeli?

Ürünün gerçek oranı ve malzemesi korunsun; “premium” parlaklık adı altında eklenen sahte yansıma ve gölgeleri [§163](10-temeller-001-222.md#sec-163) filtresinden geçirin.

---
# 1023. `/product-detail-set` — Ürün Detay Serisi

## Türkçe

> Aynı ürünün dört görselden oluşan detay serisini oluştur:
>
> 1. tam ürün hero shot,
> 2. malzeme/finish macro,
> 3. işlevsel ayrıntı,
> 4. gerçek kullanım anı.
>
> Tüm görsellerde ürün geometrisi, renk ve etiket aynı kalsın.

## English

> Create a four-image detail set of the same product:
>
> 1. full hero shot,
> 2. material/finish macro,
> 3. functional detail,
> 4. real use moment.
>
> Preserve product geometry, color, and label across every image.

## Neye dikkat edilmeli?

Ürün geometrisi ve etiket bütün karelerde sabit kalsın; seride zemin ve ışık değişiyorsa önce hero kare onaylanır.

---
# 1024. `/product-carousel` — Sosyal Medya Ürün Serisi

## Türkçe

> Aynı ürün için 4:5 oranında beş karelik sosyal carousel serisi tasarla:
>
> 1. hero,
> 2. material close-up,
> 3. benefit/context,
> 4. use moment,
> 5. quiet closing frame.
>
> Aynı ürünü her karede tekrar ortada gösterme. Her kare farklı bilgi taşısın.

## English

> Design a five-frame 4:5 social carousel for the same product:
>
> 1. hero,
> 2. material close-up,
> 3. benefit/context,
> 4. use moment,
> 5. quiet closing frame.
>
> Do not center the same product identically in every frame. Give each image a different informational role.

## Neye dikkat edilmeli?

Ürün geometrisi ve etiket bütün karelerde sabit kalsın; seride zemin ve ışık değişiyorsa önce hero kare onaylanır.

---
# 1025. `/beauty-product` — Beauty Product Without Luxury Slop

## Türkçe prompt

> [CİLT BAKIM/KOZMETİK ÜRÜNÜ]'nü gerçek malzeme ve formu öne çıkaran editoryal ürün fotoğrafı olarak göster. Bir ana ürün, bir yüzey ve yalnız ürünle ilişkili tek çevresel unsur kullan.
>
> Sıvı damlası gerekiyorsa fiziksel olarak ürün kullanımına hizmet etsin.
>
> Altın ışık, çiçek gölgesi, mermer, cam küre, su sıçraması, petal ve “luxury” dekorlarının hepsini aynı anda kullanma.

## English

> Photograph [SKINCARE/COSMETIC PRODUCT] editorially with emphasis on its real material and form. Use one hero product, one surface, and only one contextual element genuinely related to the product.
>
> If droplets are used, they should make sense for the product.
>
> Do not combine golden lighting, botanical shadows, marble, glass spheres, water splashes, petals, and every other “luxury” cliché at once.

## Neye dikkat edilmeli?

Ürünün gerçek oranı ve malzemesi korunsun; “premium” parlaklık adı altında eklenen sahte yansıma ve gölgeleri [§163](10-temeller-001-222.md#sec-163) filtresinden geçirin.

---
# 1026. `/beverage-product` — İçecek Ürün Fotoğrafı

## Türkçe

> [İÇECEK] kutu/şişesini gerçek ürün fotoğrafı olarak göster. Yoğuşma yalnız soğuk ürünse ve gerçekçi damla boyutlarında olsun. Buz veya meyve yalnız ürünle gerçekten ilişkiliyse kullan.
>
> Şişenin/kutunun şeklini, etiketini ve renklerini değiştirme.
>
> Dev sıçrama efekti, uçuşan meyve parçaları ve patlayan buz küpleri kullanma.

## English

> Photograph the [BEVERAGE] can or bottle as a real product. Add condensation only if the product is cold and keep droplet sizes believable. Use ice or fruit only when genuinely relevant.
>
> Preserve package geometry, label, and colors.
>
> Avoid giant splash effects, flying fruit, and exploding ice cubes.

## Neye dikkat edilmeli?

Ürün geometrisi ve etiket bütün karelerde sabit kalsın; seride zemin ve ışık değişiyorsa önce hero kare onaylanır.

---
# 1027. `/jewelry-product` — Mücevher Ürün Fotoğrafı

## Türkçe

> [TAKI]'yı gerçek metal ve taş davranışını gösteren kontrollü macro/close product photograph olarak çek. Takının geometrisi, taş sayısı ve montür değişmesin.
>
> Yansıma kaynakları fiziksel ve sınırlı olsun. Taş yüzeyini daha “lüks” göstermek için fazladan facet veya taş ekleme.

## English

> Photograph [JEWELRY] in a controlled macro or close product shot that reveals real metal and gemstone behavior. Preserve geometry, stone count, and setting.
>
> Keep reflections physically plausible and restrained. Do not invent extra facets or gemstones to make the piece look “more luxurious.”

## Neye dikkat edilmeli?

Ürün geometrisi ve etiket bütün karelerde sabit kalsın; seride zemin ve ışık değişiyorsa önce hero kare onaylanır.

---
# 1028. `/product-reference-map` — Çok Referanslı Ürün Çekimi

## Türkçe

> Image 1 = ürün geometrisi ve etiket
>
> Image 2 = model/kişi kimliği
>
> Image 3 = sahne/mekân
>
> Image 4 = ışık veya kompozisyon referansı
>
> Her referans yalnız belirtilen rolü etkilesin.

## English

> Image 1 = product geometry and label  
> Image 2 = model/person identity  
> Image 3 = environment  
> Image 4 = lighting or composition reference  
>
> Let each reference influence only its assigned role.

## Neye dikkat edilmeli?

Ürün geometrisi ve etiket bütün karelerde sabit kalsın; seride zemin ve ışık değişiyorsa önce hero kare onaylanır.

---
# 1029. `/album-photo-cover` — Fotoğraftan Albüm Kapağı

## Trend

**T1/T2 — Eylül 2026’da güncel cover-art rehberlerinde aktif.**

## Türkçe prompt

> Yüklediğim portreyi 1:1 kare kurmaca albüm kapağına dönüştür.
>
> Kişi tanınabilir ana görsel olarak kalsın. Müzik türü ve duygu yalnız:
>
> - renk,
> - ışık,
> - crop,
> - yüzey/baskı karakteri,
> - tek grafik fikir
>
> üzerinden anlatılsın.
>
> Başlık gerekiyorsa kısa albüm/single adı ve sanatçı adı dışında yazı kullanma.
>
> Müzik türünün klişe ikonlarını otomatik ekleme.

## English

> Transform the uploaded portrait into a square 1:1 fictional album cover while keeping the person recognizable as the visual anchor.
>
> Express genre and mood only through color, lighting, crop, print/surface character, and one primary graphic idea.
>
> If text is used, limit it to a short release title and artist name.
>
> Do not automatically add stereotypical genre icons.

---

# 1030. `/single-cover` — Minimal Single Cover

## Türkçe

> Kurmaca single için tek ana fotoğraf/nesne ve geniş boşluk kullanan kare kapak tasarla. Parça adı küçük olabilir; sanatçı adı daha da küçük kalabilir. Spotify thumbnail boyutunda ana fikir okunabilir olsun.

## English

> Design a square cover for a fictional single using one primary photograph or object with generous negative space. The track title may be small and the artist name smaller. Keep the core idea readable at streaming-thumbnail size.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 1031. `/mixtape-cover` — Mixtape Without Genre Cliché

## Türkçe

> [MÜZİK TÜRÜ] mixtape kapağını tür klişelerini listelemek yerine tek kişisel hikâye veya mekân etrafında kur. Bir ana görsel, bir güçlü başlık ve yalnız gerektiğinde tek secondary element kullan.
>
> Para, silah, lüks otomobil, alev, parental-advisory benzeri rozet ve yoğun zincir/bling öğelerini otomatik ekleme.

## English

> Build the [GENRE] mixtape cover around one personal story or place rather than a checklist of genre clichés. Use one primary image, one strong title, and only one secondary element if needed.
>
> Do not automatically add money, weapons, luxury cars, flames, advisory-style badges, and excessive chains or bling.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 1032. `/album-contact-sheet` — Albüm Fotoğraf Contact Sheet

## Türkçe

> Aynı sanatçı/kişinin 12 karelik fotoğraf contact sheet'ini albüm kapağı veya booklet görseli olarak oluştur. Aynı çekim seansı hissini koru. 1–2 kareyi grease-pencil ile seç. Başlık gerekiyorsa contact sheet dışındaki marjda küçük kullan.

## English

> Create a 12-frame photographic contact sheet of the same artist or person for album-cover or booklet use. Keep the feeling of one continuous shoot. Mark only 1–2 frames with grease pencil. If text is needed, place it small in the outer margin.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 1033. `/album-xerox` — Xerox / Zine Album Cover

## Türkçe

> Fotoğrafı siyah-beyaz fotokopi/toner karakterine dönüştür ve albüm kapağında tek güçlü yüzey olarak kullan. Bir vurgu rengi ve tek başlık yeterli olsun. Punk/zine estetiği diye sayfayı 30 kesik kelimeyle doldurma.

## English

> Transform the photograph into black-and-white photocopy/toner character and use it as the main album-cover surface. One accent color and one title are enough. Do not fill the design with dozens of cut-out words just to signal punk or zine aesthetics.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 1034. `/album-riso` — Risograph Album Cover

## Türkçe

> [ALBÜM] kapağını iki spot renkli risograph baskı mantığında tasarla. Tek ana fotoğraf/illüstrasyon, görünür kâğıt, hafif registration kayması ve kısa tipografi kullan. Her renk kanalını rastgele kaydırma.

## English

> Design the [ALBUM] cover using two-spot-color risograph print logic. Use one main photograph or illustration, visible paper, slight registration drift, and concise typography. Do not randomly misalign every color channel.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 1035. `/album-scanner` — Scanography Album Cover

## Türkçe

> [NESNE/KUMAŞ/ÇİÇEK]'i flatbed scanner üzerinde fiziksel olarak taranmış gibi ana albüm görseline dönüştür. Camla temas eden kısımlar keskin, yukarı çıkan bölgeler hızlıca karanlık/yumuşak olsun. Tek küçük başlık kullan.

## English

> Make [OBJECT/FABRIC/FLOWERS] appear physically scanned on a flatbed scanner as the primary album-cover image. Keep areas touching the glass sharp while raised portions fall quickly into softness and darkness. Use one small title.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 1036. `/pet-toy-box` — Evcil Hayvan Koleksiyon Figürü

## Trend

**T1 — action-figure trendinin en kalıcı alt türlerinden.**

## Türkçe prompt

> Yüklediğim evcil hayvanı gerçekçi küçük koleksiyon figürüne dönüştür ve fiziksel blister packaging içinde göster.
>
> Hayvanın:
>
> - türü/ırk görünümü,
> - tüy rengi,
> - tüy desenleri,
> - kulak biçimi,
> - göz rengi,
> - yüz oranı,
> - belirgin tasma veya işaretleri
>
> korunmalı.
>
> Paket içinde yalnız 2–3 gerçekten anlamlı aksesuar kullan.
>
> Hayvanı büyük gözlü jenerik chibi karaktere dönüştürme.

## English

> Transform the uploaded pet into a believable small collectible figure inside physical blister packaging.
>
> Preserve species or breed appearance, fur color, markings, ear shape, eye color, facial proportions, and distinctive collar or markings.
>
> Include only 2–3 genuinely meaningful accessories.
>
> Do not turn the animal into a generic big-eyed chibi character.

---

# 1037. `/pet-vinyl` — Designer Pet Vinyl Toy

## Türkçe

> Evcil hayvanı sade designer vinyl toy'a dönüştür. Gerçek tüy desenini renk bloklarına sadeleştirerek koru. Kulak, burun, kuyruk ve gövde oranları hayvanın tanınmasını sağlasın. Mat vinil kullan; tüylü 3B render yapma.

## English

> Transform the pet into a restrained designer vinyl toy. Preserve real fur markings as simplified color blocks. Keep ear, nose, tail, and body proportions recognizable. Use matte vinyl rather than furry CGI rendering.

## Neye dikkat edilmeli?

Evcil hayvanın türü, tüy deseni ve boyutu bütün varyantlarda aynı kalsın; model sevimlilik uğruna anatomiyi bozar.

---
# 1038. `/pet-clay` — Handmade Clay Pet

## Türkçe

> Yüklediğim evcil hayvanı 6–10 cm el yapımı polymer clay veya hava kuruyan kil figüre dönüştür. Tüy desenini küçük boya/kil renk bölgeleriyle doğru koru. Parmak/alet izleri hafifçe görülsün. Gözleri aşırı büyütme.

## English

> Transform the uploaded pet into a 6–10 cm handmade polymer-clay or air-dry-clay figure. Preserve fur markings accurately through small painted or clay color areas. Allow subtle tool or finger marks. Do not enlarge the eyes excessively.

## Neye dikkat edilmeli?

Evcil hayvanın türü, tüy deseni ve boyutu bütün varyantlarda aynı kalsın; model sevimlilik uğruna anatomiyi bozar.

---
# 1039. `/pet-felt` — Needle-felt Pet

## Türkçe

> Evcil hayvanı needle-felt el işi figüre dönüştür. Tüy yönü yün lifleriyle belirtilsin; yüz, kulak ve gövde oranları hayvana özel kalsın. Lifli yüzey gerçek keçeleştirme davranışı göstersin. Peluş oyuncak dikişleri ekleme.

## English

> Transform the pet into a needle-felt handmade figure. Use wool fibers to suggest fur direction while preserving the animal-specific face, ear, and body proportions. Keep the surface true to felted fiber behavior. Avoid plush-toy seam construction.

## Neye dikkat edilmeli?

Evcil hayvanın türü, tüy deseni ve boyutu bütün varyantlarda aynı kalsın; model sevimlilik uğruna anatomiyi bozar.

---
# 1040. `/pet-embroidered-patch` — Pet Patch

## Türkçe

> Evcil hayvanın yüzünü 6–8 cm işlemeli patch tasarımına sadeleştir. Tüy desenleri 4–6 ana iplik rengine indirgensin. Kulak ve yüz silhouette'ı ilk bakışta tanınabilir kalsın. Mikro tüy ayrıntısı ve küçük yazı kullanma.

## English

> Simplify the pet's face into a 6–8 cm embroidered patch design. Reduce fur markings to 4–6 primary thread colors. Keep the ear and face silhouette immediately recognizable. Avoid micro fur detail and tiny text.

## Neye dikkat edilmeli?

Evcil hayvanın türü, tüy deseni ve boyutu bütün varyantlarda aynı kalsın; model sevimlilik uğruna anatomiyi bozar.

---
# 1041. `/pet-magazine` — Pet Editorial Cover

## Türkçe

> Evcil hayvanı kurmaca bağımsız pet/lifestyle dergisinin kapağında doğal portre olarak göster. Gerçek tüy, göz, kulak ve yüz kimliğini koru. Kapakta yalnız kurmaca dergi adı, bir kısa başlık ve en fazla iki küçük satır kullan.
>
> Papyon, taç veya insan kıyafeti otomatik ekleme.

## English

> Show the pet as a natural portrait on the cover of a fictional independent pet or lifestyle magazine. Preserve real fur, eyes, ears, and facial identity. Use only one fictional masthead, one short headline, and up to two small lines.
>
> Do not automatically add bow ties, crowns, or human clothing.

## Neye dikkat edilmeli?

Evcil hayvanın türü, tüy deseni ve boyutu bütün varyantlarda aynı kalsın; model sevimlilik uğruna anatomiyi bozar.

---
# 1042. `/pet-story-triptych` — Evcil Hayvan Günlük Hikâye Üçlüsü

## Türkçe

> Aynı evcil hayvanı üç karede aynı günün küçük hikâyesi olarak göster:
>
> 1. ortamı keşfederken,
> 2. yakın yüz/pati ayrıntısı,
> 3. dinlenirken.
>
> Tüy deseni, tasma, göz ve beden oranı aynı kalsın.

## English

> Show the same pet in three frames as a small story from one day:
>
> 1. exploring the environment,
> 2. close face or paw detail,
> 3. resting.
>
> Keep fur markings, collar, eyes, and body proportions consistent.

## Neye dikkat edilmeli?

Evcil hayvanın türü, tüy deseni ve boyutu bütün varyantlarda aynı kalsın; model sevimlilik uğruna anatomiyi bozar.

---
# 1043. `/pet-human-concept` — Pet-to-Human, Cliché Olmadan

## Trend

**T1/T2 — viral ama kolayca stereotipe düşüyor.**

## Türkçe prompt

> Evcil hayvanı “insan olsaydı” kurmaca karakter olarak yorumla; ancak hayvanın görünüşünden kişilik, meslek veya sosyal sınıf çıkarma.
>
> Kullanıcı tarafından verilen:
>
> - yaş aralığı,
> - kıyafet,
> - ortam,
> - davranış
>
> bilgilerine göre insan karakteri oluştur.
>
> Hayvanın tüy renklerini ve ayırt edici işaretlerini saç/kıyafet renk ilişkisine çok sınırlı görsel referans olarak aktarabilirsin.

## English

> Reimagine the pet as a fictional human character, but do not infer personality, profession, or social class from the animal's appearance.
>
> Build the human version only from user-supplied age range, clothing, environment, and behavior.
>
> Fur colors and distinctive markings may inform hair or clothing color relationships only in a restrained visual way.

---

# 1044. `/paper-world` — Entire Scene as Cut Paper

## Trend

**T2 — paper-cut animation ve Reels/Shorts üretiminde canlı.**

## Türkçe prompt

> Kaynak sahnenin tamamını fiziksel kesilmiş kâğıt dünyasına dönüştür.
>
> Her nesne:
>
> - ayrı kâğıt katmanı,
> - görünür kesilmiş kenar,
> - gerçek kâğıt kalınlığı,
> - küçük temas gölgesi
>
> ile oluşsun.
>
> Perspektif ve ana kompozisyon korunmalı.
>
> Yalnız yüzeye “paper texture” kaplama; gerçek katmanlı kâğıt yapısı kur.

## English

> Transform the entire source scene into a physical cut-paper world.
>
> Construct every object from distinct paper layers with visible cut edges, real paper thickness, and small contact shadows.
>
> Preserve perspective and primary composition.
>
> Do not merely apply paper texture; build the scene through actual layered paper logic.

---

# 1045. `/paper-stopmotion` — Paper Stop-motion Still

## Türkçe

> `/paper-world` yapısını kullan ancak sahneyi stop-motion animasyonundan tek kare gibi göster. Kâğıt parçalarında küçük elle yerleştirme sapmaları ve sınırlı frame-to-frame hareket hissi olsun. Motion blur ekleme; fiziksel yeniden konumlandırma hissi ver.

## English

> Use the `/paper-world` structure but make the scene feel like one frame from a stop-motion animation. Allow tiny hand-positioning irregularities and a sense of frame-to-frame repositioning. Avoid motion blur; suggest physical movement through placement.

## Neye dikkat edilmeli?

Malzeme fiziksel olarak kurulabilir olsun; yüzeye kaplanmış doku yerine malzemenin inşa mantığı (örgü ilmeği, ahşap damarı, karton kalınlığı) görünsün.

---
# 1046. `/ceramic-world` — Entire Scene as Ceramic

## Trend

**T3 — topluluk deneylerinde görülüyor; henüz knitted/paper kadar geniş değil.**

## Türkçe prompt

> Kaynak sahnenin tüm nesnelerini gerçek seramik/stoneware karşılıklarına dönüştür. Kütle ve kompozisyon korunmalı.
>
> Malzeme:
>
> - kil kalınlığı,
> - sır akışı,
> - mat/parlak alan farkı,
> - küçük pişirme düzensizliği,
> - gerçek seramik birleşimleri
>
> üzerinden kurulmalı.
>
> Her nesneyi yalnız parlak porselen kaplamaya dönüştürme.

## English

> Rebuild every object in the source scene as a physical ceramic or stoneware equivalent while preserving massing and composition.
>
> Construct the material through clay thickness, glaze pooling, matte/gloss variation, small firing irregularities, and plausible ceramic joins.
>
> Do not simply coat every object in glossy porcelain.

---

# 1047. `/porcelain-world` — Fine Porcelain Variant

## Türkçe

> Sahneyi ince beyaz porselen dünyaya dönüştür. İnce ama fiziksel olarak mümkün duvar kalınlıkları, yarı saydam kenar davranışı ve sınırlı sır ayrıntısı kullan. Kırılgan mikro parçaları sadeleştir.

## English

> Transform the scene into a fine white-porcelain world using thin but physically plausible wall thickness, subtle edge translucency, and restrained glaze detail. Simplify fragile micro-elements.

## Neye dikkat edilmeli?

Malzeme fiziksel olarak kurulabilir olsun; yüzeye kaplanmış doku yerine malzemenin inşa mantığı (örgü ilmeği, ahşap damarı, karton kalınlığı) görünsün.

---
# 1048. `/glass-world` — Entire Scene as Glass

## Durum

**T3 — güçlü görsel potansiyel, ancak “chrome/glass AI slop” riski yüksek.**

## Türkçe prompt

> Kaynak sahnedeki ana formları gerçek cam nesnelere dönüştür. Her nesne için cam kalınlığı, kenar refraksiyonu, iç yansıma ve ağırlık fiziksel olarak anlaşılır olsun.
>
> Şeffaflık nesnenin yapısını yok etmesin.
>
> Her yüzeyi holografik, iridescent veya chrome yapma. Yalnız şeffaf/renkli cam davranışı kullan.

## English

> Rebuild the primary forms in the source scene as real glass objects. Make glass thickness, edge refraction, internal reflection, and weight physically readable.
>
> Do not let transparency destroy structural clarity.
>
> Avoid holographic, iridescent, and chrome treatment; use only plausible clear or colored glass behavior.

## Neye dikkat edilmeli?

Cam saydamlık mantığı tutarlı olsun; iç içe geçen yansımalar konuyu okunmaz hâle getiriyorsa öğe sayısını azaltın.

---
# 1049. `/wood-world` — Carved Wooden World

## Türkçe

> Tüm sahneyi fiziksel olarak oyulmuş ahşap maket dünyasına dönüştür. Ahşap damar yönü nesne formlarına göre değişsin; birleşim ve oyma izleri görülebilsin.
>
> Binalar, insanlar ve nesneler tek parça plastik gibi pürüzsüz görünmesin.

## English

> Rebuild the entire scene as a physically carved wooden model world. Let grain direction follow object geometry and show plausible joins and carving marks.
>
> Avoid smooth plastic-like surfaces on buildings, people, and objects.

## Neye dikkat edilmeli?

Malzeme fiziksel olarak kurulabilir olsun; yüzeye kaplanmış doku yerine malzemenin inşa mantığı (örgü ilmeği, ahşap damarı, karton kalınlığı) görünsün.

---
# 1050. `/cardboard-world` — Cardboard World

## Türkçe

> Kaynak sahneyi yalnız mukavva/karton, baskılı kâğıt ve basit yapıştırma teknikleriyle yapılmış fiziksel model dünyasına dönüştür.
>
> Kesilmiş oluklu kart kenarları, katlama çizgileri, slot/tab bağlantıları ve hafif baskı grafikleri görülsün.
>
> Profesyonel CGI low-poly görüntüye dönüşmesin.

## English

> Transform the source scene into a physical model world made only from cardboard, printed paper, and simple adhesive construction.
>
> Show cut corrugated edges, fold lines, slot/tab joins, and restrained printed graphics.
>
> Avoid polished CGI low-poly styling.

## Neye dikkat edilmeli?

Malzeme fiziksel olarak kurulabilir olsun; yüzeye kaplanmış doku yerine malzemenin inşa mantığı (örgü ilmeği, ahşap damarı, karton kalınlığı) görünsün.

---
# 1051. `/material-world-grid` — Aynı Sahnenin 6 Malzemesi

## Türkçe

> Aynı sahneyi 2×3 grid içinde altı fiziksel malzeme dünyasında göster:
>
> 1. knitted,
> 2. felt,
> 3. paper,
> 4. ceramic,
> 5. wood,
> 6. cardboard.
>
> Kamera, kompozisyon, özne sayısı ve ana renk ilişkileri aynı kalsın. Yalnız üretim malzemesi ve onun fiziksel davranışı değişsin.

## English

> Show the same scene in a 2×3 grid across six physical material worlds:
>
> 1. knitted,
> 2. felt,
> 3. paper,
> 4. ceramic,
> 5. wood,
> 6. cardboard.
>
> Keep camera, composition, subject count, and primary color relationships identical. Change only material and its physical construction behavior.

## Neye dikkat edilmeli?

Malzeme fiziksel olarak kurulabilir olsun; yüzeye kaplanmış doku yerine malzemenin inşa mantığı (örgü ilmeği, ahşap damarı, karton kalınlığı) görünsün.

---
# 1052. `/product-to-packaging-board` — Ürün Fotoğrafından Ambalaj Sistemi

## Türkçe prompt

> Yüklenen ürünü ana referans olarak kullan.
>
> Üst yarıda ürünün kendisini aynen koru.
>
> Alt yarıda ürünün:
>
> - geometrisi,
> - malzemesi,
> - mevcut renkleri,
> - kullanım biçimi,
> - hedef bağlamı
>
> üzerinden yeni ama ürünle uyumlu packaging identity system üret.
>
> Ürünün mevcut tasarımını veya logosunu yeniden tasarlama; yalnız destekleyici packaging family tasarla.

## English

> Use the uploaded product as the primary reference.
>
> Preserve the product itself exactly in the upper half.
>
> In the lower half, build a new but compatible packaging identity system from the product's geometry, material, existing colors, use case, and context.
>
> Do not redesign the product or its existing logo; design only the supporting packaging family.

## Neye dikkat edilmeli?

Logo, renk ve ambalaj dili bütün varyantlarda aynı kalsın; etiketteki yazıyı [§995](#sec-995)'teki kapak notundaki gibi harf harf doğrulayın. Model “ilgili görünsün” diye aileye ait olmayan öğeler ekler.

---
# 1053. `/product-board-slop-filter` — Ürün/Paketleme AI Slop Filtresi

Kaçınılması gerekenler:

- “premium” denince siyah + altın,
- beauty product denince çiçek gölgesi + su damlası + marble,
- beverage denince dev splash,
- tech product denince neon hologram,
- sustainable packaging denince her şeyi kraft kâğıda boyamak,
- packaging board'da 15 taşıyıcı,
- her yüzeyde aynı logo,
- bütün mockup'ları 45 derece izometrik açıyla dizmek,
- fiziksel üretim mantığı olmayan die-cut,
- ürün geometrisini sessizce değiştirmek,
- etiketi yeniden yazmak,
- gerçek ürün yerine “benzeri” bir AI ürün oluşturmak.

---

<a id="sec-1054"></a>
# 1054. `/album-cover-slop-filter` — Albüm Kapağı AI Slop Filtresi

Kaçınılması gerekenler:

- rap = para + araba + zincir + alev,
- rock = kırık font + skull,
- electronic = neon portal,
- indie = solmuş film + rastgele serif,
- jazz = saxophone silhouette,
- pop = parlak gradient + lens flare,
- her kapakta dev yüz,
- 8 farklı font,
- telifli mevcut albüm kapağının varyasyonu.

Daha iyi soru:

> **Bu müziğin tek görsel fikri nedir?**

*Benzer: [§2417](34-katalog-aile-077-133.md#sec-2417) — üretim ve format hatalarına odaklı ikinci filtre.*

---

# 1055. `/pet-slop-filter` — Evcil Hayvan Dönüşümlerinde AI Slop

Kaçınılması gerekenler:

- her hayvanı büyük gözlü chibi yapmak,
- tüy desenini kaybetmek,
- kulak biçimini değiştirmek,
- tüm kedileri aynı yuvarlak figüre çevirmek,
- pet-to-human dönüşümünde görünüşten kişilik/meslek çıkarmak,
- her hayvana papyon, taç veya gözlük eklemek,
- aynı hayvanı sticker grid içinde farklı hayvanlara dönüştürmek.

---

# 1056. TikTok 2026 sinyali: “Reali-TEA”

TikTok’un resmî 2026 trend raporu “Reali-TEA” başlığı altında **fazla kusursuz/fantastik içerikten daha gerçek, meraklı, insani ve biraz dağınık anlatıya** yönelimi vurguluyor.

Bu, görsel prompt rehberinde şu ilkeyle örtüşüyor:

> AI görüntüsü “insan eli değmiş gibi” görünmek için rastgele kusur eklememeli.
>
> Daha iyi yöntem:
>
> **gerçek kullanım izi + gerçek fizik + gerçek bağlam + sınırlı kusur.**

Bu nedenle:

> `/lived-in`
>
> `/direct-flash`
>
> `/mid-bite`
>
> `/used-product`
>
> `/photo-dump`

gibi promptlar yalnız stil değil, 2026’nın daha geniş görsel davranışıyla da uyumludur.

---

# 1057. `/human-not-perfect` — Reali-TEA Görsel Bloğu

## Türkçe

> Görüntüyü kusursuz reklam estetiği yerine gerçek insan kullanımına yakın tut. Yalnız bağlama uygun küçük kusurlar göster: hafif eğri kadraj, küçük kullanım izi, doğal cilt, eksik lokma, açık defter veya elde çekim hareketi gibi.
>
> Rastgele dağınıklık, kir, yırtık, kahve lekesi veya yoğun film hasarı ekleme.

## English

> Keep the image closer to real human use than flawless advertising aesthetics. Show only context-appropriate minor imperfections such as a slightly tilted frame, subtle use marks, natural skin, a missing bite, an open notebook, or small handheld movement.
>
> Avoid random mess, dirt, tears, coffee stains, and excessive film damage.

## Neye dikkat edilmeli?

Gerçekçilik iddiası abartılmasın: gözenek ve asimetri tamamen silinmişse sonuç illüstrasyondur, fotoğraf gibi sunulmaz.

---
# 1058. Yeni üst aile: `Source-to-System`

Önceki ailelere yeni bir üst sınıf eklenebilir:

> **Source-to-System — Tek bir kaynak görselden tutarlı bir görsel sistem üretme**

Bu aile şunları kapsar:

- `/packaging-board`
- `/brand-from-photo`
- `/product-to-packaging-board`
- `/editorial-split`
- `/album-photo-cover`
- `/same-person-grid`
- `/material-world-grid`
- `/pet-sticker-sheet`

Ortak yapı:

> **Kaynak → korunacak çekirdek → çıkarılacak özellik → yeni taşıyıcılar → tutarlılık kuralı**

---

# 1059. `Source-to-System` prompt formülü

## Türkçe

> Kaynak görselde değişmeyecek çekirdeği tanımla.
>
> Ardından kaynaktan yalnız şu görsel bilgileri çıkar:
>
> - biçim,
> - renk,
> - ritim,
> - malzeme,
> - sembol,
> - duygu/bağlam.
>
> Bunları [N] farklı çıktıya dönüştür.
>
> Her çıktı aynı sisteme ait olsun ancak aynı kompozisyonun tekrarı olmasın.

## English

> Define the source elements that must remain unchanged.
>
> Extract only the following reusable visual information:
>
> - form,
> - color,
> - rhythm,
> - material,
> - symbol,
> - mood/context.
>
> Transform these into [N] different outputs.
>
> Keep every output within one system without repeating the same composition.

---

# 1060. Bu turdaki yeni slash-style indeks (aile-012)

| Kısayol | Aile |
|---|---|
| `/packaging-board` | photo-to-packaging identity board |
| `/brand-from-photo` | source photo → visual identity |
| `/carrier-select` | functional packaging-format selection |
| `/packaging-family` | coherent multi-format packaging |
| `/packaging-material-study` | same package, different materials |
| `/product-hero-lock` | preserve exact product geometry |
| `/label-lock` | preserve package label/text |
| `/white-product` | clean white-background product shot |
| `/gray-product` | neutral hero product shot |
| `/product-in-hand` | believable product-in-hand image |
| `/product-use` | real use moment |
| `/product-detail-set` | hero + macro + function + use |
| `/product-carousel` | five-frame social product series |
| `/beauty-product` | beauty image without luxury clichés |
| `/beverage-product` | beverage image without splash cliché |
| `/jewelry-product` | geometry-locked jewelry macro |
| `/product-reference-map` | assign roles to product references |
| `/album-photo-cover` | portrait/photo album cover |
| `/single-cover` | minimal single artwork |
| `/mixtape-cover` | genre cover without clichés |
| `/album-contact-sheet` | photographic contact-sheet cover |
| `/album-xerox` | Xerox/zine music cover |
| `/album-riso` | risograph music cover |
| `/album-scanner` | scanography music cover |
| `/pet-toy-box` | pet collectible packaging |
| `/pet-vinyl` | designer pet vinyl toy |
| `/pet-clay` | handmade clay pet |
| `/pet-felt` | needle-felt pet |
| `/pet-embroidered-patch` | pet embroidery patch |
| `/pet-magazine` | fictional pet editorial cover |
| `/pet-story-triptych` | same-pet narrative series |
| `/pet-human-concept` | user-directed pet-to-human concept |
| `/paper-world` | entire scene in cut paper |
| `/paper-stopmotion` | paper stop-motion still |
| `/ceramic-world` | entire scene in ceramic |
| `/porcelain-world` | fine porcelain world |
| `/glass-world` | physically plausible glass world |
| `/wood-world` | carved wooden world |
| `/cardboard-world` | cardboard model world |
| `/material-world-grid` | same scene in six materials |
| `/product-to-packaging-board` | product → packaging system |
| `/human-not-perfect` | controlled real-life imperfection |

---

<a id="aile-013"></a>
# Spor, Otomotiv, Logo, Tattoo, Gıda Ambalajı ve Retro GUI — 2026 Ek Taraması

Bu turda şehir/seyahat ve portre dışına çıkarak altı alan tarandı:

- spor ve taraftar grafikleri,
- otomotiv fotoğrafçılığı,
- logo/emblem sistemleri,
- tattoo/flash tasarımı,
- gıda ve içecek ambalajı,
- retro web/GUI estetikleri.

2026 sinyallerinde ortak eğilim yine aynı: **AI ile kolayca üretilebilen steril ve birbirine benzeyen görseller yerine daha özgül, elde yapılmış, fiziksel, yerel veya kültürel olarak tanınabilir görsel sistemler** öne çıkıyor.

Pinterest'in 2026 yaz raporunda sporun yalnız maç izlemekten çıkarak forma, renk, grafik, moda, güzellik ve günlük kimliğe yayılan bir görsel dil hâline geldiği belirtiliyor. Logo trend raporlarında ise freehand mascots, hand-drawn imperfection, stamp/seal ve esnek logo sistemleri belirgin. Retro UI tarafında Windows 98 / klasik Mac / Y2K / brutalist arayüz estetiklerinin 2026'da modern web tasarımında yeniden kullanıldığı görülüyor.

---

# 1061. `/sports-hero` — Sporcu Hero Poster

## Trend

**T1 — kalıcı ve geniş.**

## Türkçe prompt

> [SPORCU]'yu 4:5 dikey spor hero posterinin ana odağı olarak göster.
>
> Tek ana portre veya aksiyon karesi kullan. Arka planda yalnız:
>
> - takım rengi,
> - tek büyük numara,
> - kısa isim,
> - gerekirse tek doku
>
> bulunsun.
>
> Aynı sporcunun üç farklı dev kopyasını arka plana ekleme. Duman, kıvılcım, yıldırım, lens flare ve parçacık efektlerini otomatik kullanma.
>
> Sporcu kimliği, forma numarası ve takım renkleri doğru kalmalı.

## English

> Present [ATHLETE] as the main focus of a vertical 4:5 sports hero poster.
>
> Use one primary portrait or action image. Limit the background to team color, one large number, one concise name, and at most one supporting texture.
>
> Do not add multiple giant duplicate portraits of the athlete or automatic smoke, sparks, lightning, lens flare, and particle effects.
>
> Preserve identity, jersey number, and team colors accurately.

---

# 1062. `/matchday-poster` — Matchday Poster

## Trend

**T1 — sosyal spor içeriğinin ana formatlarından.**

## Türkçe prompt

> [TAKIM A] vs [TAKIM B] için 4:5 matchday poster oluştur.
>
> Hiyerarşi:
>
> 1. maç,
> 2. tarih/saat,
> 3. stadyum/şehir,
> 4. iki takımın görsel kimliği.
>
> Tek bir güçlü sporcu veya sembol kullanılabilir.
>
> Score yazma; maç henüz oynanmadıysa sonuç uydurma.
>
> Logoları değiştirme veya yeni arma üretme.

## English

> Create a vertical 4:5 matchday poster for [TEAM A] vs [TEAM B].
>
> Information hierarchy:
>
> 1. fixture,
> 2. date/time,
> 3. stadium/city,
> 4. team identity.
>
> Use at most one strong player or symbolic visual.
>
> Do not invent a score for an unplayed match and do not redesign team crests.

---

# 1063. `/game-result` — Sonuç Grafiği

## Türkçe prompt

> Oynanmış [MAÇ] için sade sonuç posteri oluştur. Skoru en büyük bilgi olarak göster; takım isimleri, tarih ve gerekiyorsa tek oyuncu fotoğrafı ikincil olsun.
>
> Gerçek skor/veri kullanıcı tarafından verilmediyse uydurma. “WIN”, “VICTORY”, “GAME OVER” gibi üç ayrı büyük sloganı aynı anda kullanma.

## English

> Create a restrained result poster for a completed [MATCH]. Make the score the dominant information, with team names, date, and at most one player image as secondary elements.
>
> Do not invent results if the actual score is not supplied. Avoid stacking multiple giant slogans such as “WIN”, “VICTORY”, and “GAME OVER”.

## Neye dikkat edilmeli?

Skor, isim ve istatistik model tarafından uydurulur; karttaki her sayı kaynaktan doğrulanır. Yazı denetimi [§995](#sec-995)'teki kapak notundaki gibi harf harf yapılır.

---
# 1064. `/player-stat-card` — Sporcu İstatistik Kartı

## Ne zaman kullanılır?

Gerçek veriyi görsel olarak özetlemek için.

## Türkçe prompt

> [SPORCU] için tek maçlık veya sezonluk istatistik kartı tasarla. Kullanıcı tarafından verilen yalnız 4–6 ana metriği göster.
>
> Sporcu fotoğrafı tek tarafta; sayılar ve kısa metrik adları diğer tarafta düzenli grid içinde olsun.
>
> Veri üretme veya eksik değerleri tahmin etme.

## English

> Design a match or season stat card for [ATHLETE]. Show only 4–6 key metrics explicitly supplied by the user.
>
> Place one athlete image on one side and organize numbers with concise metric labels in a clean grid on the other.
>
> Do not invent or estimate missing statistics.

## Neye dikkat edilmeli?

Skor, isim ve istatistik model tarafından uydurulur; karttaki her sayı kaynaktan doğrulanır. Yazı denetimi [§995](#sec-995)'teki kapak notundaki gibi harf harf yapılır.

---
# 1065. `/sports-number-poster` — Numara Odaklı Spor Posteri

## Trend

**TREND — bold typography + sports identity.**

## Türkçe prompt

> [SPORCU]'nun forma numarasını posterin ana grafik öğesi yap. Sporcu tek küçük/orta figür olarak numara ile kontrollü biçimde ilişkilensin.
>
> Numara okunabilir ve doğru olsun. Aynı sayıyı arka planda onlarca kez tekrar etme.

## English

> Make the athlete's jersey number the main graphic element of the poster. Integrate one small or medium athlete figure with the number in a controlled composition.
>
> Keep the number accurate and readable. Do not repeat it dozens of times in the background.

---

# 1066. `/sports-contact-sheet` — Spor Fotoğraf Contact Sheet

## Türkçe prompt

> Aynı maç/antreman çekiminden 12 karelik sports contact sheet oluştur.
>
> Seri:
>
> - aksiyon,
> - yüz ifadesi,
> - ekipman,
> - seyirci,
> - kısa dinlenme,
> - saha ayrıntısı
>
> gibi farklı anları içersin.
>
> 1–2 kareyi grease-pencil işaretiyle seçilmiş gibi göster.

## English

> Create a 12-frame sports contact sheet from one match or training session.
>
> Include varied moments such as action, expression, equipment, crowd, brief rest, and field detail.
>
> Mark only 1–2 frames as selected with grease-pencil notation.

## Neye dikkat edilmeli?

Skor, isim ve istatistik model tarafından uydurulur; karttaki her sayı kaynaktan doğrulanır. Yazı denetimi [§995](#sec-995)'teki kapak notundaki gibi harf harf yapılır.

---
# 1067. `/fan-poster` — DIY Taraftar Posteri

## Trend

**T2 — 2026 US Open gibi etkinliklerde handmade fan art/merch görünürlüğü yüksek.**

## Türkçe prompt

> [TAKIM/SPORCU/ETKİNLİK] için profesyonel kulüp grafiği yerine taraftarın kendi yaptığı özgün poster hissi oluştur.
>
> El çizimi harf, sınırlı boya/marker, tek ana fotoğraf veya illüstrasyon ve birkaç yerel/maça özgü küçük referans kullan.
>
> Resmî logo/marka tasarımını değiştirme ve sahte resmî ürün izlenimi verme.

## English

> Create an original fan-made poster for [TEAM/ATHLETE/EVENT] rather than an official club graphic.
>
> Use hand-drawn lettering, limited paint or marker texture, one main photo or illustration, and a few small event-specific references.
>
> Do not redesign official marks or imply that the work is official merchandise.

---

# 1068. `/retro-sports-card` — Retro Spor Kartı

## Türkçe prompt

> [SPORCU]'yu 1970–1990 arası spor kartı baskı dilinden esinlenen kurmaca collectible card üzerinde göster.
>
> Ön yüzde tek portre/aksiyon, isim ve takım bilgisi; arka yüzde yalnız kullanıcı tarafından verilen kısa istatistik alanları olsun.
>
> Mevcut kart markasını veya tarihî kart tasarımını bire bir kopyalama.

## English

> Present [ATHLETE] on a fictional collectible card inspired by 1970s–1990s sports-card print language.
>
> Use one portrait or action image with name and team on the front; place only user-supplied concise statistics on the back.
>
> Do not copy an existing card brand or historical card layout exactly.

## Neye dikkat edilmeli?

Skor, isim ve istatistik model tarafından uydurulur; karttaki her sayı kaynaktan doğrulanır. Yazı denetimi [§995](#sec-995)'teki kapak notundaki gibi harf harf yapılır.

---
# 1069. `/motorsport-poster` — Motorsport Event Poster

## Türkçe prompt

> [ARAÇ/TAKIM/YARIŞ] için motorsport poster oluştur. Hızı yalnız motion blur, tyre marks veya yönsel tipografi gibi 1–2 araçla anlat.
>
> Araç geometrisini ve livery detaylarını değiştirme.
>
> Her yere alev, kıvılcım, duman ve yarış damalı desen ekleme.

## English

> Create a motorsport poster for [CAR/TEAM/RACE]. Express speed through only 1–2 devices such as directional motion blur, tire marks, or kinetic typography.
>
> Preserve vehicle geometry and livery details.
>
> Avoid automatic flames, sparks, smoke, and checkered patterns everywhere.

## Neye dikkat edilmeli?

Skor, isim ve istatistik model tarafından uydurulur; karttaki her sayı kaynaktan doğrulanır. Yazı denetimi [§995](#sec-995)'teki kapak notundaki gibi harf harf yapılır.

---
# 1070. `/rolling-shot` — Automotive Rolling Shot

## Trend

**EVERGREEN / otomotiv çekiminin temel dili.**

## Türkçe prompt

> [ARAÇ]'ı gerçek hareket hâlinde yandan veya 3/4 açıdan rolling shot olarak göster. Araç gövdesi ve logo/livery keskin kalsın; tekerleklerde dönüş blur'u ve arka planda yönsel hareket blur'u olsun.
>
> Kamera araçla benzer hızda ilerliyormuş gibi fiziksel hareket mantığı kur.

## English

> Show [CAR] in a real rolling shot from the side or three-quarter angle. Keep the vehicle body and livery sharp while showing wheel rotation blur and directional background motion.
>
> Make the camera feel as if it is traveling at a similar speed to the car.

---

# 1071. `/car-panning` — Panning Car Photograph

## Türkçe

> [ARAÇ]'ı yol üzerinde panning tekniğiyle çekilmiş gibi göster. Araç yeterince keskin, yol ve arka plan yatay hareket çizgileriyle bulanık olsun. Tekerleklerde dairesel dönüş blur'u kullan.
>
> Aracın kaporta çizgilerini blur ile eritme.

## English

> Photograph [CAR] using a panning technique. Keep the car reasonably sharp while rendering the road and background as directional horizontal motion blur. Show circular wheel-rotation blur.
>
> Do not dissolve the vehicle's body lines into the blur.

## Neye dikkat edilmeli?

Far, jant, plaka ve ayna simetrisini kontrol edin; hareket karesinde zemin ve tekerlek bulanıklığı aynı hızı anlatsın.

---
# 1072. `/car-direct-flash` — Parking-lot Direct Flash

## Trend

**TREND — otomotivde casual/social görünüm.**

## Türkçe prompt

> [ARAÇ]'ı gece otoparkta küçük kamera/telefon doğrudan flaşıyla çekilmiş doğal snapshot gibi göster. Flaş aracın yakın panelinde ve plakaya/reflector yüzeylere göre fiziksel davranmalı.
>
> Arka plan hızlıca kararsın.
>
> Profesyonel studio rim light ekleme.

## English

> Show [CAR] as a nighttime parking-lot snapshot taken with direct phone or compact-camera flash. Let the flash behave physically across nearby body panels, license plate, and reflective surfaces.
>
> Allow the background to fall off quickly.
>
> Avoid professional studio rim lighting.

---

# 1073. `/gas-station-car` — Gas-station Car Portrait

## Trend

**EVERGREEN / street automotive.**

## Türkçe prompt

> [ARAÇ]'ı gerçek bir benzin istasyonunda gece veya blue-hour sırasında göster. Işık yalnız istasyon kanopisi, pompa ekranları ve çevresel gerçek kaynaklardan gelsin.
>
> Aracı cyberpunk neon vitrinine dönüştürme. Pompa, hortum ve park geometrisi fiziksel olarak doğru olsun.

## English

> Show [CAR] at a believable gas station during night or blue hour. Let illumination come only from the canopy, pump displays, and other plausible environmental sources.
>
> Avoid cyberpunk neon styling. Keep pump, hose, and parking geometry physically coherent.

---

# 1074. `/car-detail` — Automotive Detail Macro

## Türkçe

> [ARAÇ]'ın tek önemli tasarım ayrıntısına yakın plan odaklan: far, jant, fren kaliperi, kapı kolu, kumaş/deri dikişi veya badge gibi.
>
> Parçanın gerçek geometrisini değiştirme. Üretici logosu varsa doğru biçimde koru.

## English

> Focus closely on one meaningful design detail of [CAR], such as headlight, wheel, brake caliper, door handle, upholstery stitching, or badge.
>
> Preserve real geometry and any visible manufacturer mark accurately.

## Neye dikkat edilmeli?

Far, jant, plaka ve ayna simetrisini kontrol edin; hareket karesinde zemin ve tekerlek bulanıklığı aynı hızı anlatsın.

---
# 1075. `/car-white-studio` — Otomotiv Katalog Stüdyosu

## Türkçe prompt

> [ARAÇ]'ı büyük beyaz cyclorama stüdyosunda temiz katalog çekimi olarak göster. Tüm araç görünür olsun. Zeminde doğal yumuşak temas gölgesi ve gövde formunu okuyacak kontrollü reflection kullan.
>
> Aracın model/geometri/aksesuarlarını değiştirme.

## English

> Show [CAR] in a large white cyclorama as clean catalog photography. Keep the entire vehicle visible with one restrained contact shadow and controlled reflections revealing body shape.
>
> Preserve model geometry and accessories exactly.

## Neye dikkat edilmeli?

Far, jant, plaka ve ayna simetrisini kontrol edin; dönem transferinde model modern detay (LED far, güncel logo) sızdırır.

---
# 1076. `/car-spec-card` — Araç Teknik Özellik Kartı

## Türkçe

> [ARAÇ] için katalog tarzı spec card oluştur. Kullanıcı tarafından verilen yalnız 5–7 ana veriyi göster: motor, güç, tork, ağırlık, 0–100, menzil/kapasite vb.
>
> Veri uydurma. Bir ana araç görseli ve sade tipografik grid yeterli olsun.

## English

> Design a catalog-style specification card for [CAR]. Show only 5–7 metrics supplied by the user, such as engine, power, torque, weight, acceleration, range, or capacity.
>
> Do not invent data. Use one main vehicle image and a restrained typographic grid.

## Neye dikkat edilmeli?

Far, jant, plaka ve ayna simetrisini kontrol edin; hareket karesinde zemin ve tekerlek bulanıklığı aynı hızı anlatsın.

---
# 1077. `/car-contact-sheet` — Automotive Contact Sheet

## Türkçe prompt

> Aynı araç çekiminden 12 karelik contact sheet oluştur. Aynı araç, renk, jant, body kit ve plaka ayrıntıları tüm karelerde aynı olsun.
>
> Wide 3/4, side profile, front, rear, detail, interior ve rolling frame karışımı kullan.

## English

> Create a 12-frame contact sheet from one automotive shoot. Preserve the exact car, color, wheels, body kit, and license-plate details across every frame.
>
> Mix wide three-quarter, profile, front, rear, detail, interior, and rolling views.

## Neye dikkat edilmeli?

Far, jant, plaka ve ayna simetrisini kontrol edin; dönem transferinde model modern detay (LED far, güncel logo) sızdırır.

---
# 1078. `/car-era-transfer` — Aracı Döneme Taşıma

## Türkçe prompt

> [ARAÇ]'ın kendisini değiştirmeden çevresini [1980/1990/2000] dönemine taşı. Yol, tabela, benzin istasyonu, sokak lambası ve fotoğraf davranışı döneme uygun olsun.
>
> Modern aracı eski modele dönüştürme.

## English

> Move the environment around [CAR] into the [1980s/1990s/2000s] without changing the vehicle itself. Make roads, signage, gas stations, street lighting, and photographic behavior period-appropriate.
>
> Do not redesign the modern car into an older model.

## Neye dikkat edilmeli?

Far, jant, plaka ve ayna simetrisini kontrol edin; dönem transferinde model modern detay (LED far, güncel logo) sızdırır.

---
# 1079. `/freehand-mascot` — Freehand Mascot Logo

## Trend

**T1/T2 — 2026 logo raporlarında güçlü.**

## Türkçe prompt

> [MARKA/KONU] için elde çizilmiş freehand mascot logo oluştur. Maskot:
>
> - tek güçlü silhouette,
> - temiz ama hafif kusurlu line weight,
> - çok az yüz ayrıntısı,
> - 2–3 düz renk
>
> kullansın.
>
> Küçük sticker ve büyük tabela ölçeğinde tanınabilir kalsın.
>
> Rubber-hose kol/bacak, beyaz eldiven ve retro cartoon yüzünü otomatik ekleme.

## English

> Create a hand-drawn freehand mascot logo for [BRAND/SUBJECT]. Use one strong silhouette, clean but slightly imperfect line weight, very limited facial detail, and 2–3 flat colors.
>
> Keep the mascot recognizable at both sticker and signage scale.
>
> Do not automatically add rubber-hose limbs, white gloves, and generic retro-cartoon facial features.

---

# 1080. `/naive-logo` — Kontrollü Kusurlu Logo

## Trend

**T1 — 2026'da “too perfect” logolara tepki olarak güçlü.**

## Türkçe prompt

> [MARKA] için kontrollü naive/handmade logo oluştur.
>
> Yalnız bir veya iki kasıtlı kusur kullan:
>
> - hafif eğri çizgi,
> - küçük asimetri,
> - tek el yazısı karakter,
> - düzensiz ama okunur stroke.
>
> Logonun tümünü acemi çizimine dönüştürme.

## English

> Create a controlled naive or handmade logo for [BRAND].
>
> Use only one or two deliberate imperfections such as a slightly uneven line, small asymmetry, one hand-lettered character, or irregular but readable stroke.
>
> Do not make the entire mark look amateurishly drawn.

---

# 1081. `/stamp-logo` — Stamp / Seal Logo

## Trend

**T1 — heritage ve craft kategorilerinde kalıcı.**

## Türkçe prompt

> [MARKA] için fiziksel damga basımına uygun stamp/seal logo oluştur. Yuvarlak veya oval dış sınır, kısa marka adı ve yalnız 1–2 merkezi sembol kullan.
>
> Tek renk basıldığında okunabilir kalsın.
>
> Mikro yazı, ince gölge ve çok ayrıntılı arma kullanma.

## English

> Create a stamp or seal logo for [BRAND] suitable for physical ink stamping. Use a round or oval boundary, concise brand name, and only 1–2 central symbols.
>
> Keep it readable in one-color printing.
>
> Avoid micro-text, thin shadows, and overly detailed heraldry.

---

# 1082. `/adaptive-logo` — Adaptive Logo System

## Trend

**T1/T2 — tek logodan çok esnek kimlik sistemi.**

## Türkçe prompt

> [MARKA] için aynı çekirdek kimliği koruyan dört logo varyantı oluştur:
>
> 1. full wordmark + symbol,
> 2. yatay logo,
> 3. yalnız sembol,
> 4. küçük favicon/app icon.
>
> Dört varyant birbirinin farklı logosu değil, aynı sistemin responsive sürümleri olsun.

## English

> Create four responsive variants for [BRAND] while preserving one core identity:
>
> 1. full wordmark + symbol,
> 2. horizontal logo,
> 3. symbol only,
> 4. small favicon or app icon.
>
> Make them responsive versions of the same system rather than four unrelated logos.

---

# 1083. `/custom-wordmark` — Custom Typographic Logo

## Trend

**T1 — 2026 bold/custom typography.**

## Türkçe prompt

> [MARKA ADI]'nı logonun kendisi olacak özgün wordmark olarak tasarla. Harflerin yalnız 1–2 noktasında markaya özel yapısal müdahale yap.
>
> Okunabilirliği koru.
>
> Her harfi farklı şekle sokma, bubble/chrome/gradient efektlerini otomatik ekleme.

## English

> Design [BRAND NAME] as a custom wordmark that functions as the logo itself. Introduce only 1–2 brand-specific structural modifications in the letterforms.
>
> Preserve readability.
>
> Do not distort every letter or automatically add bubble, chrome, and gradient effects.

---

# 1084. `/little-blip-logo` — Tek Kontrollü Sapma

## Trend

**TREND — “controlled imperfection” kimliği.**

## Türkçe prompt

> Son derece sade [MARKA] logosunda yalnız bir küçük beklenmedik özellik kullan: bir harfin hafif taşması, noktanın farklı konumu, küçük asimetrik kesik veya tek elde çizilmiş ayrıntı.
>
> Bu “blip” markanın ayırt edici unsuru olsun; geri kalan yapı düzenli kalsın.

## English

> Use one small unexpected feature in an otherwise restrained [BRAND] logo: a slightly protruding letter, displaced dot, asymmetrical notch, or one hand-drawn detail.
>
> Let this single “blip” become the distinctive feature while keeping the rest structurally disciplined.

---

# 1085. `/logo-family-board` — Logo Sistem Panosu

## Türkçe

> [MARKA] logo sistemini tek board üzerinde göster:
>
> - ana logo,
> - responsive varyantlar,
> - tek renk,
> - ters kullanım,
> - minimum boyut örneği,
> - sembol.
>
> Mockup sayısını sınırlı tut; logo dosyasını kahve bardağı ve tote bag üzerinde göstermek yerine sistem davranışını anlat.

## English

> Show the [BRAND] logo system on one board using the primary logo, responsive variants, one-color version, reversed use, minimum-size example, and symbol.
>
> Limit mockups and prioritize system behavior over showing the mark on cups and tote bags.

## Neye dikkat edilmeli?

Logo bütün varyantlarda aynı kalsın; küçük boyutta test edilmeyen ayrıntı sistemden çıkarılır.

---
# 1086. `/fine-line-tattoo` — Fine-line Tattoo Flash

## Trend

**T1 — kalıcı; ancak iyileşme/ölçek sınırı önemli.**

## Türkçe prompt

> [TEMA] için 6 parçalık fine-line tattoo flash sheet oluştur. İnce ama gerçek dövmede uygulanabilecek line weight, sınırlı shading ve açık negatif alan kullan.
>
> Tasarımları çok küçük ölçekte kaybolacak mikro detaylarla doldurma.
>
> Yalnız beyaz zeminde flash tasarımı göster; gerçek cilde uygulama mockup'u ayrıca istenmedikçe ekleme.

## English

> Create a six-piece fine-line tattoo flash sheet around [THEME]. Use thin but practically tattooable line weight, limited shading, and open negative space.
>
> Avoid micro-details that would collapse at small scale.
>
> Show only the flash designs on white unless a skin-placement mockup is explicitly requested.

---

# 1087. `/microrealism-tattoo` — Micro-realism Tattoo Concept

## Trend

**T1/T2 — 2026 tattoo trend raporlarında güçlü.**

## Türkçe prompt

> [KONU]'yu küçük micro-realism tattoo tasarımına dönüştür. Tek ana nesne veya portre, kontrollü tonal aralık ve dış kontur yerine küçük gerçekçi değer geçişleri kullan.
>
> Tasarımın gerçek dövme ölçüsünde hangi ayrıntıların korunabileceğini düşün; fotoğrafın tüm mikro detaylarını zorla sığdırma.

## English

> Transform [SUBJECT] into a small micro-realism tattoo concept using one primary object or portrait and controlled tonal transitions rather than heavy outer outlines.
>
> Consider which details can survive at real tattoo scale rather than forcing every photographic micro-detail into the design.

---

# 1088. `/botanical-tattoo` — Botanical Tattoo Flash

## Trend

**T1 — evergreen.**

## Türkçe prompt

> [BİTKİ] için botanik doğruluğu korunmuş tattoo flash tasarla. Yaprak dizilişi, çiçek biçimi ve gövde ilişkisi gerçek bitkiye uygun olsun.
>
> Stil [fine-line / engraving / blackwork] olabilir.
>
> Rastgele dekoratif yapraklar ekleyerek tür kimliğini değiştirme.

## English

> Design tattoo flash for [PLANT] while preserving botanical accuracy in leaf arrangement, flower form, and stem relationships.
>
> Style may be [fine-line / engraving / blackwork].
>
> Do not add random decorative foliage that changes the species identity.

---

# 1089. `/patchwork-tattoo-sheet` — Patchwork Tattoo Collection

## Trend

**T1 — büyümeye devam ediyor.**

## Türkçe prompt

> Aynı kişisel tema etrafında 8 küçük tattoo motifinden patchwork sleeve collection sheet oluştur.
>
> Her motif bağımsız çalışsın; ortak line/shading diline sahip olsun.
>
> Aralarında gerçek ciltte nefes alacak negatif alan bırakılabilecek boyut/yoğunluk düşün.

## English

> Create a patchwork sleeve collection sheet of eight small tattoo motifs around one personal theme.
>
> Let every motif work independently while sharing line and shading language.
>
> Design with enough open spacing to allow breathable negative space on real skin.

---

# 1090. `/blackwork-negative` — Blackwork + Negative Space

## Trend

**T1/T2.**

## Türkçe prompt

> [TEMA]'yı yüksek kontrast blackwork tattoo olarak tasarla. Büyük siyah kütleler ile açık negatif alanlar arasında net yapı kur.
>
> Negatif alan yalnız süs değil, ana motifin okunmasını sağlayan aktif biçim olsun.
>
> Her yeri siyaha kaplayıp okunabilirliği kaybetme.

## English

> Design [THEME] as a high-contrast blackwork tattoo using clear structure between large black masses and open negative space.
>
> Make negative space an active part of the motif rather than decoration.
>
> Avoid filling everything solid black until the design loses readability.

---

# 1091. `/fluid-tattoo` — Fluid / Flow Tattoo

## Trend

**T2 — 2026'da yükselen alanlardan.**

## Türkçe prompt

> [TEMA]'yı su, duman veya kaligrafik fırça hareketini çağrıştıran akışkan tattoo formuna dönüştür. Hareket vücut anatomisine göre tek ana yönde ilerlesin.
>
> Rastgele ornamental swirl üretme; ana konu ile hareket arasında görsel ilişki kur.

## English

> Transform [THEME] into a fluid tattoo composition inspired by water, smoke, or calligraphic brush movement. Let the flow follow one primary direction appropriate to body anatomy.
>
> Avoid random ornamental swirls; make movement relate meaningfully to the subject.

---

# 1092. `/cybersigil-flash` — Cybersigilism-inspired Flash

## Trend

**T1/T2 — 2026'da görünür ancak hızlı eskime riski var.**

## Türkçe prompt

> [KAVRAM]'ı ince, sivri, simetrik/asimetrik dijital-sigil çizgi yapısına dönüştür. Tasarım tek renk siyah flash olarak okunabilir olsun.
>
> Gerçek dinî/okült sembolleri anlamını bilmeden rastgele birleştirme. Gerekirse yalnız özgün soyut çizgi sistemi kullan.

## English

> Transform [CONCEPT] into a thin, sharp digital-sigil line structure with controlled symmetry or asymmetry. Keep the design readable as one-color black flash.
>
> Do not randomly combine real religious or occult symbols without context; use an original abstract line system when appropriate.

---

# 1093. `/script-tattoo` — Personal Lettering Tattoo

## Trend

**T1 — kişisel lettering güçleniyor.**

## Türkçe prompt

> [KISA İFADE/İSİM]'i tattoo için özgün lettering olarak tasarla. Harfler küçük ölçekte okunabilir, stroke kalınlığı uygulanabilir ve karakter aralıkları dengeli olsun.
>
> Kullanıcının açıkça istemediği uzun şiir veya alıntı ekleme.
>
> Yazım ve dil kullanıcı tarafından doğrulanmalı.

## English

> Design [SHORT PHRASE/NAME] as original tattoo lettering with readable small-scale forms, practical stroke thickness, and balanced spacing.
>
> Do not add long poetry or quotations unless explicitly requested.
>
> Final spelling and language should be verified by the user.

---

# 1094. `/tattoo-placement` — Anatomik Yerleşim Mockup'u

## Türkçe prompt

> Hazır tattoo tasarımını [ÖN KOL / BALDIR / OMUZ / SIRT] üzerinde gerçek ölçek ve cilt kıvrımına uygun yerleşim mockup'u olarak göster.
>
> Tasarımın kendisini değiştirme; yalnız yüzey eğriliğine göre perspektif ve hafif deformasyon uygula.
>
> Cilt üzerinde gereksiz kızarıklık, kan veya yeni yapılmış dövme efekti kullanma.

## English

> Show the finished tattoo design as a placement mockup on [FOREARM / CALF / SHOULDER / BACK] at believable scale and following body curvature.
>
> Do not redesign the tattoo; apply only perspective and mild deformation needed for the surface.
>
> Avoid unnecessary redness, blood, and fresh-tattoo effects.

## Neye dikkat edilmeli?

Yerleşim önizlemesinde tasarımın ters basılmadığını ve vücut kıvrımında bozulmadığını kontrol edin; kalıcı karar öncesi geçici uygulamayla test edin.

---
# 1095. Tattoo promptlarında fiziksel gerçeklik notu

AI ile üretilen güzel bir flash:

> **doğrudan uygulanabilir tattoo stencil değildir.**

Gerçek uygulamada:

- çizgi kalınlığı,
- boyut,
- cilt bölgesi,
- iyileşme,
- pigment davranışı,
- sanatçının tekniği

tasarımı değiştirebilir.

Bu nedenle prompt sonucu:

> **tasarım referansı / konuşma başlangıcı**

olarak görülmelidir.

---

# 1096. `/retro-food-pack` — Retro Food Packaging

## Trend

**T1/T2 — heritage refresh ve nostaljik ambalaj 2026'da güçlü.**

## Türkçe prompt

> [GIDA ÜRÜNÜ] için tarihî marka estetiğinden esinlenen ama özgün retro ambalaj tasarla.
>
> Tek dönemi seç: [1950s / 1970s / 1990s].
>
> Tipografi, renk, fotoğraf/illüstrasyon ve baskı davranışı o döneme uyumlu olsun.
>
> Ambalaj güncel ürün bilgisi için yeterli okunabilir alan taşısın.
>
> Yalnız sepya filtre ve “Since 19xx” yazısıyla retro görünüm yaratma.

## English

> Design original retro packaging for [FOOD PRODUCT] inspired by one specific period: [1950s / 1970s / 1990s].
>
> Make typography, color, photography or illustration, and print behavior consistent with the selected era.
>
> Preserve enough readable space for modern product information.
>
> Do not create retro styling merely through sepia and a fake “Since 19xx” label.

---

# 1097. `/heritage-refresh` — Heritage Brand Refresh

## Trend

**T2 — güncel büyük gıda markalarında görülen yaklaşım.**

## Türkçe prompt

> Mevcut [MARKA]'nın tanınabilir çekirdek işaretini koruyarak packaging refresh konsepti oluştur.
>
> Korunacak:
>
> - ana logo/simge,
> - temel marka rengi,
> - ürün adı,
> - ana ürün kimliği.
>
> Güncellenecek:
>
> - tipografik hiyerarşi,
> - ürün fotoğrafı/illüstrasyonu,
> - renk berraklığı,
> - bilgi düzeni.
>
> “Yenileme” bahanesiyle markayı tamamen yeniden tasarlama.

## English

> Create a packaging-refresh concept for an existing [BRAND] while preserving its recognizable core.
>
> Preserve the primary mark, core brand color, product name, and product identity.
>
> Update typographic hierarchy, food photography or illustration, color clarity, and information organization.
>
> Do not use “refresh” as an excuse to redesign the brand completely.

---

# 1098. `/food-window-pack` — Ürünü Gösteren Pencereli Ambalaj

## Türkçe prompt

> [GIDA]'yı gerçekten gösterecek küçük şeffaf pencereye sahip ambalaj tasarla. Pencere ürünün en karakteristik fiziksel bölümünü gösterecek yerde olsun.
>
> Pencere biçimini gereksiz dekoratif kalbe/yıldıza dönüştürme.
>
> Film/plastik kullanımı gerekiyorsa minimum fiziksel alanla sınırla.

## English

> Design packaging for [FOOD] with a small transparent window revealing the most characteristic physical part of the actual product.
>
> Avoid decorative heart or star window shapes unless contextually meaningful.
>
> Keep any required transparent film area minimal.

## Neye dikkat edilmeli?

Logo, renk ve ambalaj dili bütün varyantlarda aynı kalsın; etiketteki yazıyı [§995](#sec-995)'teki kapak notundaki gibi harf harf doğrulayın. Model “ilgili görünsün” diye aileye ait olmayan öğeler ekler.

---
# 1099. `/bakery-box` — Fırın/Pastane Kutusu

## Türkçe

> [ÜRÜN] için gerçek ölçülerine uygun karton bakery box tasarla. Ürünün ezilmemesi, taşınması ve açıldığında görülebilmesi için doğru yükseklik/boşluk düşün.
>
> Kutuda marka adı, küçük ürün etiketi ve gerekirse basit pencere yeterli olsun.

## English

> Design a cardboard bakery box sized realistically for [PRODUCT]. Allow enough height and clearance for transport without crushing the food and make opening/presentation practical.
>
> Limit graphics to the brand name, a small product label, and an optional simple window.

## Neye dikkat edilmeli?

Ambalajdaki yemek fotoğrafı ya da illüstrasyonu gerçek içeriği vaat etsin; etiketteki yazı harf harf doğrulanır.

---
# 1100. `/flavor-system` — Tat/Çeşit Ambalaj Sistemi

## Türkçe

> Aynı ürünün [N] farklı çeşidini tek packaging family olarak tasarla.
>
> Değişmeyen:
>
> - logo konumu,
> - ürün adı hiyerarşisi,
> - temel grid,
> - paket geometrisi.
>
> Değişen:
>
> - ana renk,
> - tek ingredient/illustration cue,
> - flavor adı.
>
> Her çeşidi tamamen başka marka gibi tasarlama.

## English

> Design [N] flavor variants of the same product as one packaging family.
>
> Keep logo position, product-name hierarchy, primary grid, and package geometry fixed.
>
> Change only main color, one ingredient or illustration cue, and flavor name.
>
> Do not make every flavor look like a separate brand.

## Neye dikkat edilmeli?

Ambalajdaki yemek fotoğrafı ya da illüstrasyonu gerçek içeriği vaat etsin; etiketteki yazı harf harf doğrulanır.

---
# 1101. `/seasonal-pack` — Seasonal Limited Edition

## Türkçe prompt

> Mevcut [ÜRÜN] ambalajını [MEVSİM/ÖZEL GÜN] için limited edition olarak yorumla.
>
> Ana markayı ve ürün hiyerarşisini koru. Sezonu yalnız 1–2 kontrollü görsel unsurla anlat.
>
> Noel/kış = otomatik kar tanesi; sonbahar = otomatik yaprak; yaz = otomatik palmiye klişesinden kaçın.

## English

> Reinterpret the existing [PRODUCT] packaging as a limited edition for [SEASON/OCCASION].
>
> Preserve the core brand and product hierarchy. Communicate the season through only 1–2 controlled visual elements.
>
> Avoid automatic snowflakes for winter, leaves for autumn, and palm trees for summer.

## Neye dikkat edilmeli?

Logo, renk ve ambalaj dili bütün varyantlarda aynı kalsın; etiketteki yazıyı [§995](#sec-995)'teki kapak notundaki gibi harf harf doğrulayın. Model “ilgili görünsün” diye aileye ait olmayan öğeler ekler.

---
# 1102. `/shelf-family` — Raf Üzerinde Ambalaj Ailesi

## Türkçe

> [MARKA]'nın 6 ürünlük packaging family'sini gerçek mağaza rafında yan yana göster.
>
> Her paket ayrı okunabilirken tüm aile 2–3 metre uzaktan ortak marka bloğu oluşturmalı.
>
> Rafı e-ticaret mockup gridine dönüştürme.

## English

> Show a six-product packaging family for [BRAND] on a believable retail shelf.
>
> Let each package read individually while the full range forms one recognizable brand block from 2–3 meters away.
>
> Avoid e-commerce-grid presentation.

## Neye dikkat edilmeli?

Ambalajdaki yemek fotoğrafı ya da illüstrasyonu gerçek içeriği vaat etsin; etiketteki yazı harf harf doğrulanır.

---
# 1103. `/food-photo-pack` — Ambalaj Üzerinde Gerçek Yemek Fotoğrafı

## Türkçe

> [ÜRÜN] ambalajında tek hero food photograph kullan. Fotoğraf gerçek ürünün porsiyon, doku ve içerik yapısını doğru temsil etsin.
>
> Servis önerisi ise küçük şekilde belirtilmek üzere alan bırak.
>
> Ürünü gerçekte olduğundan daha dolgun veya ingredient-rich gösterme.

## English

> Use one hero food photograph on [PRODUCT] packaging. Make the image accurately represent the real product's portion, texture, and ingredient structure.
>
> Leave a small area for a serving-suggestion note when needed.
>
> Do not make the product appear fuller or more ingredient-rich than it actually is.

## Neye dikkat edilmeli?

Ambalajdaki yemek fotoğrafı ya da illüstrasyonu gerçek içeriği vaat etsin; etiketteki yazı harf harf doğrulanır.

---
# 1104. `/food-illustrated-pack` — İllüstrasyonlu Gıda Ambalajı

## Türkçe

> [GIDA]'yı doğrudan fotoğraf yerine sade fiziksel/edityorial illüstrasyonla anlatan ambalaj oluştur.
>
> İllüstrasyon ürünün gerçek biçim ve ana içeriğini tanınabilir göstermeli.
>
> Her yiyeceğe gülümseyen yüz, el, ayak ekleyip karaktere dönüştürme.

## English

> Design packaging for [FOOD] using restrained editorial illustration rather than photography.
>
> Keep the real product form and primary ingredient recognizable.
>
> Do not automatically anthropomorphize every food item with faces, arms, and legs.

## Neye dikkat edilmeli?

Ambalajdaki yemek fotoğrafı ya da illüstrasyonu gerçek içeriği vaat etsin; etiketteki yazı harf harf doğrulanır.

---
# 1105. `/classic-mac-ui` — Classic Mac-inspired Interface

## Trend

**T1/T2 — 2026 retro OS tasarımında güçlü.**

## Türkçe prompt

> [İÇERİK]'i 1980'ler sonu–1990'lar klasik Macintosh arayüzünden esinlenen pencerelerde düzenle.
>
> Siyah-beyaz veya sınırlı gri sistem paleti, ince bitmap ikonlar, küçük title bar, net pencere sınırı ve gerçek eski masaüstü düzeni kullan.
>
> Modern yuvarlak kart, glassmorphism ve büyük gradient ekleme.
>
> Gerçek Apple logosunu veya bire bir tarihî sistem ekranını kopyalama.

## English

> Arrange [CONTENT] inside windows inspired by late-1980s to 1990s classic Macintosh interfaces.
>
> Use black-and-white or restrained gray system colors, small bitmap icons, compact title bars, clear window borders, and believable old-desktop organization.
>
> Avoid modern rounded cards, glassmorphism, and large gradients.
>
> Do not copy real Apple logos or exact historical screens.

---

# 1106. `/win98-ui` — Windows 98-inspired Interface

## Trend

**T1/T2 — modern retro web'de aktif.**

## Türkçe prompt

> [İÇERİK]'i Windows 98 dönemini çağrıştıran masaüstü/pencere düzeninde göster.
>
> Gri UI chrome, inset/outset 3B borders, küçük bitmap ikonlar, klasik title bar ve taskbar benzeri alt şerit kullan.
>
> Görsel dili referans al ama gerçek işletim sistemi ekranını bire bir taklit etme.

## English

> Present [CONTENT] in a desktop/window composition inspired by Windows 98.
>
> Use gray UI chrome, inset/outset borders, small bitmap icons, compact title bars, and a taskbar-like lower strip.
>
> Reference the visual language without reproducing an exact operating-system screen.

---

# 1107. `/brutalist-ui` — Web Brutalism

## Trend

**T1/T2 — steril SaaS tasarımına karşı tepki olarak güçlü.**

## Türkçe prompt

> [SAYFA/İÇERİK]'i web brutalism estetiğinde tasarla.
>
> Düz arka plan, sert 1–3 px border, sistem/sans/mono tipografi, açık grid ve doğrudan işlevsel bağlantılar kullan.
>
> “Brutalist” diye bilinçli olarak kötü kullanılabilirlik, üst üste binmiş okunmayan yazı veya rastgele neon renk kullanma.

## English

> Design [PAGE/CONTENT] using web-brutalist language with flat backgrounds, hard 1–3 px borders, system/sans/mono typography, explicit grid structure, and direct functional links.
>
> Do not interpret “brutalist” as deliberately unusable layout, overlapping unreadable text, or random neon colors.

---

# 1108. `/y2k-ui` — Y2K Interface

## Trend

**T1/T2 — 2026'da görünür.**

## Türkçe prompt

> [İÇERİK]'i 1998–2003 Y2K arayüz estetiğinde tasarla.
>
> Yalnız 3–4 karakteristik unsur seç:
>
> - chrome/metallic heading,
> - bitmap/pixel text,
> - pill-shaped glossy button,
> - küçük starburst,
> - translucent colored plastic UI cue.
>
> Hepsini aynı anda kullanma.
>
> Modern SaaS gridini yalnız chrome gradient ile boyayıp “Y2K” deme.

## English

> Design [CONTENT] using 1998–2003 Y2K interface language.
>
> Choose only 3–4 characteristic cues such as chrome or metallic heading, bitmap or pixel text, pill-shaped glossy buttons, small starbursts, or translucent colored-plastic UI elements.
>
> Do not use every cue at once.
>
> Avoid simply recoloring a modern SaaS grid with chrome gradients and calling it Y2K.

---

# 1109. `/os-window-poster` — Retro OS Window Poster

## Türkçe

> [KONU]'yu poster içinde 2–3 eski işletim sistemi penceresi üzerinden anlat. Bir pencere ana içerik, diğerleri kısa destek bilgi taşısın.
>
> Pencereyi gerçek kullanıcı arayüzü gibi hiyerarşik kullan; 15 farklı popup ile ekranı doldurma.

## English

> Explain [TOPIC] in a poster using 2–3 old-OS-inspired windows. Give one window the primary content role and use the others for concise supporting information.
>
> Preserve interface hierarchy and avoid filling the image with dozens of popups.

## Neye dikkat edilmeli?

Dönem arayüzü bugünün alışkanlıklarını sızdırmasın; yazı denetimi [§995](#sec-995)'teki kapak notundaki gibi yapılır.

---
# 1110. `/pixel-icon-sheet` — Pixel Icon Sheet

## Trend

**EVERGREEN / retro UI.**

## Türkçe prompt

> [TEMA] için 16 veya 32 px grid mantığında 12 pixel icon oluştur. Her ikon aynı grid, pixel density ve outline davranışını kullansın.
>
> Anti-aliasing veya yumuşak vector curve kullanma.
>
> Her ikon küçük boyutta okunabilir tek silhouette taşısın.

## English

> Create twelve pixel icons for [THEME] using a 16- or 32-pixel grid logic. Keep grid, pixel density, and outline behavior consistent.
>
> Avoid anti-aliasing and soft vector curves.
>
> Give every icon one readable small-scale silhouette.

---

# 1111. `/dialog-poster` — Dialog Box Poster

## Trend

**TREND — retro-tech sosyal poster.**

## Türkçe

> [MESAJ]'ı büyük tek retro dialog box içinde poster olarak göster. Başlık çubuğu, kısa mesaj, 1–2 button ve küçük sistem ikonu yeterli olsun.
>
> Gerçek hata kodu veya işletim sistemi mesajını bire bir kopyalama.
>
> Espriyi arayüz işlevinden çıkar; sticker kalabalığı ekleme.

## English

> Present [MESSAGE] as a poster inside one large retro dialog box. Use a title bar, concise message, 1–2 buttons, and one small system icon.
>
> Do not copy a real OS error message or code exactly.
>
> Let the visual joke come from interface logic rather than sticker clutter.

---

# 1112. `/desktop-files` — Desktop File Composition

## Türkçe

> [KONU]'yu eski bilgisayar masaüstündeki 6–8 dosya/klasör ikonu üzerinden görsel hikâye olarak anlat. Dosya adları kısa ve anlamlı olsun.
>
> Her dosyanın anlamı farklı olsun; ekrana yüzlerce ikon saçma.

## English

> Tell a visual story about [TOPIC] through 6–8 file and folder icons on an old-computer-inspired desktop. Keep filenames concise and meaningful.
>
> Give each item a distinct role and avoid scattering hundreds of icons across the screen.

## Neye dikkat edilmeli?

Dönem arayüzü bugünün alışkanlıklarını sızdırmasın; yazı denetimi [§995](#sec-995)'teki kapak notundaki gibi yapılır.

---
# 1113. `/browser-1999` — Late-1990s Browser Page

## Türkçe

> [İÇERİK]'i 1998–2000 döneminin kişisel web sitesi gibi yorumla:
>
> - dar sabit genişlik,
> - küçük bitmap/gif-benzeri grafikler,
> - underline linkler,
> - açık background,
> - basit table-layout hissi.
>
> Ancak metin okunabilir ve hiyerarşi anlaşılır kalsın.
>
> Sayfayı bilinçli olarak bozuk Geocities parodisine dönüştürme.

## English

> Reinterpret [CONTENT] as a late-1990s personal website using a narrow fixed-width layout, small bitmap or GIF-like graphics, underlined links, light background, and simple table-layout feeling.
>
> Preserve readability and hierarchy.
>
> Do not turn it into a deliberately broken Geocities parody.

## Neye dikkat edilmeli?

Dönem arayüzü bugünün alışkanlıklarını sızdırmasın; yazı denetimi [§995](#sec-995)'teki kapak notundaki gibi yapılır.

---
# 1114. `/retro-ui-slop-filter` — Retro UI AI Slop Filtresi

Kaçınılması gerekenler:

- retro = yalnız pixel font,
- Y2K = chrome + pembe/mavi gradient + sparkle,
- brutalist = kötü hizalama,
- Win98 = bütün ekranı 20 popup ile doldurmak,
- classic Mac = yalnız siyah-beyaz pixel icon,
- her arayüzde sahte “ERROR” penceresi,
- gerçek marka/OS ekranını bire bir kopyalamak,
- okunabilirliği tamamen feda etmek.

Daha doğru soru:

> **O dönemin arayüzünü hangi teknik kısıt ve kontrol dili oluşturuyordu?**

---

# 1115. `/sports-slop-filter` — Spor Poster AI Slop Filtresi

Kaçınılması gerekenler:

- sporcunun üç dev kopyası,
- alev + duman + kıvılcım + yıldırım,
- her yere motion blur,
- yanlış forma numarası,
- uydurma skor ve istatistik,
- takım armasını yeniden çizmek,
- dev 3B isim,
- her posterin siyah/koyu arka plan olması.

---

# 1116. `/car-slop-filter` — Otomotiv AI Slop Filtresi

Kaçınılması gerekenler:

- jant/model değişmesi,
- yanlış far geometrisi,
- logo/badge mutasyonu,
- her gece çekimini cyberpunk yapmak,
- gerçeğe aykırı tekerlek dönüşü,
- body panel çizgilerinin kaybolması,
- yansımaların ışık kaynaklarıyla uyuşmaması,
- aracın farklı karelerde farklı body kit'e dönüşmesi.

---

# 1117. `/logo-slop-filter` — Logo AI Slop Filtresi

Kaçınılması gerekenler:

- generic geometric monogram,
- “premium” = serif + gold,
- her mascot = rubber hose,
- sahte heraldry,
- üç ayrı sembolü anlamsızca birleştirme,
- aşırı ince detay,
- küçük ölçekte okunmayan slogan,
- mockup güzel olduğu için kötü logoyu iyi sanmak.

---

# 1118. `/food-pack-slop-filter` — Gıda Ambalajı AI Slop Filtresi

Kaçınılması gerekenler:

- ürün fotoğrafını gerçekte olduğundan zengin göstermek,
- heritage = “Since 1897” uydurmak,
- organic = kraft + yeşil yaprak,
- premium = siyah + altın,
- çocuk ürünü = her ingredient'a yüz çizmek,
- her çeşidi farklı marka gibi tasarlamak,
- zorunlu olmayan plastik pencere,
- sahte sertifika/ödül/rozet.

---

# 1119. Bu turdaki slash-style indeks (aile-013)

| Kısayol | Aile |
|---|---|
| `/sports-hero` | athlete hero poster |
| `/matchday-poster` | fixture poster |
| `/game-result` | score/result visual |
| `/player-stat-card` | athlete statistics card |
| `/sports-number-poster` | jersey-number poster |
| `/sports-contact-sheet` | sports contact sheet |
| `/fan-poster` | handmade fan graphic |
| `/retro-sports-card` | fictional sports collectible card |
| `/motorsport-poster` | motorsport graphic |
| `/rolling-shot` | automotive rolling shot |
| `/car-panning` | panning car photograph |
| `/car-direct-flash` | parking-lot flash car |
| `/gas-station-car` | gas-station automotive portrait |
| `/car-detail` | automotive detail macro |
| `/car-white-studio` | clean catalog car shot |
| `/car-spec-card` | vehicle spec visual |
| `/car-contact-sheet` | same-car shoot grid |
| `/car-era-transfer` | same car in historical environment |
| `/freehand-mascot` | freehand mascot logo |
| `/naive-logo` | controlled imperfect logo |
| `/stamp-logo` | stamp/seal mark |
| `/adaptive-logo` | responsive logo family |
| `/custom-wordmark` | custom typographic logo |
| `/little-blip-logo` | one controlled logo imperfection |
| `/logo-family-board` | logo system presentation |
| `/fine-line-tattoo` | fine-line flash |
| `/microrealism-tattoo` | micro-realism tattoo concept |
| `/botanical-tattoo` | botanically grounded tattoo |
| `/patchwork-tattoo-sheet` | patchwork tattoo collection |
| `/blackwork-negative` | blackwork + negative space |
| `/fluid-tattoo` | fluid tattoo composition |
| `/cybersigil-flash` | cybersigil-inspired abstract flash |
| `/script-tattoo` | custom tattoo lettering |
| `/tattoo-placement` | body placement mockup |
| `/retro-food-pack` | period-inspired food packaging |
| `/heritage-refresh` | heritage packaging refresh |
| `/food-window-pack` | transparent-window food pack |
| `/bakery-box` | bakery packaging |
| `/flavor-system` | flavor packaging family |
| `/seasonal-pack` | seasonal limited edition |
| `/shelf-family` | retail-shelf packaging system |
| `/food-photo-pack` | food-photo packaging |
| `/food-illustrated-pack` | illustrated food packaging |
| `/classic-mac-ui` | classic Mac-inspired interface |
| `/win98-ui` | Windows 98-inspired interface |
| `/brutalist-ui` | web brutalism |
| `/y2k-ui` | controlled Y2K interface |
| `/os-window-poster` | retro window poster |
| `/pixel-icon-sheet` | consistent pixel icons |
| `/dialog-poster` | retro dialog graphic |
| `/desktop-files` | desktop-file visual story |
| `/browser-1999` | late-1990s web layout |

---

# 1120. Yeni üst aile: `Identity / Object / Data Lock`

Rehberde giderek tekrar eden koruma talimatları üç ana kilit sistemine ayrılabilir:

### Identity Lock

İnsan veya evcil hayvan kimliğini korur.

> `/identity-lock`

### Object Lock

Ürün, otomobil, landmark veya fiziksel nesnenin geometrisini korur.

> `/product-hero-lock`
>
> aynı mantıkla `/object-lock`

### Data Lock

Skor, sayı, koordinat, tarih, fiyat veya istatistik gibi doğrulanabilir bilgiyi korur.

> `/data-lock`

Bu üç kilit özellikle uzun viral master promptları sadeleştirmek için çok değerlidir.

---

# 1121. `/object-lock` — Nesne Geometrisi Koruma Bloğu

## Türkçe

> Kaynak nesnenin ana geometrisini, parça sayısını, oranlarını, bağlantılarını, renklerini ve ayırt edici işaretlerini değiştirme. Yalnız belirtilen görsel stil, çevre veya malzemeyi değiştir.

## English

> Preserve the source object's core geometry, part count, proportions, connections, colors, and distinctive markings. Change only the specified visual style, environment, or material.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 1122. `/data-lock` — Doğrulanabilir Bilgi Koruma Bloğu

## Türkçe

> Görselde kullanılacak tüm skor, tarih, sayı, koordinat, fiyat, istatistik ve teknik değeri yalnız kullanıcı tarafından verilen veya ayrıca doğrulanmış veriden kullan. Eksik veriyi tasarım amacıyla uydurma.

## English

> Use only user-supplied or separately verified scores, dates, numbers, coordinates, prices, statistics, and technical values. Do not invent missing data for visual completeness.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 1123. Yeni ana formül: `LOCK + TRANSFORM + FORMAT`

Artık rehberde yüzlerce promptu daha kısa ve sistematik biçimde kullanmak mümkün:

### İnsan

> `/identity-lock + /ccd-night + /magazine-cover`

### Ürün

> `/product-hero-lock + /gray-product`

### Otomobil

> `/object-lock + /rolling-shot`

### Şehir

> `/data-lock + /map-emboss`

### Spor

> `/identity-lock + /data-lock + /sports-hero`

### Evcil hayvan

> `/identity-lock + /pet-felt`

### Ambalaj

> `/object-lock + /flavor-system + /shelf-family`

Bu ifadeler yine teknik ChatGPT syntax'ı değildir.

Bunlar rehberin:

> **koru → dönüştür → çıktı biçimini belirle**

mantığını kısa biçimde temsil eder.

---

<a id="aile-014"></a>
# Handmade Hacker, Cyberdeck, Kişisel Yayın, Koleksiyon ve Müze Görselleri — 2026 Ek Taraması

Pinterest'in 25 Ağustos 2026 tarihli Hobbies Trend Report'u, görsel prompt rehberi açısından önemli bir kümeyi ayrı başlık altında topluyor: **Handmade Hacker**.

Rapordaki dikkat çekici arama artışlarından bazıları:

- `birthday magazine template` +1713%
- `tracking journal` +1264%
- `cyberdeck` +1410%
- `cyberdeck diy` +691%
- `terminal aesthetic` +559%
- `diy blind bags printable templates` +507%
- `book log journal` +482%
- `digital zine design` +433%
- `headphones painting ideas` +436%
- `crochet wired headphones` +382%
- `diy photo album book` +306%
- `tunnel book template` +237%
- `memory box ideas` +156%

Bunların ortak noktası “retro” olmaları değildir.

> **Kullanıcı, hazır ve anonim bir nesneyi kendi medyasına veya kendi cihazına dönüştürüyor.**

Bu nedenle aşağıdaki prompt ailesi, yalnız estetik değil **kişiselleştirme mantığı** üzerinden kurulmalıdır.

---

# 1124. `/birthday-magazine` — Kişisel Doğum Günü Dergisi

## Trend

**T1/T2 — Pinterest'te +1713%.**

## Türkçe prompt

> [KİŞİ] için 8–12 sayfalık küçük kişisel birthday magazine konsepti oluştur.
>
> Dergi tek bir uzun kutlama posteri gibi değil, gerçek küçük yayın gibi bölümlensin:
>
> - kapak,
> - kısa giriş,
> - 2–3 fotoğraf hikâyesi,
> - “bu yıl” sayfası,
> - arkadaşlardan kısa not alanı,
> - küçük zaman çizgisi,
> - kapanış sayfası.
>
> Fotoğrafları aşırı filtreleme. Her sayfaya balon, konfeti, pasta ve “Happy Birthday” tekrarları ekleme.
>
> Görsel dil kişinin gerçek ilgi alanlarından türesin.

## English

> Create an 8–12 page personal birthday-magazine concept for [PERSON].
>
> Structure it like a real small publication rather than one long celebration poster:
>
> - cover,
> - short introduction,
> - 2–3 photo stories,
> - “this year” page,
> - space for short notes from friends,
> - small timeline,
> - closing page.
>
> Avoid heavy photo filters and repeating balloons, confetti, cakes, and “Happy Birthday” on every page.
>
> Derive the visual language from the person's actual interests.

---

# 1125. `/birthday-cover` — Birthday Magazine Cover

## Türkçe

> [KİŞİ]'yi kurmaca kişisel doğum günü dergisinin kapağında göster. Tek ana fotoğraf, kurmaca dergi adı, yaş/yıl bilgisi ve en fazla iki kısa cover line kullan.
>
> “Birthday Queen/King”, taç, konfeti ve pembe-altın şablonlarını otomatik kullanma.

## English

> Show [PERSON] on the cover of a fictional personal birthday magazine. Use one main photograph, one fictional magazine title, age or year information, and no more than two short cover lines.
>
> Avoid automatic “Birthday Queen/King” language, crowns, confetti, and pink-gold templates.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 1126. `/year-in-review-magazine` — Bir Yılın Kişisel Dergisi

## Türkçe prompt

> [YIL] boyunca yaşanan önemli anları 12–16 sayfalık kişisel year-in-review magazine olarak düzenle.
>
> Bölümler:
>
> - insanlar,
> - yerler,
> - yapılan işler,
> - öğrenilenler,
> - küçük gündelik anlar.
>
> Her sayfayı “başarı” ve “milestone” grafiğine dönüştürme. Sessiz, sıradan ve anlamlı anlara da yer ver.

## English

> Arrange meaningful moments from [YEAR] into a 12–16 page personal year-in-review magazine.
>
> Organize sections around people, places, things made, things learned, and small everyday moments.
>
> Do not turn every page into achievements and milestones; include quiet ordinary moments as part of the story.

## Neye dikkat edilmeli?

Görseldeki yazıyı harf harf okuyun; model başlık ve isimlerde harf uydurur. Uzun metin gerekiyorsa yazıyı görsele değil açıklamaya koyun, kapakta yalnız kısa ve doğrulanmış başlık kalsın.

---
# 1127. `/tracking-journal` — Takip Günlüğü

## Trend

**T1/T2 — Pinterest'te +1264%.**

## Türkçe prompt

> [ALIŞKANLIK/PROJE] için bir aylık tracking journal spread tasarla.
>
> Sayfada yalnız gerçekten takip edilecek 3–5 değişken bulunsun.
>
> Günler okunabilir grid içinde yer alsın; kullanıcı kalemle işaret koyabilecek boş alan bulsun.
>
> Günlüğü motivasyon sözü, sticker ve dekoratif ikonlarla doldurma.

## English

> Design a one-month tracking-journal spread for [HABIT/PROJECT].
>
> Include only 3–5 variables that will genuinely be tracked.
>
> Keep days in a readable grid with enough blank space for handwritten marks.
>
> Avoid filling the journal with motivational quotes, stickers, and decorative icons.

---

# 1128. `/analog-progress-log` — Fiziksel İlerleme Günlüğü

## Türkçe

> [PROJE] ilerlemesini fiziksel defter üzerinde tarih + kısa not + küçük görsel kanıt düzeniyle göster.
>
> Her kayıt:
>
> - tarih,
> - ne yapıldı,
> - ne değişti,
> - bir sonraki küçük adım
>
> alanlarından oluşsun.
>
> Dashboard gibi KPI kartları kullanma.

## English

> Show [PROJECT] progress in a physical notebook using date, concise note, and small visual evidence.
>
> Each entry should contain date, what was done, what changed, and one next step.
>
> Avoid KPI-dashboard cards.

## Neye dikkat edilmeli?

Kilit cümlesi tek ve kısa tutulur, promptun sonuna aynen eklenir; iki kilit çakışırsa (örn. poz + kıyafet) öncelik promptta yazılır.

---
# 1129. `/book-log` — Book Log Journal

## Trend

**T1/T2 — Pinterest'te +482%.**

## Türkçe

> Okunan kitapları kaydetmek için sade book-log journal sayfası tasarla.
>
> Her kitap için:
>
> - başlık,
> - yazar,
> - başlangıç/bitiş tarihi,
> - 1–5 yerine kısa kişisel not,
> - tek satırlık “bende kalan”
>
> alanı bulunsun.
>
> Gerçek kitap kapaklarını izinsiz kopyalama; gerekiyorsa yalnız kitap sırtı veya boş kapak alanı kullan.

## English

> Design a restrained book-log journal page.
>
> For each book include title, author, start/finish date, a concise personal note rather than only a star score, and one “what stayed with me” line.
>
> Avoid reproducing real copyrighted book covers; use a spine or blank cover field where necessary.

---

# 1130. `/music-journal` — Müzik Günlüğü

## Trend

**T1/T2 — Pinterest'te music journaling +127%.**

## Türkçe prompt

> Bir albüm/şarkı için music journal spread oluştur.
>
> Alanlar:
>
> - sanatçı ve eser,
> - ilk dinleme tarihi,
> - 3 ana duygu/çağrışım,
> - en çok geri dönülen bölüm için kısa zaman damgası,
> - kişisel not.
>
> Uzun şarkı sözü alıntısı üretme.

## English

> Create a music-journal spread for one album or song.
>
> Include artist and title, first-listen date, three primary feelings or associations, one short timestamp for a frequently revisited moment, and personal notes.
>
> Do not reproduce long lyrics.

---

# 1131. `/dream-journal` — Rüya Günlüğü

## Trend

**T1/T2 — dream journaling +128%.**

## Türkçe prompt

> Rüya günlüğü için iki sayfalık sade kayıt şablonu oluştur.
>
> Alanlar:
>
> - tarih,
> - ana sahne,
> - hatırlanan kişiler/nesneler,
> - duygu,
> - uyanınca akılda kalan tek ayrıntı.
>
> Rüyayı mistik kehanet, tarot veya astroloji grafiğine dönüştürme.

## English

> Design a restrained two-page dream-journal template.
>
> Include date, primary scene, remembered people or objects, emotion, and one detail that remained after waking.
>
> Do not turn the dream into mystical prophecy, tarot, or astrology graphics.

---

# 1132. `/blind-bag-template` — DIY Blind Bag Printable

## Trend

**T1/T2 — printable template aramalarında +507%.**

## Türkçe prompt

> [KOLEKSİYON] için evde yazdırılıp katlanabilecek küçük blind-bag kâğıt paketi şablonu tasarla.
>
> Ön yüz:
>
> - seri adı,
> - tek küçük görsel,
> - koleksiyonda kaç parça olduğu.
>
> Arka yüz:
>
> - basit açma alanı,
> - küçük seri listesi.
>
> Kesme ve katlama çizgileri fiziksel olarak uygulanabilir olsun.
>
> Gerçek çocuk ürünü güvenlik/sertifika işaretleri uydurma.

## English

> Design a small printable paper blind-bag template for [COLLECTION] that can be cut and folded at home.
>
> Front: series name, one small visual, and collection size.
>
> Back: simple opening area and a small series lineup.
>
> Make cut and fold lines physically practical.
>
> Do not invent real child-product safety or certification marks.

---

# 1133. `/blind-bag-series` — DIY Koleksiyon Serisi

## Türkçe

> 6 parçalık DIY blind-bag koleksiyonu oluştur.
>
> Her parça:
>
> - aynı fiziksel boyut,
> - aynı ana malzeme,
> - ortak seri dili,
> - farklı tek fikir
>
> taşısın.
>
> “Rare” parça yalnız altın, glitter veya glow-in-the-dark olmak zorunda değil; anlamlı varyasyon kullan.

## English

> Create a six-piece DIY blind-bag collection.
>
> Keep physical size, primary material, and series language consistent while giving each piece one distinct idea.
>
> Do not make the rare item automatically gold, glittery, or glow-in-the-dark; use a meaningful variation.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1134. `/memory-box` — Kişisel Anı Kutusu

## Trend

**T1/T2 — Pinterest'te +156%.**

## Türkçe prompt

> [ANI/YIL/SEYAHAT] için fiziksel memory box düzenle.
>
> Kutuda yalnız 6–8 gerçekçi nesne olsun:
>
> - küçük fotoğraf,
> - bilet,
> - not,
> - küçük obje,
> - kart,
> - kumaş/etiket parçası
>
> gibi.
>
> Her nesne aynı anlamı tekrar etmesin.
>
> Kutuyu scrapbook klişesi olan kurutulmuş çiçek + kahve lekesi + washi tape setine dönüştürme.

## English

> Arrange a physical memory box for [MEMORY/YEAR/TRIP] using only 6–8 believable objects such as a small photo, ticket, note, object, card, and textile or label fragment.
>
> Give every object a different narrative role.
>
> Avoid the standard scrapbook combination of dried flowers, coffee stains, and washi tape.

---

# 1135. `/photo-album-book` — DIY Photo Album Book

## Trend

**T1/T2 — Pinterest'te +306%.**

## Türkçe

> [ETKİNLİK/SEYAHAT/YIL] için el yapımı küçük fotoğraf albümü kitabı tasarla.
>
> Her açılımda en fazla:
>
> - 1 büyük fotoğraf,
> - 1 küçük destek fotoğrafı,
> - tarih,
> - 1–2 cümle not
>
> kullan.
>
> Her boşluğu sticker ve dekorla doldurma.

## English

> Design a small handmade photo-album book for [EVENT/TRIP/YEAR].
>
> On each spread use at most one large photograph, one small supporting image, a date, and 1–2 sentences of notes.
>
> Do not fill every blank area with stickers and decoration.

---

# 1136. `/cyberdeck` — Kişisel DIY Bilgisayar

## Trend

**T1/T2 — Pinterest +1410%; TikTok'ta 2026'nın belirgin donanım trendlerinden.**

Cyberdeck'i yalnız “cyberpunk laptop” olarak promptlamak trendi yanlış anlar.

Asıl fikir:

> **kişinin kendi kullanımına göre dönüştürdüğü, görünür parçalı, sıra dışı kasalı küçük bilgisayar.**

## Türkçe prompt

> [KULLANIM AMACI] için fiziksel DIY cyberdeck tasarla.
>
> Gerçek parça mantığı kullan:
>
> - küçük ekran,
> - fiziksel klavye veya kontrol düğmeleri,
> - compute board / mini bilgisayar için gerçek hacim,
> - güç kaynağı/batarya için alan,
> - portlara erişim,
> - havalandırma,
> - kapağın gerçekten kapanabilmesi.
>
> Kasa [ESKİ ÇANTA / METAL KUTU / AHŞAP KASA / ÖZEL 3B BASILI GÖVDE] olabilir.
>
> Estetik, gerçek donanım yerleşiminin üzerine kurulsun.
>
> Hologram, yüzen ekran ve işlevsiz sci-fi panel ekleme.

## English

> Design a physical DIY cyberdeck for [USE CASE].
>
> Use believable hardware logic:
>
> - small display,
> - physical keyboard or controls,
> - real volume for a compute board or mini computer,
> - space for power or battery,
> - accessible ports,
> - ventilation,
> - a case that can physically close.
>
> The enclosure may use a repurposed bag, metal case, wooden box, or custom 3D-printed shell.
>
> Build the aesthetic around real hardware placement.
>
> Avoid holograms, floating displays, and nonfunctional sci-fi panels.

---

# 1137. `/purse-cyberdeck` — Çanta İçinde Cyberdeck

## Trend

**T2 — 2026'da viral örneklerle görünür.**

## Türkçe prompt

> Vintage/ikinci el sert gövdeli küçük çantayı gerçekten kapanabilen taşınabilir cyberdeck'e dönüştür.
>
> İçeride:
>
> - 5–8 inç ekran,
> - küçük klavye,
> - compute board için gizli ama erişilebilir alan,
> - batarya,
> - SD/USB depolama alanı
>
> bulunsun.
>
> Çanta formunu yalnız dekor olarak kullanma; menteşe, derinlik ve kapanma fiziksel olarak çalışmalı.

## English

> Convert a small vintage or secondhand structured bag into a portable cyberdeck that can genuinely close.
>
> Include a 5–8 inch display, compact keyboard, hidden but accessible compute-board area, battery, and SD/USB storage.
>
> Do not use the bag merely as decoration; make hinge, depth, and closure physically functional.

---

# 1138. `/terminal-setup` — Terminal Aesthetic Workstation

## Trend

**T1/T2 — Pinterest +559%.**

## Türkçe prompt

> Küçük masaüstü çalışma alanını terminal aesthetic setup olarak düzenle.
>
> Tek veya iki ekran, gerçek terminal/metin arayüzü, fiziksel klavye ve yalnız gerekli masa objeleri kullan.
>
> Terminali dekoratif “Matrix code” duvarına dönüştürme.
>
> Ekrandaki metin gerçek sistem/komut çıktısı gibi kısa ve işlevsel olsun; anlamsız yüzlerce satır üretme.

## English

> Arrange a small desk as a terminal-aesthetic workstation using one or two screens, a real text-oriented terminal interface, physical keyboard, and only necessary desk objects.
>
> Avoid decorative Matrix-code walls.
>
> Keep screen text concise and functional rather than generating hundreds of meaningless lines.

---

# 1139. `/terminal-poster` — Terminal Interface Poster

## Türkçe

> [KONU]'yu terminal penceresini grafik taşıyıcı olarak kullanan poster biçiminde göster.
>
> Başlık komut satırı gibi, destek bilgi 3–5 kısa çıktı satırı gibi düzenlenebilir.
>
> Gerçek yazılım komutlarını yanlış/tehlikeli biçimde uydurma; gerekirse kurmaca placeholder kullan.

## English

> Present [TOPIC] as a poster using a terminal window as the graphic carrier.
>
> Treat the title like a command prompt and supporting information like 3–5 concise output lines.
>
> Do not invent unsafe or misleading real commands; use clearly fictional placeholders when needed.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1140. `/hardware-makeover` — Kişisel Teknoloji Dönüşümü

## Trend

**T1/T2 — headphones painting +436%, bedazzle headphones +1233%.**

## Türkçe prompt

> [KULAKLIK/FARE/KLAVYE/CİHAZ]'ı kişiselleştirilmiş fiziksel makeover olarak tasarla.
>
> Değişiklik:
>
> - boya,
> - küçük sticker/decal,
> - tekstil kaplama,
> - çıkarılabilir charm,
> - değiştirilebilir keycap
>
> gibi gerçek uygulanabilir yöntemlerden yalnız 1–3 tanesini kullansın.
>
> Cihazın buton, mikrofon, havalandırma, sensör ve bağlantı noktalarını kapatma.

## English

> Design a personalized physical makeover for [HEADPHONES/MOUSE/KEYBOARD/DEVICE].
>
> Use only 1–3 practical modification methods such as paint, small decals, textile wrapping, removable charms, or replaceable keycaps.
>
> Do not cover buttons, microphones, ventilation, sensors, or ports.

---

# 1141. `/crochet-headphones` — Örgü Kablolu Kulaklık

## Trend

**T1/T2 — Pinterest +382%.**

## Türkçe prompt

> Kablolu kulaklığın kablosuna gerçek crochet sleeve/kılıf tasarla. Örgü kablo çevresini sarsın ancak konektör, mikrofon ve strain relief bölgelerini kapatmasın.
>
> Kulaklık gövdesini büyük peluş oyuncağa dönüştürme.

## English

> Design a real crochet sleeve around the cable of wired headphones. Let the crochet wrap the cable while keeping the connector, microphone, and strain-relief areas accessible.
>
> Do not turn the headphone bodies into oversized plush toys.

---

# 1142. `/custom-cursor-sheet` — Kişisel Cursor Seti

## Trend

**T1/T2 — Pinterest'te cursor aramaları hızla yükseliyor.**

## Türkçe

> [TEMA] için 8 parçalık küçük cursor seti oluştur:
>
> - normal pointer,
> - link,
> - text,
> - loading,
> - move,
> - resize,
> - unavailable,
> - precision.
>
> Her cursor 32 px civarında okunabilir ve işlevsel olarak birbirinden ayırt edilebilir olsun.
>
> Dekor uğruna pointer hotspot'unu belirsiz hâle getirme.

## English

> Create an eight-piece cursor set for [THEME]:
>
> normal pointer, link, text, loading, move, resize, unavailable, and precision.
>
> Keep every cursor readable around 32 px and functionally distinct.
>
> Do not obscure pointer hotspots for decoration.

---

# 1143. `/tech-sticker-kit` — Custom Tech Sticker Kit

## Türkçe prompt

> Laptop/cyberdeck/cihaz kişiselleştirmesi için 10 sticker'lık küçük kit oluştur.
>
> Stickerlar:
>
> - işlevsel label,
> - kısa kişisel ifade,
> - 2–3 sembol,
> - tek büyük ana sticker
>
> karışımı olsun.
>
> Cihazı tamamen örtecek kadar yoğun veya aynı internet meme'lerinin kopyası olmasın.

## English

> Create a small 10-sticker kit for customizing a laptop, cyberdeck, or device.
>
> Mix functional labels, one short personal phrase, 2–3 symbols, and one larger primary sticker.
>
> Avoid covering the entire device or copying familiar internet memes.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1144. `/prototype-board` — Tasarım Süreci Panosu

## Trend bağlantısı

Canva'nın 2026 “Imperfect by Design” yaklaşımında yalnız sonucun değil, **ara aşamanın görünmesi** değer kazanıyor.

## Türkçe prompt

> [ÜRÜN/LOGO/AFİŞ] için gerçek tasarım sürecini gösteren prototype/process board oluştur.
>
> Panoda:
>
> - 3 küçük erken eskiz,
> - 1 başarısız/elenmiş yön,
> - 2 ara varyasyon,
> - 1 final
>
> bulunsun.
>
> Süreci sahte göstermek için aynı final tasarımın farklı opaklıklarını “sketch” diye sunma.

## English

> Create a prototype or process board showing the real development of [PRODUCT/LOGO/POSTER].
>
> Include three small early sketches, one rejected direction, two intermediate variants, and one final.
>
> Do not fake the process by showing lower-opacity copies of the final design as “sketches.”

---

# 1145. `/sketch-to-final` — Eskizden Finale

## Türkçe

> Aynı fikri dört aşamada göster:
>
> 1. kaba thumbnail,
> 2. seçilen kompozisyon,
> 3. malzeme/renk denemesi,
> 4. final.
>
> Fikir aşamalar arasında anlaşılır biçimde evrilsin; final birden bire bambaşka tasarım olmasın.

## English

> Show the same idea in four stages:
>
> 1. rough thumbnail,
> 2. selected composition,
> 3. material or color study,
> 4. final.
>
> Make the idea evolve visibly between stages rather than jumping to an unrelated final design.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1146. `/maker-desk` — Gerçek Üretim Masası

## Türkçe prompt

> [ZANAAT/TASARIM] üretim sürecini gerçek kullanılan çalışma masasında göster.
>
> Yalnız o işe ait 5–8 gerekli araç/malzeme bulunsun.
>
> Bir veya iki yarım kalmış parça, kesik malzeme veya deneme olabilir.
>
> “Creative desk” klişesi olarak kahve, MacBook, renkli kalem, Polaroid, bitki ve gözlüğü otomatik ekleme.

## English

> Show the making process for [CRAFT/DESIGN] on a genuinely used worktable.
>
> Include only 5–8 tools or materials necessary for that work.
>
> One or two unfinished pieces, offcuts, or tests may remain visible.
>
> Avoid the generic creative-desk prop list of coffee, MacBook, colored pencils, Polaroids, plants, and glasses.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1147. `/rejected-ideas` — Elenen Fikirler Sayfası

## Yeni kullanım

Yapay zekâ ile yalnız final üretmek yerine eleme sürecini de görselleştirmek için.

## Türkçe prompt

> [KONU] için altı küçük tasarım yönü üret ve bunları “final seçenekleri” gibi değil, fikir araştırması olarak göster.
>
> 2 tanesi bilinçli olarak zayıf/uygunsuz olabilir; neden elendiğini 2–4 kelimelik kısa notlarla belirt.
>
> Tüm seçenekleri eşit derecede cilalı yapma.

## English

> Generate six small design directions for [TOPIC] and present them as exploration rather than six polished final options.
>
> Allow two to be deliberately weak or unsuitable and annotate why they were rejected in 2–4 words.
>
> Do not polish every option equally.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1148. `/curiosity-cabinet` — Cabinet of Curiosities

## Trend

**T1/T2 — koleksiyon ve kişisel sergileme eğilimiyle yeniden görünür.**

V&A bu sergileme geleneğini çağdaş collecting ve art practice bağlamında araştırmaya devam ediyor. Güncel tasarım yayınlarında curio cabinet yeniden kişisel koleksiyonların görünür sergileme biçimi olarak ele alınıyor.

## Türkçe prompt

> [TEMA/KİŞİ] için cam kapaklı küçük curiosity cabinet düzenle.
>
> 8–12 nesne kullan:
>
> - doğal örnek,
> - küçük hatıra,
> - kitap/kağıt,
> - zanaat nesnesi,
> - araç/gereç,
> - fotoğraf veya etiket
>
> gibi.
>
> Nesneler tematik ilişki taşısın ama bilimsel taxonomy olmak zorunda değil.
>
> Karanlık “witch cabinet”, skull, mum ve okült sembol klişesini otomatik kullanma.

## English

> Arrange a small glass-fronted cabinet of curiosities for [THEME/PERSON] using 8–12 objects such as natural specimens, keepsakes, books or papers, crafted objects, tools, photographs, or labels.
>
> Let the objects share thematic relationships without requiring a strict scientific taxonomy.
>
> Do not automatically turn the cabinet into a dark witchy display filled with skulls, candles, and occult symbols.

---

# 1149. `/personal-museum` — Kişisel Müze Vitrini

## Türkçe prompt

> Bir kişinin yaşamından 7–9 anlamlı nesneyi küçük çağdaş müze vitrini içinde sergile.
>
> Her nesne:
>
> - ayrı fiziksel alan,
> - küçük numara,
> - 1–2 satırlık kısa label
>
> taşısın.
>
> Kişinin hayatını yalnız başarı belgeleri ve ödüller üzerinden anlatma.

## English

> Display 7–9 meaningful objects from a person's life inside a small contemporary museum case.
>
> Give every object its own physical space, a small number, and a concise 1–2 line label.
>
> Do not reduce a person's life to awards and achievement certificates.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1150. `/visible-vault` — Açık Koleksiyon Deposu

## Trend / kullanım

2026 müze tasarımında **visible storage / open collections storage**, koleksiyonu yalnız seçilmiş birkaç objeyle değil, depolama mantığını görünür kılarak anlatan güçlü bir format.

## Türkçe prompt

> [KOLEKSİYON] için visible-vault / open-storage sergileme sistemi tasarla.
>
> Cam üstlü çekmeceler, ayarlanabilir raflar ve numaralı küçük eser grupları kullan.
>
> Ziyaretçi çok sayıda nesneyi görebilsin ancak sınıflandırma okunabilir kalsın.
>
> Depoyu lüks mağaza vitrini gibi seyrekleştirme.

## English

> Design a visible-vault or open-storage display for [COLLECTION] using glass-topped drawers, adjustable shelving, and numbered groups of small artifacts.
>
> Let visitors see many objects while keeping classification readable.
>
> Do not sparsify the storage until it resembles luxury retail display.

---

# 1151. `/museum-object-label` — Müze Eser Etiketi

## Türkçe

> [ESER/NESNE] için küçük müze label tasarla.
>
> Sıra:
>
> 1. eser adı,
> 2. tarih/dönem,
> 3. malzeme,
> 4. kaynak/provenance bilgisi,
> 5. en fazla 50–80 kelimelik kısa açıklama.
>
> Eseri pazarlama sloganıyla anlatma.

## English

> Design a small museum label for [OBJECT/ARTIFACT].
>
> Use this order:
>
> 1. object title,
> 2. date or period,
> 3. material,
> 4. source or provenance,
> 5. a concise 50–80 word explanation maximum.
>
> Avoid advertising language.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1152. `/specimen-drawer` — Numune Çekmecesi

## Türkçe prompt

> [DOĞAL/BİLİMSEL KOLEKSİYON] için düz açılan müze specimen drawer oluştur.
>
> 8–16 örnek eşit olmak zorunda olmayan doğal aralıklarla yerleşsin.
>
> Her örneğin küçük numarası ve çekmece kenarında referans listesi bulunsun.
>
> Numuneleri dekoratif renk uyumuna göre değil, gerçek sınıflandırma mantığına göre düzenle.

## English

> Create a flat museum specimen drawer for [NATURAL/SCIENTIFIC COLLECTION].
>
> Arrange 8–16 specimens with natural spacing rather than forcing perfect symmetry.
>
> Give each a small number and place a reference list along the drawer edge.
>
> Organize specimens by real classification logic rather than decorative color matching.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1153. `/artifact-tray` — Arkeolojik Eser Tepsisi

## Türkçe

> Arkeolojik kazıdan gelen küçük buluntuları koruyucu köpük/kâğıt bölmeli artifact tray üzerinde göster.
>
> Her eser ayrı numaralı bölmede, yanında ölçek veya kayıt etiketiyle bulunsun.
>
> Eserleri “treasure collection” gibi altın/parlak sunma.

## English

> Show small archaeological finds in a protective artifact tray with foam or paper dividers.
>
> Place each object in its own numbered compartment with a scale or record label.
>
> Avoid presenting the collection like shiny treasure.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1154. `/museum-case` — Tek Eser Vitrini

## Türkçe prompt

> [ESER]'i konservasyon mantığına uygun sade müze vitrini içinde göster.
>
> Vitrinde:
>
> - düşük yansımaya sahip cam,
> - güvenli destek,
> - kontrollü yumuşak ışık,
> - küçük label
>
> bulunsun.
>
> Eseri dramatik lüks ürün spotuna dönüştürme.

## English

> Display [ARTIFACT] inside a restrained conservation-aware museum case with low-reflection glass, secure support, controlled soft lighting, and a small label.
>
> Avoid turning the artifact into a luxury-product spotlight image.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1155. `/collection-wall` — Kişisel Koleksiyon Duvarı

## Trend

**T1 — Curated Clutter ile ilişkili.**

## Türkçe

> [KOLEKSİYON] için yıllar içinde oluşmuş kişisel collection wall düzenle.
>
> Nesneler aynı türden olabilir ancak boyut, yaş ve kaynak farklılıkları doğal biçimde görülsün.
>
> Her şeyi mükemmel grid veya renk gökkuşağına dizme.

## English

> Arrange a personal collection wall for [COLLECTION] that feels accumulated over years.
>
> Objects may share a category while naturally varying in size, age, and source.
>
> Avoid perfect grid alignment and rainbow color sorting.

---

# 1156. `/object-biography` — Bir Nesnenin Biyografisi

## Yeni görsel anlatım ailesi

Bir nesneyi yalnız “ürün” değil, zaman içindeki kullanım hikâyesiyle göstermek için.

## Türkçe prompt

> [NESNE]'nin yaşamını dört karede göster:
>
> 1. yeni/ilk hâli,
> 2. kullanım sırasında,
> 3. onarım/değişim,
> 4. bugünkü hâli.
>
> Aynı nesne geometrisi ve ayırt edici izleri kareler boyunca korunsun.
>
> Eskimeyi dramatik grunge efektiyle değil gerçek malzeme davranışıyla göster.

## English

> Show the biography of [OBJECT] in four frames:
>
> 1. new or initial state,
> 2. during use,
> 3. repair or modification,
> 4. present state.
>
> Preserve the same core geometry and distinctive marks across all frames.
>
> Express aging through real material behavior rather than dramatic grunge effects.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1157. `/repair-story` — Onarım Hikâyesi

## Trend bağlantısı

Pinterest 2026'da darning, upcycling ve secondhand kullanım sinyalleri güçlü.

## Türkçe prompt

> [GİYSİ/NESNE]'nin onarımını üç aşamada göster:
>
> - hasarlı ama kullanılabilir hâl,
> - onarım süreci,
> - tamamlanmış onarım.
>
> Kamera ve nesne konumu eşleşsin.
>
> Onarımı “yeni gibi görünmez hâle getirme” zorunluluğu yok; görünür onarım estetik ve işlevsel olabilir.

## English

> Show the repair of [GARMENT/OBJECT] in three matched stages:
>
> - damaged but usable,
> - repair in progress,
> - completed repair.
>
> Keep camera and object placement consistent.
>
> The finished repair does not need to become invisible; visible repair may remain both functional and aesthetic.

---

# 1158. `/visible-mending` — Görünür Onarım

## Trend

**T1/T2 — darning stitch +109%.**

## Türkçe

> [GİYSİ]'deki küçük yırtık/delik üzerine gerçek visible-mending/darning onarımı tasarla.
>
> İplik yapısı kumaşın taşıyıcı dokusuna bağlansın.
>
> Onarım alanı dayanıklı ve sınırlı olsun.
>
> Bütün giysiyi dekoratif nakışla kaplama.

## English

> Design a real visible-mending or darning repair over a small tear or hole in [GARMENT].
>
> Let thread structure connect into the supporting fabric weave.
>
> Keep the repair durable and localized.
>
> Do not cover the entire garment in decorative embroidery.

---

# 1159. `/upcycle-before-after` — Upcycle Before/After

## Türkçe

> Aynı [GİYSİ/NESNE]'yi önce/sonra eşleşmiş kadrajda göster.
>
> Sonraki sürüm mevcut malzemenin büyük bölümünü gerçekten yeniden kullansın.
>
> “Upcycle” adı altında kaynak nesneyi tamamen farklı yeni ürüne dönüştürüp orijinal malzemeyi görünmez yapma.

## English

> Show the same [GARMENT/OBJECT] in a matched before-and-after composition.
>
> Make the new version genuinely reuse most of the original material.
>
> Do not label it “upcycled” if the source item effectively disappears into a completely unrelated new product.

## Neye dikkat edilmeli?

Yapım aşamaları aynı nesnenin sürekliliğini korusun; el, alet ve yarı mamul kareler arasında değişmesin.

---
# 1160. `/thrift-flip` — Secondhand Garment Flip

## Trend

**T1/T2 — Pinterest thrift flip skirt +91%.**

## Türkçe prompt

> İkinci el [GİYSİ]'yi düşük müdahaleli thrift flip olarak yeniden düzenle.
>
> Değişiklikler:
>
> - boy kısaltma,
> - bel ayarı,
> - cep ekleme,
> - patch,
> - küçük boya/nakış
>
> gibi gerçek dikiş/uyarlama yöntemlerinden 1–3 tanesi olsun.
>
> Kaynak giysinin tanınabilir temel formunu koru.

## English

> Rework a secondhand [GARMENT] as a low-intervention thrift flip.
>
> Use only 1–3 practical alterations such as shortening, waist adjustment, adding pockets, patches, or small paint or embroidery.
>
> Preserve the recognizable base form of the source garment.

---

# 1161. `/jersey-upcycle` — Spor Forması Upcycle

## Trend

**T1/T2 — Pinterest jersey upcycle +91%.**

## Türkçe

> Eski spor formasını yeni giyilebilir parçaya dönüştürürken forma numarası, arma/logo ve ana renk bloklarını mümkün olduğunca koru.
>
> Yeni parça [çanta / yelek / üst / küçük aksesuar] olabilir.
>
> Resmî takım ürününe benzeyen yeni sahte merchandise üretme; açıkça upcycled object olarak göster.

## English

> Upcycle an old sports jersey into a new wearable object while preserving the original number, crest or logo, and primary color blocks where possible.
>
> The new item may be a bag, vest, top, or small accessory.
>
> Do not present it as new official team merchandise; keep the upcycled origin clear.

---

# 1162. `/deadstock-board` — Deadstock Material Board

## Trend

**T1/T2 — deadstock stores +42%.**

## Türkçe

> Bir tasarım projesi için elde bulunan deadstock kumaş/malzeme parçalarını fiziksel selection board üzerinde göster.
>
> Her malzemenin gerçek boyut/renk/doku farklılığı korunsun.
>
> Önce mevcut malzemeyi göster; tasarımı sonra bu sınırlara göre türet.

## English

> Show available deadstock fabric or material pieces on a physical selection board for a design project.
>
> Preserve real variation in size, color, and texture.
>
> Present available material first and derive design decisions from those constraints rather than inventing unlimited material.

---

# 1163. `/explorecore-poster` — Katmanlı Keşif Posteri

## Trend

**T1/T2 — Canva 2026 Explorecore.**

## Türkçe prompt

> [KONU/MEKÂN]'ı tek bakışta tamamen açıklamak yerine katmanlı keşif posteri olarak tasarla.
>
> İlk bakışta tek ana görsel ve kısa başlık okunmalı.
>
> Yaklaştıkça görülen 3–5 ikincil ayrıntı:
>
> - küçük harita,
> - crop,
> - numara,
> - kısa not,
> - gizli bağlantı
>
> içerebilir.
>
> Katmanlı anlatımı “çok fazla şey koymak” ile karıştırma.

## English

> Design [TOPIC/PLACE] as a layered exploration poster rather than revealing everything at first glance.
>
> One primary visual and concise title should read immediately.
>
> Add only 3–5 secondary discoveries such as a small map, crop, number, concise note, or hidden relationship.
>
> Do not confuse layered storytelling with visual clutter.

---

# 1164. `/opt-out-branding` — Sadelik / Anti-clutter Branding

## Trend

**T1/T2 — Canva 2026 Opt-Out Era.**

Canva, 2026'da “clean layout”, “serif” ve “simple branding” aramalarının yıllık %54 arttığını; aşırı cute mascot ve kabarcıklı grafiklerin daha sakin görsel sistemlerle yer değiştirdiğini bildiriyor.

## Türkçe prompt

> [MARKA] için “daha az” ilkesine dayalı sakin kimlik sistemi oluştur.
>
> Kullan:
>
> - net wordmark,
> - tek ana font ailesi,
> - 2–3 renk,
> - geniş negatif alan,
> - yalnız gerektiğinde tek sembol.
>
> Minimal görünmek için her şeyi bej yapma.
>
> Logo ve sayfa düzeni sıradanlaşacak kadar anonim olmasın.

## English

> Create a restrained brand system for [BRAND] built around doing less.
>
> Use a clear wordmark, one primary font family, 2–3 colors, generous negative space, and only one symbol when genuinely necessary.
>
> Do not make everything beige merely to appear minimal.
>
> Keep enough distinctive character to avoid anonymity.

---

# 1165. `/anti-cute` — Anti-cuteness Graphic Direction

## Trend

**T1/T2 — Canva 2026 Opt-Out Era ile ilişkili.**

## Türkçe

> [KONU]'yu cute/kawaii/mascot görsel diline başvurmadan sıcak ve erişilebilir biçimde tasarla.
>
> Dostluk hissini:
>
> - insan ölçekli tipografi,
> - doğal renk,
> - gerçek fotoğraf,
> - yumuşak boşluk,
> - sade çizgi
>
> üzerinden kur.
>
> Yüz eklenmiş nesne, yuvarlak blob karakter ve pastel sticker kullanma.

## English

> Make [TOPIC] warm and approachable without relying on cute, kawaii, or mascot language.
>
> Build friendliness through human-scale typography, natural color, real photography, comfortable spacing, and restrained linework.
>
> Avoid objects with faces, rounded blob characters, and pastel sticker graphics.

---

# 1166. `/proof-of-thought` — Süreci Görünür Bırakma

## Trend

**T1/T2 — Canva'nın “polish to presence” yaklaşımıyla uyumlu.**

## Türkçe prompt

> Final [TASARIM/ÜRÜN]'ün yanında yalnızca gerçekten karar sürecini açıklayan 3 küçük iz bırak:
>
> - erken eskiz,
> - materyal denemesi,
> - kısa elle yazılmış karar notu.
>
> Bunlar dekor değil, final seçimin nedenini göstermeli.
>
> Sahte yaratıcılık göstergesi olarak rastgele post-it ve karalama ekleme.

## English

> Place only three small pieces of genuine process evidence beside the final [DESIGN/PRODUCT]:
>
> - early sketch,
> - material test,
> - concise handwritten decision note.
>
> These should explain why the final choice was made rather than function as decoration.
>
> Avoid random Post-its and scribbles as fake proof of creativity.

---

# 1167. `/process-photo` — Yapım Aşaması Fotoğrafı

## Türkçe

> Final ürünü değil, [ÜRETİM] sürecinin anlamlı orta aşamasını fotoğraflanmış gibi göster.
>
> El/alet, yarım bitmiş nesne ve gerçek çalışma yüzeyi yeterli olsun.
>
> Süreci “artisan” göstermek için gereksiz talaş, un, boya veya dağınıklık ekleme.

## English

> Photograph a meaningful middle stage of [MAKING PROCESS] rather than the finished product.
>
> One hand or tool, the partially completed object, and a real work surface are enough.
>
> Do not add unnecessary sawdust, flour, paint, or mess merely to signal craftsmanship.

## Neye dikkat edilmeli?

Yapım aşamaları aynı nesnenin sürekliliğini korusun; el, alet ve yarı mamul kareler arasında değişmesin.

---
# 1168. Yeni üst aile: `Personal Media`

Şu trendler aynı üst başlıkta toplanabilir:

- birthday magazine,
- tracking journal,
- book log,
- music journal,
- dream journal,
- DIY photo album,
- zine,
- memory box.

Ortak mekanizma:

> **kişinin hayatı → küçük editoryal/analog yayın nesnesi**

Bu, sosyal medya postundan farklıdır.

Amaç:

> “paylaşılacak içerik” değil, **saklanacak kişisel medya** üretmek.

---

# 1169. `Personal Media` prompt formülü

## Türkçe

> [KİŞİSEL KONU]'yu küçük fiziksel/dijital yayın nesnesine dönüştür.
>
> Önce içerik yapısını belirle:
>
> - kaç bölüm,
> - hangi tarihsel sıra,
> - hangi fotoğraf,
> - hangi kısa not.
>
> Sonra görsel dili seç.
>
> Dekor, içerikten sonra gelsin.

## English

> Transform [PERSONAL TOPIC] into a small physical or digital publication object.
>
> Define content structure first:
>
> - number of sections,
> - chronological order,
> - photographs,
> - concise notes.
>
> Choose visual language afterward.
>
> Decoration should follow content rather than lead it.

---

# 1170. Yeni üst aile: `Make-it-Mine`

Cyberdeck, hardware makeover, upcycling ve charm trendlerinin ortak noktası:

> **hazır nesneyi kişisel nesneye dönüştürmek.**

Bu aile:

- `/cyberdeck`
- `/hardware-makeover`
- `/crochet-headphones`
- `/custom-cursor-sheet`
- `/visible-mending`
- `/thrift-flip`
- `/jersey-upcycle`
- `/patch-tote`
- `/bag-charms`

gibi promptları bir arada tutabilir.

Prompt formülü:

> **source object + functional constraints + personal intervention + preserve usability**

---

# 1171. Yeni üst aile: `Collection-as-Story`

Bu aile:

- curiosity cabinet,
- visible vault,
- trinket shelf,
- memory box,
- specimen drawer,
- travel ephemera,
- matchbook collection,
- keychain collection,
- patch collection

gibi alanları birleştirir.

Kritik ayrım:

> Koleksiyonun amacı nesneleri “dizmek” değil, **ilişki kurmak**tır.

İyi prompt:

> `12 objects collected across different years, each with a distinct origin and role, arranged so relationships can be discovered`

Zayıf prompt:

> `beautiful aesthetic collection of vintage objects`

---

# 1172. `/collection-narrative-map` — Koleksiyon İlişki Haritası

## Türkçe

> [KOLEKSİYON]'daki 8–12 nesnenin birbirleriyle ilişkisini küçük numaralar ve ince bağlantılarla göster.
>
> Bağlantılar:
>
> - aynı yer,
> - aynı kişi,
> - aynı yıl,
> - aynı kullanım,
> - aynı malzeme
>
> gibi gerçek ilişkilere dayansın.
>
> Her nesneyi her nesneye bağlama.

## English

> Show relationships among 8–12 objects in [COLLECTION] using small numbers and restrained connectors.
>
> Base links on real relationships such as same place, person, year, use, or material.
>
> Do not connect every object to every other object.

## Neye dikkat edilmeli?

Yapım aşamaları aynı nesnenin sürekliliğini korusun; el, alet ve yarı mamul kareler arasında değişmesin.

---
# 1173. `/museum-vs-collection` — Müze ve Kişisel Koleksiyon Ayrımı

## Rehber notu

Aynı 10 nesne iki farklı promptla tamamen farklı görünmelidir.

### Müze

> sınıflandırılmış, kayıtlı, korunan, açıklanan.

### Kişisel koleksiyon

> birikmiş, hatıra taşıyan, bazen düzensiz, öznel.

Bu nedenle:

> `museum display`

ile:

> `personal curiosity cabinet`

eşanlamlı değildir.

---

# 1174. `/cyberdeck-slop-filter` — Cyberdeck AI Slop Filtresi

Kaçınılması gerekenler:

- hologram,
- işlevsiz 30 ekran,
- anlamsız neon kablo,
- portları erişilemez yapmak,
- batarya/havalandırma düşünmemek,
- klavye kapanmayı engelliyor,
- cihazı sadece “cyberpunk prop” yapmak,
- gerçek cyberdeck'in DIY/personal computing mantığını kaybetmek.

---

# 1175. `/journal-slop-filter` — Journal AI Slop Filtresi

Kaçınılması gerekenler:

- her boşluğa sticker,
- kahve lekesi,
- washi tape,
- kurutulmuş çiçek,
- rastgele el yazısı,
- motive edici slogan,
- kullanılmayacak 30 tracker,
- okunmayan minik metin.

İyi journal:

> **kullanıcının gerçekten yazabileceği boşluk bırakır.**

---

# 1176. `/museum-slop-filter` — Müze/Koleksiyon AI Slop Filtresi

Kaçınılması gerekenler:

- her müze vitrini siyah ve dramatik spotlight,
- bütün objeleri altın “treasure” gibi sunmak,
- uydurma provenance,
- sahte katalog numarası ve tarih,
- korunması hassas nesneye aşırı ışık,
- her eserin yanında QR kod zorunluluğu,
- kişisel koleksiyonu bilimsel taxonomy gibi göstermek.

---

# 1177. Bu turdaki slash-style indeks (aile-014)

| Kısayol | Aile |
|---|---|
| `/birthday-magazine` | personal birthday publication |
| `/birthday-cover` | birthday magazine cover |
| `/year-in-review-magazine` | personal annual publication |
| `/tracking-journal` | habit/project tracking spread |
| `/analog-progress-log` | physical progress journal |
| `/book-log` | book log journal |
| `/music-journal` | listening journal |
| `/dream-journal` | restrained dream journal |
| `/blind-bag-template` | printable blind-bag package |
| `/blind-bag-series` | DIY collectible series |
| `/memory-box` | personal memory box |
| `/photo-album-book` | handmade photo album |
| `/cyberdeck` | functional DIY computer |
| `/purse-cyberdeck` | bag-based portable computer |
| `/terminal-setup` | terminal workstation |
| `/terminal-poster` | terminal-based graphic poster |
| `/hardware-makeover` | physical tech customization |
| `/crochet-headphones` | crochet cable customization |
| `/custom-cursor-sheet` | personalized cursor family |
| `/tech-sticker-kit` | small device sticker system |
| `/prototype-board` | real design-process board |
| `/sketch-to-final` | four-stage design evolution |
| `/maker-desk` | authentic worktable |
| `/rejected-ideas` | rejected concept exploration |
| `/curiosity-cabinet` | personal cabinet of curiosities |
| `/personal-museum` | life objects as museum display |
| `/visible-vault` | open collection storage |
| `/museum-object-label` | museum object label |
| `/specimen-drawer` | scientific specimen drawer |
| `/artifact-tray` | archaeological artifact tray |
| `/museum-case` | conservation-aware artifact case |
| `/collection-wall` | accumulated personal collection |
| `/object-biography` | object across time |
| `/repair-story` | three-stage repair narrative |
| `/visible-mending` | localized darning repair |
| `/upcycle-before-after` | matched upcycle comparison |
| `/thrift-flip` | low-intervention secondhand redesign |
| `/jersey-upcycle` | sports jersey upcycle |
| `/deadstock-board` | existing-material selection board |
| `/explorecore-poster` | layered discovery poster |
| `/opt-out-branding` | restrained anti-clutter branding |
| `/anti-cute` | approachable without kawaii language |
| `/proof-of-thought` | visible process evidence |
| `/process-photo` | meaningful making-stage photograph |
| `/collection-narrative-map` | relationships inside a collection |

---

<a id="aile-015"></a>
# Bilimsel Görsel, Mimari Sunum, Tipografi ve Eğitim İllüstrasyonu — 2026 Ek Taraması

Bu turda dört alan birlikte ele alındı:

- bilimsel illüstrasyon ve veri figürleri,
- mimari sunum ve karar verme görselleri,
- tipografi/poster sistemleri,
- eğitim/çocuk odaklı görsel anlatım.

2026'da Nature ve Nature Methods'in bilimsel görselleştirme üzerine yeniden yoğunlaşması önemli bir sinyal. Nature, bilimsel illüstrasyonun yalnız “güzel çizim” değil; kaynak toplama, çelişkili bilgiyi değerlendirme, belirsizliği yönetme ve karmaşık bilgiyi doğru görsel yapıya dönüştürme işi olduğunu özellikle vurguluyor.

Nature Methods ise 2026'da **Points of View** sütununu yeniden başlatırken veri görselleştirmede:

- doğru grafik seçimi,
- düzen,
- renk,
- sembol,
- ok,
- etiket,
- belirsizlik

gibi konuları yeniden pratik araştırma metodolojisinin parçası olarak ele alıyor.

Bu yüzden bu rehberde bilimsel görsel için temel kural:

> **Image generation modeli biçimi gösterebilir; doğruluğu kendiliğinden garanti etmez.**

---

# 1178. `/scientific-figure` — Bilimsel Figür

## Türkçe prompt

> [BİLİMSEL KONU]'yu yayınlanabilir bilimsel figure mantığında görselleştir.
>
> Önce bilgi türünü belirle:
>
> - yapı,
> - süreç,
> - karşılaştırma,
> - zaman,
> - ölçüm,
> - dağılım,
> - mekanizma.
>
> Ardından yalnız bu bilgi türüne uygun görsel dil kullan.
>
> 2–4 ana renk, kısa etiket, açık panel hiyerarşisi ve gereksiz dekor içermeyen beyaz/açık arka plan tercih et.
>
> Bilimsel doğruluk gerektiren isim, oran, sayı ve yapıların kullanıcı/veri kaynağı tarafından doğrulanması gerektiğini varsay.

## English

> Visualize [SCIENTIFIC TOPIC] using the logic of a publication-ready scientific figure.
>
> First determine whether the information is primarily structural, procedural, comparative, temporal, quantitative, distributional, or mechanistic.
>
> Use only a visual language appropriate to that information type.
>
> Prefer 2–4 primary colors, concise labels, clear panel hierarchy, and a light undecorated background.
>
> Treat names, proportions, numbers, and structures requiring scientific accuracy as information that must be verified against the supplied source.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar (duvar dizimi, çocuk kitabı dili) içeriği sadeleştirebilir ama değiştiremez.

---
# 1179. `/mechanism-figure` — Mekanizma Şeması

## Türkçe

> [MEKANİZMA]'yı soldan sağa veya yukarıdan aşağıya tek ana mekanizma hattında göster.
>
> Başlangıç, ara etkileşimler ve sonuç açıkça ayrışsın.
>
> Her ok yalnız gerçek ilişkiyi temsil etsin.
>
> “Bilimsel görünmesi” için rastgele molekül, DNA heliksi veya neon parçacık ekleme.

## English

> Show [MECHANISM] as one primary mechanistic pathway flowing left-to-right or top-to-bottom.
>
> Separate input, intermediate interactions, and outcome clearly.
>
> Every arrow must represent a real relationship.
>
> Do not add random molecules, DNA helices, or glowing particles merely to make it look scientific.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1180. `/graphical-abstract` — Graphical Abstract

## Trend

**EVERGREEN / yayıncılıkta çok güçlü.**

## Türkçe prompt

> [ARAŞTIRMA]'yı tek sayfalık graphical abstract olarak özetle.
>
> Yapı:
>
> 1. problem/başlangıç,
> 2. yöntem veya müdahale,
> 3. ana sonuç,
> 4. kısa çıkarım.
>
> Metni toplam 30–60 kelimeyi aşmayacak kadar kısa tut.
>
> Makalenin her deneyini tek görsele sıkıştırma.

## English

> Summarize [RESEARCH] as a one-page graphical abstract.
>
> Structure it as:
>
> 1. problem/input,
> 2. method or intervention,
> 3. primary result,
> 4. concise implication.
>
> Keep total text to roughly 30–60 words.
>
> Do not squeeze every experiment from the paper into one image.

---

# 1181. `/visual-abstract` — Visual Abstract

## Ayrım

`graphical abstract` ile eşanlamlı kullanılabilir; ancak burada özellikle **okunabilir kısa özet kartı** kastedilir.

## Türkçe

> [ÇALIŞMA]'nın en önemli üç bulgusunu üç eşit blokta özetleyen visual abstract oluştur.
>
> Her blok:
>
> - bir sayı/bulgu,
> - kısa açıklama,
> - yalnız gerektiğinde küçük ikon/şema
>
> içersin.
>
> Bulgular kullanıcı tarafından verilmediyse veri uydurma.

## English

> Create a visual abstract summarizing the three most important findings of [STUDY] in three balanced sections.
>
> Each section should contain one result or number, one concise explanation, and a small icon or diagram only when useful.
>
> Do not invent findings that were not supplied.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1182. `/methods-figure` — Yöntem Akış Figürü

## Türkçe

> [DENEY/ARAŞTIRMA YÖNTEMİ]'nı 4–7 adımda methods figure olarak göster.
>
> Örnek sıralama:
>
> örnekleme → hazırlama → ölçüm → analiz → sonuç.
>
> Her panelde yalnız bir işlem olsun.
>
> Kullanılan cihaz/ölçüm adları doğru verilmediyse jenerik ama açık placeholder kullan.

## English

> Show [EXPERIMENT/RESEARCH METHOD] as a 4–7 step methods figure.
>
> A typical flow may be sampling → preparation → measurement → analysis → result.
>
> Keep one primary action per panel.
>
> If exact instruments or measurements are not supplied, use clearly generic placeholders rather than inventing equipment.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1183. `/experimental-setup` — Deney Düzeneği

## Türkçe

> [DENEY]'in gerçek fiziksel düzeneğini sade teknik illüstrasyon olarak göster.
>
> Cihazlar arası:
>
> - bağlantı,
> - yön,
> - mesafe/konum,
> - ölçüm noktası
>
> anlaşılır olsun.
>
> Görseli laboratuvar “sci-fi” sahnesine dönüştürme.

## English

> Show the real physical setup of [EXPERIMENT] as a restrained technical illustration.
>
> Make connections, direction, relative placement, and measurement points understandable.
>
> Avoid turning the laboratory into a science-fiction scene.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1184. `/control-vs-treatment` — Kontrol / Deney Karşılaştırması

## Türkçe

> Aynı deneyin control ve treatment koşullarını iki eşit panelde göster.
>
> Kamera, örnek boyutu, kap, ışık ve diğer koşullar eşleşsin.
>
> Yalnız değiştirilen bağımsız değişken farklı olsun.
>
> Sonucu daha dramatik göstermek için panel tasarımını değiştirme.

## English

> Show control and treatment conditions of the same experiment in matched side-by-side panels.
>
> Keep camera, sample size, container, light, and other conditions identical.
>
> Change only the independent variable.
>
> Do not change visual framing to exaggerate the result.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1185. `/uncertainty-figure` — Belirsizlik Görselleştirme

## Türkçe

> [VERİ]'de yalnız merkezi değeri değil belirsizliği de göster.
>
> Uygun olduğunda:
>
> - error bars,
> - confidence interval,
> - distribution,
> - range,
> - sample points
>
> kullan.
>
> Belirsizliği dekoratif gradient ile temsil etme; gerçek istatistiksel anlamı olsun.

## English

> Visualize uncertainty in [DATA] rather than showing only central values.
>
> Use error bars, confidence intervals, distributions, ranges, or individual sample points when appropriate.
>
> Do not represent uncertainty as a decorative gradient without statistical meaning.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1186. `/raw-data-overlay` — Ham Veri + Özet

## Türkçe

> [VERİ]'yi yalnız bar/ortalama ile değil, mümkün olduğunda bireysel data points ile birlikte göster.
>
> Özet çizgisi/ortalama ikincil olsun; örneklerin dağılımı görünür kalsın.

## English

> Show [DATA] with individual data points whenever appropriate rather than only bars or averages.
>
> Keep summary statistics secondary and preserve visibility of the underlying distribution.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1187. `/scientific-cover` — Bilimsel Dergi Kapağı

## Trend

**T1 — 2026 Nature özel sayısı bilimsel kapak tasarımını ayrıca öne çıkarıyor.**

## Türkçe prompt

> [BİLİMSEL KONU]'yu bilimsel dergi kapağı için tek güçlü görsel metafor veya bilimsel yapı üzerinden anlat.
>
> Görsel:
>
> - bilimsel olarak anlamlı,
> - ilk bakışta güçlü,
> - ayrıntıda zengin,
> - ama aşırı infografik olmayan
>
> tek kompozisyon olsun.
>
> DNA heliksi, atom, beyin, mavi neon ağ gibi jenerik bilim klişelerini yalnız gerçekten konuyla ilgiliyse kullan.

## English

> Create one strong scientific-journal-cover visual for [SCIENTIFIC TOPIC] built around a meaningful scientific structure or metaphor.
>
> Make it scientifically relevant, immediately legible, rich in detail, but not overloaded like an infographic.
>
> Use generic science clichés such as DNA helices, atoms, brains, and glowing blue networks only when genuinely relevant.

---

# 1188. `/specimen-plate-modern` — Modern Specimen Plate

## Türkçe

> [TÜR/ÖRNEK GRUBU]'nu modern scientific specimen plate olarak göster.
>
> Her örnek:
>
> - aynı ölçek mantığı,
> - yeterli boşluk,
> - numara,
> - kısa ad
>
> ile yerleşsin.
>
> Dekoratif vintage çerçeve kullanma.

## English

> Show [SPECIES/SPECIMEN GROUP] as a modern scientific specimen plate.
>
> Use consistent scale logic, adequate spacing, numbering, and concise names.
>
> Avoid decorative vintage framing.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1189. `/comparative-anatomy` — Karşılaştırmalı Anatomi

## Türkçe

> [TÜR A] ve [TÜR B]'nin aynı anatomik yapısını eşleşmiş görünüm ve ölçekte karşılaştır.
>
> Kamera/görüş yönü aynı olsun.
>
> Homolog veya farklı yapılar aynı renk koduyla tutarlı gösterilsin.
>
> Bilimsel ilişkiyi kaynak doğrulaması olmadan uydurma.

## English

> Compare the same anatomical structure in [SPECIES A] and [SPECIES B] using matched orientation and scale.
>
> Keep viewing direction identical.
>
> Use consistent color coding for corresponding or different structures.
>
> Do not invent biological relationships without source verification.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1190. `/fossil-reconstruction-pair` — Fosil + Rekonstrüksiyon

## Türkçe

> [FOSİL]'i iki panelde göster:
>
> 1. gerçek/teknik fosil görünümü,
> 2. kanıta dayalı yaşam rekonstrüksiyonu.
>
> İkinci panelde doğrudan kanıtlanmayan renk, tüy, deri veya yumuşak doku ayrıntılarının spekülatif olduğunu açıkça ayır.

## English

> Show [FOSSIL] in two panels:
>
> 1. fossil or technical specimen view,
> 2. evidence-based life reconstruction.
>
> Clearly distinguish speculative coloration, feathers, skin, or soft-tissue details that are not directly supported by evidence.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1191. `/evidence-layer` — Kanıt Seviyesi Katmanı

## Yeni rehber aracı

Bilimsel rekonstrüksiyonlarda görselin üzerine kanıt seviyesini eklemek için.

## Türkçe

> Görseldeki unsurları üç kategoriyle işaretle:
>
> - doğrudan kanıt,
> - güçlü çıkarım,
> - spekülatif.
>
> Renkleri yalnız legend ile ve sınırlı kullan.

## English

> Mark visual elements using three evidence categories:
>
> - directly evidenced,
> - strongly inferred,
> - speculative.
>
> Use restrained color coding with a clear legend.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar içeriği sadeleştirebilir ama değiştiremez.

---
# 1192. `/scientific-figure-slop-filter` — Bilimsel Görsel AI Slop Filtresi

Kaçınılması gerekenler:

- glow,
- neon mavi ağ,
- anlamsız DNA heliksi,
- her molekülün 3B parlak top olması,
- okların neyi gösterdiğinin belli olmaması,
- sahte ölçüm değerleri,
- uydurma organ/katman,
- gerçek olmayan ölçek ilişkileri,
- grafiklerde uydurma veri,
- bilimsel isimlerin yanlış yazılması,
- “profesyonel görünüyor” diye doğruluk varsaymak.

---

# 1193. `/architecture-review-board` — Mimari Review Board

## Trend

**T1/T2 — 2026'da mimari sunum statik finalden canlı karar alanına kayıyor.**

ArchDaily'nin Ağustos 2026 değerlendirmesi, tasarım sunumlarının yalnız sonuç göstermek yerine malzeme, seçenek ve çevresel koşulların tartışıldığı **canlı karar verme alanına** dönüştüğünü vurguluyor.

## Türkçe prompt

> [MİMARİ PROJE] için karar vermeyi destekleyen architecture review board oluştur.
>
> Board üzerinde:
>
> - tek ana mevcut öneri,
> - 2 küçük alternatif,
> - 1 plan veya diagram,
> - 1 malzeme karşılaştırması,
> - 2–3 kısa karar sorusu
>
> bulunsun.
>
> Board yalnız final render gösteren yarışma posteri olmasın.

## English

> Create an architecture review board for [PROJECT] that supports live design decisions.
>
> Include one primary current proposal, two small alternatives, one plan or diagram, one material comparison, and 2–3 concise decision questions.
>
> Do not treat it as a final competition poster containing only polished renders.

---

# 1194. `/option-board` — Tasarım Alternatifleri Board'u

## Türkçe

> Aynı proje için A/B/C olmak üzere üç alternatif göster.
>
> Kamera ve ölçek eşleşsin.
>
> Her alternatif yalnız 1–2 tasarım değişkeninde farklı olsun.
>
> Altında değişen unsurları kısa listeyle belirt.

## English

> Show three alternatives A/B/C for the same project using matched camera and scale.
>
> Let each option differ in only 1–2 design variables.
>
> Add a concise note describing what changes between them.

## Neye dikkat edilmeli?

Alternatif panolarda bakış açısı ve ışık sabit kalsın; değişen yalnız incelenen değişken olsun ([§23](10-temeller-001-222.md#sec-23) mantığı).

---
# 1195. `/material-option-board` — Malzeme Alternatifleri

## Türkçe

> Aynı cephe/oda için üç malzeme alternatifi göster.
>
> Geometri, kamera, gün saati ve ışık aynı kalsın.
>
> Yalnız malzeme ve onun yansıma/roughness davranışı değişsin.
>
> Farkı dramatik göstermek için ışığı değiştirme.

## English

> Compare three material options for the same facade or room.
>
> Keep geometry, camera, time of day, and lighting identical.
>
> Change only material and its reflection or roughness behavior.
>
> Do not alter lighting to exaggerate differences.

## Neye dikkat edilmeli?

Alternatif panolarda bakış açısı ve ışık sabit kalsın; değişen yalnız incelenen değişken olsun ([§23](10-temeller-001-222.md#sec-23) mantığı).

---
# 1196. `/daylight-option-board` — Günışığı Karşılaştırması

## Türkçe

> Aynı mekânı sabah, öğle ve akşam güneşi koşullarında üç panelde göster.
>
> Kamera ve malzemeler aynı kalsın.
>
> Güneş yönü coğrafi/yön bilgisine göre verilmişse onu koru.
>
> Geometriyi her panelde değiştirme.

## English

> Show the same space in morning, midday, and evening daylight across three panels.
>
> Keep camera and materials identical.
>
> Preserve supplied geographic or orientation information for sun direction.
>
> Do not change geometry between panels.

## Neye dikkat edilmeli?

Alternatif panolarda bakış açısı ve ışık sabit kalsın; değişen yalnız incelenen değişken olsun ([§23](10-temeller-001-222.md#sec-23) mantığı).

---
# 1197. `/season-option-board` — Mevsim Karşılaştırması

## Türkçe

> Aynı dış mekânı dört mevsimde matched-view olarak göster.
>
> Yapı, kamera, bitki türü ve çevre geometrisi aynı kalsın.
>
> Yalnız mevsime bağlı yaprak, kar, ışık ve kullanım davranışı değişsin.

## English

> Show the same exterior in four seasons using matched views.
>
> Keep building, camera, plant species, and environmental geometry identical.
>
> Change only season-dependent foliage, snow, light, and use patterns.

## Neye dikkat edilmeli?

Alternatif panolarda bakış açısı ve ışık sabit kalsın; değişen yalnız incelenen değişken olsun ([§23](10-temeller-001-222.md#sec-23) mantığı).

---
# 1198. `/architecture-sequence` — Mekânsal Deneyim Dizisi

## Türkçe

> [YAPI]'daki kullanıcı deneyimini 5 karelik yürüyüş dizisi olarak göster:
>
> yaklaşma → giriş → geçiş → ana mekân → çıkış/manzara.
>
> Aynı yapının mekânsal sürekliliğini koru.
>
> Beş kareyi birbirinden kopuk “hero render”lara dönüştürme.

## English

> Show the user experience through [BUILDING] as a five-frame spatial sequence:
>
> approach → entry → transition → primary space → exit/view.
>
> Preserve spatial continuity.
>
> Avoid turning the sequence into five unrelated hero renders.

## Neye dikkat edilmeli?

Alternatif panolarda bakış açısı ve ışık sabit kalsın; değişen yalnız incelenen değişken olsun ([§23](10-temeller-001-222.md#sec-23) mantığı).

---
# 1199. `/architecture-storyboard` — Mimari Kullanım Storyboard'u

## Türkçe

> [MEKÂN]'ın gün içindeki kullanımını 4–6 karelik storyboard olarak göster.
>
> İnsanlar yalnız ölçek ve kullanım senaryosunu açıklasın.
>
> Aynı kişinin her karede reklam modeli gibi poz vermesi gerekmez.

## English

> Show how [SPACE] is used across the day in a 4–6 frame storyboard.
>
> Use people only to explain scale and activity.
>
> Avoid having the same person pose like an advertising model in every frame.

## Neye dikkat edilmeli?

Alternatif panolarda bakış açısı ve ışık sabit kalsın; değişen yalnız incelenen değişken olsun ([§23](10-temeller-001-222.md#sec-23) mantığı).

---
# 1200. `/architecture-exploded-program` — Programatik Exploded Axon

## Türkçe

> Yapıyı kat/program zonlarına göre exploded axonometric olarak ayır.
>
> Her katın aynı footprint/aks ilişkisini koru.
>
> Programı en fazla 5 renk ile kodla.
>
> Yapısal olmayan rastgele dekor parçalarını patlatılmış görünüme dahil etme.

## English

> Separate the building by floor or program zone in an exploded axonometric.
>
> Keep each level aligned to the same footprint and axes.
>
> Use no more than five colors for program coding.
>
> Do not explode random decorative elements that do not support the explanation.

## Neye dikkat edilmeli?

Alternatif panolarda bakış açısı ve ışık sabit kalsın; değişen yalnız incelenen değişken olsun ([§23](10-temeller-001-222.md#sec-23) mantığı).

---
# 1201. `/architecture-process-board` — Eskizden Modele Mimari Süreç

## Türkçe

> [PROJE]'nin tasarım gelişimini 5 aşamada göster:
>
> 1. site/problem,
> 2. ilk kütle,
> 3. boşaltma/ekleme,
> 4. dolaşım/ışık,
> 5. final kütle.
>
> Her aşama bir öncekinin anlaşılır dönüşümü olsun.

## English

> Show the design evolution of [PROJECT] in five stages:
>
> 1. site/problem,
> 2. initial mass,
> 3. subtraction/addition,
> 4. circulation/light,
> 5. final mass.
>
> Make every stage a clear transformation of the previous one.

## Neye dikkat edilmeli?

Alternatif panolarda bakış açısı ve ışık sabit kalsın; değişen yalnız incelenen değişken olsun ([§23](10-temeller-001-222.md#sec-23) mantığı).

---
# 1202. `/architecture-pinup` — Pin-up Wall

## Türkçe prompt

> Mimari proje geliştirme sürecini fiziksel pin-up wall üzerinde göster.
>
> 8–12 çıktı:
>
> plan, kesit, eskiz, render, diyagram ve malzeme örneklerinden oluşsun.
>
> Hepsi aynı boyutta poster olmasın.
>
> Gerçek çalışma sürecindeki ölçek/hiyerarşi hissini koru.

## English

> Show an architectural project-development process on a physical pin-up wall using 8–12 outputs such as plans, sections, sketches, renders, diagrams, and material samples.
>
> Do not make every item the same poster size.
>
> Preserve the hierarchy and scale variation of a real working review.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar (duvar dizimi, çocuk kitabı dili) içeriği sadeleştirebilir ama değiştiremez.

---
# 1203. `/architecture-crit-wall` — Tasarım Kritiği Duvarı

## Türkçe

> `/architecture-pinup` düzenine az miktarda gerçek critique annotation ekle:
>
> - 3–5 kısa el yazısı soru,
> - 2 ok,
> - 1 daire içine alınmış sorun alanı.
>
> Kırmızı kalemle bütün paftayı karalama.

## English

> Add a small amount of genuine critique annotation to an `/architecture-pinup` wall:
>
> - 3–5 concise handwritten questions,
> - 2 arrows,
> - one circled problem area.
>
> Do not cover the board in red-marker scribbles.

## Neye dikkat edilmeli?

Alternatif panolarda bakış açısı ve ışık sabit kalsın; değişen yalnız incelenen değişken olsun ([§23](10-temeller-001-222.md#sec-23) mantığı).

---
# 1204. `/architecture-slop-filter` — Mimari AI Slop Filtresi

Kaçınılması gerekenler:

- her renderda golden hour,
- her iç mekânda sis/volumetric rays,
- yapının geometrisinin paneller arasında değişmesi,
- anlamsız ağaç türleri,
- yanlış ölçekli insanlar,
- her yüzeyin mermer/cam/ahşap olması,
- “minimal” = boş beyaz villa,
- her cephede dikey yeşil duvar,
- board üzerinde 20 tiny diagram,
- kullanıcı kararına hizmet etmeyen render kalabalığı.

---

# 1205. `/type-specimen-poster` — Tipografi Specimen Posteri

## Trend

**T1 — typographic experimentation 2026'da güçlü.**

## Türkçe prompt

> [FONT/TİPOGRAFİ KARAKTERİ]'ni anlatan type specimen poster oluştur.
>
> Kullan:
>
> - bir büyük kelime,
> - büyük/küçük harf dizisi,
> - rakamlar,
> - 1 kısa metin bloğu.
>
> Fontun karakterini gerçek glyph yapısı üzerinden göster.
>
> Gereksiz 3B efekt ekleme.

## English

> Create a type-specimen poster for [FONT/TYPOGRAPHIC CHARACTER].
>
> Use one large word, upper/lowercase alphabet sample, numerals, and one concise text block.
>
> Demonstrate character through actual glyph structure.
>
> Avoid unnecessary 3D effects.

---

# 1206. `/kinetic-type-still` — Kinetik Tipografi Karesi

## Türkçe

> [KELİME/KISA CÜMLE]'yi hareket hissi taşıyan tipografik kompozisyon olarak göster.
>
> Hareket:
>
> - yönsel tekrar,
> - baseline kayması,
> - ölçek değişimi,
> - kontrollü stretch
>
> gibi tek ana mekanizma ile kurulsun.
>
> Okunabilirliği tamamen kaybetme.

## English

> Show [WORD/SHORT PHRASE] as a kinetic typographic composition.
>
> Build movement through one primary device such as directional repetition, baseline shift, scale change, or controlled stretching.
>
> Do not sacrifice readability completely.

## Neye dikkat edilmeli?

Yazı görselin öznesiyse her harf denetlenir; Türkçe karakterler ve satır kırılmaları baskı boyutunda okunur.

---
# 1207. `/variable-font-poster` — Variable Font Ekseni Posteri

## Türkçe

> Aynı kelimeyi tek variable font'un weight/width/slant gibi gerçek eksenlerinden biri boyunca 5–7 aşamada göster.
>
> Değişim düzenli ve anlaşılır olsun.
>
> Beş farklı font kullanıp “variable” deme.

## English

> Show the same word across 5–7 stages along one real variable-font axis such as weight, width, or slant.
>
> Keep the progression systematic.
>
> Do not use five unrelated fonts and call it variable typography.

## Neye dikkat edilmeli?

Yazı görselin öznesiyse her harf denetlenir; Türkçe karakterler ve satır kırılmaları baskı boyutunda okunur.

---
# 1208. `/oversized-type` — Oversized Editorial Type

## Trend

**T1/T2.**

## Türkçe

> Poster veya kapakta tek kelimeyi kadrajın büyük bölümünü kaplayacak ölçekte kullan.
>
> Harfler kenarlardan taşabilir ancak okunabilir kök form kalsın.
>
> Büyük tipografiyi arka plan dekoru olarak değil ana kompozisyon elemanı yap.

## English

> Use one word at very large scale so it occupies most of the poster or cover.
>
> Letters may crop at the edges while preserving the core readable form.
>
> Treat type as the primary composition rather than background decoration.

---

# 1209. `/type-image-interlock` — Tipografi + Görsel Kilitlenmesi

## Türkçe

> [GÖRSEL] ile [BAŞLIK]'ı birbirinden bağımsız iki katman gibi değil, kontrollü overlap/interlock ilişkisiyle düzenle.
>
> Harfler yalnız 1–2 noktada öznenin önüne/arkasına geçsin.
>
> Yüz ve önemli bilgi alanlarını kapatma.

## English

> Integrate [IMAGE] and [TITLE] through a controlled overlap or interlock rather than treating them as unrelated layers.
>
> Let letters pass in front of or behind the subject at only 1–2 deliberate points.
>
> Do not cover faces or critical information.

## Neye dikkat edilmeli?

Yazı görselin öznesiyse her harf denetlenir; Türkçe karakterler ve satır kırılmaları baskı boyutunda okunur.

---
# 1210. `/type-only-poster` — Yalnız Tipografi Posteri

## Türkçe

> [MESAJ]'ı hiçbir fotoğraf, ikon veya illüstrasyon kullanmadan tipografiyle anlat.
>
> Yalnız:
>
> - ölçek,
> - ağırlık,
> - aralık,
> - hizalama,
> - satır kırılması
>
> kullanarak hiyerarşi oluştur.

## English

> Communicate [MESSAGE] using typography only, without photographs, icons, or illustration.
>
> Build hierarchy solely through scale, weight, spacing, alignment, and line breaks.

## Neye dikkat edilmeli?

Yazı görselin öznesiyse her harf denetlenir; Türkçe karakterler ve satır kırılmaları baskı boyutunda okunur.

---
# 1211. `/hand-lettered-poster` — El Yazısı / Lettering Posteri

## Türkçe

> [KISA SÖZ]'ü gerçek elle yazılmış/çizilmiş lettering olarak posterleştir.
>
> Harfler tutarlı bir el hareketinden çıkmış gibi olsun.
>
> Hafif baseline/kalınlık farklılığı olabilir.
>
> “Handmade” diye her harfi farklı stile dönüştürme.

## English

> Turn [SHORT PHRASE] into a poster using genuinely hand-drawn lettering.
>
> Keep the letterforms consistent with one hand and one drawing process.
>
> Allow slight baseline and stroke variation.
>
> Do not make every letter a different style merely to look handmade.

## Neye dikkat edilmeli?

Yazı görselin öznesiyse her harf denetlenir; Türkçe karakterler ve satır kırılmaları baskı boyutunda okunur.

---
# 1212. `/stamp-type` — Damga Tipografi

## Türkçe

> [KELİME]'yi gerçek kauçuk/metal damga baskısı gibi göster.
>
> Harf kenarlarında küçük mürekkep eksikliği ve basınç farkı olabilir.
>
> Aynı kusuru her harfte tekrar etme.

## English

> Render [WORD] as a real rubber- or metal-stamp impression.
>
> Allow small ink gaps and pressure variation at letter edges.
>
> Do not repeat identical distress patterns on every character.

## Neye dikkat edilmeli?

Yazı görselin öznesiyse her harf denetlenir; Türkçe karakterler ve satır kırılmaları baskı boyutunda okunur.

---
# 1213. `/xerox-type` — Xerox Tipografi

## Türkçe

> [BAŞLIK]'ı fotokopi makinesinden birkaç kez geçirilmiş yüksek kontrast tipografi gibi göster.
>
> Toner kırılması ve kenar roughness görülebilir.
>
> Harf formu hâlâ okunabilir olsun.

## English

> Render [TITLE] as high-contrast typography that has been passed through a photocopier several times.
>
> Allow toner breakup and edge roughness while preserving readable letterforms.

## Neye dikkat edilmeli?

Yazı görselin öznesiyse her harf denetlenir; Türkçe karakterler ve satır kırılmaları baskı boyutunda okunur.

---
# 1214. `/type-slop-filter` — Tipografi AI Slop Filtresi

Kaçınılması gerekenler:

- her posterde aynı condensed bold,
- chrome + bevel + glow,
- okunmayan deneysel deformasyon,
- 5–8 font,
- tipografinin yalnız görsel boşluğu doldurması,
- rastgele harflerin dönmesi,
- “handmade” = bilinçsiz düzensizlik,
- fake editorial = dev serif + küçük lorem ipsum.

---

# 1215. `/picturebook-scene` — Çocuk Kitabı Sahnesi

## Evergreen / eğitimle ilişkili

## Türkçe prompt

> [HİKÂYE SAHNESİ]'ni çocuk kitabı illüstrasyonu olarak oluştur.
>
> Önce:
>
> - yaş aralığı,
> - duygusal ton,
> - karakter sayısı,
> - olay,
> - ortam
>
> belirle.
>
> Çocuk kitabı = otomatik pastel/kawaii/chibi değildir.
>
> Karakterlerin eylemi hikâyeyi açıkça taşısın.

## English

> Illustrate [STORY SCENE] for a children's book.
>
> Define age range, emotional tone, number of characters, action, and setting first.
>
> Do not equate children's illustration automatically with pastel, kawaii, or chibi styling.
>
> Make character actions carry the story clearly.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe [§18](10-temeller-001-222.md#sec-18) listesiyle kaynaktan doğrulanır; estetik kararlar (duvar dizimi, çocuk kitabı dili) içeriği sadeleştirebilir ama değiştiremez.

---
# 1216. `/character-turnaround-kids` — Çocuk Kitabı Karakter Tutarlılığı

## Türkçe

> [KARAKTER]'i ön, 3/4, yan, arka ve üç temel ifade ile character turnaround/model sheet olarak göster.
>
> Kıyafet, saç, renk, aksesuar ve vücut oranı tüm görünümlerde aynı olsun.
>
> Bu sayfa sonraki illüstrasyonlarda tutarlılık referansı olarak kullanılacak.

## English

> Show [CHARACTER] in front, three-quarter, side, back, and three primary expressions as a character turnaround or model sheet.
>
> Keep clothing, hair, color, accessories, and body proportions consistent.
>
> Treat the sheet as a continuity reference for later illustrations.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1217. `/same-character-sequence` — Aynı Karakter Hikâye Dizisi

## Türkçe

> Aynı karakteri dört sahnede göster.
>
> Kimlik, kıyafet ve renkler sabit kalsın.
>
> Yalnız olay, poz ve ifade değişsin.
>
> Karakter her panelde yeniden tasarlanmasın.

## English

> Show the same character across four story scenes.
>
> Keep identity, clothing, and colors fixed.
>
> Change only action, pose, and expression.
>
> Do not redesign the character in every panel.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1218. `/wordless-sequence` — Yazısız Hikâye

## Türkçe

> [OLAY]'ı metin kullanmadan 4–6 görsel panelde anlat.
>
> Her panel bir öncekinin devamı olsun.
>
> Ana karakter, yön, nesne ve mekân sürekliliği korunmalı.
>
> Hikâye yalnız yüz ifadeleri değil, eylem ve çevresel değişimle anlaşılmalı.

## English

> Tell [EVENT] without text across 4–6 visual panels.
>
> Make every panel continue from the previous one.
>
> Preserve character, direction, object, and setting continuity.
>
> Let the story emerge through action and environmental change rather than facial expressions alone.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1219. `/educational-story-scene` — Öğretici Hikâye Sahnesi

## Türkçe

> [KAVRAM]'ı doğrudan diyagram yerine kısa gündelik hikâye sahnesiyle öğret.
>
> Sahnedeki olay kavramın gerçek neden-sonuç ilişkisini göstermeli.
>
> Görselin altında yalnız tek kısa açıklama alanı bırak.
>
> Ders konusunu maskot konuşma balonlarıyla aşırı basitleştirme.

## English

> Teach [CONCEPT] through a short everyday story scene rather than a direct diagram.
>
> Make the event demonstrate the real cause-and-effect relationship.
>
> Leave space for one concise explanatory caption.
>
> Avoid oversimplifying the topic through mascot speech bubbles.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1220. `/concept-cartoon` — Kavram Karikatürü

## Eğitim

## Türkçe

> [KAVRAM] hakkında 3 öğrencinin farklı görüş öne sürdüğü concept cartoon oluştur.
>
> Bir görüş bilimsel olarak doğru; diğer ikisi yaygın yanılgılar olsun.
>
> Karakterler nötr ve eşit görsel ağırlıkta gösterilsin; doğru cevabı yüz ifadesi veya vurgu rengiyle ele verme.

## English

> Create a concept cartoon in which three students express different ideas about [CONCEPT].
>
> One statement should be scientifically correct and two should represent common misconceptions.
>
> Give all characters equal visual weight and do not reveal the correct answer through expression or color emphasis.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1221. `/misconception-pair` — Yanılgı / Doğru Model Karşılaştırması

## Türkçe

> [KONU] için iki eşit panel oluştur:
>
> sol = yaygın yanlış model,
> sağ = doğru bilimsel model.
>
> Aynı görsel dil ve ölçek kullan.
>
> Farkı yalnız gerekli yapısal noktalar üzerinden göster.

## English

> Create matched panels for [TOPIC]:
>
> left = common misconception,
> right = scientifically correct model.
>
> Use the same visual language and scale.
>
> Highlight only the structural differences necessary for understanding.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1222. `/observe-predict-explain` — Gözle–Tahmin Et–Açıkla

## Türkçe

> [DENEY/OLAY] için üç panelli eğitim görseli oluştur:
>
> 1. Gözle — başlangıç sahnesi,
> 2. Tahmin et — sonucu göstermeyen soru alanı,
> 3. Açıkla — gerçek sonuç ve kısa açıklama.
>
> İlk iki panelde sonucu görsel ipucuyla ele verme.

## English

> Create a three-panel learning visual for [EXPERIMENT/EVENT]:
>
> 1. Observe — initial scene,
> 2. Predict — question area without revealing the outcome,
> 3. Explain — actual result with concise explanation.
>
> Do not leak the answer visually in the first two panels.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1223. `/visual-routine` — Görsel Düşünme Rutini

## Türkçe

> [GÖRSEL/KONU] için “Görüyorum – Düşünüyorum – Merak Ediyorum” çalışma sayfası oluştur.
>
> Üstte tek görsel, altta üç geniş yazma alanı olsun.
>
> Alanları sticker veya dekorla küçültme.

## English

> Create a “See – Think – Wonder” worksheet for [IMAGE/TOPIC].
>
> Use one image at the top and three generous writing areas below.
>
> Do not reduce writing space with decoration or stickers.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1224. `/picturebook-slop-filter` — Çocuk/Eğitim İllüstrasyonu AI Slop Filtresi

Kaçınılması gerekenler:

- her karakterde dev göz,
- her sayfada pastel,
- her nesneye yüz,
- eğitim = konuşan maskot,
- çocuk = “cute commercial character”,
- her sahnede gökkuşağı,
- çocukların yaşına uymayan bilgi yoğunluğu,
- her panelde farklı karakter tasarımı,
- gerçek bilimsel yapıyı sevimlilik uğruna bozmak.

---

# 1225. `/diagram-poster` — Diyagramı Posterleştirme

## Trend / kullanım

Bilimsel/eğitsel diyagramı dekoratif postere dönüştürürken bilgi kaybını önlemek için.

## Türkçe

> [DİYAGRAM]'ın gerçek bilgi yapısını koru ancak poster kompozisyonuna dönüştür.
>
> Ana bilgi merkezi veya tek eksen üzerinde okunabilir olsun.
>
> Başlık, legend ve 3–5 temel etiket dışında metni azalt.
>
> Poster estetiği uğruna okların/yönlerin anlamını değiştirme.

## English

> Preserve the real information structure of [DIAGRAM] while adapting it into a poster composition.
>
> Keep the primary information readable around one center or axis.
>
> Reduce text to title, legend, and 3–5 essential labels.
>
> Do not change directional meaning for aesthetic reasons.

---

# 1226. `/data-art-safe` — Veri Sanatı, Veriyi Bozmadan

## Türkçe

> [VERİ]'yi sanatsal bir görsel yapıya dönüştür ancak veri eşlemesini açık tut.
>
> Her:
>
> - renk,
> - boyut,
> - konum,
> - tekrar
>
> gerçek bir veri değişkenine karşılık gelsin.
>
> Görsel etkileyici olsun diye veri oranlarını değiştirme.

## English

> Transform [DATA] into an artistic visual structure while keeping the data mapping explicit.
>
> Every color, size, position, or repetition must correspond to a real variable.
>
> Do not distort quantities for visual impact.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1227. `/physical-data-art` — Fiziksel Veri Sanatı

## Türkçe

> [VERİ]'yi fiziksel malzemeyle temsil et:
>
> iplik, kâğıt, boncuk, blok, çubuk veya küçük nesnelerden yalnız birini seç.
>
> 1 fiziksel birimin kaç veri birimine karşılık geldiğini açık legend ile belirt.
>
> Nesne sayısını doğru tut.

## English

> Represent [DATA] physically using one material system such as thread, paper, beads, blocks, rods, or small objects.
>
> State clearly how one physical unit maps to the data.
>
> Keep object counts accurate.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1228. `/small-multiple-data-art` — Small Multiple Veri Sanatı

## Türkçe

> [VERİ]'yi aynı görsel gramerle 6–12 küçük panelde karşılaştır.
>
> Tüm paneller aynı ölçek ve eksen mantığını kullansın.
>
> Her paneli ayrı dekoratif sanat eserine dönüştürme.

## English

> Compare [DATA] across 6–12 small panels using one consistent visual grammar.
>
> Keep scale and axis logic identical.
>
> Do not turn each panel into an unrelated decorative artwork.

## Neye dikkat edilmeli?

Karakter ve kavram bütün karelerde sabit kalsın; eğitsel iddia ([§18](10-temeller-001-222.md#sec-18)) kaynağıyla doğrulanır, sevimlilik doğruluğun önüne geçmesin.

---
# 1229. `/data-art-slop-filter` — Veri Sanatı AI Slop Filtresi

Kaçınılması gerekenler:

- sayı doğru değil ama “güzel” görünüyor,
- veri olmadan fake dashboard,
- her şey radial chart,
- anlamsız neon node network,
- 3B bar'ların perspektifle değeri bozması,
- renk legend'ı yok,
- aynı değişkeni hem boyut hem renk hem yükseklikle gereksiz tekrar etmek.

---

# 1230. `/ui-screenshot-editorial` — UI Screenshot Editorial

## Trend

**T1/T2 — Canva Prompt Playground ile uyumlu.**

## Türkçe

> Gerçek veya kurmaca [ARAYÜZ] ekranını posterin ana görseli olarak kullan.
>
> Screenshot bütün poster olmak zorunda değil; kontrollü crop ile tek işlevi vurgula.
>
> Çevrede yalnız başlık ve 1–2 kısa annotation kullan.
>
> UI'yi 3B cam panele dönüştürme.

## English

> Use a real or fictional [INTERFACE] screenshot as the primary visual in an editorial poster.
>
> The screenshot does not need to fill the entire composition; crop it deliberately around one function.
>
> Add only a title and 1–2 concise annotations.
>
> Do not transform the UI into a floating glass 3D panel.

---

# 1231. `/ui-before-after` — UI Before/After

## Türkçe

> Aynı arayüzü önce/sonra karşılaştır.
>
> İçerik, ekran boyutu ve ana bilgi aynı kalsın.
>
> Yalnız düzen, tipografi, renk veya interaction hierarchy değişsin.
>
> “Sonra” sürümünde özellik ekleyip karşılaştırmayı haksızlaştırma.

## English

> Compare the same interface before and after.
>
> Keep content, viewport size, and primary information identical.
>
> Change only layout, typography, color, or interaction hierarchy.
>
> Do not add new features to make the “after” version unfairly stronger.

## Neye dikkat edilmeli?

Arayüz metinleri gerçek ürün diliyle yazılsın; uydurma buton ve sahte bildirim güveni bitirir.

---
# 1232. `/ui-state-sheet` — Arayüz Durumları

## Türkçe

> [BİLEŞEN]'in tüm temel durumlarını aynı sheet üzerinde göster:
>
> default, hover, active, disabled, loading, error, success.
>
> Boyut ve yerleşim aynı kalsın.
>
> Her durumun farkı işlevsel olarak görünür olsun.

## English

> Show all primary states of [COMPONENT] on one sheet:
>
> default, hover, active, disabled, loading, error, success.
>
> Keep dimensions and layout fixed.
>
> Make every state difference functionally visible.

## Neye dikkat edilmeli?

Arayüz metinleri gerçek ürün diliyle yazılsın; uydurma buton ve sahte bildirim güveni bitirir.

---
# 1233. `/ui-flow-strip` — UI Akış Şeridi

## Türkçe

> [GÖREV]'i 4–6 ekranlık yatay user-flow strip olarak göster.
>
> Her ekranda yalnız bir önemli kullanıcı kararı olsun.
>
> Oklar yalnız ekranlar arasındaki gerçek geçişi göster.

## English

> Show [TASK] as a horizontal 4–6 screen user-flow strip.
>
> Keep one important user decision per screen.
>
> Use arrows only for real transitions between states.

## Neye dikkat edilmeli?

Arayüz metinleri gerçek ürün diliyle yazılsın; uydurma buton ve sahte bildirim güveni bitirir.

---
# 1234. `/mobile-storyboard` — Mobil Kullanım Storyboard'u

## Türkçe

> [UYGULAMA]'yı yalnız ekran görüntüleriyle değil gerçek kullanım bağlamında 4 karede göster:
>
> telefonun çıkarılması → işlem → geri bildirim → işin tamamlanması.
>
> Kullanıcı ve cihaz fiziksel süreklilik taşısın.

## English

> Show [APP] across four frames in real usage context rather than screenshots alone:
>
> taking out the phone → action → feedback → task completion.
>
> Preserve continuity of user and device.

## Neye dikkat edilmeli?

Arayüz metinleri gerçek ürün diliyle yazılsın; uydurma buton ve sahte bildirim güveni bitirir.

---
# 1235. `/ui-window-collage` — Kontrollü Window Collage

## Türkçe

> [KONU]'yu 3 pencereyle anlat:
>
> bir ana pencere, bir detail panel, bir küçük note/metadata penceresi.
>
> Pencerelerin overlap'i içerik hiyerarşisini bozmasın.
>
> 20 popup kullanma.

## English

> Explain [TOPIC] using three windows:
>
> one primary window, one detail panel, and one small note or metadata window.
>
> Keep overlaps from obscuring hierarchy.
>
> Avoid dozens of popups.

## Neye dikkat edilmeli?

Arayüz metinleri gerçek ürün diliyle yazılsın; uydurma buton ve sahte bildirim güveni bitirir.

---
# 1236. `/screenshot-annotation` — Screenshot Annotation

## Türkçe

> Kaynak screenshot'u değiştirmeden 3–5 kısa annotation ile açıkla.
>
> Numara + kısa caption veya ince ok kullan.
>
> UI elemanlarının üstünü kapatacak büyük balonlar kullanma.

## English

> Explain the source screenshot without altering it using 3–5 concise annotations.
>
> Use numbered callouts with short captions or restrained arrows.
>
> Avoid large bubbles that obscure interface elements.

## Neye dikkat edilmeli?

Arayüz metinleri gerçek ürün diliyle yazılsın; uydurma buton ve sahte bildirim güveni bitirir.

---
# 1237. `/ui-slop-filter` — UI Görsel AI Slop Filtresi

Kaçınılması gerekenler:

- glassmorphism,
- her şeyin floating card olması,
- sahte 3B telefon mockup'u,
- işlevsiz placeholder text,
- fazla gradient,
- screenshot'u poster yapmak için ekranı eğip bükmek,
- UI'yi anlamadan dekoratif element eklemek,
- her ekranın farklı uygulamaya dönüşmesi.

---

# 1238. Yeni üst aile: `Evidence-aware Visual`

Bilimsel, tarihsel ve teknik görseller için yeni ortak üst sınıf:

> **Evidence-aware Visual — görselin hangi kısmının veriye/kanıta dayandığını açıkça yöneten prompt**

Bu aile:

- `/scientific-figure`
- `/fossil-reconstruction-pair`
- `/evidence-layer`
- `/historical-colorize`
- `/data-lock`
- `/comparative-anatomy`

gibi promptları bir arada tutar.

Temel formül:

> **source evidence + confirmed structure + inferred layer + speculative layer + verification**

---

# 1239. Yeni üst aile: `Decision Visual`

Mimari ve ürün tasarımında yalnız güzel sonuç değil karar verme görseli.

Aile:

- `/architecture-review-board`
- `/option-board`
- `/material-option-board`
- `/daylight-option-board`
- `/packaging-material-study`
- `/before-after`
- `/material-grid`

Ortak kural:

> **aynı kamera + aynı veri + tek değişken**

---

# 1240. Yeni üst aile: `Continuity Visual`

Aşağıdaki promptların ortak problemi “kareler arasında değişme”dir:

- `/same-character-sequence`
- `/same-person-grid`
- `/pet-story-triptych`
- `/architecture-sequence`
- `/photo-dump`
- `/three-polaroids`
- `/car-contact-sheet`

Yeni kısa kural:

> `/continuity-lock`

## Türkçe açılım

> Seri boyunca değişmemesi gereken kimlik, kıyafet, nesne geometrisi, ortam, zaman, ışık ve renk özelliklerini sabitle. Her kareyi aynı dünyanın devamı olarak üret.

## English

> Lock identity, clothing, object geometry, environment, time, lighting, and color properties that should remain unchanged across the series. Treat every frame as a continuation of the same world.

---

# 1241. `/format-matrix` — Tek Kaynaktan Çoklu Format Matrisi

## Yeni master prompt ailesi

## Türkçe

> Yüklenen tek kaynak görselden altı farklı çıktı üret:
>
> 1. 4:5 editorial poster,
> 2. 1:1 cover,
> 3. 9:16 story,
> 4. postcard,
> 5. sticker/label,
> 6. small publication cover.
>
> Her formatın kompozisyonunu kendi oranına göre yeniden düzenle.
>
> Aynı görseli yalnız crop ederek altı çıktı yapma.
>
> Kimlik, ana renk ve görsel hikâye aynı sistemde kalsın.

## English

> Create six outputs from one source image:
>
> 1. 4:5 editorial poster,
> 2. 1:1 cover,
> 3. 9:16 story,
> 4. postcard,
> 5. sticker or label,
> 6. small publication cover.
>
> Recompose each output for its actual aspect ratio rather than merely cropping the same image.
>
> Preserve identity, primary color relationships, and one coherent visual story.

## Neye dikkat edilmeli?

Arayüz metinleri gerçek ürün diliyle yazılsın; uydurma buton ve sahte bildirim güveni bitirir.

---
# 1242. `/format-matrix-lock` — Multi-format Tutarlılık

## Türkçe

> Tüm formatlarda:
>
> - aynı kişi/nesne,
> - aynı ana palet,
> - aynı tipografi ailesi,
> - aynı sembol dili
>
> korunsun.
>
> Ancak grid ve görsel ağırlık her formatın gerçek kullanımına göre değişsin.

## English

> Across all formats preserve the same person or object, primary palette, typography family, and symbol language.
>
> Let grid and visual weight change according to each format's real use.

## Neye dikkat edilmeli?

Arayüz metinleri gerçek ürün diliyle yazılsın; uydurma buton ve sahte bildirim güveni bitirir.

---
# 1243. `/campaign-system` — Tek Görselden Kampanya Sistemi

## Türkçe

> [KAYNAK/KAMPANYA FİKRİ]'nden:
>
> - hero poster,
> - social 4:5,
> - story,
> - banner,
> - thumbnail,
> - small print card
>
> oluşan kampanya sistemi üret.
>
> Her çıktıda farklı bilgi hiyerarşisi kullan.
>
> Hero posterin küçültülmüş hâlini her yerde tekrar etme.

## English

> Build a campaign system from [SOURCE/CAMPAIGN IDEA] containing hero poster, 4:5 social image, story, banner, thumbnail, and small print card.
>
> Use a different information hierarchy appropriate to every output.
>
> Do not reuse a scaled-down hero poster everywhere.

## Neye dikkat edilmeli?

Arayüz metinleri gerçek ürün diliyle yazılsın; uydurma buton ve sahte bildirim güveni bitirir.

---
# 1244. `/campaign-slop-filter` — Çoklu Format AI Slop

Kaçınılması gerekenler:

- aynı tasarımı 6 crop olarak üretmek,
- 9:16 story'de yatay poster mantığı,
- thumbnail'da 20 kelime,
- her formatta aynı font boyutu,
- aynı dekor öğesini zorunlu taşımak,
- mobilde okunmayan küçük yazı,
- format değiştiğinde kimlik/ürün değişmesi.

---

# 1245. Bu turdaki slash-style indeks (aile-015)

| Kısayol | Aile |
|---|---|
| `/scientific-figure` | publication-style scientific figure |
| `/mechanism-figure` | scientific mechanism diagram |
| `/graphical-abstract` | compact research summary |
| `/visual-abstract` | three-finding visual abstract |
| `/methods-figure` | research-method flow |
| `/experimental-setup` | physical experiment setup |
| `/control-vs-treatment` | matched experiment comparison |
| `/uncertainty-figure` | uncertainty-aware figure |
| `/raw-data-overlay` | raw observations + summary |
| `/scientific-cover` | scientific journal cover |
| `/specimen-plate-modern` | modern specimen plate |
| `/comparative-anatomy` | matched anatomical comparison |
| `/fossil-reconstruction-pair` | evidence + reconstruction |
| `/evidence-layer` | evidence-strength overlay |
| `/architecture-review-board` | live decision review board |
| `/option-board` | matched design alternatives |
| `/material-option-board` | material-only comparison |
| `/daylight-option-board` | same space, different daylight |
| `/season-option-board` | matched seasonal views |
| `/architecture-sequence` | spatial experience sequence |
| `/architecture-storyboard` | use-case storyboard |
| `/architecture-exploded-program` | programmatic exploded axon |
| `/architecture-process-board` | design-development sequence |
| `/architecture-pinup` | physical project pin-up |
| `/architecture-crit-wall` | annotated critique wall |
| `/type-specimen-poster` | type specimen |
| `/kinetic-type-still` | kinetic typographic frame |
| `/variable-font-poster` | variable-font progression |
| `/oversized-type` | large-scale type composition |
| `/type-image-interlock` | image/type overlap |
| `/type-only-poster` | typography-only poster |
| `/hand-lettered-poster` | hand-lettering poster |
| `/stamp-type` | stamped typography |
| `/xerox-type` | photocopied typography |
| `/picturebook-scene` | children's story illustration |
| `/character-turnaround-kids` | children's character model sheet |
| `/same-character-sequence` | consistent character sequence |
| `/wordless-sequence` | wordless visual narrative |
| `/educational-story-scene` | learning through story |
| `/concept-cartoon` | misconception discussion cartoon |
| `/misconception-pair` | wrong vs correct model |
| `/observe-predict-explain` | learning sequence |
| `/visual-routine` | See–Think–Wonder worksheet |
| `/diagram-poster` | diagram adapted into poster |
| `/data-art-safe` | data art with preserved mapping |
| `/physical-data-art` | data encoded as physical material |
| `/small-multiple-data-art` | repeated comparable data art |
| `/ui-screenshot-editorial` | screenshot-based editorial |
| `/ui-before-after` | matched UI redesign comparison |
| `/ui-state-sheet` | component states |
| `/ui-flow-strip` | interface task sequence |
| `/mobile-storyboard` | app in real usage |
| `/ui-window-collage` | restrained UI collage |
| `/screenshot-annotation` | annotated screenshot |
| `/continuity-lock` | multi-frame continuity |
| `/format-matrix` | one source → six formats |
| `/format-matrix-lock` | multi-format identity system |
| `/campaign-system` | cross-format campaign |

---

<a id="aile-016"></a>
# Analog Baskı, Karanlık Oda ve Çoklu Referans Master Promptları — 2026 Ek Taraması

2026'da iki farklı ama birbirini tamamlayan yön güçleniyor:

1. **Analog üretim süreci yeniden görünür hâle geliyor.** Film, karanlık oda, cyanotype, risograph, screen print, emboss/deboss ve fiziksel kâğıt davranışı dijital görsellere karşı “insan eli” ve “maddi süreç” hissi taşıyor.
2. **Çoklu referanslı görsel düzenleme daha sistematikleşiyor.** Bir görsel kimliği, biri kıyafeti, biri ışığı, biri kompozisyonu, biri de ürünü kontrol edecek şekilde referanslara görev atanıyor.

Bu iki yön için de aynı temel prensip geçerli:

> **Süreç ve rol açık değilse model boşluğu kendi klişeleriyle doldurur.**

---

# 1246. `/cyanotype` — Cyanotype / Siyanotip Baskı

## Trend

**T1/T2 — 2026'da alternatif fotoğraf süreçleri içinde güçlü.**

## Türkçe prompt

> [NESNE/BİTKİ/FOTOĞRAF]'ı gerçek cyanotype baskı mantığında oluştur.
>
> Kullan:
>
> - Prussian blue / koyu mavi baskı alanı,
> - temas eden nesnelerde açık beyaz/soluk ton,
> - UV exposure kaynaklı kontrollü ton farkı,
> - gerçek kâğıt lifleri,
> - kenarlarda hafif kimyasal/kaplama düzensizliği.
>
> Cyanotype'ı yalnız “mavi filtre” olarak uygulama.
>
> Eğer doğrudan fotogram mantığı isteniyorsa nesne formu temas gölgesiyle oluşsun.

## English

> Render [OBJECT/PLANT/PHOTO] using the physical logic of a cyanotype print.
>
> Use deep Prussian-blue exposure areas, pale or white contact regions, controlled UV-exposure variation, visible paper fibers, and slight coating irregularity near the edges.
>
> Do not treat cyanotype as a simple blue filter.
>
> If using photogram logic, let object silhouettes emerge through direct contact and exposure.

---

# 1247. `/cyanotype-botanical` — Botanik Siyanotip

## Türkçe

> [BİTKİ]'yi düz kâğıt üzerine yerleştirilmiş gerçek botanik specimen ile yapılan cyanotype photogram gibi göster.
>
> Yaprak damarları, ince saplar ve üst üste binen bitki parçaları temas yoğunluğuna göre farklı açıklıkta görünsün.
>
> Botanik yapıyı rastgele dekoratif çiçeklerle değiştirme.

## English

> Show [PLANT] as a cyanotype photogram made from a real botanical specimen placed directly on coated paper.
>
> Let veins, stems, and overlapping plant parts create different exposure densities according to contact.
>
> Do not replace the actual botanical structure with decorative flowers.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1248. `/cyanotype-textile` — Tekstil Üzerinde Cyanotype

## Trend

**T1/T2 — cyanotype'in tekstile yayılması güçlü.**

## Türkçe prompt

> [DESEN/BİTKİ] cyanotype baskısını doğal pamuk veya keten kumaş üzerinde göster.
>
> Baskı kumaş liflerini takip etsin; kumaş kıvrımlarında boya/pozlama davranışı fiziksel olarak değişsin.
>
> Sonucu dijital mavi pattern gibi düz ve kusursuz yapma.

## English

> Show a cyanotype print of [PATTERN/PLANT] on natural cotton or linen fabric.
>
> Let the print follow the textile fibers and respond physically to folds and surface variation.
>
> Avoid a flat, perfectly uniform digital-blue pattern.

---

# 1249. `/photogram` — Kamerasız Fotogram

## Evergreen

## Türkçe prompt

> [NESNELER]'i ışığa duyarlı fotoğraf kâğıdı üzerine yerleştirilmiş gerçek photogram kompozisyonu olarak göster.
>
> Nesnelerin ışık geçirgenliğine göre:
>
> - opak alanlar açık,
> - yarı saydam alanlar gri,
> - açıkta kalan alanlar koyu
>
> görünsün.
>
> Perspektif gölgesi veya kamera lensi etkisi ekleme.

## English

> Show [OBJECTS] as a real cameraless photogram made on light-sensitive photographic paper.
>
> Let opacity determine tone:
>
> - opaque areas light,
> - translucent areas gray,
> - fully exposed paper dark.
>
> Avoid perspective shadows and camera-lens effects.

## Neye dikkat edilmeli?

Fiziksel davranış (gölge yönü, gren, alan derinliği) tek ışık mantığına uysun; “film hissi” için gren eklemek zayıf kompozisyonu kurtarmaz.

---
# 1250. `/darkroom-contact-print` — Karanlık Oda Contact Print

## Türkçe

> 35mm negatif şeritlerini doğrudan fotoğraf kâğıdı üzerine basılmış analog contact print olarak göster.
>
> Film perforasyonları, frame numaraları, exposure farkları ve gerçek koyu/açık kare çeşitliliği korunsun.
>
> Tüm kareleri aynı kusursuz pozlamada yapma.

## English

> Show 35mm negative strips as an analog darkroom contact print made directly on photographic paper.
>
> Preserve perforations, frame numbers, exposure variation, and real differences between dark and light frames.
>
> Do not make every frame perfectly exposed.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1251. `/darkroom-test-strip` — Exposure Test Strip

## Türkçe

> Aynı fotoğrafın farklı exposure süreleriyle basılmış 5–7 bölümlü karanlık oda test strip'ini göster.
>
> Her bölüm kademeli olarak daha koyu veya açık olsun.
>
> Bu farkı dijital gradient yerine gerçek exposure basamakları gibi göster.

## English

> Show a darkroom test strip of the same photograph exposed in 5–7 stepped time intervals.
>
> Make each section progressively lighter or darker.
>
> Render the change as discrete exposure steps rather than a digital gradient.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1252. `/darkroom-workprint` — Work Print

## Türkçe

> Final fine-art print yerine karanlık odada yapılan çalışma baskısını göster.
>
> Kenarlarda küçük crop notları, exposure işaretleri veya grease-pencil kararları bulunabilir.
>
> Görüntü “tamamlanmış sanat baskısı” kadar temiz olmak zorunda değil.

## English

> Show a darkroom work print rather than a finished fine-art print.
>
> Allow small crop notes, exposure marks, or grease-pencil decisions around the edges.
>
> Keep the image less polished than the final exhibition print.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1253. `/darkroom-dodge-burn-map` — Dodge & Burn Planı

## Türkçe

> Aynı fotoğrafın dodge/burn planını teknik çalışma kağıdı olarak göster.
>
> Açılması gereken alanlar ve koyulaştırılacak bölgeler numaralı kısa notlarla işaretlensin.
>
> Fotoğrafın kendisini bozma; notları çalışma kopyası üzerinde tut.

## English

> Show a technical dodge-and-burn plan for the same photograph on a work print.
>
> Mark areas to lighten or darken with concise numbered notes.
>
> Keep the source photograph intact and place annotations only on the working copy.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1254. `/platinum-print` — Platinum/Palladium Print

## Trend

**T1/T2 — 2026 alternatif baskı süreçlerinde yükseliş sinyali.**

## Türkçe prompt

> [PORTRE/SAHNE]'yi platinum-palladium fine-art print karakterinde göster.
>
> Çok geniş ve yumuşak tonal geçiş, mat yüzey, sıcak/nötr siyahlar ve derin gölge ayrıntısı kullan.
>
> Parlak resin-coated photo paper veya sert dijital kontrast kullanma.

## English

> Render [PORTRAIT/SCENE] with the character of a platinum-palladium fine-art print.
>
> Use a broad subtle tonal range, matte surface, warm-neutral blacks, and rich shadow detail.
>
> Avoid glossy resin-coated photo paper and harsh digital contrast.

---

# 1255. `/risograph-two-ink` — İki Renkli Risograph

## Trend

**T1 — 2026 print tasarımında güçlü.**

## Türkçe prompt

> [GÖRSEL]'i iki spot renkli gerçek risograph baskı mantığında oluştur.
>
> Plaka 1:
>
> - büyük renk alanları.
>
> Plaka 2:
>
> - kontur, gölge veya ikinci bilgi katmanı.
>
> İki plakanın çakıştığı yerde üçüncü karışım rengi doğal olarak oluşsun.
>
> Misregistration yalnız 1–2 mm civarında ve sınırlı bölgelerde olsun.
>
> Halftone'u bütün yüzeye gürültü olarak yayma.

## English

> Render [IMAGE] using the physical logic of a two-ink Risograph print.
>
> Plate 1 should handle large color fields.
>
> Plate 2 should handle outlines, shadows, or the second information layer.
>
> Let overlaps naturally create a third mixed color.
>
> Restrict misregistration to roughly 1–2 mm and only selected areas.
>
> Do not cover the whole image with noisy halftones.

---

# 1256. `/riso-photo` — Fotoğrafı Risograph'a Çevirme

## Türkçe

> [FOTOĞRAF]'ı iki veya üç riso ink channel'a ayır.
>
> Ana tonal bilgiyi halftone/dither ile oluştur.
>
> Yüz ve temel siluet okunabilir kalsın.
>
> Smooth digital gradient kullanma.

## English

> Separate [PHOTO] into two or three Risograph ink channels.
>
> Build tonal information through halftone or dithering.
>
> Keep faces and primary silhouettes readable.
>
> Avoid smooth digital gradients.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1257. `/screenprint-two-color` — İki Renk Serigrafi

*Rehber kısayolu: `/screenprint`.*

## Türkçe

> [POSTER/GÖRSEL]'i gerçek iki renk screen-print mantığında oluştur.
>
> Her renk ayrı fiziksel stencil/plate gibi davranmalı.
>
> Büyük düz alanlar, sınırlı halftone ve gerçek overprint kullan.
>
> İki rengi dijital multiply blend gibi kusursuz karıştırma.

## English

> Render [POSTER/IMAGE] using the physical logic of two-color screen printing.
>
> Treat each color as a separate stencil or plate.
>
> Use large flat areas, restrained halftone, and believable overprint.
>
> Avoid perfectly smooth digital multiply blending.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1258. `/halftone-photo` — Halftone Fotoğraf

## Türkçe

> [FOTOĞRAF]'ı kontrollü AM-style halftone dots ile yeniden üret.
>
> Nokta boyutu ton yoğunluğunu taşısın.
>
> Yüz ve önemli detaylarda dot size okunabilirliği koruyacak kadar ince olsun.
>
> Rastgele noise kullanma.

## English

> Rebuild [PHOTO] using controlled AM-style halftone dots.
>
> Let dot size encode tonal density.
>
> Keep dot size fine enough around faces and important details to preserve readability.
>
> Avoid random noise.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1259. `/newsprint-halftone` — Gazete Baskı Noktalaması

## Türkçe

> [FOTOĞRAF]'ı düşük maliyetli gazete baskısına uygun coarse halftone karakterinde göster.
>
> Kâğıt hafif emici ve sıcak gri/off-white olabilir.
>
> Mürekkep kenarlarında küçük dot gain görülebilir.
>
> Görüntüyü comic-book Ben-Day dots ile karıştırma.

## English

> Render [PHOTO] with coarse halftone character appropriate to low-cost newspaper printing.
>
> Use slightly absorbent warm-gray or off-white paper and subtle dot gain at ink edges.
>
> Do not confuse the look with comic-book Ben-Day dots.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1260. `/letterpress` — Letterpress Baskı

## Trend

**T1/T2 — tactile print dönüşünde güçlü.**

## Türkçe prompt

> [KISA METİN/LOGO]'yu kalın pamuklu sanat kâğıdına gerçek letterpress baskı gibi göster.
>
> Harf kenarlarında çok hafif fiziksel impression/deboss olsun.
>
> Mürekkep yüzeyi mat ve sınırlı olsun.
>
> Derin 3B emboss veya metalik folyo ekleme.

## English

> Render [SHORT TEXT/LOGO] as real letterpress on thick cotton art paper.
>
> Show only a subtle physical impression around letterforms.
>
> Keep ink matte and restrained.
>
> Avoid deep 3D embossing and metallic foil.

---

# 1261. `/blind-emboss` — Mürekkepsiz Gofre

## Türkçe

> [LOGO/HARİTA/DESEN]'i kalın kâğıt üzerinde yalnız blind emboss/deboss ile göster.
>
> Görsel kontrastı ışık-gölge ve kağıt deformasyonundan gelsin.
>
> Mürekkep, gradient veya sahte metalik efekt kullanma.

## English

> Show [LOGO/MAP/PATTERN] on thick paper using only blind embossing or debossing.
>
> Let visual contrast come from light, shadow, and paper deformation.
>
> Avoid ink, gradients, and fake metallic effects.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1262. `/raised-varnish` — Kabartma Vernik

## Trend

**T1/T2 — tactile print 2026.**

## Türkçe

> [BASKI]'da yalnız tek ana detay üzerine raised spot varnish uygula.
>
> Geri kalan yüzey mat kalsın.
>
> Vernik ışıkta hafif yükselti ve parlaklık farkı oluştursun.
>
> Her yazı ve görsele kabartma vernik uygulama.

## English

> Apply raised spot varnish to only one primary detail in [PRINT].
>
> Keep the rest of the surface matte.
>
> Let the varnish create a subtle physical height and gloss difference.
>
> Do not apply raised varnish to every element.

---

# 1263. `/matte-gloss-contrast` — Mat / Parlak Yüzey Karşıtlığı

## Türkçe

> [AMBALAJ/POSTER]'ın çoğunu mat yüzeyde tut ve yalnız tek seçili formu gloss varnish ile görünür kıl.
>
> Fark yalnız uygun ışık açısında okunmalı.
>
> “Premium” görünüm için tüm yüzeyi parlaklaştırma.

## English

> Keep most of [PACKAGE/POSTER] matte and reveal only one selected form using gloss varnish.
>
> Let the difference become visible primarily at appropriate viewing angles.
>
> Do not make the entire surface glossy to signal “premium.”

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1264. `/print-process-board` — Baskı Süreci Board'u

## Türkçe

> Aynı final baskının üretim sürecini 5 küçük aşamada göster:
>
> 1. artwork,
> 2. plate/channel separation,
> 3. first ink,
> 4. second ink/overprint,
> 5. final print.
>
> Her aşamada gerçek üretim değişikliği görülsün.

## English

> Show the making of one final print in five stages:
>
> 1. artwork,
> 2. plate or channel separation,
> 3. first ink,
> 4. second ink or overprint,
> 5. final print.
>
> Make the physical production change visible at every stage.

## Neye dikkat edilmeli?

Baskı fiziği tutarlı olsun: kâğıt dokusu, mürekkep davranışı ve kenar boşlukları tek sürece uysun.

---
# 1265. `/anti-ai-print` — Kontrollü Analog İnsan İzi

## Trend

**T1/T2 — drupa 2026 “anti-AI craft” yönüyle uyumlu.**

## Türkçe

> [TASARIM]'a insan üretimi hissi vermek için yalnız gerçek baskı sürecinden çıkabilecek 2–3 iz kullan:
>
> - halftone,
> - hafif registration farkı,
> - kâğıt lifi,
> - el kesimi kenar,
> - overprint,
> - stamp variation.
>
> Rastgele grain, coffee stain, torn paper ve scratches ekleme.

## English

> Give [DESIGN] a human-made print character using only 2–3 traces that could genuinely emerge from the production process:
>
> halftone, slight registration drift, paper fibers, hand-cut edges, overprint, or stamp variation.
>
> Avoid random grain, coffee stains, torn paper, and scratches.

---

# 1266. Baskıda `process first` kuralı

Şu prompt:

> `make it look analog`

çok belirsizdir.

Daha iyi:

> `two-ink risograph, plate A for flat color, plate B for outline and shadows, slight 1 mm misregistration only at lower edge, uncoated paper`

Çünkü analog estetik:

> **efekt değil, üretim sürecinin görsel sonucu**dur.

---

# 1267. `/cover-art-not-figure` — Bilimsel Kapak ile Bilimsel Figür Ayrımı

Nature'ın güncel cover guide'ında kritik bir ayrım vardır:

> **Cover art tüm araştırmayı anlatmak zorunda değildir.**
>
> Figür ise veri ve mekanizmayı doğru ve değerlendirilebilir biçimde anlatmalıdır.

## Rehber kuralı

### Scientific figure

> açıklayıcı + değerlendirilebilir + ölçülebilir.

### Scientific cover

> merak uyandırıcı + doğru bağlama sahip + tek güçlü fikir.

Bu iki prompt ailesi birbirine karıştırılmamalıdır.

---

# 1268. `/science-cover-metaphor` — Bilimsel Kapak Metaforu

## Türkçe

> [ARAŞTIRMA KONUSU]'nu tek bilimsel metaforla kapağa dönüştür.
>
> Metafor araştırma sonucunu yanlış yönlendirmesin.
>
> Bilimsel yapının temel biçimi/ilişkisi doğru kalmalı.
>
> Kapağın tamamını mini graphical abstract'a dönüştürme.

## English

> Turn [RESEARCH TOPIC] into cover artwork built around one scientific metaphor.
>
> Make sure the metaphor does not misrepresent the research.
>
> Preserve the primary scientific structure or relationship.
>
> Do not turn the cover into a miniature graphical abstract.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1269. `/science-cover-photo` — Bilimsel Fotoğraf Kapak

## Türkçe

> [NESNE/TÜR/MEKÂN]'ı bilimsel dergi kapağında tek güçlü gerçek fotoğraf olarak kullan.
>
> Fotoğraf spesifik nesneyi veya olayı doğrudan temsil etsin.
>
> Masthead için üst bölgede doğal boşluk bırak.
>
> Fotoğrafı yalnız daha “bilimsel” görünmesi için neon/3B efektle bozma.

## English

> Use one strong real photograph of [OBJECT/SPECIES/PLACE] as scientific-journal cover artwork.
>
> Let the photograph directly represent the specific entity or event.
>
> Leave natural space for a masthead.
>
> Do not distort the image with neon or 3D effects merely to make it look more scientific.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1270. `/science-cover-process` — Eskizden Bilimsel Kapağa

## Trend

**2026 Nature özel sayısının kapağı doğrudan pencil → ink → full color sürecini görünür kıldı.**

## Türkçe

> Aynı bilimsel illüstrasyonu üç aşamada göster:
>
> 1. pencil observation sketch,
> 2. ink/structure refinement,
> 3. final color cover artwork.
>
> Her aşama gerçek karar ve bilgi eklesin.
>
> Finalin sadece soluk kopyalarını “sketch” diye gösterme.

## English

> Show the same scientific illustration in three stages:
>
> 1. pencil observation sketch,
> 2. ink or structural refinement,
> 3. final color cover artwork.
>
> Let each stage add genuine observation or design decisions.
>
> Do not present faded copies of the final as fake sketches.

---

# 1271. `/multi-ref-2` — İki Referanslı Basit Kompozisyon

## Trend

**T1 — 2026 çoklu referans iş akışlarının temel biçimi.**

## Türkçe prompt

> Reference A = kimlik/ana nesne.
>
> Reference B = stil veya ortam.
>
> Final görselde:
>
> - A'nın kişi/ürün geometrisini koru,
> - B'den yalnız belirtilen stil/ışık/ortamı al.
>
> B'deki kişinin yüzünü veya nesnesini A'ya taşıma.

## English

> Reference A = identity or primary object.
>
> Reference B = style or environment.
>
> Preserve the person or product geometry from A and borrow only the specified style, lighting, or environment from B.
>
> Do not transfer the subject from B into A.

---

# 1272. `/multi-ref-3` — Kimlik + Kıyafet + Mekân

## Türkçe

> Reference A = kişinin yüz/kimliği.
>
> Reference B = yalnız kıyafet.
>
> Reference C = yalnız mekân.
>
> A'dan yüz ve beden kimliğini koru.
>
> B'deki modeli değil yalnız giysi türü, renk, kesim ve materyali aktar.
>
> C'deki insanları kopyalama; yalnız arka plan, ışık ve perspektif bağlamını kullan.

## English

> Reference A = facial identity.
>
> Reference B = clothing only.
>
> Reference C = environment only.
>
> Preserve identity from A.
>
> Transfer only garment type, color, cut, and material from B, not the person wearing it.
>
> Use only background, lighting, and perspective context from C without copying its people.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1273. `/multi-ref-4-product` — Ürün + Model + Mekân + Işık

## Türkçe

> Reference A = ürün geometrisi ve etiket.
>
> Reference B = model/kişi kimliği.
>
> Reference C = mekân.
>
> Reference D = ışık/kompozisyon.
>
> Öncelik sırası:
>
> A ürün doğruluğu,
> B insan kimliği,
> C çevre,
> D görsel treatment.
>
> Çakışma olursa üstteki önceliği koru.

## English

> Reference A = product geometry and label.
>
> Reference B = model identity.
>
> Reference C = environment.
>
> Reference D = lighting and composition.
>
> Priority order:
>
> A product fidelity,
> B human identity,
> C environment,
> D visual treatment.
>
> If references conflict, preserve the higher-priority role.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1274. `/multi-ref-5` — Kimlik + Poz + Kıyafet + Nesne + Mekân

## Türkçe

> Beş referansın görevlerini kesin ayır:
>
> A = kimlik
>
> B = yalnız poz
>
> C = yalnız kıyafet
>
> D = yalnız hero object
>
> E = yalnız çevre.
>
> Hiçbir referans kendi rolü dışındaki kişi, yüz, renk veya nesneyi final görsele taşımamalı.

## English

> Assign five references strict roles:
>
> A = identity,
> B = pose only,
> C = wardrobe only,
> D = hero object only,
> E = environment only.
>
> Do not allow any reference to contribute subjects, faces, colors, or objects outside its assigned role.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1275. `/reference-priority` — Referans Öncelik Sırası

## Türkçe

> Referanslar çakışırsa şu sırayı kullan:
>
> 1. kimlik / ürün geometrisi,
> 2. kıyafet/nesne doğruluğu,
> 3. poz,
> 4. kompozisyon,
> 5. ışık,
> 6. genel stil.
>
> Alt öncelikli estetik karar üst öncelikli fiziksel özelliği bozmamalı.

## English

> If references conflict, use this priority:
>
> 1. identity or product geometry,
> 2. wardrobe/object accuracy,
> 3. pose,
> 4. composition,
> 5. lighting,
> 6. overall style.
>
> Lower-priority aesthetic decisions must not override higher-priority physical fidelity.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1276. `/ignore-subject-from-style-ref` — Stil Referansındaki Kişiyi Yok Say

## Türkçe

> Style reference'taki kişi, yüz, kıyafet ve nesneleri final görsele aktarma.
>
> Yalnız:
>
> - renk davranışı,
> - ışık,
> - baskı/malzeme,
> - crop,
> - negatif alan
>
> gibi görsel treatment özelliklerini kullan.

## English

> Do not transfer the person, face, clothing, or objects from the style reference.
>
> Borrow only visual-treatment properties such as color behavior, lighting, print or material character, crop, and negative space.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1277. `/ignore-style-from-identity-ref` — Kimlik Referansındaki Stili Yok Say

## Türkçe

> Identity reference yalnız kişinin yüz, saç, yaş ve ayırt edici özelliklerini tanımlasın.
>
> Kaynak fotoğraftaki arka plan, kıyafet, ışık, kamera veya color grade final estetiği kontrol etmesin.

## English

> Use the identity reference only for face, hair, age, and distinctive features.
>
> Do not let its background, clothing, lighting, camera, or color grade control the final visual style.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1278. `/reference-conflict-check` — Referans Çatışması Kontrolü

## Türkçe

> Üretimden önce referans rollerini zihinsel olarak ayır:
>
> - aynı özelliği iki farklı referans kontrol ediyor mu?
> - iki farklı kıyafet referansı çakışıyor mu?
> - poz referansında yüz görünümü kimlik referansını etkiliyor mu?
> - style reference çok baskın mı?
>
> Çakışmada öncelik sırasını uygula.

## English

> Before generation, separate reference roles conceptually:
>
> - are two references controlling the same property?
> - do wardrobe references conflict?
> - is the face in the pose reference influencing identity?
> - is the style reference overpowering subject fidelity?
>
> Resolve conflicts using the declared priority order.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1279. `/reference-audit-board` — Çoklu Referans Audit Board

## Yeni master format

## Türkçe

> Final görselin yanında küçük audit board oluştur:
>
> A — identity  
> B — wardrobe  
> C — environment  
> D — lighting
>
> ve her referanstan final görsele taşınan yalnız 2–3 özelliği kısa notla göster.
>
> Audit board'u ana görselin içine gömme; ayrı inceleme sayfası olarak düşün.

## English

> Create a small audit board beside the final image showing:
>
> A — identity  
> B — wardrobe  
> C — environment  
> D — lighting
>
> List only 2–3 properties transferred from each reference.
>
> Treat the audit board as a separate review page rather than embedding it into the artwork.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1280. `/multi-ref-group` — Ayrı Fotoğraflardan Grup Fotoğrafı

## Trend

**T1/T2 — multi-reference modellerin güçlü kullanım alanı.**

## Türkçe

> Ayrı referans fotoğraflardaki [N] kişiyi tek gerçekçi grup fotoğrafında birleştir.
>
> Her kişi kendi referansındaki yüz kimliğini korusun.
>
> İnsanların:
>
> - boy farkı,
> - beden oranı,
> - ışık,
> - perspektif,
> - ayak/zemin teması
>
> aynı mekânın fiziğine uyumlu olsun.
>
> Yüzleri birbirine karıştırma.

## English

> Combine [N] people from separate reference photos into one believable group photograph.
>
> Preserve each person's individual facial identity from their own reference.
>
> Make height relationships, body proportions, lighting, perspective, and ground contact consistent with one shared environment.
>
> Do not blend faces between subjects.

---

# 1281. `/multi-ref-couple` — İki Kimliği Koruyan Çift Fotoğrafı

## Türkçe

> Reference A = kişi 1.
>
> Reference B = kişi 2.
>
> İki kişiyi aynı sahneye yerleştirirken her yüzün kendi referansına ait kalmasını sağla.
>
> Yüz özelliklerini birbirine karıştırma.
>
> Poz/temas fiziksel ve doğal olsun.
>
> Güzelleştirme veya ortak bir “AI face” üretme.

## English

> Reference A = person 1.
>
> Reference B = person 2.
>
> Place both people into one scene while preserving each face from its own reference.
>
> Do not blend facial features.
>
> Keep pose and contact physically natural.
>
> Avoid beautification and generic shared “AI face” characteristics.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1282. `/multi-ref-pet-family` — Çoklu Evcil Hayvan Kompozisyonu

## Türkçe

> Her evcil hayvanın referansını ayrı kimlik kaynağı olarak kullan.
>
> Tüy rengi, desen, göz, kulak ve beden oranları hayvanlar arasında karışmasın.
>
> Aynı sahneye yerleştirirken gerçek boyut farklarını koru.

## English

> Use each pet reference as a separate identity source.
>
> Do not mix fur color, markings, eyes, ears, or body proportions between animals.
>
> Preserve believable relative size when placing them in one scene.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1283. `/multi-ref-product-campaign` — Ürünü Çoklu Referansla Kampanyaya Taşıma

## Türkçe

> A = gerçek ürün.
>
> B = kampanya renk/ışık referansı.
>
> C = surface/environment.
>
> D = model/hand pose reference.
>
> Ürün A'dan bire bir korunmalı.
>
> B–D yalnız kendi rollerini kontrol etsin.
>
> Aynı kampanya içinde 4–6 görüntü üretirken ürün ve label değişmemeli.

## English

> A = real product.
>
> B = campaign color and lighting reference.
>
> C = surface or environment.
>
> D = model or hand-pose reference.
>
> Preserve product A exactly.
>
> Let B–D control only their assigned roles.
>
> Keep product and label unchanged across a 4–6 image campaign.

## Neye dikkat edilmeli?

Hangi görselin kimlik, hangisinin stil referansı olduğu promptta adıyla yazılsın; karışan kimlik en sık hatadır ([§2623](40-model-arac-duzenleme-2622-2673.md#sec-2623)).

---
# 1284. `/reference-role-table` — Çoklu Referans İçin Hızlı Tablo

| Referans | Kontrol ettiği şey | Kontrol etmemesi gereken |
|---|---|---|
| Identity | yüz, saç, yaş, ayırt edici özellik | arka plan, style |
| Body | beden oranı, duruş | yüz kimliği |
| Pose | poz, el/kol yönü | yüz, kıyafet |
| Wardrobe | giysi türü, renk, kesim | model yüzü |
| Product | geometri, etiket, malzeme | ışık/stil |
| Environment | mekân, perspektif bağlamı | kişiler |
| Lighting | ışık yönü/kontrast | nesne geometrisi |
| Style | renk, baskı, materyal dili | kişi/ürün kimliği |
| Composition | crop, negatif alan, yerleşim | kimlik |

---

# 1285. Çoklu referans prompt formülü

## Türkçe

> **ROLE → PRESERVE → BORROW → IGNORE → PRIORITY → OUTPUT**

### Örnek

> Reference A — identity. Preserve face and hair. Ignore background and lighting.  
> Reference B — outfit. Borrow clothing only. Ignore model identity.  
> Reference C — composition. Borrow crop and negative space only.  
> Priority: A > B > C.  
> Output: 4:5 editorial portrait.

## English

> **ROLE → PRESERVE → BORROW → IGNORE → PRIORITY → OUTPUT**

Bu yapı, “üç fotoğraf yükledim, bunları birleştir” demekten çok daha güvenilirdir.

---

# 1286. `/exam-diagram` — Sınav Diyagramı

## Eğitim

## Türkçe

> [KONU] için sınav sorusunda kullanılabilecek sade siyah-beyaz diyagram oluştur.
>
> Gereksiz dekor, renk, arka plan ve gölge kullanma.
>
> Etiketlenecek alanları A–D veya 1–4 gibi boş işaretlerle göster.
>
> Doğru cevabı görsel vurgu ile ele verme.

## English

> Create a clean black-and-white diagram for an exam question about [TOPIC].
>
> Avoid decorative color, backgrounds, and shadows.
>
> Mark unlabeled target areas as A–D or 1–4.
>
> Do not reveal the correct answer through visual emphasis.

## Neye dikkat edilmeli?

Öğrenci sürümüyle öğretmen anahtarı birebir eşleşsin; doldurulabilir alanlar yazdırılan boyutta gerçekten yazılabilir olsun.

---
# 1287. `/exam-figure-key` — Öğretmen Cevap Anahtarı

## Türkçe

> `/exam-diagram` ile aynı görseli kullan ancak öğretmen answer-key sürümünde doğru etiketleri açıkça göster.
>
> Geometri, kadraj ve numaralandırma öğrenci sürümüyle bire bir aynı kalsın.

## English

> Use the exact same visual as `/exam-diagram`, but create a teacher answer-key version with correct labels revealed.
>
> Keep geometry, framing, and numbering identical to the student version.

## Neye dikkat edilmeli?

Öğrenci sürümüyle öğretmen anahtarı birebir eşleşsin; doldurulabilir alanlar yazdırılan boyutta gerçekten yazılabilir olsun.

---
<a id="sec-1288"></a>
# 1288. `/worksheet-student` — Öğrenci Worksheet Sürümü

## Türkçe

> [KONU] için öğrenci çalışma sayfası oluştur.
>
> İçerik:
>
> - bir ana görsel,
> - 3–5 soru,
> - yeterli yazma/işaretleme alanı.
>
> Cevapları görselde gizli ipuçlarıyla verme.
>
> Baskıya uygun sade arka plan kullan.

## English

> Create a student worksheet for [TOPIC] containing one main visual, 3–5 questions, and enough writing or marking space.
>
> Do not reveal answers through hidden visual cues.
>
> Use a print-friendly restrained background.

## Neye dikkat edilmeli?

Öğrenci sürümüyle öğretmen anahtarı birebir eşleşsin; doldurulabilir alanlar yazdırılan boyutta gerçekten yazılabilir olsun.

---
# 1289. `/worksheet-key` — Öğretmen Anahtarı

## Türkçe

> `/worksheet-student` ile aynı sayfa yapısını koru.
>
> Yalnız cevapları ve kısa değerlendirme notlarını ekle.
>
> Öğrenci ve öğretmen sürümünün sayfa numarası/soru sırası aynı olsun.

## English

> Preserve the same page structure as `/worksheet-student`.
>
> Add only answers and concise evaluation notes.
>
> Keep page numbering and question order identical between student and teacher versions.

## Neye dikkat edilmeli?

Öğrenci sürümüyle öğretmen anahtarı birebir eşleşsin; doldurulabilir alanlar yazdırılan boyutta gerçekten yazılabilir olsun.

---
# 1290. `/fillable-diagram` — Doldurulabilir Diyagram

## Türkçe

> [KONU]'nun ana diyagramını oluştur ancak temel terimleri boş kutu/çizgi olarak bırak.
>
> Öğrencinin yazabileceği gerçek fiziksel boşluk bırak.
>
> Kutuları minik yapma.

## English

> Create the main diagram for [TOPIC] while leaving key terms as blank boxes or lines.
>
> Provide enough physical writing space for students.
>
> Do not make blanks too small.

## Neye dikkat edilmeli?

Öğrenci sürümüyle öğretmen anahtarı birebir eşleşsin; doldurulabilir alanlar yazdırılan boyutta gerçekten yazılabilir olsun.

---
# 1291. `/ink-saving-worksheet` — Mürekkep Tasarruflu Baskı

## Türkçe

> [WORKSHEET]'i siyah-beyaz yazıcıda ekonomik basılacak şekilde düzenle.
>
> Geniş koyu dolguları kaldır.
>
> İnce ama okunabilir çizgiler, beyaz arka plan ve taramasız alanlar kullan.
>
> Bilgi hiyerarşisini renge bağımlı yapma.

## English

> Adapt [WORKSHEET] for economical black-and-white printing.
>
> Remove large dark fills.
>
> Use thin but readable lines, white background, and unfilled areas.
>
> Do not make information hierarchy dependent on color.

## Neye dikkat edilmeli?

Öğrenci sürümüyle öğretmen anahtarı birebir eşleşsin; doldurulabilir alanlar yazdırılan boyutta gerçekten yazılabilir olsun.

---
# 1292. `/teacher-overlay` — Öğretmen Açıklama Katmanı

## Türkçe

> Aynı öğrenci görselinin üzerinde ayrı öğretmen overlay sürümü oluştur.
>
> Yalnız:
>
> - doğru cevap,
> - kritik açıklama,
> - yaygın hata,
> - öğretmen notu
>
> için farklı ama sınırlı annotation kullan.
>
> Öğrenci görselini yeniden tasarlama.

## English

> Create a teacher-overlay version on top of the same student visual.
>
> Add only the correct answer, critical explanation, common error, and teacher note using restrained annotations.
>
> Do not redesign the underlying student visual.

## Neye dikkat edilmeli?

Öğrenci sürümüyle öğretmen anahtarı birebir eşleşsin; doldurulabilir alanlar yazdırılan boyutta gerçekten yazılabilir olsun.

---
# 1293. `/assessment-pair` — Öğrenci + Öğretmen Eşleşmiş Set

## Türkçe

> Aynı içerikten iki çıktı üret:
>
> A — student version  
> B — teacher key
>
> İki sürümde:
>
> - sayfa düzeni,
> - görsel,
> - soru numarası,
> - boşluklar
>
> aynı kalsın.
>
> B yalnız cevap/annotation katmanını eklesin.

## English

> Create two matched outputs from the same material:
>
> A — student version  
> B — teacher key
>
> Keep layout, visual, question numbering, and blanks identical.
>
> Let B add only the answer or annotation layer.

## Neye dikkat edilmeli?

Öğrenci sürümüyle öğretmen anahtarı birebir eşleşsin; doldurulabilir alanlar yazdırılan boyutta gerçekten yazılabilir olsun.

---
# 1294. `/print-slop-filter` — Analog Baskı AI Slop Filtresi

Kaçınılması gerekenler:

- analog = random grain,
- vintage = sepia,
- riso = her yerde noise,
- screen print = photoshop multiply,
- cyanotype = mavi filtre,
- letterpress = aşırı derin 3B emboss,
- tactile = her yüzeyde foil/varnish,
- misregistration = tüm görüntüyü kaydırmak,
- handmade = yırtık kenar + coffee stain.

---

# 1295. `/multi-ref-slop-filter` — Çoklu Referans AI Slop Filtresi

Kaçınılması gerekenler:

- style reference'taki yüzün kimliğe karışması,
- wardrobe reference modelinin vücut yapısının taşınması,
- product label'ın yeniden yazılması,
- pose reference'taki arka planın sızması,
- her referanstan “biraz” alıp yeni hibrit kimlik oluşturmak,
- çakışan referanslarda öncelik tanımlamamak,
- role assignment yazmadan “combine these” demek.

---

# 1296. `/assessment-slop-filter` — Eğitim/Sınav Görseli AI Slop Filtresi

Kaçınılması gerekenler:

- sınav görselinde doğru cevabı renk ile ele vermek,
- answer key'de geometriyi değiştirmek,
- öğrenci sürümünde dekoratif dikkat dağıtıcılar,
- yazma alanını küçültmek,
- siyah-beyaz baskıda kaybolan renk kodu,
- yanlış terim/etiket,
- öğretmen ve öğrenci sürümünün farklı soru sırasına sahip olması.

---

# 1297. Yeni üst aile: `Process-authentic Visual`

Analog baskı, craft ve bilimsel illüstrasyondan çıkan ortak prensip:

> **Bir görsel “X style” demek yerine X sürecinin fiziksel adımlarından türetilirse daha inandırıcı olur.**

Aile:

- `/risograph-two-ink`
- `/screenprint-two-color`
- `/cyanotype`
- `/letterpress`
- `/blind-emboss`
- `/scientific-cover-process`
- `/embroidery`
- `/whittled`
- `/paper-world`

Prompt formülü:

> **production process + material + constraint + artifact + output**

---

# 1298. Yeni üst aile: `Reference Orchestration`

Çoklu referans kullanımının üst kavramı:

> **Reference Orchestration — her referansın neyi kontrol edeceğini ve neyi kontrol etmeyeceğini açıkça yönetmek**

Aile:

- `/multi-ref-2`
- `/multi-ref-3`
- `/multi-ref-4-product`
- `/multi-ref-5`
- `/reference-priority`
- `/ignore-subject-from-style-ref`
- `/ignore-style-from-identity-ref`
- `/reference-conflict-check`
- `/reference-audit-board`

Bu ailede ana soru:

> **“Hangi görsel hangi kararı veriyor?”**

---

# 1299. Yeni üst aile: `Student / Teacher Dual`

Aynı eğitsel varlığın iki kontrollü sürümü:

> **öğrenci görür → öğretmen doğrular**

Aile:

- `/exam-diagram`
- `/exam-figure-key`
- `/worksheet-student`
- `/worksheet-key`
- `/teacher-overlay`
- `/assessment-pair`

Ana kural:

> **Görsel değişmez; bilgi katmanı değişir.**

---

# 1300. Bu turdaki slash-style indeks (aile-016)

| Kısayol | Aile |
|---|---|
| `/cyanotype` | cyanotype print |
| `/cyanotype-botanical` | botanical cyanotype |
| `/cyanotype-textile` | textile cyanotype |
| `/photogram` | cameraless photogram |
| `/darkroom-contact-print` | analog contact sheet |
| `/darkroom-test-strip` | exposure test strip |
| `/darkroom-workprint` | working darkroom print |
| `/darkroom-dodge-burn-map` | print adjustment plan |
| `/platinum-print` | platinum-palladium print character |
| `/risograph-two-ink` | two-ink Risograph |
| `/riso-photo` | photograph separated into riso plates |
| `/screenprint-two-color` | two-color screen print |
| `/halftone-photo` | AM halftone photograph |
| `/newsprint-halftone` | newspaper halftone |
| `/letterpress` | letterpress print |
| `/blind-emboss` | inkless emboss/deboss |
| `/raised-varnish` | spot raised varnish |
| `/matte-gloss-contrast` | matte/gloss tactile contrast |
| `/print-process-board` | physical print-process sequence |
| `/anti-ai-print` | controlled analogue human signals |
| `/cover-art-not-figure` | scientific cover vs figure distinction |
| `/science-cover-metaphor` | evidence-grounded cover metaphor |
| `/science-cover-photo` | photographic science cover |
| `/science-cover-process` | sketch-to-cover scientific artwork |
| `/multi-ref-2` | identity/object + style/environment |
| `/multi-ref-3` | identity + wardrobe + environment |
| `/multi-ref-4-product` | product + model + environment + lighting |
| `/multi-ref-5` | identity + pose + wardrobe + object + environment |
| `/reference-priority` | reference conflict hierarchy |
| `/ignore-subject-from-style-ref` | style-only extraction |
| `/ignore-style-from-identity-ref` | identity-only extraction |
| `/reference-conflict-check` | role-conflict audit |
| `/reference-audit-board` | reference-role review page |
| `/multi-ref-group` | combine separately photographed people |
| `/multi-ref-couple` | preserve two individual identities |
| `/multi-ref-pet-family` | combine multiple pets |
| `/multi-ref-product-campaign` | multi-reference product campaign |
| `/reference-role-table` | reference role cheat sheet |
| `/exam-diagram` | student exam figure |
| `/exam-figure-key` | teacher answer figure |
| `/worksheet-student` | student worksheet |
| `/worksheet-key` | teacher worksheet key |
| `/fillable-diagram` | unlabeled fill-in figure |
| `/ink-saving-worksheet` | economical printable version |
| `/teacher-overlay` | answer/annotation overlay |
| `/assessment-pair` | matched student/teacher set |

---
