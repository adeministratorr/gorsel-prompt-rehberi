> [← Genel İçindekiler](gorsel-prompt-rehberi.md) · [Süleyman’a Umut Ol — Dayanışma Çağrısı](gorsel-prompt-rehberi.md#suleymana-umut-ol)

<a id="aile-017"></a>
# Kamera, Lens, Işık ve “Capture Source” Prompt Dili — Teknik Terimleri Gerçek Anlamıyla Kullanmak

GitHub’daki güncel görsel prompt rehberleri ve prompt-builder projeleri, 2026’da fotoğraf tabanlı promptların giderek daha modüler yazıldığını gösteriyor:

> **subject + environment + composition + lighting + camera/lens behavior + restrictions**

Bu bölümde amaç, marka/model adlarını büyülü kelimeler gibi kullanmak değil; **görüntünün hangi optik ve çekim davranışıyla oluşacağını** tarif etmektir.

Önemli not:

> `85mm`, `f/2`, `Rembrandt light`, `35mm documentary`, `top-down`, `direct flash`

gibi terimler teknik fotoğraf dilinde anlamlıdır.

Ama:

> `Hasselblad X2D`, `Leica M11`, `RAW`, `8K`, `32K`

gibi ifadeler görüntü üretim modelinde gerçek kamera ayarı veya kalite garantisi değildir.

Model bu adlardan çoğunlukla bir **görsel beklenti/stil ipucu** çıkarır.

Bu nedenle:

> **kamera markası yerine optik sonucu tarif etmek genellikle daha güvenlidir.**

---

# 1301. `/24mm-wide` — 24 mm Geniş Açı

## Ne yapar?

Mekânı ve çevreyi özneyle birlikte gösterir. Kenarlarda perspektif büyümesi artar.

## Türkçe prompt

> [ÖZNE]'yi yaklaşık 24 mm geniş açı hissiyle çevresiyle birlikte göster. Kamera özneye çok yaklaşmasın. Mekânın ön–orta–arka plan derinliği belirgin olsun. Kadraj kenarlarındaki objelerde hafif perspektif büyümesi doğal kalsın.
>
> Yüzü geniş açı deformasyonuyla bozacak kadar yaklaşma.

## English

> Show [SUBJECT] with the spatial behavior of an approximately 24 mm wide-angle lens. Keep enough camera distance to preserve the subject while revealing strong foreground, middle-ground, and background depth. Allow mild edge perspective enlargement.
>
> Avoid extreme close distance that distorts the face.

## Neye dikkat edilmeli?

Fiziksel davranış (gölge yönü, gren, alan derinliği) tek ışık mantığına uysun; “film hissi” için gren eklemek zayıf kompozisyonu kurtarmaz.

---
# 1302. `/35mm-documentary` — 35 mm Belgesel Perspektifi

## Kullanım

Sokak, gündelik yaşam, çevresel portre, kafe, atölye, öğretmen/öğrenci sahnesi.

## Türkçe

> [ÖZNE]'yi yaklaşık 35 mm belgesel perspektifiyle göster. Kişi ve bulunduğu ortam birlikte okunabilsin. Perspektif doğal, mesafe günlük insan gözü deneyimine yakın olsun. Arka plan tamamen erimesin.

## English

> Show [SUBJECT] with an approximately 35 mm documentary perspective. Keep both the subject and meaningful environmental context readable. Preserve natural perspective and avoid dissolving the entire background.

## Neye dikkat edilmeli?

Odak davranışı fiziksel olsun: makro karede alan derinliği sığlaşır, telefotoda planlar sıkışır; model her şeyi net vermeye eğilimlidir.

---
# 1303. `/50mm-natural` — 50 mm Doğal Perspektif

## Türkçe

> [ÖZNE]'yi 50 mm civarında doğal ve dengeli perspektifle göster. Ne geniş açı dramatizasyonu ne de güçlü telefoto sıkıştırması olsun. Çevre bağlamı mevcut fakat ikincil kalsın.

## English

> Show [SUBJECT] with the balanced natural perspective of roughly a 50 mm lens, avoiding both exaggerated wide-angle depth and strong telephoto compression. Keep environmental context present but secondary.

## Neye dikkat edilmeli?

Odak davranışı fiziksel olsun: makro karede alan derinliği sığlaşır, telefotoda planlar sıkışır; model her şeyi net vermeye eğilimlidir.

---
# 1304. `/85mm-portrait` — 85 mm Portre Sıkıştırması

## Türkçe

> [KİŞİ]'yi yaklaşık 85 mm portre perspektifinde göster. Kamera kişiye fiziksel olarak yeterli mesafede olsun. Yüz oranları doğal, arka plan hafif sıkışmış ve yumuşak olsun.
>
> “85 mm” diye otomatik creamy bokeh ve beauty retouch ekleme.

## English

> Show [PERSON] with the perspective behavior of an approximately 85 mm portrait lens, photographed from adequate physical distance. Preserve natural facial proportions with mild background compression.
>
> Do not automatically add extreme creamy bokeh or beauty retouching.

## Neye dikkat edilmeli?

Odak davranışı fiziksel olsun: makro karede alan derinliği sığlaşır, telefotoda planlar sıkışır; model her şeyi net vermeye eğilimlidir.

---
# 1305. `/135mm-compression` — Telefoto Sıkıştırma

## Türkçe

> [ÖZNE]'yi yaklaşık 135 mm telefoto perspektifiyle göster. Ön ve arka plan arasındaki mesafe görsel olarak sıkışsın. Uzak mimari/dağ/şehir özneye daha yakın görünürken perspektif doğal kalsın.

## English

> Show [SUBJECT] with the visual compression of an approximately 135 mm telephoto lens. Make distant architecture, terrain, or city elements appear visually closer to the subject while preserving believable perspective.

## Neye dikkat edilmeli?

Odak davranışı fiziksel olsun: makro karede alan derinliği sığlaşır, telefotoda planlar sıkışır; model her şeyi net vermeye eğilimlidir.

---
# 1306. `/telephoto-layering` — Telefoto Katmanlama

## Türkçe

> Uzak manzara veya şehir sahnesinde 135–200 mm telefoto sıkıştırması kullan. Ön, orta ve arka plan katmanları üst üste yaklaşmış gibi görünsün. Atmosferik perspektif katmanları birbirinden ayırsın.

## English

> Use 135–200 mm telephoto compression in a distant landscape or urban scene so foreground, middle ground, and background appear visually stacked. Separate them through atmospheric perspective.

## Neye dikkat edilmeli?

Odak davranışı fiziksel olsun: makro karede alan derinliği sığlaşır, telefotoda planlar sıkışır; model her şeyi net vermeye eğilimlidir.

---
# 1307. `/macro-100mm` — Gerçek Makro Davranışı

## Türkçe

> [KÜÇÜK NESNE/DETAY]'ı yaklaşık 100 mm macro lens davranışıyla göster. Tek gerçek odak düzlemi çok net, ön ve arka alan hızlı yumuşasın. Malzeme mikro dokusu fiziksel olarak okunabilsin.
>
> “Macro” diye nesneye gerçek dışı dev damla veya aşırı sharpening ekleme.

## English

> Show [SMALL OBJECT/DETAIL] with the behavior of an approximately 100 mm macro lens. Keep one real focal plane extremely clear while foreground and background fall off quickly. Reveal physically plausible micro-texture.
>
> Avoid oversized artificial droplets and excessive sharpening.

## Neye dikkat edilmeli?

Odak davranışı fiziksel olsun: makro karede alan derinliği sığlaşır, telefotoda planlar sıkışır; model her şeyi net vermeye eğilimlidir.

---
# 1308. `/deep-focus` — Derin Alan Netliği

## Türkçe

> Ön plandan arka plana kadar önemli görsel katmanları net tut. Özellikle mimari, eğitim düzeneği, flat lay veya teknik görselde shallow bokeh kullanma.

## English

> Keep important visual layers sharp from foreground through background. Avoid shallow bokeh, especially for architecture, educational setups, flat lays, and technical imagery.

## Neye dikkat edilmeli?

Odak davranışı fiziksel olsun: makro karede alan derinliği sığlaşır, telefotoda planlar sıkışır; model her şeyi net vermeye eğilimlidir.

---
# 1309. `/shallow-focus` — Sığ Alan Derinliği

## Türkçe

> Yalnız ana özne veya kritik ayrıntı net kalsın; odak düzleminin ön ve arkasında doğal optik yumuşama oluşsun. Blur miktarı öznenin boyutu ve kamera mesafesiyle uyumlu olsun.

## English

> Keep only the primary subject or critical detail in focus and allow natural optical falloff in front of and behind the focal plane. Make blur strength consistent with subject size and camera distance.

## Neye dikkat edilmeli?

Odak davranışı fiziksel olsun: makro karede alan derinliği sığlaşır, telefotoda planlar sıkışır; model her şeyi net vermeye eğilimlidir.

---
# 1310. `/focus-plane` — Odak Düzlemini Açıkça Tanımlama

## Türkçe

> Odak düzlemi: [GÖZLER / ÜRÜN ETİKETİ / ÖN ÇİÇEK / DEVRE PARÇASI].
>
> Bu düzlem en net alan olsun. Diğer katmanların netliği mesafeye göre doğal azalsın.

## English

> Focus plane: [EYES / PRODUCT LABEL / FRONT FLOWER / CIRCUIT COMPONENT].
>
> Keep this plane as the sharpest area and let other layers soften naturally with distance.

## Neye dikkat edilmeli?

Odak davranışı fiziksel olsun: makro karede alan derinliği sığlaşır, telefotoda planlar sıkışır; model her şeyi net vermeye eğilimlidir.

---
# 1311. `/eye-level` — Göz Hizası

## Türkçe

> Kamerayı öznenin doğal göz/gövde seviyesine yerleştir. Yukarıdan veya aşağıdan güç/drama ilişkisi kurma. Sahne gözlemci oradaymış gibi nötr hissedilsin.

## English

> Place the camera at the subject’s natural eye or body level. Avoid high- or low-angle power cues and make the scene feel neutrally observed.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1312. `/low-angle` — Alçak Açı

## Türkçe

> Kamerayı öznenin altında konumlandır ve hafif yukarı bak. Perspektif, özneyi daha baskın gösterebilir ancak mimari dikeyleri ve beden oranlarını kontrol altında tut.

## English

> Place the camera below the subject and look slightly upward. Allow a stronger sense of presence while keeping architectural verticals and body proportions controlled.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1313. `/worm-eye` — Çok Alçak / Zeminden Görüş

## Türkçe

> Kamerayı zemine çok yakın yerleştir. Ön plandaki yüzey/nesneler büyük, arka plan güçlü perspektif kaçışıyla küçük görünsün.
>
> Bu açıyı sıradan portrelerde gereksiz dramatizasyon için kullanma.

## English

> Place the camera very close to ground level. Let foreground surfaces or objects loom large while the background recedes strongly.
>
> Avoid using this angle merely to over-dramatize ordinary portraits.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1314. `/high-angle` — Yüksek Açı

## Türkçe

> Kamerayı öznenin üstüne çıkar ancak tam kuş bakışı yapma. Mekânsal düzen ve öznenin çevresi birlikte okunabilsin.

## English

> Raise the camera above the subject without going fully overhead. Keep both the subject and surrounding spatial arrangement readable.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1315. `/top-down` — Tam Tepeden Görünüm

## Türkçe

> Kamerayı yüzeye tam dik, 90 derece top-down konumlandır. Paralel çizgiler perspektifle daralmasın. Flat lay, yiyecek, materyal, worksheet veya koleksiyon düzeni için ortografiye yakın görüntü kullan.

## English

> Place the camera exactly perpendicular to the surface in a 90-degree top-down view. Avoid perspective convergence. Use near-orthographic behavior for flat lays, food, materials, worksheets, and collections.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1316. `/birds-eye` — Kuş Bakışı Çevresel Görüş

## Ayrım

`top-down` bir yüzeye dik teknik görünüm olabilir.

`bird’s-eye` daha yüksekten çevresel/şehirsel görüşü anlatır.

## Türkçe

> [SAHNE]'yi yüksek kuş bakışı açıdan göster. Yapılar/insanlar/araçlar mekânsal ilişki içinde okunmalı. Tam harita görünümüne dönüşmek zorunda değil.

## English

> Show [SCENE] from a high bird’s-eye perspective while preserving the spatial relationship among buildings, people, vehicles, or terrain. It does not need to become a strict map view.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1317. `/dutch-angle` — Eğik Ufuk

## Türkçe

> Kamerayı yaklaşık 8–15 derece bilinçli eğerek hafif Dutch angle oluştur. Bu açı yalnız gerilim, hareket veya dengesizlik anlatıya hizmet ediyorsa kullanılsın.
>
> Görüntüyü 30–45 derece rastgele yatırma.

## English

> Tilt the camera deliberately by roughly 8–15 degrees for a restrained Dutch angle, using it only when tension, movement, or imbalance serves the story.
>
> Avoid arbitrary 30–45 degree tilts.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1318. `/over-shoulder` — Omuz Üstü Görüş

## Türkçe

> Kamera ana kişinin omuz arkasından ikinci kişi/nesne/ekrana baksın. Ön plandaki omuz ve baş hafif yumuşak; asıl ilgi noktası net olsun. İki kişinin mekânsal yönü mantıklı kalsın.

## English

> Frame the view from behind one person’s shoulder toward a second person, object, or screen. Keep the foreground shoulder/head slightly soft and the main point of interest sharp. Preserve coherent spatial direction.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1319. `/two-shot` — İki Kişilik Kare

## Türkçe

> İki kişiyi aynı karede birbirleriyle mekânsal ilişki içinde göster. İki yüz de tanınabilir ve aynı ışık dünyasında olsun. İnsanları ayrı ayrı çekilip kolajlanmış gibi göstermeyin.

## English

> Frame two people within one coherent shot, preserving spatial relationship, recognizable faces, and one shared lighting environment. Avoid a composited “two separate portraits” appearance.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1320. `/insert-shot` — Nesne Ayrıntı Karesi

## Türkçe

> Ana sahneden tek kritik nesne/eylem ayrıntısını yakın insert shot olarak göster: el, anahtar, bilet, ekran, düğme veya yiyecek gibi.
>
> Yeni dekor nesnesi icat etme.

## English

> Show one critical object or action detail from the primary scene as a close insert shot, such as a hand, key, ticket, screen, button, or food item.
>
> Do not invent a new prop.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1321. `/establishing-shot` — Kurucu Geniş Plan

## Türkçe

> Sahnenin nerede geçtiğini ilk bakışta anlatan geniş kurucu kare oluştur. İnsan varsa küçük/orta ölçekte çevrenin içinde yer alsın. Mekânı yalnız dekoratif arka plan değil anlatı bilgisi olarak kullan.

## English

> Create a wide establishing shot that immediately communicates where the scene takes place. If people are present, keep them small to medium within the environment and treat location as narrative information rather than decoration.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1322. `/medium-shot` — Orta Plan

## Türkçe

> Kişiyi yaklaşık bel/göğüs üstü doğal orta planda göster. El hareketi veya yakın çevre bağlamı gerektiğinde kadraja dahil olsun.

## English

> Show the person in a natural medium shot around waist or chest level, including hand gestures or nearby context when relevant.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1323. `/close-up` — Yakın Plan

## Türkçe

> Kişinin yüzünü veya nesnenin ana işlevsel bölümünü kadrajın çoğunu kaplayacak yakın planda göster. Çevresel bilgi ikincil olsun.

## English

> Frame the person’s face or the primary functional area of an object in close-up so it fills most of the composition, keeping environment secondary.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1324. `/extreme-closeup` — Aşırı Yakın Plan

## Türkçe

> Tek fiziksel ayrıntıyı kadrajın ana konusu yap: göz, dikiş, baskı noktası, vida, yaprak damarı veya yiyecek dokusu gibi.
>
> Ayrıntının neye ait olduğu tamamen kaybolacak kadar soyutlaştırma, aksi özellikle istenmedikçe.

## English

> Make one physical detail the main subject of the frame, such as an eye, seam, print dot, screw, leaf vein, or food texture.
>
> Avoid making it so abstract that its source becomes unrecognizable unless explicitly intended.

## Neye dikkat edilmeli?

Açı adıyla sonuç eşleşsin: kuş bakışı ufku siler, kurucu plan mekânı tanıtır; yanlış açı sahnenin anlamını değiştirir.

---
# 1325. `/rembrandt-light` — Rembrandt Işığı

## Türkçe

> Tek ana ışığı yüzün bir tarafından yaklaşık 45 derece konumlandır. Gölgedeki yanakta küçük üçgen ışık alanı oluşsun. Dolgu ışığını düşük tut.
>
> Yüzün yarısını tamamen kaybetme.

## English

> Place one primary light roughly 45 degrees to one side of the face, producing a small triangular highlight on the shadow-side cheek. Keep fill low but preserve facial information.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1326. `/butterfly-light` — Butterfly / Paramount Işık

## Türkçe

> Ana ışığı yüzün önünde ve hafif yukarısında konumlandır. Burun altında küçük simetrik gölge oluşsun. Işık yüzü temiz ve grafik olarak anlatsın.
>
> Beauty filter veya plastik cilt kullanma.

## English

> Place the key light in front of and slightly above the face, producing a small symmetrical shadow below the nose. Keep the face cleanly modeled without beauty-filter skin.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1327. `/split-light` — Split Lighting

## Türkçe

> Yüzün bir tarafını ana ışıkla aydınlat, diğer tarafı belirgin gölgede bırak. Yine de gölgeli tarafta gerekli yüz bilgisi az miktarda okunabilsin.

## English

> Illuminate one side of the face while leaving the other in pronounced shadow, retaining just enough information on the dark side for facial structure to remain readable.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1328. `/window-light` — Pencere Işığı

## Türkçe

> Tek gerçek büyük pencereyi ana ışık kaynağı yap. Yüzeylerde pencere yönüne uygun yumuşak ışık geçişi ve doğal gölge oluşsun.
>
> İkinci görünmez sinematik key light ekleme.

## English

> Use one real large window as the primary light source, with soft directional transitions and natural shadows consistent with its position.
>
> Avoid adding an invisible cinematic second key light.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1329. `/overcast-light` — Kapalı Hava Yumuşak Işık

## Türkçe

> Bulutlu açık havada geniş gökyüzü softbox gibi çalışsın. Sert cast shadow oluşmasın; cilt ve materyal renkleri doğal, kontrast düşük/orta olsun.

## English

> Treat an overcast sky as a broad natural softbox. Avoid hard cast shadows and keep skin and material colors natural with low-to-moderate contrast.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1330. `/hard-sun` — Sert Öğle Güneşi

## Türkçe

> Öğle güneşini yüksek ve sert tek kaynak olarak göster. Keskin gölge kenarı, yüksek lokal kontrast ve gerçek göz/kaş gölgeleri oluşsun.
>
> Sert ışığı otomatik “kötü fotoğraf” gibi düzeltme.

## English

> Use high hard midday sun as one primary source, creating crisp shadow edges, strong local contrast, and realistic eye or brow shadows.
>
> Do not automatically soften or “fix” the hard light.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1331. `/backlight` — Ters Işık

## Türkçe

> Ana ışık öznenin arkasından gelsin. Kenarlarda doğal ışık ayrımı oluşabilir fakat ön yüz yalnız gerçek ortam dolgusuyla okunmalı.
>
> Her kenarı yapay rim light ile çizme.

## English

> Place the primary light behind the subject. Allow natural edge separation while letting the front remain readable only through believable ambient fill.
>
> Avoid outlining every edge with artificial rim light.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1332. `/practical-light` — Kadraj İçindeki Gerçek Işık Kaynağı

## Türkçe

> Sahnenin ana ışığını kadrajda gerçekten görünen [LAMBA / EKRAN / VİTRİN / SOKAK LAMBASI] sağlasın. Yüzey yansımaları ve gölge yönleri bu kaynağa uyumlu olsun.

## English

> Let a visible practical source such as a lamp, screen, shop window, or streetlight provide the primary illumination. Keep reflections and shadow directions consistent with that source.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1333. `/direct-flash` — Doğrudan Flaş

## Türkçe

> Kamera eksenine çok yakın küçük doğrudan flaş kullan. Ön plan sert ve eşit aydınlansın; arka plan mesafeyle hızlıca kararsın. Parlak yüzeylerde küçük frontal reflection oluşabilir.
>
> Stüdyo fill ve rim light ekleme.

## English

> Use a small direct flash close to the camera axis. Illuminate the foreground hard and evenly while letting the background fall off rapidly with distance. Allow small frontal reflections on glossy surfaces.
>
> Avoid studio fill and rim lighting.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1334. `/bounce-flash` — Tavandan/Satıhtan Sekmeli Flaş

## Türkçe

> Flaş doğrudan özneye değil açık renkli tavana/duvara sekmiş gibi geniş ve daha yumuşak ışık üretsin. Işık yönü sekme yüzeyine göre mantıklı olsun.

## English

> Make flash illumination appear bounced from a light ceiling or wall rather than fired directly at the subject, producing broader softer light with direction consistent with the bounce surface.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1335. `/drag-shutter` — Yavaş Enstantane + Flaş

## Türkçe

> Ana özneyi kısa flaşla nispeten net dondur, arka plan/pratik ışıkları daha uzun exposure nedeniyle yönlü harekete yayılsın.
>
> Flaşlı öznenin kendisini tamamen motion blur'a dönüştürme.

## English

> Freeze the main subject relatively sharply with a short flash while allowing background and practical lights to trail through a longer exposure.
>
> Do not blur the flash-lit subject completely.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1336. `/rear-curtain-flash` — Arka Perde Flaş Hissi

## Türkçe

> Hareket eden nesnenin arkasında yönlü motion trail oluşsun; final pozisyon flaşla daha net dondurulmuş görünsün.
>
> Trail hareket yönüyle fiziksel uyumlu olsun.

## English

> Show directional motion trails behind the moving subject while the final position appears sharply frozen by flash. Keep the trail physically consistent with movement direction.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1337. `/long-exposure` — Uzun Pozlama

## Türkçe

> Sabit mimari/zemin net kalsın; hareket eden su, araç ışığı veya insanlar zaman boyunca blur/trail oluştursun.
>
> Aynı nesneyi hem tamamen net hem güçlü hareketli gösterme.

## English

> Keep stationary architecture or ground sharp while moving water, vehicle lights, or people accumulate blur or trails over time.
>
> Avoid showing the same moving object both perfectly frozen and strongly motion-blurred.

## Neye dikkat edilmeli?

Tek ışık mantığı: gölge yönü, sertliği ve renk ısısı bütün öğelerde aynı kaynağı göstersin.

---
# 1338. `/0.5x-phone` — Smartphone 0.5x Ultra-wide

## Trend

**T1/T2 — gündelik sosyal fotoğraf dilinde güçlü.**

## Türkçe

> Görüntüyü telefonun 0.5x ultra-wide kamerasıyla yakın mesafeden çekilmiş gündelik fotoğraf gibi göster. Kadraj kenarında belirgin geniş açı gerilmesi, merkeze yakın bölgede daha doğal oranlar olsun.
>
> İnsan yüzünü merkezin dışına taşıyıp aşırı deforme etme.

## English

> Make the image feel captured close-up with a smartphone 0.5x ultra-wide camera. Use visible edge stretching while keeping proportions more natural near the center.
>
> Avoid placing faces far off-center where distortion becomes extreme.

---

# 1339. `/front-camera` — Telefon Ön Kamerası

## Türkçe

> Sahneyi telefon ön kamerasıyla çekilmiş doğal selfie gibi göster. Kol/telefon mesafesine uygun perspektif, küçük sensör keskinliği ve geniş açı davranışı olsun.
>
> Profesyonel 85 mm portre bokeh'i ekleme.

## English

> Show the scene as a natural front-camera phone selfie with perspective consistent with arm’s-length distance, small-sensor sharpness, and mild wide-angle behavior.
>
> Avoid professional 85 mm portrait bokeh.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1340. `/webcam` — Laptop Webcam

## Türkçe

> Kişiyi laptop webcam'i ile çekilmiş düşük/orta çözünürlüklü doğal görüntü gibi göster. Kamera ekranın üst kenarında hafif aşağı/yukarı açı farkıyla konumlanmış olsun. İç mekân ışığında küçük noise ve sınırlı dynamic range olabilir.

## English

> Show the person as a natural laptop-webcam image with modest resolution, camera position near the top of the screen, mild angle bias, small low-light noise, and limited dynamic range.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1341. `/cctv` — Güvenlik Kamerası Görünümü

## Kullanım

Kurgu, mekân analizi, güvenlik senaryosu veya görsel anlatı.

## Türkçe

> [MEKÂN]'ı sabit yüksek köşe konumlu güvenlik kamerası gibi göster. Geniş açı, yüksek viewpoint, sabit kadraj ve işlevsel tüm alan görünürlüğü olsun.
>
> Timestamp gerekiyorsa kurmaca ve kısa olsun.
>
> Güvenlik kamera görünümünü kişisel gözetleme/mahremiyet ihlali amacıyla kullanma.

## English

> Show [SPACE] from a fixed high-corner security-camera viewpoint with wide-angle coverage and a static functional frame.
>
> If a timestamp is needed, keep it clearly fictional and concise.
>
> Do not use this visual language to facilitate invasive real-person surveillance.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1342. `/doorbell-cam` — Kapı Zili Kamerası

## Türkçe

> Kapı önündeki sahneyi geniş açılı doorbell camera viewpoint'undan göster. Kamera yaklaşık göğüs/kapı zili yüksekliğinde ve kapıya çok yakın olsun. Kenarlarda barrel distortion doğal olabilir.

## English

> Show the doorstep scene from a wide-angle doorbell-camera viewpoint positioned close to the door around chest or bell height. Allow natural edge barrel distortion.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1343. `/dashcam` — Araç Ön Kamera Görünümü

## Türkçe

> Sahneyi aracın ön camı arkasındaki sabit dashcam viewpoint'undan göster. Kaputun çok küçük bir bölümü alt kenarda olabilir. Yol geometrisi, trafik ve ufuk doğal sürüş perspektifinde olsun.
>
> Gerçek olay kaydı gibi sahte tarih/konum üretme.

## English

> Show the scene from a fixed dashcam viewpoint behind the windshield, with only a small portion of hood visible if appropriate. Preserve believable road geometry, traffic, and driving perspective.
>
> Do not fabricate real-event timestamps or locations.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1344. `/bodycam-fictional` — Kurmaca Bodycam Estetiği

## Türkçe

> Kurmaca hikâye sahnesini göğüs hizasında takılı bodycam viewpoint'undan göster. El/kol kadraja girebilir; kamera hareketi insan gövdesine bağlı hafif eğimli olabilir.
>
> Gerçek kolluk kuvveti kaydı, gerçek olay veya gerçek kişiye ait delil gibi sunma.

## English

> Show a fictional story scene from a chest-mounted body-camera viewpoint. Hands or arms may enter the frame and the camera may tilt slightly with body movement.
>
> Do not present it as genuine evidence from law enforcement, a real incident, or a real person.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1345. `/action-cam` — Action Camera

## Türkçe

> [AKSİYON]'ı vücuda/ekipmana sabitlenmiş ultra-wide action camera ile göster. Güçlü çevresel hareket, yakın ön plan ve geniş görüş açısı olsun. Öznenin hareket yönü fiziksel olarak anlaşılır kalsın.

## English

> Show [ACTION] through a body- or equipment-mounted ultra-wide action camera, with strong environmental motion, close foreground, and broad field of view. Keep movement direction physically clear.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1346. `/helmet-cam` — Kask Kamerası

## Türkçe

> Bisiklet, kayak, motorsporu veya benzeri eylemi kask seviyesinden first-person viewpoint ile göster. Ekipmanın küçük kenar parçaları görüş alanına girebilir. Kamera baş hareketine bağlı olsun.

## English

> Show cycling, skiing, motorsport, or similar action from a helmet-height first-person viewpoint. Small parts of equipment may enter the frame and camera orientation should follow head movement.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1347. `/drone-topdown` — Drone Tam Tepeden

## Türkçe

> [MEKÂN]'ı drone ile yüksekten tam dik top-down görüşte göster. Yollar, kıyı, insanlar veya araçlar gerçek ölçek ilişkisi taşısın. Gereksiz tilt-shift minyatür efekti ekleme.

## English

> Show [PLACE] from a high drone view looking straight down. Preserve real scale relationships among roads, shoreline, people, and vehicles. Avoid unnecessary tilt-shift miniature effect.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1348. `/drone-oblique` — Drone Eğik Açı

## Türkçe

> Drone kamerasını yüksek ancak eğik açıyla kullan; hem plan ilişkileri hem ufuk/cepheler okunabilsin. Mimariyi imkânsız kuş bakışı perspektife bükme.

## English

> Use a high oblique drone view that reveals both plan relationships and facades or horizon. Avoid impossible warped aerial perspective.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1349. `/camcorder-handheld` — El Kamerası / Camcorder

## Türkçe

> Görüntüyü 1990–2000'ler consumer camcorder ile elde çekilmiş video karesi gibi göster. Hafif interlaced/video softness, küçük white-balance hatası ve gerçek zoom davranışı olabilir.
>
> Her kareye büyük timestamp ekleme.

## English

> Make the image feel like a handheld frame from a 1990s–2000s consumer camcorder, with mild video softness, small white-balance imperfection, and believable optical zoom behavior.
>
> Avoid adding oversized timestamps automatically.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1350. `/nightvision` — Gece Görüş Simülasyonu

## Türkçe

> Kurmaca/teknik sahneyi düşük ışık night-vision visualization olarak göster. Tek renk yeşil veya gri ton, düşük detay ve güçlü noise olabilir.
>
> Gerçek güvenlik/taktik bilgi çıkarmak için kullanma; görsel simülasyon olarak değerlendir.

## English

> Render a fictional or technical scene as low-light night-vision visualization using monochrome green or gray, limited detail, and stronger noise.
>
> Treat it as a visual simulation rather than a tool for extracting real security or tactical information.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1351. `/thermal-style-safe` — Termal Görselleştirme Simülasyonu

`/thermal-cam` ile aynı aileyi güçlendirir.

## Türkçe

> Görseli termal renk haritasını taklit eden sanatsal/öğretici simülasyon olarak göster. Gerçek sıcaklık değeri yazma ve görüntünün gerçek termal ölçüm olduğunu iddia etme.

## English

> Render the image as an artistic or educational simulation of a thermal color map. Do not display fabricated temperature values or imply genuine thermographic measurement.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1352. `/microscope-view` — Mikroskop Görüşü

## Türkçe

> [NUMUNE]'yi belirtilen mikroskop türünün görsel mantığında göster: brightfield / fluorescence / stereo microscope gibi.
>
> Büyütme, boya/fluorophore ve yapı bilgisi verilmediyse bilimsel ayrıntı icat etme.
>
> Dekoratif renkleri veriymiş gibi sunma.

## English

> Show [SPECIMEN] according to the visual logic of the specified microscopy mode such as brightfield, fluorescence, or stereo microscopy.
>
> Do not invent magnification, stain, fluorophore, or structural detail when not supplied.
>
> Avoid presenting decorative color as scientific measurement.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1353. `/endoscope-view` — Endoskopik / Dar Optik Görüş

## Kullanım

Teknik boru içi, makine içi veya medikal olmayan eğitim/cihaz senaryolarında da kullanılabilir.

## Türkçe

> Dar lensli endoscope/inspection camera viewpoint'u kullan. Dairesel veya çok geniş yakın görüş, güçlü yakın perspektif ve sınırlı ışık kaynağı olsun.
>
> Görseli bilimsel/medikal teşhis olarak sunma.

## English

> Use the viewpoint of a narrow inspection or endoscope-style camera with close wide perspective and limited onboard illumination.
>
> Do not present the generated image as medical or scientific diagnosis.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1354. `/capture-source` — Çekim Kaynağını Önce Tanımla

## Yeni üst kısayol

> `/capture-source: smartphone / webcam / CCTV / camcorder / drone / macro / scanner / film`

Bu, “style”dan önce **görüntünün hangi cihaz/optik sistemden geldiğini** belirler.

Örnek:

> `/capture-source smartphone + /direct-flash + /photo-dump`

veya:

> `/capture-source drone + /top-down`

---

# 1355. `Capture-source` neden önemlidir?

Çünkü aynı sahne:

> DSLR,
>
> smartphone,
>
> webcam,
>
> CCTV,
>
> camcorder,
>
> scanner

ile farklı görünür.

Fark yalnız çözünürlük değildir.

Değişir:

- kamera konumu,
- focal behavior,
- dynamic range,
- sharpening,
- noise,
- depth of field,
- motion,
- ışık davranışı,
- kullanım amacı.

Bu yüzden:

> `make it look like CCTV`

yerine:

> `fixed high-corner wide-angle camera, static framing, deep focus, limited dynamic range`

daha açıklayıcıdır.

---

# 1356. `/camera-brand-free` — Marka Yerine Optik Davranış

## Türkçe

> Kamera marka/model adı kullanmadan çekimi tarif et:
>
> - focal length behavior,
> - camera distance,
> - depth of field,
> - light source,
> - motion behavior,
> - color/contrast response.
>
> Görsel karakter gerçek davranıştan çıksın.

## English

> Describe the shot without relying on camera brand or model names. Specify focal-length behavior, camera distance, depth of field, light source, motion behavior, and color/contrast response.
>
> Let visual character emerge from actual photographic behavior.

## Neye dikkat edilmeli?

Kamera dili gözetim izlenimi vermesin: CCTV, bodycam ve gece görüşü estetiği kurmaca çerçevede ve rıza bağlamında kullanılır.

---
# 1357. `/fake-camera-parameter-filter` — Sözde Kamera Parametresi Filtresi

İnternette sık geçen:

> `Hasselblad 100MP`
>
> `RAW 16-bit`
>
> `32K`
>
> `ISO 64`
>
> `f/1.2`
>
> `Leica color science`

gibi ifadeler her modelde gerçek teknik simülasyon yapmaz.

### Yararlı olan

Gözle görülür sonucu tarif etmek:

> `shallow depth of field`
>
> `high highlight retention`
>
> `soft tonal roll-off`
>
> `telephoto compression`
>
> `hard direct flash`

### Rehber ilkesi

> **Değer ancak görsel sonucu açıklıyorsa kullan.**

---

# 1358. `/shot-sequence` — Sinematik Çekim Dizisi

## Türkçe prompt

> Aynı sahneyi 6 karelik çekim dizisi olarak oluştur:
>
> 1. establishing,
> 2. wide,
> 3. medium,
> 4. over-the-shoulder,
> 5. close-up,
> 6. insert.
>
> Karakter, kıyafet, ışık, zaman ve mekân sürekliliği korunsun.
>
> Her plan gerçekten farklı bilgi taşısın.

## English

> Create the same scene as a six-shot sequence:
>
> 1. establishing,
> 2. wide,
> 3. medium,
> 4. over-the-shoulder,
> 5. close-up,
> 6. insert.
>
> Preserve character, wardrobe, lighting, time, and location continuity.
>
> Give every shot a distinct informational purpose.

## Neye dikkat edilmeli?

Fiziksel davranış (gölge yönü, gren, alan derinliği) tek ışık mantığına uysun; “film hissi” için gren eklemek zayıf kompozisyonu kurtarmaz.

---
# 1359. `/shot-reverse-shot` — Diyalog Çekim Karşılığı

## Türkçe

> İki kişinin konuşmasını shot/reverse-shot çifti olarak göster.
>
> İki kamerada eyeline, background direction ve screen direction tutarlı kalsın.
>
> Karakterleri kameralar arasında sağ-sol yer değiştirerek continuity bozma.

## English

> Show a two-person conversation as a shot/reverse-shot pair.
>
> Preserve eyeline, background direction, and screen direction between cameras.
>
> Do not flip character positions and break continuity.

## Neye dikkat edilmeli?

Seride ışık, nesne konumu ve hareket yönü kareler arasında sabit kalsın; sapan kare tek değişiklikle düzeltilir.

---
# 1360. `/180-rule-lock` — 180 Derece Kuralı Tutarlılığı

## Türkçe

> Çok kareli diyalog/aksiyon dizisinde hayali aks çizgisini koru. Karakter A tüm karşı planlarda aynı ekran tarafında, karakter B diğer tarafta kalsın; bilinçli aks kırılması istenmedikçe kamerayı çizginin ötesine taşıma.

## English

> Preserve the imaginary action axis across a multi-shot dialogue or action sequence. Keep Character A on the same screen side and Character B on the opposite side unless an intentional axis break is requested.

## Neye dikkat edilmeli?

Seride ışık, nesne konumu ve hareket yönü kareler arasında sabit kalsın; sapan kare tek değişiklikle düzeltilir.

---
# 1361. `/continuity-props` — Nesne Sürekliliği

## Türkçe

> Seri boyunca fincan, kitap, telefon, çanta, araç, ürün veya diğer tekrar eden nesnelerin:
>
> - konumu,
> - rengi,
> - doluluk seviyesi,
> - yönü,
> - hasarı/kullanım izi
>
> sahne zamanına uygun biçimde devam etsin.

## English

> Preserve continuity of recurring props such as cups, books, phones, bags, vehicles, and products across the sequence, including position, color, fill level, orientation, and wear state according to scene chronology.

## Neye dikkat edilmeli?

Seride ışık, nesne konumu ve hareket yönü kareler arasında sabit kalsın; sapan kare tek değişiklikle düzeltilir.

---
# 1362. `/continuity-light` — Işık Sürekliliği

## Türkçe

> Aynı sahne dizisinde ana ışık kaynağının yönü, günün saati, gölge yönü ve renk sıcaklığı planlar arasında değişmesin.

## English

> Preserve primary light direction, time of day, shadow direction, and color temperature across shots from the same scene.

## Neye dikkat edilmeli?

Seride ışık, nesne konumu ve hareket yönü kareler arasında sabit kalsın; sapan kare tek değişiklikle düzeltilir.

---
# 1363. `/continuity-screen-direction` — Hareket Yönü Sürekliliği

## Türkçe

> Karakter veya araç bir karede soldan sağa hareket ediyorsa sonraki continuity planında ekran yönünü anlamsızca tersine çevirme.

## English

> If a character or vehicle moves left-to-right in one shot, preserve screen direction in continuity shots unless a deliberate reversal is narratively intended.

## Neye dikkat edilmeli?

Seride ışık, nesne konumu ve hareket yönü kareler arasında sabit kalsın; sapan kare tek değişiklikle düzeltilir.

---
# 1364. `/camera-language-slop-filter` — Kamera Promptlarında AI Slop Filtresi

Kaçınılması gerekenler:

- `85mm` yazınca her şeyi portre bokeh'ine çevirmek,
- `cinematic` = teal-orange,
- `35mm` = grain,
- `film` = light leak,
- `macro` = dev su damlası,
- `wide angle` = fisheye,
- `night` = neon,
- `backlight` = yapay rim-light outline,
- `professional` = shallow depth of field,
- her prompta marka kamera adı eklemek,
- teknik olarak çelişen kamera davranışlarını aynı anda istemek.

---

# 1365. Yeni üst aile: `Capture Grammar`

Bu bölümden çıkan üst kavram:

> **Capture Grammar — Görselin “neye benzediğinden” önce “nasıl çekildiğini” tarif etmek.**

Aile:

- focal length,
- camera angle,
- shot size,
- focus behavior,
- lighting,
- motion,
- capture device,
- continuity.

Prompt formülü:

> **capture source + camera position + focal behavior + focus + light + motion + subject**

Örnek:

> `/capture-source smartphone + /0.5x-phone + /direct-flash + candid group`

Bu, yalnız:

> `cool Y2K photo`

demekten çok daha denetlenebilirdir.

---

# 1366. Yeni üst aile: `Cinematic Continuity`

Tek güzel kare değil, **aynı dünyanın art arda gelen kareleri** için.

Aile:

- `/shot-sequence`
- `/shot-reverse-shot`
- `/180-rule-lock`
- `/continuity-props`
- `/continuity-light`
- `/continuity-screen-direction`
- `/continuity-lock`

Ana kural:

> **Her yeni kare yeni bir görsel üretim değil; önceki karenin devamıdır.**

---

# 1367. Bu turdaki slash-style indeks (aile-017)

| Kısayol | Aile |
|---|---|
| `/24mm-wide` | wide environmental perspective |
| `/35mm-documentary` | documentary environmental view |
| `/50mm-natural` | neutral natural perspective |
| `/85mm-portrait` | portrait compression |
| `/135mm-compression` | telephoto compression |
| `/telephoto-layering` | stacked distant planes |
| `/macro-100mm` | real macro behavior |
| `/deep-focus` | broad focus depth |
| `/shallow-focus` | narrow focus depth |
| `/focus-plane` | explicit focal plane |
| `/eye-level` | neutral eye-level camera |
| `/low-angle` | low-angle viewpoint |
| `/worm-eye` | ground-level viewpoint |
| `/high-angle` | elevated viewpoint |
| `/top-down` | perpendicular overhead view |
| `/birds-eye` | high environmental view |
| `/dutch-angle` | controlled tilted horizon |
| `/over-shoulder` | over-the-shoulder shot |
| `/two-shot` | two-person composition |
| `/insert-shot` | detail insert |
| `/establishing-shot` | location-establishing wide |
| `/medium-shot` | medium human framing |
| `/close-up` | close framing |
| `/extreme-closeup` | single-detail framing |
| `/rembrandt-light` | Rembrandt portrait lighting |
| `/butterfly-light` | frontal upper beauty light |
| `/split-light` | half-lit face |
| `/window-light` | natural window source |
| `/overcast-light` | broad cloud-softened light |
| `/hard-sun` | hard midday sun |
| `/backlight` | rear primary illumination |
| `/practical-light` | visible real light source |
| `/direct-flash` | on-axis direct flash |
| `/bounce-flash` | bounced flash |
| `/drag-shutter` | flash + slow shutter |
| `/rear-curtain-flash` | motion trail + frozen endpoint |
| `/long-exposure` | time-accumulated movement |
| `/0.5x-phone` | smartphone ultra-wide |
| `/front-camera` | phone selfie camera |
| `/webcam` | laptop webcam |
| `/cctv` | fixed security-camera framing |
| `/doorbell-cam` | doorbell camera |
| `/dashcam` | vehicle dashboard camera |
| `/bodycam-fictional` | fictional body-camera POV |
| `/action-cam` | action-camera view |
| `/helmet-cam` | helmet-mounted POV |
| `/drone-topdown` | vertical aerial view |
| `/drone-oblique` | oblique aerial view |
| `/camcorder-handheld` | consumer camcorder |
| `/nightvision` | simulated night vision |
| `/thermal-style-safe` | non-measurement thermal simulation |
| `/microscope-view` | microscopy visual grammar |
| `/endoscope-view` | narrow inspection-camera POV |
| `/capture-source` | declare capture device first |
| `/camera-brand-free` | behavior instead of brand |
| `/fake-camera-parameter-filter` | pseudo-technical camera filter |
| `/shot-sequence` | multi-shot cinematic sequence |
| `/shot-reverse-shot` | dialogue shot pair |
| `/180-rule-lock` | preserve action axis |
| `/continuity-props` | prop continuity |
| `/continuity-light` | lighting continuity |
| `/continuity-screen-direction` | movement direction continuity |

---

<a id="aile-018"></a>
# Wayfinding, Çevresel Grafik, Etkileşimli Baskı ve Scrollytelling — 2026 Ek Taraması

2026 araştırmalarında bu turda dört alan öne çıktı:

- **wayfinding ve experiential graphic design**,
- **erişilebilir yönlendirme ve multisensory navigation**,
- **etkileşimli fiziksel baskı / packaging mechanics**,
- **scrollytelling ve adım adım veri anlatımı**.

SEGD’nin 2026 yayınları wayfinding’i yalnız tabela tasarımı değil; **insanın mekânda yön bulmasını, aidiyet kurmasını ve güvenli biçimde hareket etmesini sağlayan bir sistem** olarak ele alıyor. Erişilebilirlik, dijital araçlar, insan psikolojisi, ses ve mekân ilişkisi de artık bu alanın parçası.

Drupa’nın 2026 print değerlendirmesi de baskının yalnız yüzey değil, fiziksel etkileşim alanı olduğunu vurguluyor: peel/reveal, scratch, punch-out, emboss/deboss, NFC/QR, değişken veri ve lenticular gibi mekanikler tek başına “gimmick” değil, işlevle birleştiğinde güçlü.

Flourish’in 2026 scrollytelling rehberi de veri hikâyesinin başarısını “çok grafik göstermek” yerine **bilgiyi doğru sırayla, bir şey bir şey açmak** üzerinden tanımlıyor.

Bu nedenle bu bölümün ana prensibi:

> **Yönlendirme, etkileşim ve veri hikâyesi; dekor değil davranış tasarımıdır.**

---

# 1368. `/wayfinding-system` — Yönlendirme Sistemi

## Türkçe prompt

> [MEKÂN] için bütünsel wayfinding system tasarla.
>
> Sistem yalnız tabelalardan oluşmasın. Şunları birlikte düşün:
>
> - giriş tanımlama,
> - yön karar noktaları,
> - kat/alan kimliği,
> - oda/kapı numarası,
> - harita,
> - çıkış,
> - erişilebilir rota.
>
> Aynı tipografi, ikon ve renk sistemi kullan ancak her yüzeyi aynı renkli tabela ile doldurma.
>
> Önce kullanıcının hangi noktada hangi kararı vermesi gerektiğini belirle.

## English

> Design a complete wayfinding system for [SPACE].
>
> Include more than signs: entry identification, decision points, floor or zone identity, room numbering, maps, exits, and accessible routes.
>
> Use one coherent typography, icon, and color system without covering every surface in identical signage.
>
> Determine what decision a person must make at each point before designing the sign.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1369. `/decision-point-sign` — Karar Noktası Tabelası

## Türkçe

> [MEKÂN]'daki gerçek karar noktasında kullanılacak yön tabelası tasarla.
>
> Yalnız o noktada gerekli 2–5 hedefi göster.
>
> Ok yönleri fiziksel rota ile uyuşsun.
>
> Kullanıcının henüz karar veremeyeceği uzak ayrıntıları aynı tabelaya ekleme.

## English

> Design a directional sign for a real decision point in [SPACE].
>
> Show only the 2–5 destinations relevant at that location.
>
> Make arrow directions correspond to the actual routes.
>
> Do not overload the sign with distant destinations the user does not need yet.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1370. `/you-are-here-map` — “Buradasınız” Haritası

## Türkçe

> [MEKÂN] için sade “Buradasınız” haritası oluştur.
>
> Kullanıcının bakış yönü ile harita yönünü mümkün olduğunca eşleştir.
>
> “Buradasınız” noktası belirgin ancak diğer bilgileri bastırmayacak kadar kontrollü olsun.
>
> En önemli rota ve hedefler ilk bakışta okunmalı.
>
> Dekoratif 3B bina perspektifi kullanıp navigasyonu zorlaştırma.

## English

> Create a clear “You Are Here” map for [SPACE].
>
> Align map orientation with the viewer’s facing direction whenever possible.
>
> Make the current-location marker prominent but not overwhelming.
>
> Primary routes and destinations should read immediately.
>
> Avoid decorative 3D building perspectives that make navigation harder.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1371. `/accessible-wayfinding` — Erişilebilir Yönlendirme

## Türkçe prompt

> [MEKÂN] wayfinding sistemini erişilebilirlik önceliğiyle tasarla.
>
> Yüksek okunabilirlik, güçlü kontrast, yeterli yazı boyutu, tutarlı ikon, açık yön okları ve mantıklı yerleşim kullan.
>
> Bilgiyi yalnız renk ile kodlama.
>
> Gerektiğinde dokunsal/Braille veya ses/dijital yönlendirme için alan düşün.
>
> Erişilebilirliği dekoratif “engelli simgesi” eklemekle sınırlama.

## English

> Design the [SPACE] wayfinding system with accessibility as a primary requirement.
>
> Use strong legibility, sufficient contrast, readable type size, consistent icons, clear arrows, and logical placement.
>
> Do not encode critical information by color alone.
>
> Allow for tactile, Braille, audio, or digital navigation where appropriate.
>
> Do not reduce accessibility to adding a wheelchair symbol.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1372. `/tactile-map` — Dokunsal Harita

## Türkçe

> [MEKÂN] için gerçek fiziksel tactile map tasarla.
>
> Ana koridor, duvar, giriş, asansör/merdiven ve önemli hedefleri farklı kabartma/tekstür kodlarıyla ayır.
>
> Parmakla izlenebilecek açık rotalar kullan.
>
> İnce dekoratif çizgileri kabartmaya dönüştürme.
>
> Braille kullanılıyorsa gerçek standarda göre ayrıca doğrulanmalı.

## English

> Design a real physical tactile map for [SPACE].
>
> Distinguish primary corridors, walls, entrances, lifts or stairs, and key destinations using different raised or textured codes.
>
> Keep routes easy to trace by touch.
>
> Do not emboss fine decorative linework.
>
> Any Braille must be verified against the relevant standard.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1373. `/floor-identity` — Kat / Bölge Kimliği

## Türkçe

> Çok katlı [BİNA]'da her kata farklı ama aynı sistem içinde zone identity ver.
>
> Renk, büyük sayı, kısa isim ve gerektiğinde tek sembol birlikte kullanılabilir.
>
> Kullanıcı katı yalnız renkten anlamak zorunda kalmasın.

## English

> Give each floor or zone of [BUILDING] a distinct identity within one coherent system.
>
> Combine color, large numerals, concise names, and at most one symbol.
>
> Do not make users depend on color alone to know their location.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1374. `/landmark-wayfinding` — Mekânsal Landmark ile Yön Bulma

## Trend bağlantısı

SEGD’nin 2026 “Logos to Landmarks” yaklaşımında yönlendirme, kimlik ve fiziksel landmark birbirine bağlanıyor.

## Türkçe prompt

> [MEKÂN]'da yön bulmayı kolaylaştıracak 3–5 fiziksel landmark noktası tasarla.
>
> Her landmark:
>
> - farklı konum,
> - farklı işlev,
> - net silhouette veya malzeme,
> - navigasyon dilinde kullanılabilecek kısa isim
>
> taşısın.
>
> Landmarkları yalnız dev logo heykeli yapma.

## English

> Design 3–5 physical landmarks that help navigation in [SPACE].
>
> Give each a distinct location, function, recognizable silhouette or material, and a concise name that can be used in directions.
>
> Do not reduce landmarks to oversized logo sculptures.

---

# 1375. `/environmental-graphic-wall` — Çevresel Grafik Duvarı

## Türkçe

> [MEKÂN]'ın kimliğini anlatan environmental graphic wall tasarla.
>
> Duvar:
>
> - yerel hikâye,
> - kurum geçmişi,
> - tipografi,
> - fotoğraf veya illüstrasyon
>
> öğelerinden yalnız 2–3 tanesini güçlü biçimde kullansın.
>
> Wayfinding işlevi varsa yön bilgisi dekorun içinde kaybolmasın.

## English

> Design an environmental graphic wall for [SPACE] using only 2–3 strong elements such as local story, institutional history, typography, photography, or illustration.
>
> If the wall also carries wayfinding information, keep navigation clearly distinguishable from decoration.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1376. `/placemaking-signage` — Yer Kimliği + Yönlendirme

## Türkçe

> [YER] için signage sistemini o yerin gerçek malzeme, mimari, kültür ve kullanım biçiminden türet.
>
> Yerel kimliği rastgele motif yapıştırarak kurma.
>
> Tabela formu, malzeme ve tipografi çevrenin karakteriyle ilişki kursun.

## English

> Derive the signage system for [PLACE] from its real material, architectural, cultural, and functional context.
>
> Do not signal locality by pasting arbitrary motifs.
>
> Let sign form, material, and typography relate genuinely to the place.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1377. `/signage-family-board` — Tabela Ailesi Panosu

## Türkçe

> [PROJE] için bütün signage family'yi tek board üzerinde göster:
>
> - gateway,
> - directional,
> - identification,
> - room sign,
> - map,
> - regulatory,
> - accessibility.
>
> Her türün aynı tasarım sistemi içindeki rolü açıkça görülsün.
>
> Hepsini aynı boyutta tabela mockup'u yapma.

## English

> Show the full signage family for [PROJECT] on one board:
>
> gateway, directional, identification, room sign, map, regulatory, and accessibility.
>
> Make each sign type’s role clear within one coherent system.
>
> Do not present every sign as the same-size mockup.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1378. `/signage-placement-review` — Tabela Yerleşim İncelemesi

## Türkçe

> Kaynak mekân görseli üzerinde tabelaların gerçek görüş mesafesi ve yaklaşma yönüne göre placement review oluştur.
>
> Her tabelanın:
>
> - görüş yüksekliği,
> - yaklaşma yönü,
> - yaklaşık okuma mesafesi,
> - engellenme riski
>
> kontrol edilsin.
>
> Tabelayı yalnız “boş duvar var” diye oraya koyma.

## English

> Create a signage-placement review over the source space, considering real viewing distance and approach direction.
>
> Check viewing height, approach, approximate reading distance, and obstruction risk for each sign.
>
> Do not place signs merely because a wall is visually empty.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1379. `/multisensory-wayfinding` — Çok Duyulu Yönlendirme

## Trend

**T2 — 2026 SEGD omnispatial / accessibility konuşmalarında güçlü.**

## Türkçe prompt

> [MEKÂN] için görsel tabelaya ek olarak sınırlı multisensory wayfinding sistemi düşün.
>
> Gerektiğinde:
>
> - dokunsal yüzey,
> - zemin değişimi,
> - ses işareti,
> - aydınlatma ritmi,
> - dijital yönlendirme
>
> kullanılabilir.
>
> Her duyu kanalını aynı anda kullanma; her biri gerçek navigasyon görevine hizmet etsin.

## English

> Design a restrained multisensory wayfinding system for [SPACE] that can supplement visual signage through tactile surfaces, floor changes, sound cues, lighting rhythm, or digital guidance where appropriate.
>
> Do not use every sensory channel at once; assign each one a real navigation function.

---

# 1380. `/wayfinding-user-journey` — Yön Bulma Kullanıcı Yolculuğu

## Türkçe

> [KULLANICI]'nın girişten [HEDEF]'e kadar hareketini 6 aşamada göster.
>
> Her aşamada:
>
> - kullanıcının gördüğü işaret,
> - verdiği karar,
> - bir sonraki referans noktası
>
> yer alsın.
>
> Yolculuğu yalnız floor plan üzerinde çizgi olarak gösterme.

## English

> Show the journey of [USER] from entry to [DESTINATION] in six stages.
>
> At each stage identify the visible cue, the decision made, and the next reference point.
>
> Do not reduce the journey to a single line on a floor plan.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1381. `/wayfinding-slop-filter` — Wayfinding AI Slop Filtresi

Kaçınılması gerekenler:

- yalnız renkli tabela ailesi,
- her işarette 10 hedef,
- ok yönlerinin gerçek rotayla uyuşmaması,
- renk-körlüğünü göz ardı etmek,
- “accessible” = yalnız tekerlekli sandalye ikonu,
- tüm haritayı perspektif 3B yapmak,
- dekoratif font nedeniyle okunabilirliği kaybetmek,
- tabelayı yalnız iç mekân mockup dekoru gibi kullanmak,
- karar noktalarını analiz etmeden tabela yerleştirmek.

---

# 1382. `/lenticular-flip` — Lenticular İki Görsel Flip

## Trend

**T1/T2 — interactive print ve packaging alanında görünür.**

## Türkçe prompt

> [GÖRSEL A] ile [GÖRSEL B]'yi iki bakış açısında değişen gerçek lenticular flip baskı olarak tasarla.
>
> İki görüntünün ana kompozisyonu hizalı olsun.
>
> İzleyici sağa/sola hareket ettiğinde A → B geçişi okunabilsin.
>
> Hologram, iridescent foil veya screen animation gibi davranma.

## English

> Design [IMAGE A] and [IMAGE B] as a real two-state lenticular flip print.
>
> Keep the main composition aligned between states so the image changes from A to B as the viewer moves laterally.
>
> Do not treat it like holographic foil or a digital screen animation.

---

# 1383. `/lenticular-motion` — Lenticular Hareket Dizisi

## Türkçe

> Tek hareketin 4–8 aşamasını lenticular motion print için hizalı frame serisi olarak tasarla.
>
> Kamera sabit, özne konumu kontrollü ilerlesin.
>
> Çok karmaşık arka plan kullanma; hareket ilk bakışta okunabilsin.

## English

> Design 4–8 aligned frames of one movement for lenticular motion printing.
>
> Keep camera fixed and progress subject position in a controlled sequence.
>
> Avoid complex backgrounds so the movement reads immediately.

## Neye dikkat edilmeli?

Etkileşim tek dokunuşta anlaşılsın: soyma, katlama ve QR davranışı görselde tarif edilsin; çalışmayan etkileşim vaat edilmesin.

---
# 1384. `/lenticular-depth` — Lenticular Derinlik

## Türkçe

> [SAHNE]'yi 3–5 net derinlik düzlemine ayır:
>
> ön plan,
> orta ön,
> ana özne,
> arka plan,
> uzak fon.
>
> Lenticular depth illusion için her düzlem ayrı katman gibi çalışsın.
>
> Her nesneye farklı derinlik verme.

## English

> Separate [SCENE] into 3–5 clear depth planes for lenticular depth:
>
> foreground, near-middle, main subject, background, and distant background.
>
> Treat each as a coherent layer rather than assigning unique depth to every object.

## Neye dikkat edilmeli?

Etkileşim tek dokunuşta anlaşılsın: soyma, katlama ve QR davranışı görselde tarif edilsin; çalışmayan etkileşim vaat edilmesin.

---
# 1385. `/scratch-reveal` — Kazı-Kazan / Scratch Reveal

## Türkçe prompt

> [BASKI/KART]'ta tek bilgi veya görsel alanı scratch-off kaplama altında gizle.
>
> Kullanıcı kazıdığında:
>
> - sonuç,
> - küçük mesaj,
> - kod,
> - ikinci görsel
>
> açığa çıksın.
>
> Etkileşim gerçek amaç taşısın; rastgele her alanı scratch yapma.

## English

> Hide one meaningful information or image area beneath a scratch-off layer on [PRINT/CARD].
>
> Reveal a result, small message, code, or second visual when scratched.
>
> Give the interaction a real purpose rather than applying scratch coating everywhere.

## Neye dikkat edilmeli?

En uzak okuma mesafesinde test edin; ok-yazı-zemin kontrastı ve ok yönleri §21 mantığıyla tek tek izlenir.

---
# 1386. `/peel-reveal-print` — Katman Soyma Etkileşimi

## Türkçe

> [KART/AMBALAJ]'da üst kâğıt katmanının bir köşeden fiziksel olarak soyularak alttaki ikinci bilgi/görseli ortaya çıkardığı mekanizma tasarla.
>
> Peel tab ve katman sınırı anlaşılır olsun.
>
> Etkileşimi yalnız “sürpriz” için değil bilgi hiyerarşisi için kullan.

## English

> Design [CARD/PACKAGE] so one paper layer peels from a clear tab to reveal a second layer of information or imagery.
>
> Make the peel mechanism physically understandable.
>
> Use it to structure information rather than for surprise alone.

## Neye dikkat edilmeli?

Etkileşim tek dokunuşta anlaşılsın: soyma, katlama ve QR davranışı görselde tarif edilsin; çalışmayan etkileşim vaat edilmesin.

---
# 1387. `/punch-out-print` — Koparıp Kullanılan Baskı

## Türkçe

> [POSTER/KART/AMBALAJ]'ın bir bölümünü gerçek perforation/die-cut ile koparılıp kullanılabilir küçük nesneye dönüştür.
>
> Örneğin:
>
> - bookmark,
> - ticket,
> - tag,
> - mini card.
>
> Ana tasarım, parça çıkarıldığında da çalışmaya devam etsin.

## English

> Turn part of [POSTER/CARD/PACKAGE] into a removable functional object using real perforation or die-cutting, such as a bookmark, ticket, tag, or mini card.
>
> Keep the main design coherent after the piece is removed.

## Neye dikkat edilmeli?

Etkileşim tek dokunuşta anlaşılsın: soyma, katlama ve QR davranışı görselde tarif edilsin; çalışmayan etkileşim vaat edilmesin.

---
# 1388. `/fold-reveal` — Katlama ile İkinci Görsel

## Türkçe

> [PRINT] açıkken bir görsel/mesaj, belirli şekilde katlandığında ikinci bir görsel/mesaj oluşturacak şekilde tasarla.
>
> Kat çizgileri fiziksel ve baskı üretimine uygun olsun.
>
> İki durumu aynı anda aşırı bilgiyle doldurma.

## English

> Design [PRINT] so one visual or message appears when open and a second one appears after a specific physical fold.
>
> Keep fold lines realistic and manufacturable.
>
> Avoid overloading both states with excessive information.

## Neye dikkat edilmeli?

Etkileşim tek dokunuşta anlaşılsın: soyma, katlama ve QR davranışı görselde tarif edilsin; çalışmayan etkileşim vaat edilmesin.

---
# 1389. `/uv-reveal` — UV / Siyah Işıkla Gizli Katman

## Türkçe

> [POSTER/AMBALAJ]'da normal ışıkta sade ana tasarım göster; UV/blacklight altında yalnız ikinci küçük bilgi katmanı ortaya çıksın.
>
> UV katman ana tasarımın yerine geçmesin.
>
> Efekti gerçek özel mürekkep davranışı gibi kullan.

## English

> Keep [POSTER/PACKAGE] restrained under normal light and reveal only one secondary information layer under UV or blacklight.
>
> Do not let the UV layer replace the primary design.
>
> Treat the effect like real specialty-ink behavior.

## Neye dikkat edilmeli?

Etkileşim tek dokunuşta anlaşılsın: soyma, katlama ve QR davranışı görselde tarif edilsin; çalışmayan etkileşim vaat edilmesin.

---
# 1390. `/thermochromic-reveal` — Isıyla Değişen Baskı

## Türkçe

> [KART/AMBALAJ]'ın tek alanında thermochromic ink mantığı kullan. El sıcaklığı/ısı arttığında üst renk geçici olarak şeffaflaşarak alttaki küçük bilgi veya görseli açsın.
>
> Bütün tasarımı renk değiştiren gimmick'e dönüştürme.

## English

> Use thermochromic ink logic on one selected area of [CARD/PACKAGE]. Let hand warmth or heat temporarily reveal a small underlying message or image.
>
> Avoid turning the entire design into a color-changing gimmick.

## Neye dikkat edilmeli?

Etkileşim tek dokunuşta anlaşılsın: soyma, katlama ve QR davranışı görselde tarif edilsin; çalışmayan etkileşim vaat edilmesin.

---
# 1391. `/smart-print-qr` — İşlevsel QR Entegrasyonu

## Türkçe

> QR kodu dekoratif köşeye yapıştırmak yerine [BASKI/AMBALAJ] bilgi hiyerarşisinin gerçek parçası olarak yerleştir.
>
> QR çevresinde yeterli quiet zone bırak.
>
> Yanında kullanıcının tarayınca ne bulacağını açıkça yaz:
>
> “Ürün kaynağı”, “Kurulum videosu”, “Detaylı içerik” gibi.
>
> Gerçek QR üretimi ve testini görsel model yerine ayrı araçla yap.

## English

> Integrate a QR code into the real information hierarchy of [PRINT/PACKAGE] rather than treating it as corner decoration.
>
> Leave sufficient quiet zone and explain what the user will find after scanning, such as product origin, setup video, or detailed ingredients.
>
> Generate and test the actual QR using a dedicated tool rather than relying on image generation.

## Neye dikkat edilmeli?

Etkileşim tek dokunuşta anlaşılsın: soyma, katlama ve QR davranışı görselde tarif edilsin; çalışmayan etkileşim vaat edilmesin.

---
# 1392. `/nfc-touchpoint` — NFC Temas Noktası

## Türkçe

> [ÜRÜN/SERGİ/AMBALAJ]'da NFC temas bölgesini küçük ve anlaşılır fiziksel işaretle göster.
>
> Kullanıcının telefonu nereye yaklaştıracağını belli et.
>
> Büyük Wi-Fi dalgası veya futuristik hologram ikonları kullanma.

## English

> Mark the NFC touchpoint on [PRODUCT/EXHIBIT/PACKAGE] with a small clear physical cue showing where to place the phone.
>
> Avoid oversized wireless-wave graphics and futuristic hologram icons.

## Neye dikkat edilmeli?

Etkileşim tek dokunuşta anlaşılsın: soyma, katlama ve QR davranışı görselde tarif edilsin; çalışmayan etkileşim vaat edilmesin.

---
# 1393. `/interactive-print-slop-filter` — Etkileşimli Baskı AI Slop Filtresi

Kaçınılması gerekenler:

- her baskıya QR kod,
- etkileşim = gimmick,
- lenticular ile hologramı karıştırmak,
- mekanizmanın fiziksel olarak üretilememesi,
- scratch/peel alanının neden kullanıldığı belli olmaması,
- her yüzeyde foil + UV + emboss + varnish,
- kullanıcı hareketini hesaba katmamak,
- erişilebilirlik/okunabilirliği efekt uğruna bozmak.

---

# 1394. `/scrollytelling-sequence` — Scrollytelling Akışı

## Trend

**T1/T2 — 2026 veri hikâyesinde güçlü.**

## Türkçe prompt

> [KONU/VERİ]'yi 6–10 scroll adımına böl.
>
> Her adım yalnız bir yeni bilgi veya görsel değişiklik açsın.
>
> Kullanıcı ilerledikçe:
>
> - harita zoom,
> - veri highlight,
> - zaman ilerleme,
> - karşılaştırma,
> - annotation
>
> gibi tek değişken ortaya çıkabilir.
>
> İlk ekranda bütün grafikleri gösterme.

## English

> Divide [TOPIC/DATA] into a 6–10 step scrollytelling sequence.
>
> Reveal only one new idea or visual change at each step.
>
> As the reader scrolls, introduce a single change such as map zoom, data highlight, timeline progression, comparison, or annotation.
>
> Do not display the entire story on the first screen.

---

# 1395. `/scrolly-map` — Adım Adım Harita Hikâyesi

## Türkçe

> [COĞRAFİ HİKÂYE]'yi scroll boyunca ilerleyen harita anlatısına dönüştür.
>
> Her adımda:
>
> - aynı harita tabanı,
> - tek yeni konum/rota/katman,
> - kısa açıklama
>
> kullan.
>
> Harita her scroll'da tamamen başka projeksiyon veya tasarıma dönüşmesin.

## English

> Turn [GEOGRAPHIC STORY] into a scroll-driven map narrative.
>
> At each step preserve the same base map and introduce only one new location, route, or layer with a concise explanation.
>
> Do not change map projection or visual system between steps.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1396. `/scrolly-timeline` — Scroll ile İlerleyen Zaman Çizelgesi

## Türkçe

> [OLAY/DÖNEM]'ı yatay uzun timeline yerine scroll adımlarında ilerleyen zaman anlatısı yap.
>
> Her adım:
>
> - tarih,
> - tek olay,
> - bir görsel,
> - kısa bağlam
>
> içersin.
>
> Önceki olayların hafif bağlamı görünür kalsın.

## English

> Present [EVENT/PERIOD] as a scroll-driven timeline rather than one long static strip.
>
> Each step should contain one date, one event, one visual, and concise context.
>
> Keep enough of previous events visible to preserve continuity.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1397. `/scrolly-comparison` — Kademeli Karşılaştırma

## Türkçe

> [A] ve [B]'yi ilk ekranda tam karşılaştırmak yerine aşamalı göster.
>
> 1. ortak bağlam,
> 2. A,
> 3. B,
> 4. aynı ölçekte üst üste/yan yana,
> 5. ana fark.
>
> Ölçek ve veri eşlemesini adımlar boyunca sabit tut.

## English

> Compare [A] and [B] progressively instead of revealing the entire comparison at once:
>
> 1. shared context,
> 2. A,
> 3. B,
> 4. matched-scale overlay or side-by-side,
> 5. main difference.
>
> Keep scale and data mapping consistent across steps.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1398. `/progressive-annotation` — Annotation'ı Aşamalı Açma

## Türkçe

> Karmaşık grafik veya görsel üzerinde bütün açıklamaları aynı anda gösterme.
>
> Scroll/adım ilerledikçe yalnız ilgili annotation görünür olsun.
>
> Ana görsel sabit kalabilir; bilgi katmanı sırayla açılır.

## English

> Do not display every annotation on a complex figure at once.
>
> Reveal only the relevant annotation at each scroll or step.
>
> The primary visual may remain fixed while explanatory layers appear sequentially.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1399. `/sticky-visual-story` — Sabit Görsel + Değişen Metin

## Türkçe

> Ana görsel ekranın bir bölümünde sticky olarak sabit kalsın.
>
> Scroll boyunca yanında 4–8 kısa metin bölümü ilerlesin ve ana görselin yalnız ilgili katmanı değişsin/vurgulansın.
>
> Her adımda tamamen yeni görsel yükleme.

## English

> Keep one primary visual sticky in part of the viewport while 4–8 concise text sections scroll beside it.
>
> Change or highlight only the relevant visual layer at each step rather than replacing the entire graphic.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1400. `/scrolly-storyboard` — Scrollytelling Ön Taslak

## Türkçe

> [HİKÂYE]'nin uygulanmasından önce 8 karelik scrollytelling storyboard oluştur.
>
> Her karede:
>
> - kullanıcı ne görüyor,
> - ne değişiyor,
> - ana cümle,
> - etkileşim varsa ne olduğu
>
> belirtilsin.
>
> Bu çıktı final web tasarımı değil, anlatı planı olsun.

## English

> Create an eight-frame scrollytelling storyboard before implementation.
>
> For each frame specify what the reader sees, what changes, the primary sentence, and any interaction.
>
> Treat it as a narrative plan rather than final webpage design.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1401. `/scrolly-mobile` — Mobil Scrollytelling

## Türkçe

> Aynı scrollytelling hikâyesini mobil ekran için yeniden düzenle.
>
> Tek sütun, kısa metin, parmakla kaydırmaya uygun adım uzunluğu ve küçük ekranda okunabilir grafik kullan.
>
> Masaüstü sticky iki kolon düzenini yalnız küçültme.

## English

> Recompose the same scrollytelling story for mobile using one column, concise text, touch-friendly step length, and graphics readable on a small screen.
>
> Do not merely shrink a desktop sticky two-column layout.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1402. `/scrolly-slop-filter` — Scrollytelling AI Slop Filtresi

Kaçınılması gerekenler:

- her scroll'da yeni grafik,
- gereksiz animasyon,
- tüm veriyi baştan göstermek,
- scroll mesafesini uzatmak için boş adımlar,
- mobilde çalışmayan sticky layout,
- veri ölçeğinin adımlar arasında değişmesi,
- anlatı yerine “wow effect” amaçlı zoom,
- kullanıcının nerede olduğunu kaybettirmek.

---

# 1403. Yeni üst aile: `Navigation Visual`

Wayfinding, harita ve çevresel grafiklerden çıkan ortak aile:

> **Navigation Visual — kullanıcının “neredeyim, nereye gidiyorum, şimdi ne yapmalıyım?” sorularını görsel olarak cevaplayan sistem**

Aile:

- `/wayfinding-system`
- `/decision-point-sign`
- `/you-are-here-map`
- `/accessible-wayfinding`
- `/tactile-map`
- `/floor-identity`
- `/landmark-wayfinding`
- `/wayfinding-user-journey`

Temel formül:

> **user + location + decision + destination + cue + confirmation**

---

# 1404. Yeni üst aile: `Interactive Physical Visual`

Etkileşimli baskı ailesi:

- `/lenticular-flip`
- `/lenticular-motion`
- `/scratch-reveal`
- `/peel-reveal-print`
- `/punch-out-print`
- `/fold-reveal`
- `/uv-reveal`
- `/thermochromic-reveal`
- `/smart-print-qr`
- `/nfc-touchpoint`

Temel soru:

> **Kullanıcı ne yapıyor ve bu eylem neyi açığa çıkarıyor?**

---

# 1405. Yeni üst aile: `Progressive Disclosure Visual`

Scrollytelling ve eğitim görsellerinde ortak mantık:

> **Bilgiyi aynı anda değil, doğru sırayla göster.**

Aile:

- `/scrollytelling-sequence`
- `/scrolly-map`
- `/scrolly-timeline`
- `/scrolly-comparison`
- `/progressive-annotation`
- `/sticky-visual-story`
- `/observe-predict-explain`
- `/progressive-disclosure`

Bu aile özellikle:

- karmaşık süreç,
- veri hikâyesi,
- harita,
- timeline,
- öğretim,
- onboarding

için güçlüdür.

---

# 1406. `/interaction-before-style` — Etkileşimi Stilden Önce Yaz

## Türkçe

> Önce kullanıcı davranışını tarif et:
>
> - bakar,
> - çevirir,
> - söker,
> - kazır,
> - katlar,
> - tarar,
> - dokunur,
> - scroll eder.
>
> Sonra görsel stil ekle.
>
> Etkileşim mekanizması stilin içinde kaybolmasın.

## English

> Describe the user action first:
>
> look, tilt, peel, scratch, fold, scan, touch, or scroll.
>
> Add visual style afterward.
>
> Do not let the interaction mechanism disappear beneath decoration.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1407. `/real-world-distance` — Gerçek Görüş Mesafesi

## Wayfinding / poster / signage için

## Türkçe

> [TASARIM]'ın okunacağı gerçek mesafeyi belirt:
>
> - 30 cm,
> - 1 m,
> - 5 m,
> - 20 m.
>
> Tipografi, bilgi miktarı ve kontrast buna göre ayarlansın.
>
> Masaüstünde güzel görünen küçük yazıyı uzak tabela için kullanma.

## English

> Specify the real viewing distance for [DESIGN]:
>
> 30 cm, 1 m, 5 m, or 20 m.
>
> Adjust typography, information density, and contrast accordingly.
>
> Do not use desktop-scale typography on distant signage.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1408. `/real-world-use-test` — Gerçek Kullanım Testi Görseli

## Türkçe

> [TASARIM]'ı yalnız temiz mockup'ta değil gerçek kullanım anında test eden görsel oluştur.
>
> Örneğin:
>
> - tabela = yürüyen insan mesafesi,
> - ambalaj = raf,
> - ticket = elde,
> - map = kullanıcının yön bulduğu an,
> - UI = telefonda gerçek görev.
>
> Tasarımın anlaşılır olup olmadığını çevreyle birlikte değerlendir.

## English

> Show [DESIGN] being tested in real use rather than only in a clean mockup.
>
> For example:
>
> signage at walking distance,
> packaging on shelf,
> ticket in hand,
> map during navigation,
> UI during an actual task.
>
> Evaluate legibility and function within its context.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1409. `/system-not-artifact` — Tek Parça Değil Sistem

## Yeni kısa kural

> `/system-not-artifact`

## Türkçe

> Tek güzel çıktı üretmek yerine aynı tasarım mantığının farklı gerçek kullanım noktalarında nasıl davrandığını göster.
>
> Kurallar sabit, uygulama formatları farklı olsun.

## English

> Show how one design logic behaves across multiple real use cases rather than producing one isolated beautiful artifact.
>
> Keep rules consistent while adapting to different formats.

## Neye dikkat edilmeli?

Her adım tek fikir taşısın; sabit görsel değişen metinle çelişirse adım bölünür.

---
# 1410. Bu turdaki slash-style indeks (aile-018)

| Kısayol | Aile |
|---|---|
| `/wayfinding-system` | complete navigation system |
| `/decision-point-sign` | sign for an actual decision point |
| `/you-are-here-map` | orientation map |
| `/accessible-wayfinding` | accessibility-first navigation |
| `/tactile-map` | touch-readable map |
| `/floor-identity` | floor/zone identity |
| `/landmark-wayfinding` | navigation through landmarks |
| `/environmental-graphic-wall` | environmental graphic installation |
| `/placemaking-signage` | place-derived signage |
| `/signage-family-board` | complete sign family |
| `/signage-placement-review` | placement/visibility audit |
| `/multisensory-wayfinding` | multisensory navigation |
| `/wayfinding-user-journey` | navigation journey |
| `/lenticular-flip` | two-state angle-changing print |
| `/lenticular-motion` | lenticular motion sequence |
| `/lenticular-depth` | lenticular depth planes |
| `/scratch-reveal` | scratch-off interaction |
| `/peel-reveal-print` | peel-layer interaction |
| `/punch-out-print` | removable functional print |
| `/fold-reveal` | fold-based reveal |
| `/uv-reveal` | UV-visible second layer |
| `/thermochromic-reveal` | heat-reactive print |
| `/smart-print-qr` | functional QR integration |
| `/nfc-touchpoint` | NFC interaction cue |
| `/scrollytelling-sequence` | staged scroll narrative |
| `/scrolly-map` | map-based scrollytelling |
| `/scrolly-timeline` | scroll timeline |
| `/scrolly-comparison` | progressive comparison |
| `/progressive-annotation` | annotation by step |
| `/sticky-visual-story` | sticky graphic narrative |
| `/scrolly-storyboard` | scrollytelling plan |
| `/scrolly-mobile` | mobile-first scroll story |
| `/interaction-before-style` | define action before aesthetic |
| `/real-world-distance` | viewing-distance-aware design |
| `/real-world-use-test` | contextual use test |
| `/system-not-artifact` | design system over single artifact |

---

<a id="aile-019"></a>
# AR, Mekânsal Grafik, Motion Poster ve Değişken Kimlik Sistemleri — 2026 Ek Taraması

2026 araştırmalarında dört yeni alan görsel prompt rehberi için ayrı aileler oluşturacak kadar belirginleşiyor:

- **Augmented Reality / WebAR ile fiziksel-dijital geçiş**
- **Projection mapping ve yüzeye bağlı mekânsal grafik**
- **Motion poster / kinetic typography**
- **Değişken veri ve kişiselleştirilmiş kimlik/ambalaj sistemleri**

Bunların ortak noktası şudur:

> **Görsel artık tek sabit yüzey değildir.**

Bir ambalaj tarandığında değişebilir, bir duvar gerçek geometrisine göre ışıkla yeniden çizilebilir, bir logo harekette davranış gösterebilir, bir poster kişiye göre veri değiştirebilir.

Bu yüzden statik görüntü promptlarından farklı olarak burada yalnız görünüş değil:

> **trigger + state + transition + surface + user action + fallback**

tanımlanmalıdır.

---

# 1411. `/ar-packaging` — AR Destekli Ambalaj

## Trend

**T1/T2 — 2026'da food packaging ve smart packaging araştırmalarında belirgin.**

AR ambalajın amacı yalnız paketten “3B şey çıkarmak” değildir.

2026 araştırmaları AR ambalaj kullanımını kabaca üç işleve ayırıyor:

- bilgi aktarımı,
- etkileşim/oyun,
- işlevsel uzantı.

## Türkçe prompt

> [ÜRÜN] için fiziksel ambalaj + WebAR deneyimi tasarla.
>
> Ambalajın kendisi tarama olmadan da:
>
> - ürün adı,
> - temel bilgi,
> - kullanım,
> - zorunlu bilgi
>
> açısından çalışır durumda olsun.
>
> AR yalnız ikincil bir katman açsın:
>
> - ürün kaynağı,
> - 3B kullanım gösterimi,
> - kısa hikâye,
> - etkileşimli içerik
>
> gibi.
>
> Telefon ekranından rastgele hologram karakter çıkarmayı varsayma.
>
> AR trigger alanı açık ama ambalajın ana görselini bozmayacak kadar sade olsun.

## English

> Design physical packaging plus a WebAR layer for [PRODUCT].
>
> The package must remain fully functional without scanning, carrying the product name, essential information, usage, and required details.
>
> Let AR add only a secondary layer such as provenance, 3D usage explanation, short story, or interactive content.
>
> Do not default to random holographic characters emerging from the phone.
>
> Keep the AR trigger clear but visually secondary.

---

# 1412. `/ar-info-layer` — AR Bilgi Katmanı

## Türkçe

> Fiziksel [NESNE/AMBALAJ/ESER] tarandığında ana nesnenin çevresinde yalnız 3–5 kısa bilgi katmanı göster.
>
> Bilgiler gerçek nesneye mekânsal olarak bağlansın.
>
> Kullanıcı nesneyi hâlâ görebilsin.
>
> Ekranı tooltip, ikon ve floating card ile doldurma.

## English

> When scanning the physical [OBJECT/PACKAGE/ARTIFACT], reveal only 3–5 concise information layers spatially anchored to the real object.
>
> Keep the physical object visible.
>
> Avoid covering the screen in tooltips, icons, and floating cards.

## Neye dikkat edilmeli?

AR katmanı gerçek mekâna otursun: ölçek, ışık ve sabitleme noktası belirtilsin; AR'sız yedek sürüm her zaman hazır olsun.

---
# 1413. `/ar-instruction` — AR Kurulum / Kullanım Talimatı

## Türkçe

> [ÜRÜN/CİHAZ]'ın gerçek görüntüsü üzerinde yalnız sıradaki fiziksel adımı AR overlay ile göster.
>
> Örneğin:
>
> - hangi parçaya dokunulacak,
> - hangi vida çıkarılacak,
> - hangi yönde döndürülecek,
> - parçanın nereye takılacağı.
>
> Her adımı aynı anda gösterme.
>
> Overlay gerçek parçaya doğru hizalansın.

## English

> Overlay only the next physical instruction step on the real [PRODUCT/DEVICE].
>
> Show which part to touch, remove, rotate, or install and where it goes.
>
> Do not display all steps simultaneously.
>
> Keep the overlay precisely aligned to the real component.

## Neye dikkat edilmeli?

AR katmanı gerçek mekâna otursun: ölçek, ışık ve sabitleme noktası belirtilsin; AR'sız yedek sürüm her zaman hazır olsun.

---
# 1414. `/ar-assembly` — AR Montaj Rehberi

## Türkçe

> [ÜRÜN]'ün montajını 5–8 AR adımına ayır.
>
> Her adımda yalnız:
>
> - aktif parça,
> - yön oku,
> - bağlantı noktası,
> - tek kısa talimat
>
> görünsün.
>
> Tamamlanan parçaları düşük vurguda bırak.
>
> Exploded view ile gerçek montaj sırasını karıştırma.

## English

> Divide [PRODUCT] assembly into 5–8 AR steps.
>
> At each step show only the active component, movement direction, connection point, and one concise instruction.
>
> Keep completed components de-emphasized.
>
> Do not confuse exploded-view separation with actual assembly sequence.

## Neye dikkat edilmeli?

AR katmanı gerçek mekâna otursun: ölçek, ışık ve sabitleme noktası belirtilsin; AR'sız yedek sürüm her zaman hazır olsun.

---
# 1415. `/ar-try-in-space` — Nesneyi Gerçek Mekânda Önizleme

## Kullanım

Mobilya, sanat eseri, cihaz, aydınlatma vb.

## Türkçe

> [ÜRÜN]'ü gerçek oda görüntüsüne gerçek fiziksel ölçekte yerleştirilmiş AR preview olarak göster.
>
> Zemin teması, perspektif, gölge ve boyut gerçek mekânla uyumlu olsun.
>
> Ürünü odaya sığdırmak için sessizce küçültme.
>
> Ölçek gerekiyorsa kullanıcıya gerçek ölçüyü ayrıca göster.

## English

> Show [PRODUCT] as an AR preview placed at real scale in the user's actual room.
>
> Match floor contact, perspective, shadows, and physical dimensions.
>
> Do not silently shrink the product to make it fit.
>
> Display real dimensions when relevant.

## Neye dikkat edilmeli?

AR katmanı gerçek mekâna otursun: ölçek, ışık ve sabitleme noktası belirtilsin; AR'sız yedek sürüm her zaman hazır olsun.

---
# 1416. `/ar-before-buy` — Satın Almadan Önce AR Karşılaştırması

## Türkçe

> Aynı mekânda [A/B/C] üç ürün seçeneğini sırayla gerçek ölçekle göster.
>
> Kamera, oda ve ışık değişmesin.
>
> Kullanıcı yalnız:
>
> - boyut,
> - renk,
> - form,
> - mekânsal uyum
>
> farklarını karşılaştırsın.
>
> Bir seçeneği daha iyi göstermek için ışığı değiştirip manipüle etme.

## English

> Preview options A/B/C sequentially at real scale in the same room.
>
> Keep camera, room, and lighting identical.
>
> Let the user compare only size, color, form, and spatial fit.
>
> Do not manipulate lighting to favor one option.

## Neye dikkat edilmeli?

AR katmanı gerçek mekâna otursun: ölçek, ışık ve sabitleme noktası belirtilsin; AR'sız yedek sürüm her zaman hazır olsun.

---
# 1417. `/ar-art-overlay` — Kamusal Sanat AR Katmanı

## Trend

**T2 — 2026 Scientific Reports çalışmaları AR'ın kamusal sanatta spatial storytelling için kullanımını inceliyor.**

## Türkçe

> [KAMUSAL ESER/DUVAR/MEKÂN] üzerine AR katmanı tasarla.
>
> Dijital katman fiziksel eseri yok etmesin; onunla ilişki kursun.
>
> Kullanıcı hareket ettikçe:
>
> - farklı detay,
> - geçmiş/gelecek katmanı,
> - ses/görsel bağlam,
> - kısa anlatı
>
> açılabilir.
>
> AR içeriğini fiziksel eserin önünde ayrı bir 3B reklam objesi gibi yüzdürme.

## English

> Design an AR layer for [PUBLIC ART/WALL/PLACE] that extends rather than replaces the physical work.
>
> As the user moves, reveal contextual detail, past/future layers, audiovisual interpretation, or concise storytelling.
>
> Avoid floating unrelated 3D advertising objects in front of the artwork.

---

# 1418. `/ar-museum-object` — Müze Eseri AR Katmanı

## Türkçe

> [ESER]'in gerçek vitrindeki görünümünü koru.
>
> AR'da yalnız kullanıcı istediğinde:
>
> - 360° görünüm,
> - eksik parça rekonstrüksiyonu,
> - kullanım biçimi,
> - dönem bağlamı
>
> açılabilsin.
>
> Rekonstrüksiyon spekülatifse bunu görsel olarak ayır.

## English

> Preserve the real museum object in its display.
>
> Reveal optional AR layers such as a 360° view, reconstruction of missing elements, use context, or historical environment only on demand.
>
> Visually distinguish speculative reconstruction when evidence is incomplete.

## Neye dikkat edilmeli?

AR katmanı gerçek mekâna otursun: ölçek, ışık ve sabitleme noktası belirtilsin; AR'sız yedek sürüm her zaman hazır olsun.

---
# 1419. `/ar-wayfinding` — AR Yönlendirme

## Türkçe

> [MEKÂN] içinde AR yönlendirmeyi fiziksel wayfinding'e destek olarak kullan.
>
> Ekranda yalnız:
>
> - sıradaki dönüş,
> - hedef mesafesi,
> - landmark
>
> göster.
>
> Sürekli yerde dev ok döşeme.
>
> Fiziksel signage yoksa AR'ı tek navigasyon sistemi olarak varsayma.

## English

> Use AR navigation as a supplement to physical wayfinding in [SPACE].
>
> Show only the next turn, distance, and relevant landmark.
>
> Avoid covering the floor with giant arrows.
>
> Do not assume AR should replace physical signage entirely.

## Neye dikkat edilmeli?

AR katmanı gerçek mekâna otursun: ölçek, ışık ve sabitleme noktası belirtilsin; AR'sız yedek sürüm her zaman hazır olsun.

---
# 1420. `/ar-fallback` — AR Olmadan Çalışan Sürüm

## Yeni kontrol kuralı

AR deneyimlerinde her zaman sorulmalı:

> Telefon çalışmazsa ne olur?

## Türkçe

> AR kullanılamadığında aynı temel bilgiyi sağlayan non-AR fallback tasarla:
>
> kısa URL,
> basılı diagram,
> standart harita,
> kısa kullanım talimatı
>
> gibi.
>
> Kritik bilgiyi yalnız AR içine gömme.

## English

> Provide a non-AR fallback carrying the same essential information, such as a short URL, printed diagram, standard map, or concise instructions.
>
> Do not hide critical information exclusively inside AR.

## Neye dikkat edilmeli?

AR katmanı gerçek mekâna otursun: ölçek, ışık ve sabitleme noktası belirtilsin; AR'sız yedek sürüm her zaman hazır olsun.

---
# 1421. `/ar-slop-filter` — AR Görsel AI Slop Filtresi

Kaçınılması gerekenler:

- hologram insan,
- floating glass card,
- her yüzeyde neon outline,
- dijital katmanın fiziksel nesneyi kapatması,
- gerçek scale'in unutulması,
- AR trigger'ın ne olduğu belli olmaması,
- her bilgi için 3B ikon,
- erişilebilirlik ve fallback düşünmemek,
- fiziksel ışık/perspektifle uyumsuz overlay.

---

# 1422. `/projection-map-facade` — Cephe Projection Mapping

## Trend

**T1/T2 — projection mapping hâlâ güçlü, 2026 araştırmaları masadan kamusal alana kadar kullanımını inceliyor.**

## Türkçe prompt

> [BİNA CEPHESİ]'ni projection mapping için fiziksel yüzey olarak kullan.
>
> İçerik cephe geometrisine bağlansın:
>
> - pencere,
> - kolon,
> - kemer,
> - çıkıntı,
> - boşluk
>
> gibi gerçek yapısal elemanlarla çalışsın.
>
> Cepheyi düz sinema perdesi gibi kullanma.
>
> Animasyon içerik gerekiyorsa mimari formun açılması, katmanlanması veya ritmiyle ilişki kursun.

## English

> Use [BUILDING FACADE] as the physical surface for projection mapping.
>
> Anchor content to real architectural elements such as windows, columns, arches, projections, and voids.
>
> Do not treat the facade as a flat cinema screen.
>
> Let motion respond to architectural structure.

---

# 1423. `/projection-map-table` — Masaüstü Projection Mapping

## Türkçe

> Fiziksel masa üzerindeki [HARİTA/MAKET/NESNE]'ye projection mapping uygula.
>
> Projeksiyon gerçek yüzey sınırlarına ve yüksekliklerine uysun.
>
> Kullanıcı eli/nesnesi yüzeye girdiğinde kritik bilgiyi tamamen kaybetmeyecek tasarım düşün.
>
> Projeksiyonu masadan taşan hologram gibi gösterme.

## English

> Apply projection mapping to a physical tabletop [MAP/MODEL/OBJECT].
>
> Align projection to real boundaries and height changes.
>
> Design so temporary hand or object occlusion does not destroy all critical information.
>
> Avoid holographic content floating above the table.

## Neye dikkat edilmeli?

Projeksiyon yüzeyi ve izleyici konumu sabitlensin; kalibrasyon karesi olmadan mapping vaadi verilmesin.

---
# 1424. `/projection-map-model` — Mimari Maket Üzerinde Projeksiyon

## Türkçe

> Beyaz fiziksel mimari maket üzerine:
>
> - program,
> - güneş,
> - dolaşım,
> - kullanım,
> - zaman
>
> katmanlarından yalnız birini projection mapping ile göster.
>
> Maketin geometrisi değişmesin.
>
> Veri yüzeye doğru hizalansın.

## English

> Project one information layer such as program, sunlight, circulation, use, or time onto a physical white architectural model.
>
> Preserve model geometry and align data precisely to the physical surfaces.

## Neye dikkat edilmeli?

Projeksiyon yüzeyi ve izleyici konumu sabitlensin; kalibrasyon karesi olmadan mapping vaadi verilmesin.

---
# 1425. `/projection-map-object` — Ürün / Nesne Üzerine Mapping

## Türkçe

> [NESNE]'nin gerçek hacmini projection surface olarak kullan.
>
> Grafik/animasyon nesnenin:
>
> - kenar,
> - oyuk,
> - yüzey,
> - hareket
>
> özellikleriyle ilişki kursun.
>
> Nesnenin önüne bağımsız video oynatma.

## English

> Use the real volume of [OBJECT] as a projection surface.
>
> Make graphics or motion respond to its edges, recesses, surfaces, and movement.
>
> Do not simply play an unrelated video in front of the object.

## Neye dikkat edilmeli?

Projeksiyon yüzeyi ve izleyici konumu sabitlensin; kalibrasyon karesi olmadan mapping vaadi verilmesin.

---
# 1426. `/projection-story-sequence` — Mapping Hikâye Dizisi

## Türkçe

> Projection mapping hikâyesini 6 sahnelik storyboard olarak planla.
>
> Her sahne:
>
> - fiziksel yüzey,
> - ana değişim,
> - ışık durumu,
> - süre
>
> içersin.
>
> Her sahneyi tamamen başka görsel stile çevirmeden tek anlatı akışı koru.

## English

> Plan a projection-mapping story as a six-scene storyboard.
>
> Define physical surface, primary visual change, lighting state, and duration for each scene.
>
> Preserve one coherent visual narrative rather than switching styles every scene.

## Neye dikkat edilmeli?

Projeksiyon yüzeyi ve izleyici konumu sabitlensin; kalibrasyon karesi olmadan mapping vaadi verilmesin.

---
# 1427. `/projection-calibration-view` — Kalibrasyon Görünümü

## Türkçe

> Projection mapping hazırlığı için dekoratif final değil calibration view oluştur.
>
> Yüzey köşeleri, grid, maske sınırları ve önemli fiziksel referans noktaları açıkça görünsün.
>
> Bu çıktı show artwork değil teknik hazırlık sayfası olsun.

## English

> Create a projection-mapping calibration view rather than final show artwork.
>
> Show surface corners, grid, mask boundaries, and key physical reference points clearly.
>
> Treat it as a technical setup page.

## Neye dikkat edilmeli?

Projeksiyon yüzeyi ve izleyici konumu sabitlensin; kalibrasyon karesi olmadan mapping vaadi verilmesin.

---
# 1428. `/projection-slop-filter` — Projection Mapping AI Slop Filtresi

Kaçınılması gerekenler:

- düz yüzeye video projekte etmek = mapping sanmak,
- ışığın fiziksel yüzeye uymaması,
- bina geometrisini ihmal etmek,
- hologramlaştırmak,
- aşırı partikül/ışık patlaması,
- hikâye yerine demo reel efektleri,
- projection brightness/ambient light ilişkisini düşünmemek.

---

# 1429. `/motion-poster` — Hareketli Afiş

## Trend

**T1/T2 — 2026'da akademik tasarım literatüründe de ayrı bir alan olarak inceleniyor.**

Motion poster:

> video klip değildir.

Statik posterin:

- hiyerarşi,
- tipografi,
- ana görsel,
- mesaj

yapısını koruyarak **zamanda davranmasıdır**.

## Türkçe prompt

> [ETKİNLİK/KONU] için 6–10 saniyelik loop motion poster tasarla.
>
> İlk ve son kare birbirine bağlanabilsin.
>
> Hareket yalnız 1–2 ana öğede olsun:
>
> - başlık,
> - ana form,
> - fotoğraf crop'u,
> - tek pattern
>
> gibi.
>
> Her şeyi aynı anda hareket ettirme.
>
> Poster 1 saniyede durdurulduğunda da okunabilir kompozisyon taşısın.

## English

> Design a 6–10 second looping motion poster for [EVENT/TOPIC].
>
> Make the first and last frames connect naturally.
>
> Animate only 1–2 primary elements such as the title, main form, image crop, or one pattern.
>
> Do not animate everything simultaneously.
>
> Any paused frame should still preserve readable poster hierarchy.

---

# 1430. `/motion-poster-loop` — Kusursuz Loop Mantığı

## Türkçe

> Hareket başlangıç ve bitiş durumunu eşleştirsin.
>
> Loop reset noktası gözle görünür sıçrama yapmasın.
>
> Hareket döngüsü anlamlı bir ritme sahip olsun; yalnız sonsuz rotate kullanma.

## English

> Match beginning and ending states so the loop does not visibly jump.
>
> Build a meaningful rhythm rather than relying on endless rotation.

## Neye dikkat edilmeli?

Loop noktası görünmez olsun; tipografi hareketi okunabilirliği bozuyorsa hız düşürülür (§1464).

---
# 1431. `/motion-poster-type` — Tipografi Hareketli Afiş

## Türkçe

> Poster içinde hareketi yalnız tipografiden üret.
>
> Kelime/başlık:
>
> - weight,
> - width,
> - tracking,
> - baseline,
> - mask reveal
>
> gibi bir veya iki özellik üzerinden değişsin.
>
> Harfleri rastgele zıplatma.

## English

> Generate motion in the poster through typography alone.
>
> Animate one or two properties such as weight, width, tracking, baseline, or mask reveal.
>
> Avoid random bouncing letters.

## Neye dikkat edilmeli?

Loop noktası görünmez olsun; tipografi hareketi okunabilirliği bozuyorsa hız düşürülür (§1464).

---
# 1432. `/variable-font-motion` — Variable Font Hareketi

## Trend

Adobe After Effects 26.0 ile variable font eksenlerinin motion typography içinde doğrudan keyframe/expression ile animasyonu daha görünür hâle geldi.

## Türkçe prompt

> Aynı kelimenin variable font:
>
> - weight,
> - width,
> - slant
>
> eksenlerinden yalnız birini 3–5 saniyelik kontrollü hareket boyunca değiştir.
>
> Glyph kimliği korunmalı.
>
> Aynı anda bütün eksenleri değiştirip okunabilirliği kaybetme.

## English

> Animate only one variable-font axis—weight, width, or slant—across a controlled 3–5 second motion.
>
> Preserve glyph identity.
>
> Avoid animating every axis simultaneously until readability collapses.

---

# 1433. `/kinetic-headline` — Kinetik Başlık

## Türkçe

> [KISA BAŞLIK]'ı videonun ana hareket öğesi yap.
>
> Metnin ritmi:
>
> - konuşma,
> - müzik,
> - kesme,
> - vurgu
>
> ile ilişkili olsun.
>
> Her kelimeye ayrı animasyon efekti verme.

## English

> Make [SHORT HEADLINE] the main motion element.
>
> Tie its rhythm to speech, music, cuts, or emphasis.
>
> Do not assign a different animation effect to every word.

## Neye dikkat edilmeli?

Loop noktası görünmez olsun; tipografi hareketi okunabilirliği bozuyorsa hız düşürülür (§1464).

---
# 1434. `/type-on-beat` — Müziğe Senkron Tipografi

## Türkçe

> [METİN]'i müzik ritmine göre zamanla.
>
> Her beat'te zorunlu hareket yerine yalnız önemli ritmik vurgularda:
>
> - scale,
> - weight,
> - appearance,
> - cut
>
> değişsin.

## English

> Time [TEXT] to the music rhythm, but animate only meaningful beats through scale, weight, appearance, or cut.
>
> Do not force movement on every beat.

## Neye dikkat edilmeli?

Loop noktası görünmez olsun; tipografi hareketi okunabilirliği bozuyorsa hız düşürülür (§1464).

---
# 1435. `/type-scroll-reveal` — Scroll ile Kinetik Tipografi

## Türkçe

> Scroll ilerledikçe başlığın harfleri sırayla veya variable font ekseni boyunca değişsin.
>
> Hareket kullanıcının scroll miktarıyla doğrudan ilişkili olsun.
>
> Auto-play video gibi bağımsız hareket etmesin.

## English

> Let the headline reveal or transform along a variable-font axis in direct response to scroll progress.
>
> Make motion scroll-driven rather than behaving like an autoplay video.

## Neye dikkat edilmeli?

Loop noktası görünmez olsun; tipografi hareketi okunabilirliği bozuyorsa hız düşürülür (§1464).

---
# 1436. `/motion-grid` — Grid'in Hareket Etmesi

## Türkçe

> Sabit poster gridini bozmak yerine grid kolonlarının genişliği veya panel oranlarını kontrollü biçimde hareket ettir.
>
> İçerik yeni gride uyum sağlasın.
>
> Grid değişirken metin overlap/okunmaz hâle gelmesin.

## English

> Animate grid column widths or panel proportions in a controlled way rather than arbitrarily breaking the grid.
>
> Let content adapt while preserving readability.

## Neye dikkat edilmeli?

Loop noktası görünmez olsun; tipografi hareketi okunabilirliği bozuyorsa hız düşürülür (§1464).

---
# 1437. `/motion-collage` — Hareketli Kolaj

## Türkçe

> 3–5 fiziksel/dijital kolaj katmanını farklı derinlik ve hızlarda hareket ettir.
>
> Hareket paper-layer/parallax mantığı taşısın.
>
> Her katmanı bağımsız 3B objeye dönüştürme.

## English

> Animate 3–5 collage layers at different depths and speeds using paper-layer or restrained parallax logic.
>
> Avoid turning every layer into an independent 3D object.

## Neye dikkat edilmeli?

Loop noktası görünmez olsun; tipografi hareketi okunabilirliği bozuyorsa hız düşürülür (§1464).

---
# 1438. `/motion-poster-slop-filter` — Motion Poster AI Slop Filtresi

Kaçınılması gerekenler:

- her elemanın hareket etmesi,
- sürekli zoom,
- random glitch,
- her harfin bounce yapması,
- neon trails,
- particle explosion,
- okunamayan kinetic type,
- loop noktasında sıçrama,
- motion design = transition pack,
- hareketin mesaja hiçbir katkı sağlamaması.

---

# 1439. `/dynamic-logo` — Hareketli Logo Sistemi

## Trend

**T1/T2 — multisensory/adaptive brand systems 2026'da güçlü.**

## Türkçe prompt

> [MARKA] logosunun sabit ana formunu koruyan 3–5 saniyelik motion behavior tanımla.
>
> Logo:
>
> - açılabilir,
> - sıkışabilir,
> - segmentlere ayrılabilir,
> - tek eksende morph edebilir.
>
> Ancak sonunda her zaman aynı tanınabilir core mark'a dönsün.
>
> Logoyu her animasyonda başka sembole dönüştürme.

## English

> Define a 3–5 second motion behavior for [BRAND] while preserving the core logo form.
>
> It may expand, compress, segment, or morph along one controlled axis, but should always resolve to the same recognizable mark.
>
> Do not transform it into an unrelated symbol each time.

---

# 1440. `/logo-motion-principles` — Logo Hareket Kuralları

## Türkçe

> Logo animation için yalnız 3 hareket kuralı belirle:
>
> 1. giriş,
> 2. dönüşüm,
> 3. çıkış.
>
> Bu kurallar farklı platformlarda tekrar kullanılabilsin.
>
> Tek seferlik showreel animasyonu değil sistem davranışı üret.

## English

> Define only three reusable motion rules for the logo:
>
> 1. entrance,
> 2. transformation,
> 3. exit.
>
> Make them reusable across platforms rather than designing one showreel-only animation.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1441. `/responsive-motion-logo` — Ekran Boyutuna Göre Hareket

## Türkçe

> Logo motion systemini büyük ekran, mobil ve küçük icon için üç seviyede tanımla.
>
> Büyük ekranda tam hareket; mobilde kısa hareket; küçük icon'da tek micro-motion kullan.
>
> Her yerde aynı uzun animasyonu oynatma.

## English

> Define three motion levels for large display, mobile, and small icon:
>
> full motion on large screens, shortened motion on mobile, and one micro-motion for small icons.
>
> Do not play the same long animation everywhere.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1442. `/living-identity` — Yaşayan Görsel Kimlik

## Trend

**T1/T2 — 2026'da static logo yerine davranış sistemi yaklaşımı güçleniyor.**

## Türkçe

> [MARKA]'nın kimliğini tek sabit grafik yerine davranış kurallarıyla tanımla.
>
> Değişebilecek:
>
> - pattern,
> - crop,
> - renk sırası,
> - hareket,
> - data-driven element.
>
> Değişmeyecek:
>
> - ana logo,
> - tipografi karakteri,
> - temel oran,
> - grid mantığı.
>
> Değişkenliği tutarsızlığa dönüştürme.

## English

> Define [BRAND] as a living identity with controlled behavior rather than one frozen graphic.
>
> Allow pattern, crop, color order, motion, or data-driven elements to vary while keeping the core logo, typography character, key proportions, and grid logic fixed.
>
> Do not confuse variability with inconsistency.

---

# 1443. `/generative-pattern-system` — Üretken Pattern Sistemi

## Türkçe

> [MARKA/KONU] için kurala bağlı generative pattern tasarla.
>
> Pattern:
>
> - 2–4 temel modül,
> - sabit spacing/aralık kuralı,
> - sınırlı rotation/scale,
> - belirli renk paleti
>
> ile üretilebilsin.
>
> Her çıktıda rastgele tamamen farklı şekiller oluşturma.

## English

> Build a rule-based generative pattern system for [BRAND/TOPIC].
>
> Use 2–4 base modules, fixed spacing logic, restrained rotation or scale variation, and a limited palette.
>
> Avoid generating completely unrelated shapes in every output.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1444. `/data-driven-identity` — Veriye Göre Değişen Kimlik

## Türkçe

> [VERİ KAYNAĞI]'nı marka görsel sisteminde tek bir değişkeni kontrol etmek için kullan.
>
> Örneğin:
>
> - hava → pattern yoğunluğu,
> - saat → renk sıcaklığı,
> - konum → line orientation,
> - kullanıcı grubu → layout variation.
>
> Veri değiştiğinde markanın core kimliği korunmalı.
>
> Aynı veriyi 5 farklı görsel özellikte tekrar kodlama.

## English

> Use [DATA SOURCE] to control one visual variable in the brand system, such as weather controlling pattern density, time controlling color temperature, location controlling line orientation, or audience segment controlling layout variation.
>
> Preserve core identity as data changes.
>
> Do not encode the same variable redundantly across many visual properties.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1445. `/personalized-pack` — Kişiselleştirilmiş Ambalaj

## Trend

**T1 — digital print'in variable data avantajlarıyla kalıcı.**

## Türkçe prompt

> [ÜRÜN] ambalajında ana marka sistemi sabit kalsın; yalnız tek kişiselleştirme alanı değişsin:
>
> - isim,
> - kısa mesaj,
> - şehir,
> - numara,
> - pattern varyantı.
>
> Kişiselleştirme marka/ürün bilgisini bastırmasın.
>
> Her kişiye tamamen farklı ambalaj tasarlama.

## English

> Keep the core [PRODUCT] packaging system fixed and vary only one personalization field such as name, short message, city, number, or pattern variant.
>
> Do not let personalization overpower brand and product information.
>
> Avoid designing an entirely different package for every person.

---

# 1446. `/variable-data-poster` — Değişken Veri Posteri

## Türkçe

> Aynı etkinlik/kampanya için [N] poster varyantı oluştur.
>
> Değişken:
>
> - tarih,
> - konum,
> - isim,
> - sayı,
> - kısa veri
>
> olabilir.
>
> Grid ve ana marka dili sabit kalsın.
>
> Variable data'yı yalnız farklı renk yapmakla sınırlama.

## English

> Create [N] poster variants for one event or campaign.
>
> Let date, location, name, number, or a concise data field vary while preserving the core grid and brand language.
>
> Do not reduce variable-data design to color swaps alone.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1447. `/serial-unique-pack` — Her Paket Benzersiz, Sistem Aynı

## Türkçe

> [ÜRÜN] için her bir pakette küçük benzersiz generative pattern varyasyonu üret.
>
> Logo, ürün adı, bilgi hiyerarşisi ve ana palet aynı kalsın.
>
> Varyasyon yalnız background/pattern sisteminde olsun.
>
> Koleksiyon bir arada görüldüğünde aynı marka ailesi olarak okunmalı.

## English

> Give every [PRODUCT] package a small unique generative-pattern variation while keeping logo, product name, information hierarchy, and primary palette fixed.
>
> Restrict variation to the background or pattern system.
>
> The full collection should still read clearly as one brand family.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1448. `/city-personalized-poster` — Şehre Göre Değişen Kampanya

## Türkçe

> Aynı kampanyayı [ŞEHİRLER] için yerel varyantlara dönüştür.
>
> Ana slogan, logo ve grid sabit kalsın.
>
> Yalnız gerçek yerel:
>
> - landmark,
> - renk/ulaşım işareti,
> - mahalle/yer adı,
> - gündelik obje
>
> gibi 1–2 unsur değişsin.
>
> Şehri turistik klişe ikon setine indirgeme.

## English

> Adapt the same campaign to [CITIES] while keeping slogan, logo, and grid fixed.
>
> Change only 1–2 real local cues such as landmark, transit sign, neighborhood name, or everyday object.
>
> Avoid reducing each city to a generic tourist-icon set.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1449. `/personalization-slop-filter` — Kişiselleştirme AI Slop Filtresi

Kaçınılması gerekenler:

- kişiselleştirme = yalnız isim,
- her varyantta marka düzeninin değişmesi,
- şehir = landmark sticker,
- veri = gradient rengi,
- her paketi tamamen benzersiz yapıp seri kimliğini kaybetmek,
- variable data'yı yanlış/uydurma üretmek,
- isimleri görsel modelin yanlış yazması.

---

# 1450. `/spatial-brand-zone` — Mekânda Marka Bölgesi

## Trend

**T1/T2 — SEGD 2026 branded environments / omnispatial design.**

## Türkçe prompt

> [MARKA]'yı fiziksel [MEKÂN]'da yalnız logo tekrarıyla değil:
>
> - malzeme,
> - ışık,
> - signage,
> - grafik yüzey,
> - ses/etkileşim
>
> arasından 2–4 araçla mekânsal olarak ifade et.
>
> Marka rengiyle bütün duvarları boyama.
>
> Ziyaretçi girdiğinde marka hissi logo okumadan da anlaşılabilsin.

## English

> Express [BRAND] spatially within [SPACE] using 2–4 tools such as material, lighting, signage, graphic surfaces, sound, or interaction rather than repeated logos.
>
> Do not paint every wall in the brand color.
>
> Let the environment communicate identity even before visitors read the logo.

---

# 1451. `/branded-journey` — Marka Mekânı Kullanıcı Yolculuğu

## Türkçe

> [MEKÂN]'daki ziyaretçi deneyimini 6 aşamada görselleştir:
>
> giriş → orient → engage → core experience → pause → exit.
>
> Her noktada markanın farklı ama tutarlı bir fiziksel/dijital teması olsun.
>
> Her aşamada büyük logo kullanma.

## English

> Visualize the visitor journey through [SPACE] in six stages:
>
> entry → orient → engage → core experience → pause → exit.
>
> Give each stage a different but coherent physical or digital brand touchpoint.
>
> Avoid placing a giant logo at every step.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1452. `/immersive-room` — Sürükleyici Oda

## Türkçe

> [KONU/HİKÂYE]'yi immersive room deneyimine dönüştür.
>
> Oda:
>
> - fiziksel mimari,
> - projection/light,
> - sound,
> - tactile object
>
> arasından yalnız gerektiği kadarını kullansın.
>
> Kullanıcının odadaki yönü ve hareketi anlatının parçası olsun.
>
> Her yüzeyi 360° video wallpaper ile kaplama.

## English

> Transform [TOPIC/STORY] into an immersive room experience using only the necessary combination of physical architecture, projection or light, sound, and tactile objects.
>
> Make visitor movement part of the narrative.
>
> Avoid covering every surface with generic 360° video wallpaper.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1453. `/immersive-entry` — Deneyim Girişi

## Türkçe

> Immersive deneyimin girişini “ne yapacağım?” sorusuna 5 saniyede cevap verecek şekilde tasarla.
>
> Kullanıcı:
>
> - nereye gireceğini,
> - etkileşim olup olmadığını,
> - bekleme/başlama noktasını
>
> anlayabilsin.
>
> Girişi yalnız dramatik karanlık tünele dönüştürme.

## English

> Design the entrance to an immersive experience so users understand within five seconds where to go, whether interaction is expected, and where the experience begins.
>
> Avoid relying solely on a dramatic dark tunnel.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1454. `/immersive-exit` — Deneyim Çıkışı / Son Bellek

## Türkçe

> Immersive deneyimin sonunda tek güçlü “memory object / final image / short takeaway” bırak.
>
> Çıkışta yeni bir bilgi bombardımanı yapma.
>
> Deneyimin ana fikri tek son görselde/nesnede toparlansın.

## English

> End the immersive experience with one strong memory object, final image, or concise takeaway.
>
> Do not introduce a new information overload at the exit.
>
> Let the core idea resolve into one final visual or object.

## Neye dikkat edilmeli?

Değişken kimlikte sabit çekirdek (logo iskeleti, renk kodu) yazıyla sabitlensin; her varyant çekirdeğe karşı denetlenir.

---
# 1455. `/spatial-slop-filter` — Mekânsal Deneyim AI Slop Filtresi

Kaçınılması gerekenler:

- immersion = karanlık + projection,
- her yerde LED,
- her duvarda logo,
- fiziksel yön bulmayı unutmak,
- interaktif ekranı boş duvara yapıştırmak,
- sound/light/AR'ı aynı anda gereksiz kullanmak,
- mekânın gerçek malzemesini yok etmek,
- kullanıcının hareketini planlamamak,
- experience design = “Instagram moment”.

---

# 1456. Yeni üst aile: `Physical–Digital Bridge`

Aile:

- `/ar-packaging`
- `/ar-info-layer`
- `/ar-instruction`
- `/ar-try-in-space`
- `/ar-art-overlay`
- `/ar-museum-object`
- `/smart-print-qr`
- `/nfc-touchpoint`
- `/projection-map-*`

Ortak formül:

> **physical anchor + trigger + digital layer + user action + fallback**

---

# 1457. Yeni üst aile: `Motion Identity`

Aile:

- `/motion-poster`
- `/motion-poster-type`
- `/variable-font-motion`
- `/kinetic-headline`
- `/dynamic-logo`
- `/logo-motion-principles`
- `/responsive-motion-logo`
- `/living-identity`

Ortak soru:

> **Marka/görsel harekete geçtiğinde hangi davranış değişir, hangisi sabit kalır?**

---

# 1458. Yeni üst aile: `Variable System`

Aile:

- `/generative-pattern-system`
- `/data-driven-identity`
- `/personalized-pack`
- `/variable-data-poster`
- `/serial-unique-pack`
- `/city-personalized-poster`

Ortak kural:

> **değişken alan küçük, sistem çekirdeği sabit.**

---

# 1459. `/state-machine-visual` — Görsel Durum Makinesi

## Yeni master kontrol

Motion, AR ve interaction promptlarını netleştirmek için.

## Türkçe

> [DENEYİM]'i durumlar üzerinden tanımla:
>
> State 1 — idle  
> State 2 — user approaches  
> State 3 — interaction  
> State 4 — result  
> State 5 — return/reset
>
> Her durumun görsel farkı sınırlı ve işlevsel olsun.
>
> Transition'ları ayrıca belirt.

## English

> Define [EXPERIENCE] through states:
>
> State 1 — idle  
> State 2 — user approaches  
> State 3 — interaction  
> State 4 — result  
> State 5 — return/reset
>
> Keep visual differences between states functional and restrained.
>
> Define transitions separately.

## Neye dikkat edilmeli?

Hareket azaltılmış sürümde de anlam korunsun; statik yedek, hareketli işin özeti gibi dursun.

---
# 1460. `/motion-storyboard` — Motion Tasarım Storyboard'u

## Türkçe

> [MOTION TASARIM]'ı final renderdan önce 6–8 keyframe storyboard olarak göster.
>
> Her karede:
>
> - zaman,
> - hangi öğe hareket ediyor,
> - yön,
> - başlangıç/bitiş konumu
>
> belirt.
>
> Storyboard'u final posterin sekiz farklı ekran görüntüsü hâline getirme.

## English

> Plan [MOTION DESIGN] as a 6–8 keyframe storyboard before final rendering.
>
> For each frame specify time, moving element, direction, and start/end state.
>
> Do not simply show eight screenshots of the finished animation.

## Neye dikkat edilmeli?

Hareket azaltılmış sürümde de anlam korunsun; statik yedek, hareketli işin özeti gibi dursun.

---
# 1461. `/motion-styleframe` — Motion Styleframe

## Türkçe

> Hareketli tasarımın tek temsili styleframe'ini oluştur.
>
> Styleframe:
>
> - tipografi,
> - renk,
> - doku,
> - grid,
> - ana hareket yönü için ipucu
>
> taşısın.
>
> Zaman davranışı ayrıca storyboard ile çözülmeli.

## English

> Create one representative styleframe for the motion design showing typography, color, texture, grid, and a cue for primary motion direction.
>
> Resolve temporal behavior separately through storyboarding.

## Neye dikkat edilmeli?

Hareket azaltılmış sürümde de anlam korunsun; statik yedek, hareketli işin özeti gibi dursun.

---
# 1462. `/motion-keyframes` — Ana Kareler

## Türkçe

> [HAREKET]'in başlangıç, orta, vurgu ve final olmak üzere dört ana keyframe'ini göster.
>
> Değişimin hangi parametrede olduğunu açıkça koru.
>
> Kamera/keyframe arasında kimlik veya tasarım değişmesin.

## English

> Show four keyframes—start, middle, emphasis, and final—for [MOTION].
>
> Keep the changing parameter explicit.
>
> Do not let identity or design change between keyframes.

## Neye dikkat edilmeli?

Hareket azaltılmış sürümde de anlam korunsun; statik yedek, hareketli işin özeti gibi dursun.

---
# 1463. `/motion-slop-audit` — Hareket Tasarımı Denetimi

Sor:

1. Hareket neyi anlatıyor?
2. Hareket olmasa mesaj kaybolur mu?
3. Her şey mi hareket ediyor?
4. İlk kare okunuyor mu?
5. Son kare okunuyor mu?
6. Loop gerekiyorsa gerçekten loop mu?
7. Küçük ekranda okunuyor mu?
8. Reduced-motion sürümü var mı?

---

# 1464. `/reduced-motion` — Azaltılmış Hareket Sürümü

## Erişilebilirlik

## Türkçe

> Aynı motion/interactive tasarım için reduced-motion sürümü üret.
>
> Büyük zoom, hızlı parallax, sürekli rotation ve flashing yerine:
>
> - opacity,
> - kısa dissolve,
> - küçük positional shift
>
> kullan.
>
> Bilgi ve işlev aynı kalsın.

## English

> Create a reduced-motion version of the same motion or interactive design.
>
> Replace large zooms, fast parallax, continuous rotation, and flashing with opacity changes, short dissolves, or small positional shifts.
>
> Preserve information and functionality.

## Neye dikkat edilmeli?

Hareket azaltılmış sürümde de anlam korunsun; statik yedek, hareketli işin özeti gibi dursun.

---
# 1465. `/motion-static-fallback` — Statik Yedek Görsel

## Türkçe

> Motion poster/interactive visual için tek statik fallback frame seç.
>
> Başlık, ana görsel ve kritik bilgi bu karede tek başına anlaşılır olsun.
>
> Rastgele bir animation frame kullanma.

## English

> Choose one intentional static fallback frame for the motion poster or interactive visual.
>
> Make sure title, primary visual, and critical information work independently in that frame.
>
> Do not use a random animation frame.

## Neye dikkat edilmeli?

Hareket azaltılmış sürümde de anlam korunsun; statik yedek, hareketli işin özeti gibi dursun.

---
# 1466. Bu turdaki slash-style indeks (aile-019)

| Kısayol | Aile |
|---|---|
| `/ar-packaging` | physical package + AR layer |
| `/ar-info-layer` | spatial information overlay |
| `/ar-instruction` | step-specific AR instruction |
| `/ar-assembly` | AR assembly sequence |
| `/ar-try-in-space` | real-scale AR preview |
| `/ar-before-buy` | matched AR option comparison |
| `/ar-art-overlay` | public-art AR extension |
| `/ar-museum-object` | museum interpretation layer |
| `/ar-wayfinding` | AR-assisted navigation |
| `/ar-fallback` | non-AR fallback |
| `/projection-map-facade` | facade projection mapping |
| `/projection-map-table` | tabletop projection mapping |
| `/projection-map-model` | architecture-model projection |
| `/projection-map-object` | object-surface projection |
| `/projection-story-sequence` | projection storyboard |
| `/projection-calibration-view` | technical calibration view |
| `/motion-poster` | animated poster |
| `/motion-poster-loop` | seamless loop |
| `/motion-poster-type` | typography-led motion poster |
| `/variable-font-motion` | animated variable-font axis |
| `/kinetic-headline` | kinetic headline |
| `/type-on-beat` | beat-synchronized typography |
| `/type-scroll-reveal` | scroll-driven type |
| `/motion-grid` | animated grid system |
| `/motion-collage` | layered motion collage |
| `/dynamic-logo` | logo motion behavior |
| `/logo-motion-principles` | reusable motion rules |
| `/responsive-motion-logo` | platform-scaled logo motion |
| `/living-identity` | adaptive visual identity |
| `/generative-pattern-system` | rule-based pattern generation |
| `/data-driven-identity` | data-controlled brand variable |
| `/personalized-pack` | variable-data packaging |
| `/variable-data-poster` | personalized poster system |
| `/serial-unique-pack` | unique but coherent package series |
| `/city-personalized-poster` | localized campaign variants |
| `/spatial-brand-zone` | brand expressed in physical space |
| `/branded-journey` | branded visitor journey |
| `/immersive-room` | immersive room experience |
| `/immersive-entry` | understandable experience entry |
| `/immersive-exit` | final memory object |
| `/state-machine-visual` | interaction-state planning |
| `/motion-storyboard` | motion keyframe plan |
| `/motion-styleframe` | representative motion frame |
| `/motion-keyframes` | key motion states |
| `/reduced-motion` | accessibility motion variant |
| `/motion-static-fallback` | static fallback frame |

---

<a id="aile-020"></a>
# 3B Tarama, Photogrammetry, Gaussian Splatting, Digital Twin ve Sonification — 2026 Ek Taraması

2026'da görsel üretim dünyasının önemli bir kısmı artık yalnız **“resim oluşturma”** değil, fiziksel dünyayı ölçerek, tarayarak veya çoklu fotoğraftan yeniden kurarak temsil etme yönünde ilerliyor.

Özellikle:

- photogrammetry,
- LiDAR / point cloud,
- scan-to-mesh,
- Gaussian Splatting,
- HBIM / digital twin,
- 4D heritage reconstruction,
- change detection,
- surface inspection

alanları mimari, endüstri ve kültürel miras çalışmalarında hızla yayılıyor.

2026 Scientific Reports çalışmaları photogrammetry ile 3D Gaussian Splatting'i yüzey incelemesinde birlikte değerlendiriyor. Heritage alanında ise digital twin yaklaşımı geometri, tarih, çevresel sensörler, tahmin ve koruma kararlarını tek sistem içinde birleştiriyor.

Bu teknolojiler için kritik rehber notu:

> **Bir image-generation modeli “point cloud görünümü” veya “Gaussian Splat estetiği” simüle edebilir; ama bu onu gerçek ölçüm verisi yapmaz.**

Gerçek tarama, ölçüm veya dijital ikiz:

> **ölçülmüş/veri kaynağına bağlıdır.**

---

# 1467. `/photogrammetry-model` — Photogrammetry 3B Model

## Türkçe prompt

> [NESNE/YAPI]'yı çoklu gerçek fotoğraftan photogrammetry ile yeniden oluşturulmuş 3B model gibi göster.
>
> Modelde:
>
> - gerçek yüzey dokusu,
> - fotoğraf kaynaklı texture,
> - küçük görüş eksikliği,
> - bazı zor yüzeylerde düşük detay
>
> bulunabilir.
>
> Bütün modeli kusursuz CAD yüzeyine dönüştürme.
>
> Bu görüntü gerçek ölçüm değildir; gerçek doğruluk gerekiyorsa gerçek capture verisi kullanılmalıdır.

## English

> Show [OBJECT/BUILDING] as a 3D model reconstructed from multiple real photographs using photogrammetry.
>
> Preserve photographic surface texture, small view-coverage gaps, and lower detail on difficult surfaces where plausible.
>
> Do not turn the entire model into a perfect CAD surface.
>
> Treat the result as a visual simulation unless actual capture data is supplied.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; ölçüm iddiası varsa ölçek çubuğu ve eksen ekleyin.

---
# 1468. `/photogrammetry-capture-plan` — Photogrammetry Çekim Planı

## Türkçe

> [NESNE/YAPI]'nın photogrammetry çekim planını göster.
>
> Kamera konumlarını nesne çevresinde kontrollü halkalar/rotalar olarak yerleştir.
>
> Komşu çekimler yeterli overlap taşısın.
>
> Kör noktalar ve parlak/şeffaf yüzey riskleri işaretlenebilsin.
>
> Her kamera konumunu estetik bir orbit olarak eşit aralıklı dizmek zorunda değilsin; gerçek görüş ihtiyacına göre yerleştir.

## English

> Show a photogrammetry capture plan for [OBJECT/BUILDING].
>
> Arrange camera positions around the subject with sufficient overlap between neighboring views.
>
> Identify potential blind spots and difficult reflective or transparent surfaces.
>
> Place cameras according to coverage needs rather than forcing a decorative perfect orbit.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1469. `/turntable-capture` — Döner Tabla Nesne Taraması

## Türkçe

> Küçük [NESNE]'nin turntable photogrammetry çekimini teknik setup olarak göster.
>
> Sabit kamera, sabit ışık ve dönen nesne yaklaşımı kullanılabilir.
>
> Her adımda yaklaşık eşit açı farkı olsun.
>
> Parlak highlight'ların kareler arasında değişmesi gerekiyorsa polarizasyon/ışık kontrolü ayrıca düşünülmeli.

## English

> Show a technical turntable-photogrammetry setup for a small [OBJECT].
>
> Use a fixed camera and lighting with controlled object rotation at regular angular intervals.
>
> If specular highlights cause inconsistency, account for polarization or controlled lighting separately.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1470. `/point-cloud` — Nokta Bulutu Görselleştirmesi

## Türkçe prompt

> [NESNE/YAPI/MEKÂN]'ı 3B point cloud olarak göster.
>
> Noktalar yüzey geometrisini tanımlasın; yoğunluk yüzey/mesafe/scan coverage mantığına göre değişebilir.
>
> Arka plan sade olsun.
>
> Point cloud'u yalnız parçacık efekti veya yıldız alanı gibi göstermeyin.

## English

> Show [OBJECT/BUILDING/SPACE] as a 3D point cloud where points describe the measured surface geometry.
>
> Allow density to vary according to plausible surface, distance, or scan coverage.
>
> Keep the background restrained.
>
> Do not treat the point cloud as decorative particles or a star field.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; ölçüm iddiası varsa ölçek çubuğu ve eksen ekleyin.

---
# 1471. `/lidar-scan` — LiDAR Tarama Görselleştirmesi

## Türkçe

> [MEKÂN]'ı LiDAR tarama sonucu gibi point-cloud görünümünde göster.
>
> Mesafe veya yükseklik verisi verilmişse yalnız o gerçek veriyle renk kodu kullan.
>
> Veri yoksa estetik rainbow depth map uydurma.
>
> Tarama kaynağı/konumu gerekiyorsa sade scanner positions ile göster.

## English

> Show [SPACE] as a LiDAR-style point-cloud capture.
>
> Use distance or elevation color coding only when real data is supplied.
>
> Do not invent a decorative rainbow depth map.
>
> If useful, show scanner positions as restrained acquisition markers.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1472. `/point-cloud-slice` — Nokta Bulutu Kesiti

## Türkçe

> 3B point cloud'u belirtilen düzlem boyunca ince slice/kesit olarak göster.
>
> Kesit dışındaki noktaları kaldır veya çok düşük opacity ile göster.
>
> Bu görünüm geometrik deformasyon ve iç mekân ölçülerini okumaya yardımcı olsun.

## English

> Show a thin slice through the 3D point cloud along the specified plane.
>
> Remove points outside the section or show them at very low opacity.
>
> Use the slice to reveal geometry, deformation, or interior dimensions.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1473. `/scan-section` — Taramadan Teknik Kesit

## Türkçe

> Kaynak point cloud/scan geometrisinden teknik section üret.
>
> Kesilen yüzeyler daha güçlü çizgi, arka plandaki geometri daha hafif line weight ile gösterilsin.
>
> Ölçüm verisi yoksa kesin boyut uydurma.

## English

> Derive a technical section from the source scan or point-cloud geometry.
>
> Show cut surfaces with stronger line weight and background geometry more lightly.
>
> Do not invent exact dimensions without measured data.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1474. `/scan-to-mesh` — Nokta Bulutundan Mesh'e

## Türkçe

> Aynı taramayı üç aşamada göster:
>
> 1. point cloud,
> 2. reconstructed mesh,
> 3. textured mesh.
>
> Her aşamada aynı kamera ve geometri devam etsin.
>
> Mesh oluşurken taramada olmayan keskin detayları icat etme.

## English

> Show the same scan in three stages:
>
> 1. point cloud,
> 2. reconstructed mesh,
> 3. textured mesh.
>
> Preserve camera and core geometry.
>
> Do not invent sharp features absent from the capture during meshing.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1475. `/mesh-wireframe-overlay` — Mesh + Wireframe

## Türkçe

> 3B modelin gerçek yüzey renderı üzerinde ince wireframe overlay göster.
>
> Polygon yoğunluğu yüzey karmaşıklığına göre mantıklı değişsin.
>
> Wireframe'i dekoratif neon grid yapma.

## English

> Overlay a restrained wireframe on the rendered 3D model.
>
> Let polygon density vary logically with surface complexity.
>
> Avoid decorative neon-grid styling.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1476. `/scan-gap-map` — Tarama Eksik Alan Haritası

## Türkçe

> Photogrammetry/LiDAR modelindeki eksik veya düşük güvenli bölgeleri açıkça işaretle.
>
> Kategoriler:
>
> - yeterli coverage,
> - düşük coverage,
> - occlusion,
> - reflective/transparent failure.
>
> Eksik alanları model tarafından “tamamlanmış” gibi gizleme.

## English

> Mark missing or low-confidence areas in a photogrammetry or LiDAR model.
>
> Distinguish adequate coverage, low coverage, occlusion, and reflective or transparent failure.
>
> Do not visually hide missing capture by pretending the model is complete.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1477. `/gaussian-splat` — 3D Gaussian Splatting Görünümü

## Trend

**T1/T2 — 2026'da reconstruction ve digital twin alanında çok güçlü.**

## Türkçe prompt

> [MEKÂN/NESNE]'yi 3D Gaussian Splatting ile yeniden oluşturulmuş serbest kamera sahnesi gibi göster.
>
> Görünüm:
>
> - fotoğrafik renk,
> - hacimsel/soft splat kenar davranışı,
> - görüş dışında veya zor bölgelerde küçük reconstruction artifact'ları
>
> taşıyabilir.
>
> Sonucu yalnız “pointillism” veya particle cloud estetiğine dönüştürme.
>
> Gerçek 3DGS sonucu için gerçek image/camera capture gerekir.

## English

> Show [SPACE/OBJECT] as a free-view scene reconstructed with 3D Gaussian Splatting.
>
> Preserve photographic color and the characteristic soft volumetric splat behavior, allowing mild reconstruction artifacts in poorly observed regions.
>
> Do not reduce it to pointillism or decorative particle clouds.
>
> Genuine 3DGS requires real capture and camera data.

---

# 1478. `/splat-vs-mesh` — Gaussian Splat / Mesh Karşılaştırması

## Türkçe

> Aynı sahneyi iki eşit panelde göster:
>
> A — Gaussian Splat reconstruction  
> B — textured polygon mesh.
>
> Kamera, crop ve lighting eşleşsin.
>
> Yalnız temsil biçimi değişsin.

## English

> Show the same scene in matched panels:
>
> A — Gaussian Splat reconstruction  
> B — textured polygon mesh.
>
> Keep camera, crop, and lighting aligned.
>
> Change only the representation method.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1479. `/sparse-view-reconstruction` — Az Görüşten Rekonstrüksiyon

## Türkçe

> [NESNE]'nin yalnız sınırlı sayıda kamera görünümünden yeniden kurulduğu senaryoyu görselleştir.
>
> Capture edilen alanları güçlü, belirsiz/eksik bölgeleri yarı saydam veya düşük güven ile göster.
>
> Modelin görmediği yüzeyleri kesinmiş gibi sunma.

## English

> Visualize reconstruction of [OBJECT] from only a sparse set of camera views.
>
> Show well-observed regions clearly and uncertain or missing regions with lower confidence or transparency.
>
> Do not present unseen surfaces as certain.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1480. `/surface-inspection-map` — Yüzey İnceleme Haritası

## Trend

2026 Scientific Reports çalışmaları photogrammetry ve Gaussian Splatting'in yüzey incelemesi için kullanılmasını doğrudan araştırıyor.

## Türkçe

> [YÜZEY/NESNE]'nin dijital modelinde incelenecek alanları numaralı inspection regions olarak göster.
>
> Çatlak, deformasyon, aşınma veya yüzey bozukluğu ancak gerçek veri verilmişse işaretlensin.
>
> Hasar icat etme.

## English

> Mark numbered inspection regions on the digital model of [SURFACE/OBJECT].
>
> Show cracks, deformation, wear, or defects only when supplied by real inspection data.
>
> Do not invent damage.

---

# 1481. `/deviation-map` — Geometrik Sapma Haritası

## Türkçe

> Ölçülen scan ile reference/CAD geometri arasındaki sapmayı heatmap ile göster.
>
> Legend üzerinde gerçek tolerans/değerler yalnız veri verilmişse kullanılmalı.
>
> Pozitif/negatif sapmayı açıkça ayır.
>
> Veri yoksa renkli deviation map taklidi üretme.

## English

> Show deviation between measured scan geometry and reference or CAD geometry as a heatmap.
>
> Use real tolerance values only when supplied.
>
> Distinguish positive and negative deviation clearly.
>
> Do not fabricate a colorful deviation map without measurement data.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1482. `/change-detection-scan` — Zaman İçinde Değişim Tespiti

## Türkçe

> Aynı [YAPI/NESNE]'nin iki tarihteki scan'ini aynı coordinate frame içinde karşılaştır.
>
> Değişmeyen alanlar nötr, gerçek değişim alanları vurgulu olsun.
>
> Kamera/perspektif farkını yapısal değişim gibi göstermeyin.

## English

> Compare scans of the same [STRUCTURE/OBJECT] from two dates in one aligned coordinate frame.
>
> Keep unchanged regions neutral and highlight only measured changes.
>
> Do not mistake viewpoint or registration differences for physical change.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1483. `/scan-before-after` — Eşleşmiş Tarama Karşılaştırması

## Türkçe

> Önce/sonra taramasını aynı viewpoint, crop, scale ve coordinate alignment ile göster.
>
> Değişiklik gerçek data layer üzerinden ortaya çıksın.
>
> Sonraki modeli daha dramatik göstermek için lighting değiştirme.

## English

> Show before and after scans using matched viewpoint, crop, scale, and coordinate alignment.
>
> Reveal differences through the data layer.
>
> Do not alter lighting to exaggerate change.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1484. `/orthophoto` — Ortorektifiye Görünüm

## Türkçe

> [CEPHE/ZEMİN/ARKEOLOJİK ALAN]'ı perspective distortion kaldırılmış orthophoto görünümünde göster.
>
> Ölçek ilişkileri yüzey boyunca tutarlı olsun.
>
> Fotoğrafı yalnız “düz cephe” görünümüne perspektif warp ederek gerçek orthophoto gibi sunma; gerçek orthorectification ölçüm verisi gerektirir.

## English

> Show [FACADE/GROUND/ARCHAEOLOGICAL SITE] as an orthophoto with perspective distortion removed and consistent surface scale.
>
> Do not present a simple perspective warp as a true measured orthophoto; real orthorectification requires geometric data.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1485. `/orthomosaic` — Orthomosaic

## Türkçe

> Çok sayıda aerial/overhead image'ın geometrik olarak birleştirildiği orthomosaic görünümünü göster.
>
> Stitch sınırları görünmez veya çok sınırlı olsun.
>
> Perspektif ve ölçek alan boyunca tutarlı kalmalı.

## English

> Show an orthomosaic assembled geometrically from many aerial or overhead images.
>
> Keep stitch seams invisible or minimal and preserve consistent scale and perspective across the mapped area.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1486. `/scan-audit-board` — 3B Tarama Kalite Panosu

## Türkçe

> [TARAMA]'nın kalite değerlendirmesini tek teknik board üzerinde göster:
>
> - capture coverage,
> - missing regions,
> - point density,
> - mesh quality,
> - texture quality,
> - scale/control points.
>
> “High quality” gibi genel puan yerine hangi alanın neden sorunlu olduğunu göster.

## English

> Present a technical quality board for [SCAN] showing capture coverage, missing regions, point density, mesh quality, texture quality, and scale or control points.
>
> Explain where and why quality is limited instead of using a generic “high quality” score.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1487. `/digital-twin-board` — Digital Twin Sistem Panosu

## Trend

**T1 — 2026 endüstri ve heritage çalışmalarında çok güçlü.**

## Türkçe prompt

> [FİZİKSEL VARLIK]'ın digital twin sistemini beş katmanda göster:
>
> 1. physical asset,
> 2. measured 3D model,
> 3. sensors/data,
> 4. analysis/simulation,
> 5. decision/action.
>
> Oklar yalnız gerçek veri/geri besleme ilişkilerini anlatsın.
>
> Digital twin'i yalnız “3B model” olarak tanımlama.

## English

> Show the digital twin of [PHYSICAL ASSET] in five layers:
>
> 1. physical asset,
> 2. measured 3D model,
> 3. sensors and data,
> 4. analysis or simulation,
> 5. decision and action.
>
> Use arrows only for real data or feedback relationships.
>
> Do not define a digital twin as merely a 3D model.

---

# 1488. `/physical-digital-pair` — Fiziksel Varlık / Dijital İkiz

## Türkçe

> Aynı [NESNE/YAPI]'yı iki eşit panelde:
>
> sol = physical reality  
> sağ = measured digital twin
>
> olarak göster.
>
> Geometri ve viewpoint eşleşsin.
>
> Dijital panelde yalnız gerçekten modellenen data layers görünsün.

## English

> Show the same [OBJECT/BUILDING] in matched panels:
>
> left = physical reality  
> right = measured digital twin.
>
> Align geometry and viewpoint.
>
> Display only data layers that actually belong to the digital model.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1489. `/digital-twin-live-state` — Canlı Durum Katmanı

## Türkçe

> Digital twin üzerinde gerçek zamanlı veri için yalnız 3–5 kritik sensor/state göstergesi kullan.
>
> Değer, alarm veya status gerçek data ile beslenmiyorsa placeholder olduğunu açıkça belirt.
>
> 30 dashboard card ile modeli kaplama.

## English

> Overlay only 3–5 critical real-time sensor or state indicators on the digital twin.
>
> Clearly mark placeholders when data is not live.
>
> Do not cover the model with dozens of dashboard cards.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1490. `/digital-twin-maintenance` — Bakım Karar Görseli

## Türkçe

> [VARLIK]'ın digital twin görünümünde:
>
> - normal alanlar,
> - inspection due,
> - maintenance required,
> - unavailable/unknown
>
> durumlarını açık ve sınırlı kodla göster.
>
> Bakım gereksinimi gerçek inspection data yoksa uydurulmasın.

## English

> Show maintenance states on the digital twin of [ASSET] using restrained categories such as normal, inspection due, maintenance required, and unavailable or unknown.
>
> Do not invent maintenance needs without real inspection data.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1491. `/heritage-digital-twin` — Kültürel Miras Dijital İkizi

## Türkçe

> [TARİHÎ YAPI/ESER] için digital twin sistemini yalnız güzel 3B model değil:
>
> - measured geometry,
> - historical records,
> - material condition,
> - environment,
> - conservation interventions
>
> katmanlarıyla göster.
>
> Rekonstrüksiyon ile mevcut gerçek durumu açıkça ayır.

## English

> Represent the digital twin of [HERITAGE BUILDING/ARTIFACT] through measured geometry, historical records, material condition, environment, and conservation interventions rather than as a decorative 3D model.
>
> Clearly distinguish reconstruction from current measured reality.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1492. `/heritage-time-states` — Geçmiş / Bugün / Olası Gelecek

## Trend

2026 Temple of Debod çalışması, 4D heritage anlatımında orijinal bağlam, mevcut durum ve gelecekteki koruma senaryosunu tek interaktif ortamda karşılaştırıyor.

## Türkçe

> [TARİHÎ YAPI]'yı üç matched state içinde göster:
>
> 1. tarihsel durum,
> 2. mevcut ölçülmüş durum,
> 3. önerilen/olasılıklı gelecek.
>
> Her state'in kanıt seviyesi açıkça farklı gösterilsin.
>
> Gelecek senaryosunu “gerçek olacak” gibi sunma.

## English

> Show [HERITAGE SITE] in three matched states:
>
> 1. historical state,
> 2. current measured condition,
> 3. proposed or plausible future.
>
> Make evidence levels visually explicit.
>
> Do not present the future scenario as certain.

---

# 1493. `/historical-reconstruction-evidence` — Tarihsel Rekonstrüksiyon Kanıt Haritası

## Türkçe

> Rekonstrüksiyondaki her ana parçayı:
>
> - surviving evidence,
> - archival evidence,
> - comparative inference,
> - speculative reconstruction
>
> kategorilerinden biriyle ilişkilendir.
>
> Kullanıcı hangi ayrıntının ne kadar güvenilir olduğunu görebilsin.

## English

> Associate each major reconstructed element with one evidence category:
>
> surviving evidence, archival evidence, comparative inference, or speculative reconstruction.
>
> Make confidence transparent to the viewer.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1494. `/heritage-4d-sequence` — 4B Zaman İçinde Miras

## Türkçe

> Aynı structure/site için 4–6 tarihsel zaman noktasını matched spatial frame içinde göster.
>
> Kamera ve temel geometrik referans sabit olsun.
>
> Her tarihte yalnız gerçekten değişen yapı/çevre katmanları değişsin.

## English

> Show 4–6 historical time states of the same structure or site using one matched spatial frame.
>
> Keep camera and primary geometric reference fixed.
>
> Change only elements that actually differ across time.

## Neye dikkat edilmeli?

Nokta bulutu ve tarama estetiği veriyi gizlemesin; taranmayan yer doldurulmuş gibi gösterilmesin, eksik alan haritada dürüstçe işaretlensin.

---
# 1495. `/scan-slop-filter` — Scan / Point Cloud AI Slop Filtresi

Kaçınılması gerekenler:

- point cloud = particle effect,
- LiDAR = rainbow,
- Gaussian Splat = blur cloud,
- orthophoto = perspective-warped photo,
- digital twin = 3B render,
- taramada olmayan yüzeyi “AI tamamladı” diye gerçek veri saymak,
- uydurma ölçü,
- sahte tolerans heatmap,
- “scientific” görünmesi için grid/neon,
- missing data'yı gizlemek.

---

# 1496. Yeni üst aile: `Measured Visual`

Aşağıdaki görseller stil değil **ölçüm temsili** olabilir:

- point cloud,
- photogrammetry,
- LiDAR,
- orthophoto,
- deviation map,
- digital twin,
- scan section.

Bu yüzden rehberde yeni ayrım:

### Simulated appearance

> Model tarama görünümünü taklit eder.

### Measured visual

> Görsel gerçekten ölçüm/capture verisinden türetilir.

Promptta gerektiğinde açıkça yaz:

> `visual simulation, not measured data`

veya:

> `derive only from supplied scan/measurement data`.

---

# 1497. Yeni üst aile: `Spatio-temporal Visual`

Aile:

- `/heritage-time-states`
- `/heritage-4d-sequence`
- `/change-detection-scan`
- `/object-biography`
- `/before-after`
- `/season-option-board`

Ortak mantık:

> **same space/object + time changes + matched reference frame**

---

# 1498. `/waveform` — Ses Dalgası Görselleştirmesi

## Kullanım

Gerçek audio dosyasının amplitude-over-time görünümü.

## Türkçe prompt

> [SES KAYDI]'nı yatay waveform olarak göster.
>
> X ekseni zaman, dikey genlik amplitude olsun.
>
> Gerçek audio data yoksa waveform'u “gerçek kayıt” gibi sunma.
>
> Dekoratif simetrik ses dalgası oluşturmakla gerçek waveform'u karıştırma.

## English

> Show [AUDIO RECORDING] as a waveform with time on the horizontal axis and amplitude vertically.
>
> Do not present a decorative waveform as measured audio when no real audio data is supplied.

## Neye dikkat edilmeli?

Ses dalgası formunun temsili mi gerçek veri mi olduğu görselde belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1499. `/spectrogram` — Spektrogram

## Türkçe

> [SES]'i spectrogram olarak göster:
>
> x = zaman,
> y = frekans,
> renk/yoğunluk = enerji/amplitude.
>
> Gerçek veri yoksa frekans içeriği uydurma.
>
> Spectrogram'ı neon müzik posterine dönüştürme.

## English

> Show [AUDIO] as a spectrogram with time on the x-axis, frequency on the y-axis, and color or intensity representing energy.
>
> Do not invent frequency content without real data.
>
> Avoid turning the spectrogram into decorative neon music art.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1500. `/mel-spectrogram` — Mel Spectrogram

## Türkçe

> [SES]'in Mel-scale spectrogram görünümünü oluştur. Frekans ekseni insan işitmesine daha yakın mel ölçeğinde sıkıştırılsın.
>
> Model eğitim/veri görseli olarak kullanılacaksa gerçek audio preprocessing ile üretilmesi gerekir; image generation ile çizilen görsel yalnız şematik örnektir.

## English

> Show [AUDIO] as a Mel-scale spectrogram where frequency is compressed according to the mel scale.
>
> For machine-learning or analytical use, generate it from real audio preprocessing; an image-generation result is only illustrative.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1501. `/audio-feature-map` — Ses Özellik Haritası

## Türkçe

> [SES]'in gerçek analizinden:
>
> - loudness,
> - pitch,
> - spectral centroid,
> - onset,
> - tempo
>
> gibi yalnız gerekli 3–5 feature'ı zaman boyunca göster.
>
> Ölçülmemiş özellikleri uydurma.

## English

> Plot only 3–5 required audio features such as loudness, pitch, spectral centroid, onset, or tempo over time, based on real analysis.
>
> Do not fabricate unmeasured features.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1502. `/sound-event-timeline` — Ses Olay Zaman Çizelgesi

## Türkçe

> [SES KAYDI]'ndaki önemli eventleri zaman çizgisi üzerinde işaretle:
>
> konuşma,
> kapı,
> müzik,
> alkış,
> makine sesi
>
> gibi.
>
> Olaylar gerçek annotation verilmişse kullanılmalı.
>
> Modelin tahminini gerçek kayıt analizi gibi sunma.

## English

> Mark important sound events on a timeline, such as speech, door, music, applause, or machine sounds.
>
> Use real annotations when available.
>
> Do not present model guesses as measured audio analysis.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1503. `/sonification-map` — Veriyi Sese Eşleme Planı

## 2026 erişilebilirlik araştırmalarıyla ilişkili

## Türkçe

> [VERİ]'yi sesle temsil etmek için mapping planı oluştur.
>
> Her veri değişkeni tek işitsel özelliğe bağlansın:
>
> - değer → pitch,
> - kategori → instrument/timbre,
> - zaman → playback time,
> - işaret/yön → spatial audio
>
> gibi.
>
> Aynı değişkeni gereksiz yere beş farklı ses özelliğine bağlama.

## English

> Create a sonification mapping plan for [DATA].
>
> Map each variable to one auditory property such as value to pitch, category to timbre, time to playback position, or sign and direction to spatial audio.
>
> Avoid redundant mappings of one variable to many sound dimensions.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1504. `/pitch-sonification` — Pitch ile Veri Seslendirme

## Türkçe

> [SERİ]'de düşük değerleri düşük pitch, yüksek değerleri yüksek pitch ile zaman sırasına göre çal.
>
> Pitch range insan işitmesinde rahat ayırt edilebilir ama yorucu olmayacak kadar sınırlı olsun.
>
> Kesin sayısal değer gerekiyorsa yalnız pitch'e güvenme.

## English

> Sonify [SERIES] over time by mapping low values to lower pitch and high values to higher pitch.
>
> Keep the pitch range distinguishable but comfortable.
>
> Do not rely on pitch alone when exact numeric values are required.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1505. `/spatial-sonification` — Mekânsal Ses ile Veri

## Trend

**T1/T2 — Mayıs 2026 IEEE çalışmasında erişilebilir fine-grained data representation için araştırılıyor.**

## Türkçe

> [VERİ DEĞERİ]'ni yalnız pitch değil yatay spatial-audio direction ile temsil eden plan oluştur.
>
> Örneğin negatif değerler sol, pozitif sağ; merkez sıfır gibi.
>
> Ses yönü/azimuth mapping'i legend ile açıkla.
>
> Bu yöntemin kesin kullanılabilirliği kullanıcı testine bağlıdır.

## English

> Map [DATA VALUE] to horizontal spatial-audio direction rather than pitch alone, for example negative values left, positive values right, and zero centered.
>
> Explain azimuth mapping clearly.
>
> Treat usability as something to validate with users rather than assume.

---

# 1506. `/audio-tactile-chart` — Ses + Dokunma Veri Temsili

## 2026 accessibility araştırmalarıyla ilişkili

## Türkçe

> [GRAFİK]'i yalnız görsel değil audio + tactile alternatifle temsil et.
>
> Dokunsal yüzey ana shape/trend'i taşısın.
>
> Ses seçilen veri noktasının değer/etiket bilgisini desteklesin.
>
> İki kanal birbirini tekrar etmek yerine tamamlasın.

## English

> Represent [CHART] through a combined audio and tactile alternative.
>
> Let the tactile layer carry primary shape or trend while audio supports selected-point value or label information.
>
> Make the channels complementary rather than redundant.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1507. `/accessible-chart-package` — Çok Modlu Grafik Paketi

## Türkçe

> [GRAFİK] için erişilebilir çıktı paketi tasarla:
>
> 1. görsel grafik,
> 2. kısa alt-text,
> 3. uzun veri açıklaması,
> 4. tablo,
> 5. isteğe bağlı sonification/tactile mapping.
>
> Hiçbir tek yöntemi herkes için evrensel çözüm olarak varsayma.

## English

> Create an accessible output package for [CHART]:
>
> 1. visual chart,
> 2. concise alt text,
> 3. detailed data description,
> 4. data table,
> 5. optional sonification or tactile mapping.
>
> Do not assume one representation works universally for every user.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1508. `/sound-to-visual` — Sesten Görsele Eşleme

## Türkçe

> [SES/MÜZİK]'in gerçek analiz edilen bir özelliğini tek görsel değişkene eşle:
>
> - amplitude → çizgi kalınlığı,
> - pitch → yükseklik,
> - frequency band → renk,
> - rhythm → spacing.
>
> Görsel ilişki açık legend ile açıklansın.
>
> “Müziğin ruhu” gibi ölçülmeyen soyut nitelikleri veriymiş gibi göstermeyin.

## English

> Map one genuinely analyzed property of [AUDIO/MUSIC] to one visual variable, such as amplitude to line thickness, pitch to height, frequency band to color, or rhythm to spacing.
>
> Explain the mapping explicitly.
>
> Do not present subjective qualities like “the soul of the music” as measured data.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1509. `/chladni-pattern` — Chladni Deseni

## Trend / bilimsel + sanatsal

2026 DRS ve yeni medya çalışmalarında ses-görsel eşlemesi için Chladni pattern'ları yeniden ele alınıyor.

## Türkçe

> Belirli frekansta titreşen gerçek plaka üzerindeki Chladni nodal pattern'ını bilimsel görsel olarak göster.
>
> Desen plaka sınırı ve titreşim modu ile ilişkili olsun.
>
> Rastgele simetrik kum mandalası üretme.
>
> Frekans kesin verilecekse fiziksel/simülasyon kaynağıyla doğrulanmalı.

## English

> Show a Chladni nodal pattern formed on a vibrating plate at a specified frequency.
>
> Keep the pattern related to plate geometry and vibration mode.
>
> Avoid generating arbitrary symmetrical sand mandalas.
>
> Verify exact frequency-pattern relationships through physical or numerical simulation when accuracy matters.

---

# 1510. `/audio-visual-performance` — Ses-Tepkili Görsel Performans

## Türkçe

> Canlı ses/müzik ile görselin yalnız 2–3 parametresini eşle:
>
> - low frequency → large-form scale,
> - high frequency → fine texture,
> - overall amplitude → brightness.
>
> Mapping sabit ve izleyici tarafından zamanla anlaşılabilir olsun.
>
> Her beat'te tüm sahneyi değiştirip visualizer slop üretme.

## English

> Map live audio to only 2–3 visual parameters, such as low frequencies to large-form scale, high frequencies to fine texture, and overall amplitude to brightness.
>
> Keep mappings stable enough for viewers to learn.
>
> Avoid changing the entire scene on every beat.

## Neye dikkat edilmeli?

Ses görselleştirmesinin temsili mi gerçek veri mi olduğu belirtilsin; uydurma dalga formu analiz gibi sunulmamalı.

---
# 1511. `/sonification-slop-filter` — Sonification / Ses Görselleştirme AI Slop Filtresi

Kaçınılması gerekenler:

- waveform = simetrik dekor,
- spectrogram = neon renkli poster,
- pitch mapping'i kesin sayı ölçümü sanmak,
- erişilebilirlik = sadece ses eklemek,
- yüksek veri değerini her zaman “daha yüksek ses” yapmak,
- kullanıcı testi olmadan mapping'in sezgisel olduğunu varsaymak,
- audio/tactile/visual üç kanalın aynı bilgiyi gereksiz tekrar etmesi,
- gerçek audio data yokken analitik grafik üretmek.

---

# 1512. Yeni üst aile: `Captured Reality`

Aile:

- `/photogrammetry-model`
- `/point-cloud`
- `/lidar-scan`
- `/gaussian-splat`
- `/orthophoto`
- `/scan-section`

Ortak kural:

> **görsel kaynak fiziksel dünyadan capture edilir; model boşlukları stil olarak değil veri eksikliği olarak ele alınır.**

---

# 1513. Yeni üst aile: `Digital Twin Visual`

Aile:

- `/digital-twin-board`
- `/physical-digital-pair`
- `/digital-twin-live-state`
- `/digital-twin-maintenance`
- `/heritage-digital-twin`
- `/heritage-time-states`

Ortak ayrım:

> **3B model ≠ digital twin.**
>
> Digital twin:
>
> physical asset + measured model + data + analysis + feedback/decision.

---

# 1514. Yeni üst aile: `Multisensory Data Representation`

2026 accessibility araştırmalarının önemli sonucu:

> Veri anlatımı yalnız görsel olmak zorunda değildir.

Aile:

- visual chart,
- sonification,
- spatial audio,
- tactile chart,
- haptic feedback,
- text/table description.

Temel kural:

> **modality chosen according to task.**

Trend bulmak için pitch yeterli olabilir; kesin değer için başka kanal daha iyi olabilir. Aynı şekilde tactile veya spatial audio bazı görevlerde güçlü, bazı görevlerde daha yavaş/zor olabilir.

---

# 1515. `/modality-task-map` — Veri Görevi / Modalite Haritası

## Türkçe

> [VERİ GÖREVİ] için hangi representation biçiminin uygun olduğunu eşle:
>
> - trend bulma,
> - kesin değer,
> - karşılaştırma,
> - kategori,
> - spatial relation,
> - distribution.
>
> Görsel, işitsel, dokunsal ve metinsel seçenekleri ayrı değerlendir.
>
> “Erişilebilir” diye tek kanalı otomatik seçme.

## English

> Map [DATA TASK] to suitable representations such as visual, auditory, tactile, or textual for trend finding, exact value, comparison, category, spatial relation, and distribution.
>
> Do not automatically treat one modality as universally accessible.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1516. Bu turdaki slash-style indeks (aile-020)

| Kısayol | Aile |
|---|---|
| `/photogrammetry-model` | multi-photo 3D reconstruction |
| `/photogrammetry-capture-plan` | capture coverage plan |
| `/turntable-capture` | object turntable capture |
| `/point-cloud` | point-cloud geometry |
| `/lidar-scan` | LiDAR-style scan |
| `/point-cloud-slice` | sliced point cloud |
| `/scan-section` | section from measured scan |
| `/scan-to-mesh` | point cloud → mesh → texture |
| `/mesh-wireframe-overlay` | mesh topology overlay |
| `/scan-gap-map` | missing/low-confidence capture |
| `/gaussian-splat` | 3D Gaussian Splat reconstruction |
| `/splat-vs-mesh` | matched representation comparison |
| `/sparse-view-reconstruction` | sparse-view confidence visual |
| `/surface-inspection-map` | surface inspection regions |
| `/deviation-map` | measured geometry deviation |
| `/change-detection-scan` | temporal scan comparison |
| `/scan-before-after` | aligned scan pair |
| `/orthophoto` | rectified measured surface view |
| `/orthomosaic` | stitched mapped image |
| `/scan-audit-board` | 3D capture quality audit |
| `/digital-twin-board` | full digital twin system |
| `/physical-digital-pair` | physical asset vs twin |
| `/digital-twin-live-state` | live sensor overlay |
| `/digital-twin-maintenance` | maintenance decision view |
| `/heritage-digital-twin` | heritage digital twin |
| `/heritage-time-states` | past/current/future states |
| `/historical-reconstruction-evidence` | reconstruction evidence map |
| `/heritage-4d-sequence` | time-based heritage sequence |
| `/waveform` | amplitude over time |
| `/spectrogram` | time-frequency-energy map |
| `/mel-spectrogram` | mel-frequency spectrogram |
| `/audio-feature-map` | audio feature timeline |
| `/sound-event-timeline` | annotated sound events |
| `/sonification-map` | data-to-sound mapping plan |
| `/pitch-sonification` | value-to-pitch |
| `/spatial-sonification` | value-to-audio direction |
| `/audio-tactile-chart` | multimodal chart |
| `/accessible-chart-package` | visual + text + table + optional audio/touch |
| `/sound-to-visual` | measured audio-to-visual mapping |
| `/chladni-pattern` | physical sound pattern |
| `/audio-visual-performance` | stable sound-reactive mapping |
| `/modality-task-map` | data task to representation modality |

---

<a id="aile-021"></a>
# Pinterest 2026’nın Kalan Güçlü Aileleri — Kitchen Witch, Cosmic Reset, Weekend Equestrian ve Secondhand Sidequest

Pinterest’in 25 Ağustos 2026 Hobbies Trend Report’unda daha önce rehberin bazı bölümlerine dağılmış olan dört büyük eğilim hâlâ ayrı prompt aileleri oluşturacak kadar belirgin:

- **Kitchen Witch**
- **Cosmic Reset**
- **Weekend Equestrian**
- **Secondhand Sidequest**

Burada özellikle dikkat edilmesi gereken nokta şu:

> Trend adı, içerikteki iddiaların doğru olduğu anlamına gelmez.

Örneğin:

- herbal apothecary görsel dili → sağlık iddiası değildir,
- natal chart → astronomik ölçüm değildir,
- crystal meanings → bilimsel özellik değildir,
- moon water → fiziksel/sağlık etkisi kanıtı olarak sunulmamalıdır.

Rehber bu alanları **görsel kültür ve tasarım dili** olarak ele alır.

---

# 1517. `/kitchen-apothecary` — Mutfak Apothecary Rafı

## Trend

**T1/T2 — Pinterest 2026’da `herbal apothecary` aramaları +595%.**

## Türkçe prompt

> Gerçek bir ev mutfağında küçük kitchen-apothecary rafı düzenle.
>
> Raf yalnız 8–12 işlevsel mutfak malzemesi içersin:
>
> - kurutulmuş ot,
> - baharat,
> - sirke,
> - infüzyonluk bitki,
> - balmumu,
> - tuz,
> - küçük kavanozlar.
>
> Etiketler yalnız içerik adını ve gerekiyorsa tarihi göstersin.
>
> Şifa, detox, hormon, bağışıklık veya hastalık tedavisi iddiası ekleme.
>
> Rafı karanlık büyücü laboratuvarına dönüştürme.

## English

> Arrange a small kitchen-apothecary shelf in a believable home kitchen using only 8–12 functional pantry materials such as dried herbs, spices, vinegar, infusion ingredients, beeswax, salt, and small jars.
>
> Labels should identify contents and, where useful, dates only.
>
> Do not add medical, detox, hormonal, immunity, or disease-treatment claims.
>
> Avoid turning the shelf into a dark fantasy potion laboratory.

---

# 1518. `/spice-blending-board` — Baharat Karışımı Panosu

## Türkçe

> [BAHARAT KARIŞIMI] için gerçek ingredient board oluştur.
>
> Her bileşeni küçük ayrı miktarda göster:
>
> - adı,
> - yaklaşık oranı,
> - öğütülmüş/tane formu.
>
> Final karışımı ayrı küçük kasede göster.
>
> Baharatları sırf renk uyumu için uydurma veya oranları görsel olarak abartma.

## English

> Create a real ingredient board for [SPICE BLEND].
>
> Show each component separately with its name, approximate proportion, and whole or ground form.
>
> Show the finished blend in a small separate bowl.
>
> Do not invent ingredients merely for color balance or visually exaggerate proportions.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1519. `/herbal-infusion-card` — Bitkisel İnfüzyon Kartı

## Türkçe

> [İÇECEK/İNFÜZYON] için sade tarif kartı tasarla.
>
> Kart:
>
> - ingredient list,
> - su miktarı,
> - süre,
> - hazırlama adımı
>
> içersin.
>
> Sağlık etkisi, şifa veya tıbbi fayda vaat etme.
>
> Görsel dili mutfak hazırlığı olarak tut.

## English

> Design a restrained preparation card for [INFUSION/DRINK] containing ingredients, water amount, time, and preparation steps.
>
> Do not promise healing, medical benefit, or health outcomes.
>
> Keep the visual language grounded in ordinary kitchen preparation.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1520. `/beeswax-wrap-process` — Balmumlu Kumaş Yapım Süreci

## Trend bağlantısı

Pinterest Kitchen Witch açıklamasında beeswax-and-fabric hacks bu alanın pratik taraflarından biri olarak geçiyor.

## Türkçe prompt

> Balmumlu tekrar kullanılabilir kumaş sargının yapımını 4 adımda göster:
>
> 1. pamuklu kumaşı kes,
> 2. balmumunu kontrollü dağıt,
> 3. ısı ile kumaşa yedir,
> 4. soğutup kullan.
>
> Fiziksel malzeme davranışı gerçekçi olsun.
>
> Süreci dekoratif “witchcraft ritual” gibi göstermeyin.

## English

> Show the making of a reusable beeswax fabric wrap in four steps:
>
> 1. cut cotton fabric,
> 2. distribute beeswax,
> 3. apply heat so wax penetrates the textile,
> 4. cool and use.
>
> Keep material behavior physically plausible.
>
> Avoid framing the process as a fantasy ritual.

---

# 1521. `/fermentation-shelf` — Fermantasyon Rafı

## Türkçe

> Ev tipi küçük fermentation shelf düzenle.
>
> Farklı aşamadaki 4–6 kavanoz üzerinde:
>
> - içerik adı,
> - başlangıç tarihi,
> - batch numarası
>
> bulunabilir.
>
> Kavanozlarda gerçek taşma/bozulma belirtilerini estetik uğruna ekleme.
>
> Gıda güvenliği bilgisi gerekiyorsa doğrulanmış kaynaktan ayrıca verilmelidir.

## English

> Arrange a small home fermentation shelf with 4–6 jars at different stages.
>
> Allow concise labels for contents, start date, and batch number.
>
> Do not add spoilage or overflow as decorative texture.
>
> Any food-safety instructions should come from verified sources separately.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1522. `/pantry-label-system` — Kiler Etiket Sistemi

## Türkçe

> [MUTFAK/KİLER] için 12 parçalık okunabilir label family oluştur.
>
> Büyük içerik adı, gerekiyorsa küçük tarih/kategori alanı yeterli olsun.
>
> Script font ve süs çerçevesi nedeniyle okunabilirliği düşürme.
>
> Gerçek mutfakta uzaktan okunabilirliği düşün.

## English

> Create a 12-label pantry system with large ingredient names and, where necessary, a small date or category field.
>
> Avoid decorative script and frames that reduce legibility.
>
> Design for real viewing distance in a working kitchen.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1523. `/kitchen-witch-slop-filter` — Kitchen Witch AI Slop Filtresi

Kaçınılması gerekenler:

- her rafta potion bottle,
- sahte Latince etiket,
- sağlık/şifa iddiası,
- her kavanozda kristal,
- her görselde mum,
- karanlık yeşil-gold “witch” paleti,
- gerçek mutfak işlevini kaybetmek,
- otların/bitkilerin yanlış tanımlanması.

---

# 1524. `/celestial-journal` — Göksel Gözlem Günlüğü

## Trend

**Cosmic Reset ailesinin güvenli ve pratik karşılığı.**

## Türkçe

> Gece gökyüzü gözlemleri için celestial journal spread oluştur.
>
> Alanlar:
>
> - tarih/saat,
> - konum,
> - Ay evresi,
> - görülen parlak yıldız/gezegen,
> - hava/bulut durumu,
> - kısa kişisel not.
>
> Astrolojik kişilik veya kader yorumu ekleme.

## English

> Create a celestial observation-journal spread with fields for date and time, location, moon phase, visible bright stars or planets, weather or cloud conditions, and a concise personal note.
>
> Do not add astrological personality or destiny claims.

---

# 1525. `/moon-phase-observation` — Ay Evresi Gözlem Şeridi

## Türkçe

> Aynı Ay diskini 8 temel phase boyunca bilimsel olarak tutarlı sırada göster.
>
> Aydınlık/karanlık sınırı gerçek phase geometrisine uygun olsun.
>
> Dekoratif hilal şekillerini astronomik evre diyagramı gibi sunma.

## English

> Show the Moon through eight primary phases in scientifically consistent order.
>
> Keep illuminated and shadowed geometry appropriate to each phase.
>
> Do not use decorative crescent shapes as if they were an accurate astronomical diagram.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1526. `/celestial-field-card` — Gökyüzü Alan Kartı

## Türkçe

> [TAKIMYILDIZ/GÖKYÜZÜ ALANI] için sade field card oluştur.
>
> Yalnız kullanıcı tarafından verilen veya doğrulanmış:
>
> - ana yıldızlar,
> - yön,
> - mevsim,
> - yaklaşık görünüm
>
> bilgilerini kullan.
>
> Takımyıldız çizgilerini aşırı güçlü ana görsel yapma.

## English

> Create a restrained field card for [CONSTELLATION/SKY REGION] using only verified or supplied information about primary stars, direction, season, and approximate appearance.
>
> Keep constellation connecting lines secondary.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1527. `/astrology-chart-design` — Astroloji Haritasını Grafik Tasarım Nesnesi Olarak Kullanma

## Kritik not

Bu kısayol:

> astrolojiyi bilimsel gerçeklik olarak doğrulamaz.

## Türkçe prompt

> Kullanıcının verdiği hazır natal-chart verisini yalnız grafik tasarım nesnesi olarak düzenle.
>
> Dairesel harita, ev bölümleri, semboller ve legend okunabilir olsun.
>
> Görselden yeni kişilik, sağlık, ilişki veya gelecek tahmini çıkarma.
>
> Hesaplama gerekiyorsa ayrı ve güvenilir astroloji hesaplama kaynağı kullanılmalıdır.

## English

> Present user-supplied natal-chart data purely as a graphic-design object.
>
> Keep the circular chart, house divisions, symbols, and legend readable.
>
> Do not infer new personality, health, relationship, or future predictions from the image.
>
> Any chart calculation should come from a dedicated external calculation source.

## Neye dikkat edilmeli?

Burç ve gezegen sembolleri gelişi güzel dizilmesin; yanlış sembol, konuyu bilen izleyicide güveni bitirir.

---
# 1528. `/astrocartography-map-design` — Astrocartography Harita Tasarımı

## Türkçe

> Kullanıcı tarafından sağlanmış astrocartography line data'sını dünya haritası üzerinde okunabilir biçimde göster.
>
> Hat isimleri ve legend açık olsun.
>
> Çizgilerin bulunduğu şehirlerin kullanıcı için gerçekten “iyi/kötü” olduğunu görselden iddia etme.

## English

> Display user-supplied astrocartography line data on a readable world map with clear labels and legend.
>
> Do not claim that cities under particular lines are objectively good or bad for the user.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1529. `/crystal-display` — Mineral / Kristal Koleksiyon Sunumu

## Türkçe

> [MİNERAL/KRİSTAL KOLEKSİYONU]'nu specimen display olarak göster.
>
> Her örnek:
>
> - gerçek adı,
> - renk,
> - kristal habit/form,
> - küçük numara
>
> ile düzenlenebilir.
>
> “Enerji”, “şifa”, “koruma” etkilerini bilimsel özellik gibi etiketleme.

## English

> Present [MINERAL/CRYSTAL COLLECTION] as a specimen display using real names, color, crystal habit or form, and small numbering.
>
> Do not label energy, healing, or protection claims as scientific properties.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1530. `/celestial-symbol-sheet` — Göksel Sembol Sayfası

## Türkçe

> Ay, yıldız, güneş, gezegen ve yörünge temalı 12 sembolden oluşan sade grafik sheet oluştur.
>
> Astronomik semboller kullanılacaksa gerçek sembollerle dekoratif uydurma işaretleri açıkça ayır.
>
> Bütün sembolleri okült sigil'e dönüştürme.

## English

> Create a restrained 12-symbol sheet around moon, star, sun, planet, and orbit themes.
>
> Distinguish genuine astronomical symbols from decorative invented marks.
>
> Do not turn the entire set into occult sigils.

## Neye dikkat edilmeli?

Gözlem ve tarif iddiaları doğrulanabilir olsun; ay evresi ve karışım oranı gibi bilgiler uydurulmaz.

---
# 1531. `/cosmic-reset-slop-filter` — Cosmic Reset AI Slop Filtresi

Kaçınılması gerekenler:

- her görselde tarot,
- her görselde kristal + mum + ay,
- bilimsel astroloji iddiası,
- kişilik/gelecek tahmini,
- “enerji alanı”nı ölçüm gibi göstermek,
- gökyüzü diyagramında uydurma yıldız düzeni,
- mor-neon galaxy klişesi.

---

# 1532. `/equestrian-outfit-board` — Binicilik Esintili Kıyafet Panosu

## Trend

**T1/T2 — Pinterest 2026 Weekend Equestrian.**

Arama sinyalleri arasında:

- `rosette ribbon` +3816%
- `barn jacket outfit women` +1109%
- `equestrian aesthetic outfit` +219%
- `horse riding aesthetic outfit` +170%

bulunuyor.

## Türkçe prompt

> Binicilik esintili günlük outfit board oluştur.
>
> Kullan:
>
> - barn jacket,
> - düz gömlek/triko,
> - breeches/jodhpur esintili alt,
> - gerçekçi riding/rubber boots,
> - yalnız bir küçük equestrian cue.
>
> Outfit'i kostüm veya yarış binicisi üniformasına dönüştürme.

## English

> Create an equestrian-inspired everyday outfit board using a barn jacket, restrained shirt or knit, breeches- or jodhpur-inspired bottoms, believable riding or rubber boots, and only one small equestrian cue.
>
> Avoid turning the outfit into costume or competition riding uniform.

---

# 1533. `/barn-jacket-editorial` — Barn Jacket Editorial

## Türkçe

> [KİŞİ]'yi kırsal/stable çevresinde gerçek barn jacket ile sade editoryal fotoğraf olarak göster.
>
> Ceket işlevsel outerwear gibi davransın.
>
> At, eyer, ahır, saman ve riding crop'un hepsini aynı kareye ekleme.

## English

> Photograph [PERSON] editorially in a real barn jacket within a restrained rural or stable environment.
>
> Treat the jacket as functional outerwear.
>
> Avoid filling the frame with horses, saddles, hay, riding crops, and every equestrian cue at once.

## Neye dikkat edilmeli?

Kumaş, dikiş ve aksesuar aynı sette tutarlı kalsın; dönem ve marka birbirine karışmasın.

---
# 1534. `/rosette-ribbon` — Rosette Ribbon

## Trend

**T1/T2 — Pinterest +3816%.**

## Türkçe

> Gerçek kumaş rosette ribbon tasarla.
>
> Katlanmış/ruch edilmiş şerit yapısı, merkez disk, iki kısa kuyruk ve gerçek dikiş/birleşim mantığı görülsün.
>
> Üzerinde kategori/isim gerekiyorsa kısa ve okunabilir olsun.
>
> Her ribbon'u altın “winner badge” olarak yapma.

## English

> Design a real fabric rosette ribbon with pleated or gathered ribbon structure, central disc, two short tails, and believable stitching or assembly.
>
> Keep any category or name concise and readable.
>
> Do not make every rosette a gold winner badge.

---

# 1535. `/equestrian-gear-flatlay` — Binicilik Ekipmanı Flat Lay

## Türkçe

> Gerçek binicilik ekipmanından 6–8 parçayı top-down flat lay olarak düzenle:
>
> eldiven, helmet, boot, grooming brush, lead rope vb.
>
> Nesneler gerçek kullanım ve ölçek ilişkisi taşısın.
>
> Görseli “luxury country lifestyle” prop setine dönüştürme.

## English

> Arrange 6–8 real equestrian equipment items in a top-down flat lay, such as gloves, helmet, boots, grooming brush, or lead rope.
>
> Preserve real use and scale relationships.
>
> Avoid turning it into a luxury-country-lifestyle prop set.

## Neye dikkat edilmeli?

Kumaş, dikiş ve aksesuar aynı sette tutarlı kalsın; dönem ve marka birbirine karışmasın.

---
# 1536. `/stable-field-guide` — Ahır / Binicilik Alan Rehberi

## Türkçe

> Başlangıç düzeyi için 8 temel binicilik ekipmanını field-guide plate olarak göster.
>
> Her nesne:
>
> - tek görünüm,
> - kısa ad,
> - tek satır işlev
>
> taşısın.
>
> Güvenlik ekipmanını dekoratif aksesuar gibi göstermeyin.

## English

> Show eight basic equestrian equipment items as a beginner field-guide plate.
>
> Give each one a single view, concise name, and one-line function.
>
> Do not treat safety equipment as decorative accessories.

## Neye dikkat edilmeli?

Kumaş, dikiş ve aksesuar aynı sette tutarlı kalsın; dönem ve marka birbirine karışmasın.

---
# 1537. `/horse-motif-patch` — At Motifli Patch

## Türkçe

> At temasını doğrudan gerçekçi tam at illüstrasyonu yerine sade:
>
> - baş profili,
> - nal,
> - eyer çizgisi,
> - rosette formu
>
> gibi tek sembolle 6–8 cm embroidered patch'e dönüştür.
>
> Aynı patch içinde bütün sembolleri kullanma.

## English

> Translate the equestrian theme into a 6–8 cm embroidered patch using one restrained symbol such as a horse-head profile, horseshoe, saddle line, or rosette form rather than a full realistic horse illustration.
>
> Avoid combining every symbol into one patch.

## Neye dikkat edilmeli?

Kumaş, dikiş ve aksesuar aynı sette tutarlı kalsın; dönem ve marka birbirine karışmasın.

---
# 1538. `/equestrian-slop-filter` — Equestrian AI Slop Filtresi

Kaçınılması gerekenler:

- her karede at,
- luxury estate klişesi,
- beige/brown heritage paleti zorunluluğu,
- yanlış tack/equipment,
- riding safety ekipmanını moda aksesuarı gibi kullanmak,
- rastgele crest,
- her kombinde tall boot + riding crop + helmet.

---

# 1539. `/deadstock-archive` — Deadstock Arşiv Panosu

## Trend

**T1/T2 — Pinterest 2026 Secondhand Sidequest.**

## Türkçe prompt

> [GİYSİ/ÜRÜN] deadstock arşivini katalog panosu olarak göster.
>
> Her parça:
>
> - üretim dönemi,
> - model/kod,
> - malzeme,
> - ölçü,
> - kondisyon
>
> gibi gerçek bilgiler varsa bunlarla etiketlensin.
>
> “Vintage” görünmesi için sahte yıpranma ekleme; deadstock kullanılmamış olabilir.

## English

> Present a deadstock archive of [GARMENT/PRODUCT] as a catalog board.
>
> Where real information exists, label production period, model or code, material, size, and condition.
>
> Do not add fake wear to make it look vintage; deadstock may be unused.

---

# 1540. `/archive-streetwear-board` — Archive Streetwear Koleksiyonu

## Türkçe

> [DÖNEM/MARKA TİPİ] archive streetwear koleksiyonunu 6 parçalık sistemli selection board olarak göster.
>
> Aynı dönem/alt kültür içindeki farklı:
>
> - kesim,
> - grafik,
> - kumaş,
> - işlev
>
> çeşitlerini karşılaştır.
>
> Gerçek marka/telifli grafik gerekiyorsa referans doğruluğunu koru; aksi hâlde kurmaca tasarım kullan.

## English

> Show a six-piece archive-streetwear selection board from [ERA/TYPE], comparing variation in cut, graphics, fabric, and function within one coherent period or subculture.
>
> Preserve real brand references accurately when supplied; otherwise use fictional designs.

## Neye dikkat edilmeli?

Kumaş, dikiş ve aksesuar aynı sette tutarlı kalsın; dönem ve marka birbirine karışmasın.

---
# 1541. `/provenance-tag` — Ürün Köken / Geçmiş Etiketi

## Türkçe

> İkinci el [NESNE/GİYSİ] için küçük provenance tag tasarla.
>
> Biliniyorsa:
>
> - üretim yılı,
> - üretim yeri,
> - önceki kullanım,
> - onarım,
> - malzeme
>
> alanları bulunsun.
>
> Bilinmeyen bilgiyi romantik hikâye uydurarak doldurma.

## English

> Design a small provenance tag for a secondhand [OBJECT/GARMENT].
>
> Where known, include production year, place, previous use, repair history, and material.
>
> Do not invent romantic backstories for unknown information.

## Neye dikkat edilmeli?

Kumaş, dikiş ve aksesuar aynı sette tutarlı kalsın; dönem ve marka birbirine karışmasın.

---
# 1542. `/repair-aesthetic-board` — Onarım Estetiği Panosu

## Trend

Pinterest Secondhand Sidequest'ta `repair aesthetic` aramaları +167%.

## Türkçe

> Aynı giyim parçası üzerinde dört gerçek onarım yaklaşımını matched close-up olarak karşılaştır:
>
> - invisible repair,
> - darning,
> - patch,
> - visible stitched repair.
>
> Aynı hasar boyutu ve kumaş türü üzerinden karşılaştır.
>
> Her onarımı dekoratif nakışa dönüştürme.

## English

> Compare four real repair approaches on the same garment using matched close-ups:
>
> invisible repair, darning, patching, and visible stitched repair.
>
> Keep damage size and fabric type consistent.
>
> Do not turn every repair into decorative embroidery.

---

# 1543. `/sashiko-inspired-repair` — Sashiko Esintili Onarım

## Kültürel doğruluk notu

Sashiko belirli Japon tekstil geleneklerine dayanır.

## Türkçe prompt

> [GİYSİ]'de sashiko'dan esinlenen görünür onarım kullan.
>
> Basit tekrar eden running-stitch grid/geometrisi, yapısal patch ve sınırlı indigo/beyaz ilişkisi kullanılabilir.
>
> Gerçek tarihsel sashiko kalıplarını bağlamını bilmeden rastgele karıştırma.
>
> “Japanese aesthetic” diye kanji, dalga, sakura gibi ilgisiz semboller ekleme.

## English

> Use a sashiko-inspired visible repair on [GARMENT] through restrained running-stitch geometry and structural patching.
>
> Avoid randomly mixing historical sashiko patterns without context.
>
> Do not add unrelated kanji, waves, or cherry blossoms merely to signal “Japanese aesthetic.”

## Neye dikkat edilmeli?

Motif onarım mantığına uysun (yama ve dikiş yönü kumaş dokusuyla); kültürel motifi süs diye rastgele dağıtmayın.

---
# 1544. `/corset-back-conversion` — Corset-back Dönüşümü

## Trend bağlantısı

Pinterest Secondhand Sidequest'ta `corset back blouse` +385%.

## Türkçe

> Kaynak [BLUZ/GİYSİ]'nin arka kapanışını gerçek dikiş mantığıyla corset-back conversion'a dönüştür.
>
> Ön yüz ve temel garment geometry korunmalı.
>
> Eyelet, facing, reinforcement ve lacing gerçek yük taşımaya uygun görünsün.

## English

> Convert the back closure of [GARMENT] into a physically plausible corset-back alteration while preserving the front and core garment geometry.
>
> Make eyelets, facing, reinforcement, and lacing structurally believable.

---

# 1545. `/patchwork-leather-repair` — Patchwork Deri Onarım

## Trend bağlantısı

Pinterest'te `patchwork leather bag` +207%.

## Türkçe prompt

> Aşınmış [DERİ ÇANTA/NESNE]'yi yeni ürünle değiştirmek yerine 2–4 uyumlu deadstock deri parçasıyla patchwork repair olarak onar.
>
> Patch kenarları, dikiş ve kalınlık farkı gerçek olsun.
>
> Eski gövdenin büyük bölümü görünür kalsın.

## English

> Repair worn [LEATHER BAG/OBJECT] using 2–4 compatible deadstock leather patches rather than replacing the item entirely.
>
> Keep patch edges, stitching, and thickness differences physically believable.
>
> Preserve most of the original body.

---

# 1546. `/secondhand-catalog` — İkinci El Katalog Fotoğrafı

## Türkçe

> [İKİNCİ EL ÜRÜN]'ü satış/katalog için dürüst product record olarak göster.
>
> Şunları ayrı karelerde göster:
>
> - ön,
> - arka,
> - label,
> - önemli wear/damage,
> - repair.
>
> Kusurları gizlemek için dramatik ışık veya shallow focus kullanma.

## English

> Document [SECONDHAND PRODUCT] honestly for resale or cataloging with separate views of front, back, label, significant wear or damage, and repair.
>
> Do not hide defects through dramatic lighting or shallow focus.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1547. `/condition-map-garment` — Giysi Kondisyon Haritası

## Türkçe

> [GİYSİ]'yi düz technical flat görünümünde göster ve mevcut kondisyonu 4 kategoriyle işaretle:
>
> iyi,
> aşınma,
> onarım,
> eksik/hasarlı.
>
> Durum bilgisi gerçek gözlemden gelmeli.
>
> AI'ın kendi hasarını icat etmesine izin verme.

## English

> Show [GARMENT] as a flat technical view and mark observed condition using four categories:
>
> good, wear, repaired, missing or damaged.
>
> Condition information must come from real inspection.
>
> Do not let the model invent defects.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1548. `/secondhand-sidequest-slop-filter` — Secondhand AI Slop Filtresi

Kaçınılması gerekenler:

- vintage = kir,
- deadstock = distressed,
- provenance uydurmak,
- her onarımı dekoratif patch yapmak,
- ikinci el ürünü kusursuzlaştırmak,
- kültürel onarım tekniklerini yüzeysel motif olarak kullanmak,
- gerçek condition bilgisini gizlemek.

---

# 1549. Adobe 2026: `/sensory-closeup` — All the Feels Yakın Planı

## Trend

Adobe 2026 **All the Feels**, görselin yalnız görüntüyü değil dokunma, tat, ses ve malzeme hissini çağrıştırmasını öne çıkarıyor.

## Türkçe prompt

> [NESNE/YİYECEK/MALZEME]'yi birincil duyusal özelliği üzerinden yakın planda göster.
>
> Tek duyuyu seç:
>
> - çıtırlık,
> - yumuşaklık,
> - yapışkanlık,
> - lif,
> - buhar,
> - soğuk yüzey,
> - kuru toz
>
> gibi.
>
> Aynı karede her duyuyu abartma.

## English

> Show [OBJECT/FOOD/MATERIAL] in close-up through one primary sensory cue such as crispness, softness, stickiness, fibers, steam, cold surface, or dry powder.
>
> Avoid exaggerating every sensory cue at once.

---

# 1550. `/texture-sequence` — Dokunun Zaman İçindeki Davranışı

## Türkçe

> [MALZEME/YİYECEK]'in dokusunu üç aşamada göster:
>
> başlangıç → etkileşim → sonuç.
>
> Örneğin:
>
> kırılmadan önce → kırılırken → kırıntı.
>
> Aynı nesne ve kamera devam etsin.

## English

> Show the texture behavior of [MATERIAL/FOOD] in three stages:
>
> before interaction → during interaction → result.
>
> Preserve the same object and camera.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1551. `/sound-implied-photo` — Sesi Görselden Hissettirme

## Türkçe

> [OLAY]'ı ses duygusunu görsel ipuçlarıyla hissettiren fotoğraf olarak göster:
>
> çarpan zil,
> kırılan kabuk,
> alkışlayan eller,
> kahve öğütücü,
> yağmurun yüzeye vurması
>
> gibi.
>
> Görsele dekoratif waveform ekleme.

## English

> Photograph [EVENT] so the viewer can almost infer the sound through visible physical cues such as ringing metal, cracking crust, clapping hands, a grinder in motion, or rain striking a surface.
>
> Do not add decorative waveforms.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1552. `/material-touch-board` — Dokunma Odaklı Malzeme Panosu

## Türkçe

> [ÜRÜN/MEKÂN] için malzemeleri yalnız renk örneği olarak değil dokunma davranışıyla göster:
>
> pürüzlü,
> yumuşak,
> sık dokulu,
> soğuk,
> kuru,
> parlak/kaygan.
>
> Her swatch gerçek yüzey yakın planı ve kısa fiziksel descriptor taşısın.

## English

> Present materials for [PRODUCT/SPACE] not only through color but through tactile behavior such as rough, soft, tightly woven, cool, dry, or slick.
>
> Give every swatch one real close surface view and a concise physical descriptor.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1553. `/shared-task-candid` — Birlikte Bir Şey Yapan İnsanlar

## Trend

Adobe 2026 **Connectioneering** temasının en pratik prompt karşılıklarından.

## Türkçe

> 2–4 kişiyi kameraya poz verirken değil, gerçekten ortak bir işi yaparken göster:
>
> yemek hazırlamak,
> tamir,
> oyun,
> çizim,
> bahçe,
> proje,
> masa kurmak
>
> gibi.
>
> Eller ve bakışlar ortak göreve yönelsin.
>
> “Diversity stock photo” gibi kameraya gülümseyen sıra insan üretme.

## English

> Show 2–4 people genuinely doing one shared task rather than posing for the camera, such as cooking, repairing, playing, drawing, gardening, building, or setting a table.
>
> Let hands and gaze focus on the shared activity.
>
> Avoid the generic stock-photo line of people smiling at the camera.

---

# 1554. `/hands-together-detail` — Ortak Eylem El Ayrıntısı

## Türkçe

> Birlikte yapılan [EYLEM]'in yalnız eller ve kullanılan nesne üzerinden close detail karesini oluştur.
>
> Farklı eller aynı fiziksel göreve katkı versin.
>
> Sembolik “eller üst üste” takım fotoğrafı üretme.

## English

> Show a close detail of [SHARED ACTION] through hands and the object being used.
>
> Let different hands contribute to the same real task.
>
> Avoid the symbolic stacked-hands team-photo cliché.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1555. `/intergenerational-making` — Kuşaklar Arası Üretim

## Türkçe

> Farklı yaşlardan iki kişinin aynı gerçek zanaat/gündelik beceri üzerinde birlikte çalıştığı doğal sahne oluştur.
>
> Bir kişi anlatabilir, diğeri deneyebilir.
>
> Yaşlı kişiyi otomatik “bilge usta”, genç kişiyi “öğrenen çocuk” klişesine indirgeme.

## English

> Show two people of different generations naturally working together on one real craft or everyday skill.
>
> One may demonstrate while the other experiments.
>
> Avoid reducing the older person to a wise-master stereotype and the younger person to a passive learner.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1556. `/connection-slop-filter` — Connectioneering AI Slop Filtresi

Kaçınılması gerekenler:

- kameraya gülen ekip,
- eller üst üste,
- yapay “diverse office” stoğu,
- herkesin aynı anda gülmesi,
- fiziksel etkileşimin olmaması,
- ortamın jenerik coworking ofis olması,
- “authentic” = kötü crop + grain sanmak.

---

# 1557. `/local-shopfront` — Yerel Dükkân Cephesi

## Trend

Adobe 2026 **Local Flavor**, kültürel özgüllüğü yerel insan, yer, zanaat ve gerçek gündelik hayat üzerinden tanımlıyor.

## Türkçe prompt

> [ŞEHİR/MAHALLE]'de gerçekçi küçük yerel dükkân cephesi oluştur.
>
> Yerel kimlik:
>
> - tabela dili,
> - malzeme,
> - vitrin düzeni,
> - sokak ölçüsü,
> - gündelik kullanım
>
> üzerinden gelsin.
>
> Turistik landmark sticker'ları veya “oriental/exotic” klişeleri kullanma.

## English

> Create a believable small local storefront in [CITY/NEIGHBORHOOD].
>
> Express locality through signage language, materials, window display, street scale, and everyday use.
>
> Avoid tourist-landmark stickers and exoticizing visual clichés.

---

# 1558. `/vernacular-signage` — Yerel Tabela Dili

## Türkçe

> [BÖLGE]'nin gerçek yerel signage karakterinden esinlenen küçük tabela seti oluştur.
>
> Yazı biçimi, malzeme, boya, ölçü ve montaj çevredeki gerçek üretim alışkanlıklarına dayansın.
>
> Dili yanlış yazma veya tüm bölgeyi tek “folkloric font” ile temsil etme.

## English

> Create a small signage set inspired by the real vernacular sign-making practices of [REGION].
>
> Base letterform, material, paint, scale, and mounting on plausible local production methods.
>
> Avoid misspelled language and reducing an entire region to one folkloric font.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1559. `/local-object-portrait` — Yerel Nesne Portresi

## Türkçe

> [YER]'i landmark yerine o yerde gerçekten kullanılan tek gündelik nesne üzerinden anlat:
>
> çay bardağı,
> pazar kasası,
> yerel otobüs bileti,
> ekmek kabı,
> zanaat aleti,
> sokak sandalyesi
>
> gibi.
>
> Nesneyi gerçek bağlamında fotoğraflanmış gibi göster.

## English

> Represent [PLACE] through one genuine everyday local object rather than a landmark, such as a tea glass, market crate, transit ticket, bread container, craft tool, or street chair.
>
> Show the object within its real context.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1560. `/local-material-palette` — Yerel Malzeme Paleti

## Türkçe

> [YER]'den 6 gerçek malzeme/yüzey seç:
>
> taş,
> ahşap,
> sıva,
> kumaş,
> metal,
> seramik
>
> gibi.
>
> Palette renklerden çok fiziksel malzeme ve yaşlanma davranışını göstersin.
>
> Bölgeye ait olmayan “rustic texture” ekleme.

## English

> Select six real materials or surfaces from [PLACE], such as stone, wood, plaster, textile, metal, or ceramic.
>
> Show physical material and aging behavior rather than only a color palette.
>
> Do not add generic rustic textures unrelated to the location.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1561. `/craft-provenance-board` — Yerel Zanaat Köken Panosu

## Türkçe

> [ZANAAT]'ı yalnız bitmiş süs ürünü olarak değil:
>
> - malzeme,
> - araç,
> - üretim adımı,
> - usta eli,
> - final parça
>
> üzerinden küçük provenance/process board olarak anlat.
>
> Motifi bağlamından koparıp dekoratif pattern'e indirgeme.

## English

> Present [CRAFT] through a small provenance and process board showing material, tool, making step, maker’s hand, and finished object.
>
> Do not detach the motif from context and reduce it to decorative pattern.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1562. `/local-language-poster` — Yerel Dil / Gerçek Yazı Kullanımı

## Türkçe

> [YER/KAMPANYA] posterinde yerel dili yalnız dekoratif birkaç kelime olarak değil ana tipografik iletişim dili olarak doğru kullan.
>
> Yazım ve anlam doğrulanmalı.
>
> Yerel alfabenin biçimini “exotic font” olarak bozma.

## English

> Use the local language of [PLACE/CAMPAIGN] as the actual primary communication language rather than as decorative vocabulary.
>
> Verify spelling and meaning.
>
> Do not distort the writing system into an exotic display font.

## Neye dikkat edilmeli?

Kondisyon dürüst gösterilsin: yıpranma gizlenmesin, köken etiketi belgelenebilir olsun.

---
# 1563. `/local-flavor-slop-filter` — Local Flavor AI Slop Filtresi

Kaçınılması gerekenler:

- landmark kolajı,
- bayrak rengi = kültür,
- rastgele geleneksel motif,
- “exotic” insan,
- yanlış yerel alfabe,
- kültürü yalnız yemekle temsil etmek,
- bütün şehirleri vintage postcard yapmak,
- turistik imgeyi gündelik hayat sanmak,
- gerçek yerel üreticiyi/insanı görünmez bırakmak.

---

# 1564. `/one-rule-surreal` — Tek Fizik Kuralı Bozulan Sürrealizm

## Adobe 2026 Surreal Silliness ile uyumlu

## Türkçe

> Normal ve tanınabilir [SAHNE]'de yalnız bir fizik kuralını değiştir:
>
> - bir nesne aşırı büyük,
> - yerçekimi tek nesnede ters,
> - sert nesne yumuşak malzeme gibi davranıyor,
> - gölge farklı nesneye ait.
>
> Geri kalan dünya tamamen normal kalsın.
>
> Beş farklı sürreal fikri aynı kareye koyma.

## English

> Alter only one physical rule inside an otherwise normal and recognizable [SCENE]:
>
> one object becomes oversized, gravity reverses for one object, a hard object behaves like soft material, or a shadow belongs to something else.
>
> Keep the rest of the world completely ordinary.
>
> Do not combine five surreal concepts in one frame.

## Neye dikkat edilmeli?

Tek kural bozulsun, gerisi fiziğe uysun; çok sapma tek fikri öldürür.

---
# 1565. `/absurd-product-use` — Ürünü Absürt ama Tek Fikirli Kullanma

## Türkçe

> [ÜRÜN]'ü tek absürt kullanım fikri içinde göster.
>
> Ürünün gerçek formu tanınabilir kalsın.
>
> Absürtlük:
>
> - ölçek,
> - bağlam,
> - malzeme,
> - işlev kayması
>
> seçeneklerinden yalnız biri olsun.
>
> Ürünü tamamen başka nesneye dönüştürme.

## English

> Show [PRODUCT] through one absurd usage idea while keeping the product recognizable.
>
> Make the absurdity come from only one dimension: scale, context, material, or shifted function.
>
> Do not transform the product into an unrelated object.

## Neye dikkat edilmeli?

Tek kural bozulsun, gerisi fiziğe uysun; çok sapma tek fikri öldürür.

---
# 1566. `/surreal-silliness-slop-filter` — Sürreal AI Slop Filtresi

Kaçınılması gerekenler:

- rastgele uçan meyve,
- melting clock kopyası,
- her yüzeye göz,
- dev insan + minik şehir klişesi,
- 10 fizik kuralı aynı anda,
- anlamsız neon portal,
- “surreal” = rastgele kolaj,
- sürreal fikrin ürün/mesajla hiçbir ilişkisi olmaması.

---

# 1567. Yeni üst aile: `Culturally Grounded Visual`

Aile:

- `/local-shopfront`
- `/vernacular-signage`
- `/local-object-portrait`
- `/local-material-palette`
- `/craft-provenance-board`
- `/local-language-poster`
- city souvenir aileleri
- heritage packaging
- local food / local transit görselleri.

Ortak kural:

> **Kültür, dekoratif motif değil yaşayan bağlamdır.**

Prompt formülü:

> **place + real people/use + material + language + ordinary object + verified specificity**

---

# 1568. Yeni üst aile: `Sensory Visual`

Aile:

- `/sensory-closeup`
- `/texture-sequence`
- `/sound-implied-photo`
- `/material-touch-board`
- tactile food macro,
- material study,
- sound-to-visual.

Ortak kural:

> **Bir karede tek baskın duyusal ipucu.**

---

# 1569. Yeni üst aile: `Repair / Provenance Visual`

Aile:

- `/provenance-tag`
- `/repair-aesthetic-board`
- `/sashiko-inspired-repair`
- `/patchwork-leather-repair`
- `/visible-mending`
- `/deadstock-archive`
- `/secondhand-catalog`
- `/condition-map-garment`
- `/object-biography`.

Ortak soru:

> **Bu nesne nereden geldi, nasıl kullanıldı, nasıl değişti?**

---

# 1570. `/context-not-costume` — Bağlam, Kostüm Değil

## Yeni rehber kontrolü

Yerel, tarihsel veya alt-kültür promptlarında:

> `/context-not-costume`

## Türkçe açılım

> Kültürel veya tarihsel kimliği kostüm, aksesuar ve motif yığınıyla anlatma. Önce gerçek mekân, kullanım, malzeme, davranış ve dil bağlamını kur. Gerekli sembolleri daha sonra ve sınırlı ekle.

## English

> Do not represent cultural or historical identity through a pile of costumes, accessories, and motifs. Build real place, use, material, behavior, and language context first, then add symbols only where necessary.

## Neye dikkat edilmeli?

Bağlam kurulmadan eklenen her sembol klişeye kayar; sembol sayısı sınırlı tutulsun, her sembolün gerekçesi sorulsun.

---

# 1571. `/claim-safe-visual` — İddia Güvenliği Bloğu

## Kullanım

Astroloji, kristal, wellness, herbal, tarihsel spekülasyon ve benzeri alanlarda.

## Türkçe

> Görsel kültürel/kişisel pratikleri estetik olarak gösterebilir ancak bilimsel, tıbbi, tarihsel veya kişisel sonucu kanıtlanmış gerçek gibi sunmasın. Ölçülmemiş, doğrulanmamış veya spekülatif öğeleri açıkça ayır.

## English

> The visual may represent cultural or personal practices aesthetically, but it must not present unverified scientific, medical, historical, or personal outcomes as established fact. Clearly distinguish measured, verified, and speculative content.

## Neye dikkat edilmeli?

Tek kural bozulsun, gerisi fiziğe uysun; çok sapma tek fikri öldürür.

---
# 1572. Bu turdaki slash-style indeks (aile-021)

| Kısayol | Aile |
|---|---|
| `/kitchen-apothecary` | practical pantry apothecary |
| `/spice-blending-board` | ingredient/proportion board |
| `/herbal-infusion-card` | non-medical infusion preparation |
| `/beeswax-wrap-process` | reusable wrap making |
| `/fermentation-shelf` | batch-based fermentation display |
| `/pantry-label-system` | readable pantry labels |
| `/celestial-journal` | sky-observation journal |
| `/moon-phase-observation` | moon-phase sequence |
| `/celestial-field-card` | sky field guide |
| `/astrology-chart-design` | astrology data as graphic design |
| `/astrocartography-map-design` | supplied astrocartography map |
| `/crystal-display` | mineral specimen presentation |
| `/celestial-symbol-sheet` | astronomy/celestial symbols |
| `/equestrian-outfit-board` | equestrian-inspired outfit system |
| `/barn-jacket-editorial` | functional barn-jacket portrait |
| `/rosette-ribbon` | fabric rosette |
| `/equestrian-gear-flatlay` | riding equipment flat lay |
| `/stable-field-guide` | beginner equipment guide |
| `/horse-motif-patch` | restrained horse/equestrian patch |
| `/deadstock-archive` | unused archive stock catalog |
| `/archive-streetwear-board` | archival clothing selection |
| `/provenance-tag` | object history tag |
| `/repair-aesthetic-board` | matched repair methods |
| `/sashiko-inspired-repair` | context-aware visible repair |
| `/corset-back-conversion` | structural garment conversion |
| `/patchwork-leather-repair` | deadstock leather repair |
| `/secondhand-catalog` | honest resale documentation |
| `/condition-map-garment` | garment condition mapping |
| `/sensory-closeup` | one dominant tactile/sensory cue |
| `/texture-sequence` | texture through time/action |
| `/sound-implied-photo` | photograph suggesting sound |
| `/material-touch-board` | tactile material comparison |
| `/shared-task-candid` | people doing one real task |
| `/hands-together-detail` | shared-action hand detail |
| `/intergenerational-making` | cross-generation making |
| `/local-shopfront` | real local storefront |
| `/vernacular-signage` | locally grounded signage |
| `/local-object-portrait` | place represented by everyday object |
| `/local-material-palette` | place-specific material palette |
| `/craft-provenance-board` | craft process and provenance |
| `/local-language-poster` | verified local-language design |
| `/one-rule-surreal` | one controlled impossible rule |
| `/absurd-product-use` | one absurd product idea |
| `/context-not-costume` | cultural-context safeguard |
| `/claim-safe-visual` | separate culture from factual claims |

---

<a id="aile-022"></a>
# Refill–Reuse Ambalaj, Erişilebilir Sergi, Haptik Müze ve İnsan Eli İllüstrasyonu — 2026 Ek Taraması

Bu turda dört alan öne çıktı:

- **refill / reuse / mono-material packaging**,
- **erişilebilir ve inclusive exhibition design**,
- **haptic-mediated museum experiences**,
- **“made by humans” hissini süreç üzerinden kuran illüstrasyon**.

World Packaging Organisation'ın 2026 trend özetinde ambalaj için açık biçimde:

- mono-material flexible packaging,
- refill and reuse systems,
- advanced fiber-based solutions,
- yüksek recycled content,
- structural optimization,
- smart packaging / QR / traceability

başlıkları öne çıkıyor.

Bu yüzden “sustainable packaging” promptunu yalnız:

> kraft kâğıt + yeşil yaprak + recycle icon

şeklinde kullanmak artık özellikle yetersizdir.

Aynı şekilde 2026 müze araştırmalarında erişilebilirlik ve haptik deneyim, sonradan eklenen bir özellik değil; sergi mimarisinin başından itibaren tasarlanan bir **mediation layer** olarak ele alınıyor.

---

# 1573. `/refill-system` — Refill / Yeniden Dolum Sistemi

## Trend

**T1 — 2026 packaging trend raporlarında ana başlıklardan.**

## Türkçe prompt

> [ÜRÜN] için tek kullanımlık ambalaj yerine gerçek refill system tasarla.
>
> Sistem iki ana parçaya ayrılsın:
>
> 1. uzun ömürlü ana kap,
> 2. daha az malzemeli refill ünitesi.
>
> Ana kap:
>
> - temizlenebilir,
> - tekrar doldurulabilir,
> - rahat tutulabilir,
> - kolay açılıp kapanabilir
>
> olsun.
>
> Refill paketi ana kabın içine fiziksel olarak aktarılabilsin.
>
> “Refill” etiketi yazılmış normal ikinci şişe üretme.

## English

> Design a real refill system for [PRODUCT] rather than a disposable package labeled “refill.”
>
> Separate the system into:
>
> 1. a durable reusable primary container,
> 2. a lower-material refill unit.
>
> Make the primary container cleanable, refillable, easy to hold, and easy to open and close.
>
> The refill should transfer physically into the main container.

---

# 1574. `/refill-station` — Yeniden Dolum İstasyonu

## Türkçe

> [ÜRÜN] için mağaza içi refill station tasarla.
>
> Kullanıcı akışı:
>
> 1. kabı yerleştir,
> 2. ürünü seç,
> 3. miktarı ölç,
> 4. doldur,
> 5. etiketi/fişi al.
>
> Her adım fiziksel olarak anlaşılır olsun.
>
> İstasyonu sci-fi vending machine veya hologram kioska dönüştürme.

## English

> Design an in-store refill station for [PRODUCT] with a clear user flow:
>
> place container → choose product → measure amount → refill → receive label or receipt.
>
> Make every physical step understandable.
>
> Avoid futuristic vending-machine or holographic-kiosk styling.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1575. `/returnable-pack` — İade Edilebilir Ambalaj

## Türkçe

> [ÜRÜN] için depozitolu/returnable packaging sistemi tasarla.
>
> Ambalaj:
>
> - çoklu kullanım,
> - taşıma,
> - yıkama,
> - yeniden dolum,
> - istifleme
>
> döngüsüne dayanacak formda olsun.
>
> Tek kullanımlık ince ambalajı yalnız “return me” etiketiyle iade edilebilir gibi gösterme.

## English

> Design returnable packaging for [PRODUCT] that can survive repeated transport, washing, refilling, and stacking.
>
> Do not take lightweight disposable packaging and simply add a “return me” label.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1576. `/reuse-loop` — Ambalaj Döngüsü

## Türkçe

> [AMBALAJ]'ın reuse loop'unu 5 adımda göster:
>
> kullanım → iade → kontrol/yıkama → refill → yeniden dağıtım.
>
> Her adım gerçek operasyonel nesne/işlem taşısın.
>
> Döngüyü sadece recycle arrows ikonu ile temsil etme.

## English

> Show the reuse loop for [PACKAGE] in five real operational stages:
>
> use → return → inspection/washing → refill → redistribution.
>
> Do not reduce the system to a generic recycling-arrow icon.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1577. `/mono-material-pack` — Mono-material Ambalaj

## Trend

**T1 — 2026 packaging innovation başlıklarından.**

## Türkçe

> [ÜRÜN] için mümkün olduğunca tek ana malzeme ailesinden mono-material packaging tasarla.
>
> Etiket, kapak, bariyer ve ana gövdenin recycling stream ile uyumu düşünülmeli.
>
> “Sustainable” görünmek için farklı doğal dokuları üst üste ekleme.
>
> Malzeme sadeliği fiziksel sistemden gelsin.

## English

> Design mono-material packaging for [PRODUCT] using one primary material family wherever practical.
>
> Consider compatibility of label, closure, barrier, and body with the intended recycling stream.
>
> Do not signal sustainability by layering unrelated natural textures.

---

# 1578. `/fiber-packaging` — Fiber-based Ambalaj

## Türkçe

> [ÜRÜN]'ü koruyacak fiber-based packaging sistemi tasarla.
>
> Pulp/fiber kalınlığı, köşe güçlendirme, tutma noktası ve nesting mantığı fiziksel olarak çalışsın.
>
> Plastik blister geometrisini sadece kahverengi kâğıt dokusuna çevirme.

## English

> Design fiber-based packaging for [PRODUCT] with physically plausible pulp or fiber thickness, reinforced corners, grip points, and nesting logic.
>
> Do not simply repaint plastic blister geometry with brown-paper texture.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1579. `/molded-pulp-insert` — Kalıplanmış Selüloz İç Yatak

## Türkçe

> [ÜRÜN]'ün gerçek geometrisine oturan molded-pulp insert oluştur.
>
> Yatak:
>
> - kritik temas noktalarını desteklesin,
> - darbeye karşı boşluk yaratsın,
> - ürünü çıkarmayı zorlaştırmasın,
> - gereksiz malzeme kullanmasın.
>
> Ürünü havada tutan imkânsız ince pulp yüzeyler üretme.

## English

> Create a molded-pulp insert fitted to the real geometry of [PRODUCT].
>
> Support critical contact points, allow impact clearance, keep product removal practical, and minimize unnecessary material.
>
> Avoid impossibly thin pulp structures holding the product in mid-air.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1580. `/packaging-nesting` — İstifleme / İç İçe Geçme Optimizasyonu

## Türkçe

> Boş [AMBALAJ]'ların taşıma sırasında iç içe geçerek veya kompakt biçimde istiflenerek hacim azaltmasını göster.
>
> Full ve empty durumlarını karşılaştır.
>
> Form yalnız rafta güzel değil lojistikte de anlamlı olsun.

## English

> Show how empty [PACKAGES] nest or stack compactly to reduce logistics volume.
>
> Compare full and empty states.
>
> Make the form work operationally rather than only look attractive on shelf.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1581. `/packaging-logistics-board` — Ambalaj + Lojistik Panosu

## Türkçe

> [AMBALAJ]'ı yalnız hero mockup olarak değil:
>
> - tek ürün,
> - koli içi,
> - palet,
> - raf,
> - boş ambalaj geri dönüşü
>
> bağlamlarında tek board üzerinde göster.
>
> Ambalaj geometrisinin lojistiğe etkisi anlaşılabilsin.

## English

> Show [PACKAGE] across real logistics contexts on one board:
>
> single unit, shipping case, pallet, retail shelf, and empty-package return.
>
> Make the effect of packaging geometry on logistics visible.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1582. `/traceability-pack` — İzlenebilirlik Ambalajı

## Trend

**T1 — packaging as data carrier.**

## Türkçe

> [ÜRÜN] ambalajında traceability bilgisini küçük ama gerçek bilgi mimarisi içinde göster.
>
> Kullanıcı:
>
> - lot/batch,
> - üretim tarihi,
> - kaynak,
> - QR/data link
>
> bilgisine ulaşabilsin.
>
> Rastgele blockchain, NFC ve QR ikonlarını birlikte kullanma.

## English

> Integrate traceability into [PRODUCT] packaging through a clear information architecture for lot or batch, production date, source, and one digital data link where appropriate.
>
> Avoid stacking blockchain, NFC, and QR icons without function.

---

# 1583. `/recycled-content-honest` — Geri Dönüştürülmüş İçeriği Dürüst Gösterme

## Türkçe

> Ambalajın recycled-content oranı kullanıcı tarafından verilmişse okunabilir küçük alanda göster.
>
> Belirsiz “eco”, “green”, “planet friendly” rozetleri üretme.
>
> Yüzeyde recycled fiber speckle görünmesi gerçek malzeme davranışından gelsin; dekoratif overlay olmasın.

## English

> Show recycled-content percentage only when supplied by the user.
>
> Avoid vague “eco,” “green,” or “planet friendly” badges.
>
> Any visible recycled-fiber speckling should emerge from actual material behavior rather than decorative overlay.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1584. `/sustainability-claim-lock` — Sürdürülebilirlik İddiası Kilidi

## Türkçe

> Çevresel fayda yalnız kullanıcı tarafından sağlanan veya doğrulanmış bilgiye dayanmalı.
>
> “Compostable”, “biodegradable”, “recyclable”, “carbon neutral”, “plastic free” gibi ifadeleri tasarım tamamlamak için uydurma.

## English

> Environmental claims must come only from supplied or verified information.
>
> Do not invent claims such as compostable, biodegradable, recyclable, carbon neutral, or plastic free to complete the design.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1585. `/circular-packaging-board` — Döngüsel Ambalaj Karar Panosu

## Türkçe

> [ÜRÜN] için dört circular packaging yaklaşımını aynı işlev üzerinden karşılaştır:
>
> A — reuse  
> B — refill  
> C — mono-material recycle  
> D — fiber-based
>
> Aynı ürün miktarı, koruma gereksinimi ve dağıtım senaryosu kullan.
>
> Her seçeneğin malzeme/operasyon farkını kısa notla belirt.
>
> Bir yaklaşımı estetik olarak “daha yeşil” göstermeyin.

## English

> Compare four circular-packaging approaches for the same [PRODUCT]:
>
> A — reuse  
> B — refill  
> C — mono-material recycling  
> D — fiber-based.
>
> Keep product quantity, protection needs, and distribution scenario matched.
>
> Annotate material and operational differences without visually favoring one option through “greener” styling.

## Neye dikkat edilmeli?

Döngü iddiası mekanizmayla gösterilsin: dolum, iade ve yıkama adımları eksikse iddia kilitlenir (§1584).

---
# 1586. `/circular-pack-slop-filter` — Sürdürülebilir Ambalaj AI Slop Filtresi

Kaçınılması gerekenler:

- kraft = sustainable,
- yeşil yaprak = eco,
- sahte recycle badge,
- uydurma compostable iddiası,
- refill adı altında ikinci disposable bottle,
- mono-material deyip 4 farklı malzeme kullanmak,
- lojistik/temizlik/dolum döngüsünü düşünmemek,
- camı her durumda otomatik “daha sürdürülebilir” varsaymak,
- sustainability ile “rustic organic aesthetic”i karıştırmak.

---

# 1587. `/inclusive-exhibition` — Inclusive Exhibition Design

## Trend

**T1 — 2026 müze interaction-design araştırmalarında inclusive design yeni ana yönlerden biri.**

## Türkçe prompt

> [SERGİ]'yi tek “ideal ziyaretçi” varsaymadan tasarla.
>
> Aynı içerik için mümkün olduğunda:
>
> - ayakta,
> - oturarak,
> - farklı görüş yüksekliğinden,
> - görsel,
> - işitsel,
> - dokunsal
>
> erişim seçenekleri düşün.
>
> Erişilebilirliği sergi bittikten sonra eklenen yan panel gibi tasarlama.

## English

> Design [EXHIBITION] without assuming one ideal visitor.
>
> Where relevant, provide access from standing and seated positions, different viewing heights, and visual, auditory, or tactile modes.
>
> Do not treat accessibility as an add-on panel after the exhibition is already designed.

---

# 1588. `/multi-height-display` — Farklı Görüş Yükseklikleri

## Türkçe

> [SERGİ/VİTRİN]'de kritik bilgi ve eser görünürlüğünü:
>
> - çocuk,
> - oturan ziyaretçi,
> - ayakta yetişkin
>
> görüş yüksekliklerinde kontrol et.
>
> Her şeyi tek ortalama yetişkin göz seviyesine yerleştirme.

## English

> Test critical exhibit and label visibility from child height, seated visitor height, and standing adult height.
>
> Avoid placing everything for one average standing eye level.

## Neye dikkat edilmeli?

Tasarım gerçek bedenle test edilsin: oturarak görüş, uzanma mesafesi ve okuma yüksekliği varsayılmasın, ölçülsin.

---
# 1589. `/seated-view-audit` — Oturarak Görüş Denetimi

## Türkçe

> Sergi mekânını wheelchair/seated eye-level viewpoint'tan audit et.
>
> Kontrol:
>
> - vitrin içi görüş,
> - label,
> - interaktif ekran,
> - masa altı boşluk,
> - dönüş alanı.
>
> Zemine yalnız erişilebilir rota çizgisi ekleyip sorunu çözülmüş sayma.

## English

> Audit the exhibition from a seated or wheelchair eye-level viewpoint, checking case visibility, labels, interactive screens, knee clearance, and turning space.
>
> Do not assume accessibility is solved by adding a route line on the floor.

## Neye dikkat edilmeli?

Tasarım gerçek bedenle test edilsin: oturarak görüş, uzanma mesafesi ve okuma yüksekliği varsayılmasın, ölçülsin.

---
# 1590. `/low-vision-label` — Düşük Görme İçin Eser Etiketi

## Türkçe

> [ESER LABEL]'ını güçlü kontrast, yeterli font boyutu, açık satır aralığı ve sade hiyerarşiyle tasarla.
>
> Yazıyı eser estetiğine uydurmak için düşük kontrast veya ince dekoratif font kullanma.
>
> Gerekirse kısa label + uzun alternatif format ayrımı yap.

## English

> Design [OBJECT LABEL] with strong contrast, sufficient type size, clear line spacing, and restrained hierarchy.
>
> Do not sacrifice legibility through low contrast or decorative thin type to match the artwork.
>
> Separate concise wall text from optional longer interpretation where useful.

## Neye dikkat edilmeli?

Tasarım gerçek bedenle test edilsin: oturarak görüş, uzanma mesafesi ve okuma yüksekliği varsayılmasın, ölçülsin.

---
# 1591. `/easy-read-exhibit` — Easy-read Sergi Metni

## Türkçe

> [SERGİ BİLGİSİ]'ni easy-read formatında düzenle.
>
> Her bölüm:
>
> - tek ana fikir,
> - kısa cümle,
> - açık başlık,
> - gerektiğinde anlamlı görsel
>
> kullansın.
>
> Çocukça bir tona veya emoji diline dönüştürme.

## English

> Structure [EXHIBITION INFORMATION] in an easy-read format using one main idea per section, short sentences, clear headings, and meaningful imagery only where needed.
>
> Do not turn the tone childish or replace language with emojis.

## Neye dikkat edilmeli?

Tasarım gerçek bedenle test edilsin: oturarak görüş, uzanma mesafesi ve okuma yüksekliği varsayılmasın, ölçülsin.

---
# 1592. `/sensory-map-museum` — Müze Duyusal Haritası

## Türkçe

> [MÜZE/SERGİ]'nin sensory map'ini oluştur.
>
> Alanlar:
>
> - yüksek ses,
> - düşük ışık,
> - parlak ışık,
> - yoğun kalabalık,
> - güçlü koku,
> - sakin alan
>
> gibi gerçek gözlem/veriye göre işaretlensin.
>
> Kullanıcı kendi rotasını planlayabilsin.
>
> Veri yoksa sensory risk uydurma.

## English

> Create a sensory map for [MUSEUM/EXHIBITION] marking real observed or supplied areas such as loud sound, low light, bright light, crowds, strong smell, and quiet zones.
>
> Help visitors plan their route.
>
> Do not invent sensory conditions without evidence.

## Neye dikkat edilmeli?

Tasarım gerçek bedenle test edilsin: oturarak görüş, uzanma mesafesi ve okuma yüksekliği varsayılmasın, ölçülsin.

---
# 1593. `/quiet-route` — Düşük Uyaranlı Rota

## Türkçe

> Aynı sergide daha düşük ses/ışık/kalabalık maruziyeti sunan quiet route tasarla.
>
> Temel sergi içeriğinin önemli bölümüne yine erişebilsin.
>
> Quiet route'u “arka servis koridoru” gibi ikincil ve değersiz göstermeyin.

## English

> Design a quieter route through the same exhibition with reduced exposure to noise, intense light, or crowds while preserving access to meaningful core content.
>
> Do not treat the quiet route as an inferior back corridor.

## Neye dikkat edilmeli?

Tasarım gerçek bedenle test edilsin: oturarak görüş, uzanma mesafesi ve okuma yüksekliği varsayılmasın, ölçülsin.

---
# 1594. `/exhibit-rest-point` — Dinlenme / Regülasyon Noktası

## Türkçe

> Sergi akışı içinde gerçek bir rest point tasarla.
>
> Oturma, yön bilgisi ve düşük bilgi yoğunluğu olsun.
>
> Kullanıcının sergi dışına çıkmadan kısa süreli dinlenebilmesini sağla.
>
> Alanı sponsor logosu ve reklam ekranlarıyla doldurma.

## English

> Design a real rest point within the exhibition flow using seating, orientation information, and low information density.
>
> Let visitors pause without leaving the exhibition.
>
> Avoid filling the space with sponsor logos and advertising screens.

## Neye dikkat edilmeli?

Tasarım gerçek bedenle test edilsin: oturarak görüş, uzanma mesafesi ve okuma yüksekliği varsayılmasın, ölçülsin.

---
# 1595. `/inclusive-interactive-height` — Erişilebilir İnteraktif Yüksekliği

## Türkçe

> [ETKİLEŞİMLİ SERGİ]'de ekran/düğme/nesne erişim yüksekliğini farklı kullanıcılar için test et.
>
> Kritik kontrol tek yüksek noktada olmasın.
>
> Ekran tilt ve glare davranışını da düşün.

## English

> Test screen, button, and object reach in [INTERACTIVE EXHIBIT] across different user heights and positions.
>
> Avoid placing critical controls only at one high level.
>
> Account for screen tilt and glare.

## Neye dikkat edilmeli?

Tasarım gerçek bedenle test edilsin: oturarak görüş, uzanma mesafesi ve okuma yüksekliği varsayılmasın, ölçülsin.

---
# 1596. `/inclusive-exhibition-slop-filter` — Inclusive Sergi AI Slop Filtresi

Kaçınılması gerekenler:

- erişilebilirlik = wheelchair icon,
- erişilebilir rota = mavi çizgi,
- bütün ekranlar yetişkin göz hizasında,
- dokunsal öğeyi çocuk aktivitesi gibi göstermek,
- düşük görme için yalnız font büyütmek,
- easy-read = çocuk dili,
- sensory map'i veri olmadan uydurmak,
- erişilebilir çözümü ana sergiden ayrı “special section” yapmak.

---

# 1597. `/haptic-object` — Dokunsal Eser Temsili

## Trend

**T1/T2 — 2026 Heritage Science review'unda haptic-mediated museum experiences önemli büyüyen alan.**

## Türkçe prompt

> Dokunulamayan [ESER/NESNE]'nin dokunsal öğrenme için fiziksel haptic replica'sını oluştur.
>
> Replica:
>
> - ana form,
> - önemli surface relief,
> - ölçek,
> - kavranabilir kritik yapı
>
> bilgilerini taşısın.
>
> Orijinal malzemeyi taklit etmek zorunda değil; dokunma ile okunabilirlik öncelikli olsun.
>
> Replica ile gerçek eseri karıştırmamak için açık etiket kullan.

## English

> Create a physical haptic replica of [ARTIFACT/OBJECT] for tactile learning where the original cannot be touched.
>
> Preserve primary form, important surface relief, scale relationships, and graspable structural information.
>
> Exact original material imitation is not required when tactile legibility is more important.
>
> Clearly identify the object as a replica.

---

# 1598. `/haptic-relief` — Dokunsal Kabartma Görsel

## Türkçe

> [2B GÖRSEL/HARİTA/ESER]'i tactile relief'e dönüştür.
>
> Yalnız dokunarak ayırt edilmesi gereken 3–5 ana seviye kullan.
>
> Görseldeki tüm ince ayrıntıları kabartmaya taşıma.
>
> Farklı yükseklik/tekstürler anlamlı kategori taşısın.

## English

> Convert [2D IMAGE/MAP/ARTWORK] into tactile relief using only 3–5 meaningful height or texture levels that can be distinguished by touch.
>
> Do not emboss every fine visual detail.
>
> Make relief differences correspond to meaningful information categories.

## Neye dikkat edilmeli?

Dokunsal öğe tek başına anlam taşısın; kabartma yüksekliği ve malzeme hedef kitleyle test edilsin.

---
# 1599. `/haptic-map` — Haptik / Dokunsal Harita

## Türkçe

> [MEKÂN]'ın dokunsal haritasında:
>
> - ana rota,
> - duvar/sınır,
> - giriş,
> - önemli hedef,
> - yön değişimi
>
> parmakla kolay ayırt edilsin.
>
> Görsel haritadaki bütün küçük oda ve ikonları taşımaya çalışma.

## English

> Create a haptic map where primary route, boundaries, entrance, important destinations, and directional changes are easy to distinguish by touch.
>
> Do not transfer every small room and visual icon from the sighted map.

## Neye dikkat edilmeli?

Dokunsal öğe tek başına anlam taşısın; kabartma yüksekliği ve malzeme hedef kitleyle test edilsin.

---
# 1600. `/haptic-timeline` — Dokunsal Zaman Çizelgesi

## Türkçe

> [TARİHSEL SÜREÇ]'i fiziksel çizgi boyunca dokunarak takip edilebilen timeline olarak tasarla.
>
> Kritik olaylar farklı node/form ile, dönemler farklı yüzey veya aralıkla ayrılabilir.
>
> Her tarih için ayrı karmaşık kabartma üretme.

## English

> Design [HISTORICAL PROCESS] as a tactile timeline that can be followed physically along one line.
>
> Mark critical events using distinct nodes or forms and separate periods through texture or spacing.
>
> Avoid complex relief for every date.

## Neye dikkat edilmeli?

Dokunsal öğe tek başına anlam taşısın; kabartma yüksekliği ve malzeme hedef kitleyle test edilsin.

---
# 1601. `/haptic-cause-effect` — Dokunsal Neden–Sonuç Şeması

## Türkçe

> [SÜREÇ]'te neden ve sonucu tactile diagram olarak göster.
>
> Ana öğeler fiziksel node, ilişkiler kalın takip edilebilir bağlantılar olsun.
>
> Bağlantı sayısını sınırlı tut.
>
> Karmaşık network grafiğini bire bir kabartmaya aktarma.

## English

> Show [PROCESS] as a tactile cause-and-effect diagram with physical nodes and thick traceable connectors.
>
> Keep the number of relationships limited.
>
> Do not directly emboss a dense visual network diagram.

## Neye dikkat edilmeli?

Dokunsal öğe tek başına anlam taşısın; kabartma yüksekliği ve malzeme hedef kitleyle test edilsin.

---
# 1602. `/haptic-audio-pair` — Dokunma + Ses Eşleşmesi

## Türkçe

> Dokunsal [HARİTA/ESER/GRAFİK] üzerinde kullanıcı belirli noktaya dokunduğunda kısa audio description açılacak sistem tasarla.
>
> Dokunma ana spatial yapıyı, ses ise isim/detay bilgisini tamamlasın.
>
> İki kanalda aynı uzun metni tekrar etme.

## English

> Design a tactile [MAP/ARTIFACT/CHART] where touching selected points triggers concise audio description.
>
> Let touch carry spatial structure and audio provide names or detail.
>
> Avoid repeating the same long information through both channels.

## Neye dikkat edilmeli?

Dokunsal öğe tek başına anlam taşısın; kabartma yüksekliği ve malzeme hedef kitleyle test edilsin.

---
# 1603. `/haptic-guidance` — Dokunsal Yönlendirme İpucu

## Türkçe

> Etkileşimli sergide haptic feedback'i:
>
> - doğru seçim,
> - sınır,
> - yön,
> - tamamlanma
>
> gibi tek işlevsel olaya bağla.
>
> Her dokunuşta titreşim verme.

## English

> Use haptic feedback in an interactive exhibit only for meaningful events such as confirmation, boundary, direction, or completion.
>
> Do not vibrate on every touch.

## Neye dikkat edilmeli?

Dokunsal öğe tek başına anlam taşısın; kabartma yüksekliği ve malzeme hedef kitleyle test edilsin.

---
# 1604. `/haptic-threshold` — Deneyim Geçişini Dokunmayla İşaretleme

## 2026 review ile ilişkili

Haptic-mediated museum research'unda **threshold orchestration** ziyaretçinin bir anlatı aşamasından diğerine geçtiğini hissettiren mekanizmalardan biri olarak inceleniyor.

## Türkçe

> Sergide önemli bölüm geçişinde tek tactile/haptic cue kullan.
>
> Örneğin:
>
> zemin değişimi,
> el rayında tekstür,
> kısa titreşim,
> fiziksel eşik.
>
> Geçiş işaretini sürekli tekrarlama.

## English

> Use one tactile or haptic cue at an important exhibition transition, such as a floor-texture change, handrail texture, brief vibration, or physical threshold.
>
> Do not repeat the transition cue continuously.

## Neye dikkat edilmeli?

Dokunsal öğe tek başına anlam taşısın; kabartma yüksekliği ve malzeme hedef kitleyle test edilsin.

---
# 1605. `/haptic-evaluation-board` — Haptik Deneyim Değerlendirme Panosu

## Türkçe

> [HAPTİK ETKİLEŞİM]'i yalnız “immersive / enjoyable” anketiyle değil şu açılardan değerlendir:
>
> - görev anlaşılabilirliği,
> - sensory congruence,
> - motor response,
> - accessibility,
> - fatigue,
> - error,
> - completion time.
>
> Kullanıcı değerlendirmesi yoksa başarı iddiası üretme.

## English

> Evaluate [HAPTIC INTERACTION] beyond generic “immersive” or “enjoyable” ratings through task clarity, sensory congruence, motor response, accessibility, fatigue, error, and completion time.
>
> Do not claim success without user evaluation.

## Neye dikkat edilmeli?

Dokunsal öğe tek başına anlam taşısın; kabartma yüksekliği ve malzeme hedef kitleyle test edilsin.

---
# 1606. `/haptic-slop-filter` — Haptik Sergi AI Slop Filtresi

Kaçınılması gerekenler:

- haptic = titreşim,
- her etkileşimde titreşim,
- dokunsal yüzeye bütün görsel detayları aktarmak,
- dokunsal kopyayı orijinal eser gibi göstermek,
- ses/dokunma ilişkisini düşünmemek,
- tactile element'i yalnız çocuklar için tasarlamak,
- erişilebilirlik iddiasını kullanıcı testi olmadan yapmak.

---

# 1607. `/childlike-line` — Kontrollü Çocukça Çizgi

## Trend

**T1/T2 — 2026 illustration trend raporlarında “childlike and playful” güçlü.**

Buradaki “childlike”:

> kötü çizim

demek değildir.

## Türkçe prompt

> [KONU]'yu sade, spontan, çocuk çizimini çağrıştıran ama kompozisyonu bilinçli line illustration olarak oluştur.
>
> Kullan:
>
> - tek kalem/marker hissi,
> - hafif düzensiz çizgi,
> - basit form,
> - sınırlı renk.
>
> Çizgileri bilgisizce bozuk yapma.
>
> Her nesneye yüz, yıldız ve kalp ekleme.

## English

> Illustrate [TOPIC] using spontaneous, childlike linework with deliberate composition.
>
> Use one pen or marker feel, slightly irregular line, simple forms, and limited color.
>
> Do not confuse childlike drawing with careless structure.
>
> Avoid adding faces, stars, and hearts to every object.

---

# 1608. `/naive-editorial-illustration` — Naive Editorial Illustration

## Türkçe

> [SOYUT KAVRAM/HABER]'ı tek güçlü görsel metaforla naive editorial illustration olarak anlat.
>
> Formlar sade, çizgiler hafif kusurlu olabilir.
>
> Metafor kavramla doğrudan ilişkili olsun.
>
> “Naive” diye anlamsız doodle kalabalığı oluşturma.

## English

> Explain [ABSTRACT CONCEPT/ARTICLE] through one strong visual metaphor using naive editorial illustration.
>
> Keep forms simple and linework slightly imperfect while maintaining deliberate structure.
>
> Avoid meaningless doodle clutter.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1609. `/rough-ink-editorial` — Kaba Mürekkep Editorial

## Türkçe

> [KONU]'yu kuru/kaba ink brush veya kalemle yapılmış editorial illustration olarak göster.
>
> Siyah alanlar, çizgi yoğunluğu ve boşluk bilinçli kompozisyon oluştursun.
>
> Dijital grunge texture ile her yüzeyi kirletme.

## English

> Illustrate [TOPIC] with rough ink-brush or pen editorial language using deliberate black masses, line density, and negative space.
>
> Avoid coating the entire image in digital grunge texture.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1610. `/cut-paper-editorial` — Kesilmiş Kâğıt Editorial Illustration

## Türkçe

> [KAVRAM]'ı 4–7 fiziksel kesilmiş kâğıt şekliyle anlat.
>
> Her şekil gerçek bir kavram/ilişki temsil etsin.
>
> Kağıt katmanı ve küçük gölgeler fiziksel olsun.
>
> Her detay için yeni shape ekleme.

## English

> Explain [CONCEPT] using only 4–7 physically cut paper shapes.
>
> Make each shape correspond to a real idea or relationship.
>
> Keep paper layering and small shadows physically plausible.
>
> Do not add a new shape for every minor detail.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1611. `/marker-editorial` — Marker / Keçeli Kalem Editorial

## Türkçe

> [KONU]'yu birkaç geniş marker stroke ve sınırlı contour çizgiyle anlat.
>
> Marker'daki overlap, uç yönü ve boya yoğunluğu gerçek çizim sürecine uysun.
>
> Dijital vector fill üzerine marker texture kaplama.

## English

> Illustrate [TOPIC] using a few broad marker strokes with restrained contour lines.
>
> Let overlap, nib direction, and ink density reflect real marker behavior.
>
> Avoid merely applying marker texture over vector fills.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1612. `/scribble-portrait` — Karalama Portre

## Türkçe

> [KİŞİ]'nin yüzünü tek kesintisiz veya kontrollü tekrarlanan scribble line sistemiyle portreye dönüştür.
>
> Ana yüz oranları, göz-burun-ağız ilişkisi ve silhouette tanınabilir kalsın.
>
> Karalamayı yüzün üzerine rastgele çizgi overlay'i gibi kullanma.

## English

> Transform [PERSON] into a portrait built from one continuous or controlled repeated scribble-line system.
>
> Preserve recognizable facial proportions and silhouette.
>
> Do not simply overlay random scribbles on a normal portrait.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1613. `/personal-symbol-illustration` — Kişisel Sembol İllüstrasyonu

## Türkçe

> [KİŞİ/KONU]'yu jenerik ikonlarla değil gerçek anlam taşıyan 5–7 kişisel nesne/sembol üzerinden editorial illustration olarak anlat.
>
> Nesneler birbirleriyle tek kompozisyon ilişkisi kursun.
>
> “Creativity” için ampul, “idea” için beyin, “growth” için bitki gibi otomatik stock metaforları kullanma.

## English

> Represent [PERSON/TOPIC] through 5–7 genuinely meaningful objects or symbols rather than generic icons.
>
> Build one coherent composition.
>
> Avoid automatic stock metaphors such as lightbulb for creativity, brain for ideas, and plant for growth.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1614. `/story-rich-scene` — Hikâye Zengin Tek Sahne

## Trend

2026 illustration trend kaynaklarında **story-rich scenes** insan eli hissinin güçlü karşılıklarından biri.

## Türkçe

> [KONU]'yu tek sahnede 5–8 küçük anlatı detayıyla göster.
>
> Ana olay ilk bakışta okunmalı.
>
> İkincil detaylar yakından bakıldığında keşfedilsin.
>
> Her boşluğa Easter egg doldurma.
>
> Tüm detaylar aynı zaman/mekân hikâyesine ait olsun.

## English

> Show [TOPIC] in one scene containing 5–8 small narrative details.
>
> Make the primary event readable immediately and allow secondary details to emerge on closer inspection.
>
> Avoid filling every empty area with Easter eggs.
>
> Keep all details within one coherent time and place.

---

# 1615. `/human-mark-layer` — İnsan İzi Katmanı

## Türkçe

> Dijital görselde yalnız 2–3 gerçekten üretim sürecinden gelebilecek insan izi bırak:
>
> - pencil correction,
> - marker overlap,
> - cut edge,
> - ink variation,
> - registration shift.
>
> Rastgele kusur ekleyerek insan eli taklidi yapma.

## English

> Leave only 2–3 human-production traces that could genuinely emerge from the process, such as pencil correction, marker overlap, cut edge, ink variation, or registration shift.
>
> Do not imitate humanity through random defects.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1616. `/illustration-process-strip` — İllüstrasyon Süreç Şeridi

## Türkçe

> Aynı illüstrasyonu dört gerçek aşamada göster:
>
> 1. thumbnail/composition,
> 2. line drawing,
> 3. color/block,
> 4. final.
>
> Her aşama bir karar eklesin.
>
> Final görselin sadece opacity azaltılmış kopyalarını süreç diye gösterme.

## English

> Show the same illustration through four real stages:
>
> 1. thumbnail or composition,
> 2. line drawing,
> 3. color blocking,
> 4. final.
>
> Let each stage add a real decision.
>
> Do not present faded copies of the final artwork as process.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1617. `/illustration-slop-filter` — “Human-made” İllüstrasyon AI Slop Filtresi

Kaçınılması gerekenler:

- insan eli = rastgele yamukluk,
- handmade = paper texture,
- childlike = kötü anatomi,
- naive = doodle kalabalığı,
- editorial = soyut yüz + bitki,
- her konsepte ampul/beyin/merdiven metaforu,
- fake sketch layer,
- bütün görselde aynı “organic blob” şekilleri,
- her şeyi pastel yapmak.

---

# 1618. Yeni üst aile: `Circular Packaging Visual`

Aile:

- `/refill-system`
- `/refill-station`
- `/returnable-pack`
- `/reuse-loop`
- `/mono-material-pack`
- `/fiber-packaging`
- `/molded-pulp-insert`
- `/packaging-nesting`
- `/traceability-pack`
- `/circular-packaging-board`

Temel kural:

> **environmental claim değil, fiziksel ve operasyonel döngü göster.**

---

# 1619. Yeni üst aile: `Inclusive Exhibition Visual`

Aile:

- `/inclusive-exhibition`
- `/multi-height-display`
- `/seated-view-audit`
- `/low-vision-label`
- `/easy-read-exhibit`
- `/sensory-map-museum`
- `/quiet-route`
- `/exhibit-rest-point`
- `/inclusive-interactive-height`

Temel soru:

> **Aynı içerik farklı bedenler, duyular ve bilişsel ihtiyaçlarla nasıl deneyimleniyor?**

---

# 1620. Yeni üst aile: `Haptic Interpretation`

Aile:

- `/haptic-object`
- `/haptic-relief`
- `/haptic-map`
- `/haptic-timeline`
- `/haptic-cause-effect`
- `/haptic-audio-pair`
- `/haptic-guidance`
- `/haptic-threshold`

Ana ilke:

> **dokunma dekoratif texture değil, bilgi kanalıdır.**

---

# 1621. Yeni üst aile: `Human-made Illustration`

Aile:

- `/childlike-line`
- `/naive-editorial-illustration`
- `/rough-ink-editorial`
- `/cut-paper-editorial`
- `/marker-editorial`
- `/scribble-portrait`
- `/story-rich-scene`
- `/human-mark-layer`
- `/illustration-process-strip`

Ana kural:

> **insan eli hissi = gerçek karar + gerçek süreç izi.**

---

# 1622. `/function-before-green` — “Yeşil” Görünmeden Önce İşlev

## Yeni kontrol bloğu

## Türkçe

> Ambalajı önce ürün koruma, lojistik, kullanım, tekrar kullanım/dolum ve gerçek malzeme sistemi açısından çöz. Çevresel görsel dili ancak bu sistemden sonra oluştur.
>
> “Sustainable” görünüm uğruna işlevi bozma.

## English

> Solve protection, logistics, use, reuse or refill, and material system first. Build environmental visual language only afterward.
>
> Do not sacrifice function merely to make the design look sustainable.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1623. `/access-before-effect` — Efektten Önce Erişim

## Yeni kontrol bloğu

## Türkçe

> Sergi, AR, projection, motion veya haptic deneyimde önce kritik bilgiye erişimi çöz. Görsel/teknolojik efekt ikinci katman olsun.
>
> Efekt kapatıldığında deneyimin ana içeriği tamamen kaybolmamalı.

## English

> In exhibitions, AR, projection, motion, or haptic experiences, solve access to critical information first and treat visual or technological effect as a secondary layer.
>
> The core content should not disappear completely when the effect is unavailable.

## Neye dikkat edilmeli?

İnsan izi bilinçli dozda kalsın: karalama ve mürekkep dokusu konuyu kapatıyorsa katman seyreltilir.

---
# 1624. Bu turdaki slash-style indeks (aile-022)

| Kısayol | Aile |
|---|---|
| `/refill-system` | durable container + refill |
| `/refill-station` | in-store refill interaction |
| `/returnable-pack` | reusable return loop |
| `/reuse-loop` | packaging reuse lifecycle |
| `/mono-material-pack` | single-material-family packaging |
| `/fiber-packaging` | fiber-based structural pack |
| `/molded-pulp-insert` | pulp protective insert |
| `/packaging-nesting` | logistics-efficient empty pack |
| `/packaging-logistics-board` | package across distribution stages |
| `/traceability-pack` | packaging as data carrier |
| `/recycled-content-honest` | evidence-based recycled-content claim |
| `/sustainability-claim-lock` | verified environmental claims only |
| `/circular-packaging-board` | matched circular-system comparison |
| `/inclusive-exhibition` | inclusion-first exhibition |
| `/multi-height-display` | multiple viewing heights |
| `/seated-view-audit` | seated accessibility review |
| `/low-vision-label` | low-vision-friendly label |
| `/easy-read-exhibit` | easy-read interpretation |
| `/sensory-map-museum` | museum sensory map |
| `/quiet-route` | lower-stimulus route |
| `/exhibit-rest-point` | pause/regulation space |
| `/inclusive-interactive-height` | accessible control placement |
| `/haptic-object` | tactile artifact replica |
| `/haptic-relief` | tactile relief image |
| `/haptic-map` | touch-readable navigation |
| `/haptic-timeline` | tactile chronological structure |
| `/haptic-cause-effect` | tactile causal diagram |
| `/haptic-audio-pair` | touch + audio interpretation |
| `/haptic-guidance` | functional haptic feedback |
| `/haptic-threshold` | tactile transition cue |
| `/haptic-evaluation-board` | evaluation of haptic interaction |
| `/childlike-line` | deliberate childlike linework |
| `/naive-editorial-illustration` | naive editorial metaphor |
| `/rough-ink-editorial` | rough ink illustration |
| `/cut-paper-editorial` | paper-built editorial image |
| `/marker-editorial` | real marker-process illustration |
| `/scribble-portrait` | scribble-constructed portrait |
| `/personal-symbol-illustration` | meaningful-symbol illustration |
| `/story-rich-scene` | one scene with narrative details |
| `/human-mark-layer` | restrained process traces |
| `/illustration-process-strip` | real illustration process |
| `/function-before-green` | functional sustainability control |
| `/access-before-effect` | accessibility before technology |

---

<a id="aile-023"></a>
# Handwritten Notes, Sketchnote, Specimen Board, Material Board ve Müze Yorumlama — 2026 Ek Taraması

Bu turda rehberin başlangıçtaki örnek görselinde bulunan ancak henüz bağımsız ve yeterince ayrıntılı ailelere dönüşmemiş konular tamamlanıyor:

- `handwritten`
- `sketchnote`
- `visual study notes`
- `labeled ingredient breakdown`
- `material breakdown`
- `specimen board`
- `collection sheet`
- `museum interpretation panel`
- `diorama`
- `editorial illustration`

2026 not alma araştırmaları önemli bir uyarı yapıyor: **“elle yazılmış görünüm” ile öğrenme aynı şey değildir.** Etkili not alma; bilgiyi seçmek, dönüştürmek, ilişkilendirmek ve tekrar düşünmekle ilgilidir. Haziran 2026’da yayımlanan guided doodle note-taking çalışması ile yakın dönem sketchnote araştırmaları, çizim ve yazının birlikte kullanılabileceğini gösteriyor; ancak çizim yalnız dekor olduğunda öğrenme kazancı otomatik değildir. Drawing-to-learn meta-analizleri de özellikle görsel ve sözel bilginin **entegrasyonu** desteklendiğinde faydanın daha anlamlı olduğunu gösteriyor.

Bu nedenle:

> **handwritten ≠ rastgele el yazısı fontu**
>
> **sketchnote ≠ doodle ile süslenmiş ders notu**
>
> **visual notes ≠ infographic**

---

# 1625. `/handwritten` — El Yazısı Görsel Dili

## Başlangıç örneğindeki terim

`handwritten`, ürün tanıtımından ders notuna kadar çok farklı alanlarda kullanılabilir.

Ancak modelin sık yaptığı hata:

> tüm metni okunaksız el yazısına çevirmek.

## Türkçe prompt

> [İÇERİK]'i gerçek bir kişinin kısa notlar aldığı doğal handwritten presentation olarak düzenle.
>
> El yazısı yalnız:
>
> - başlık,
> - kısa vurgu,
> - ok yanında 1–4 kelimelik not,
> - küçük kişisel açıklama
>
> için kullanılsın.
>
> Uzun metin bloklarını okunabilir normal tipografiyle bırak.
>
> El yazısı stroke kalınlığı, kalem basıncı ve harf karakteri aynı kişiden çıkmış gibi tutarlı olsun.
>
> Rastgele üç farklı handwriting font kullanma.

## English

> Present [CONTENT] using natural handwritten annotation from one consistent hand.
>
> Use handwriting only for headings, short emphasis, 1–4 word arrow notes, and concise personal comments.
>
> Keep long text blocks in readable conventional typography.
>
> Preserve one consistent pen pressure, stroke behavior, and handwriting character.
>
> Avoid mixing several unrelated handwriting styles.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1626. `/handwritten-product` — Ürün Üzerinde El Yazısı Annotation

## Kullanım

Başlangıçtaki “product marketing with handwriting” örneğinin kontrollü sürümü.

## Türkçe

> [ÜRÜN]'ün gerçek fotoğrafını ana görsel olarak koru.
>
> Çevresinde yalnız 3–5 kısa elle yazılmış annotation kullan:
>
> - bir özellik,
> - bir materyal,
> - bir kullanım ayrıntısı,
> - küçük kişisel not.
>
> Oklar gerçekten gösterdikleri ürüne temas etsin.
>
> Ürünün üzerine büyük el yazısı slogan yığma.

## English

> Preserve the real photograph of [PRODUCT] as the primary visual.
>
> Add only 3–5 concise handwritten annotations around it for a feature, material, use detail, or small personal note.
>
> Make arrows physically point to the referenced product feature.
>
> Avoid covering the product in large handwritten slogans.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1627. `/handwritten-photo-notes` — Fotoğraf Üzerinde El Yazısı Notlar

## Türkçe prompt

> Kaynak fotoğrafı değiştirme.
>
> Fotoğrafın kenar boşluklarında veya negatif alanında yalnız kısa handwritten notes ekle.
>
> Notlar görüntüde gerçekten görülebilen ayrıntılara bağlı olsun.
>
> Fotoğraf üzerine sahte tarih, yer veya olay bilgisi uydurma.

## English

> Keep the source photograph unchanged.
>
> Add concise handwritten notes only in margins or negative space.
>
> Tie notes to details genuinely visible in the image.
>
> Do not invent dates, places, or event information.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1628. `/handwritten-recipe` — El Yazısı Tarif Kartı

## Türkçe

> [TARİF]'i gerçek mutfak defteri gibi düzenle.
>
> Başlık ve kısa kişisel not el yazısı olabilir.
>
> Malzeme miktarları ve kritik süre/sıcaklık bilgileri net, yüksek okunabilirlikte kalsın.
>
> Tarif sayfasını kahve lekesi, un izi, kurutulmuş çiçek ve yırtık kâğıtla otomatik yaşlandırma.

## English

> Present [RECIPE] like a real kitchen notebook.
>
> Allow handwriting in the title and short personal notes while keeping ingredient quantities and critical time or temperature information highly legible.
>
> Avoid automatic coffee stains, flour, dried flowers, and torn-paper aging.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1629. `/handwritten-map` — Harita Üzerinde El Yazısı Not

## Türkçe

> Kaynak haritayı okunabilir tut.
>
> Yalnız kişisel rota, buluşma noktası veya kısa gözlem için el yazısı annotation kullan.
>
> El yazısı yer adı veya koordinat gibi temel kartografik bilgiyi değiştirmesin.

## English

> Keep the underlying map readable.
>
> Use handwriting only for personal route notes, meeting points, or concise observations.
>
> Do not let handwritten annotation replace or alter core geographic labels or coordinates.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1630. `/handwritten-slop-filter` — Handwritten AI Slop Filtresi

Kaçınılması gerekenler:

- her metni el yazısına çevirmek,
- üç farklı el yazısı karakteri,
- okunmayan uzun paragraf,
- rastgele kıvrımlı ok,
- Post-it + tape + coffee stain zorunluluğu,
- kaynakta olmayan kişisel not uydurmak,
- el yazısını “authentic” görünüm için dekor olarak serpiştirmek.

---

# 1631. `/sketchnote` — Görsel Not Alma / Sketchnote

## Eğitim

Sketchnote:

> **metin + görsel + bağlantı + hiyerarşi**

kombinasyonudur.

Dekoratif doodle sayfası değildir.

## Türkçe prompt

> [DERS/KONU]'yu tek sayfalık sketchnote olarak düzenle.
>
> Önce 4–7 ana fikir çıkar.
>
> Her ana fikir için:
>
> - kısa başlık,
> - 1–2 cümle veya anahtar kelime,
> - anlamlı küçük çizim,
> - gerektiğinde tek bağlantı oku
>
> kullan.
>
> Görsel, kavramı gerçekten açıklasın; boşluğu doldurmak için ikon ekleme.
>
> Okuma yolu tamamen rastgele olmasın.

## English

> Turn [LESSON/TOPIC] into a one-page sketchnote.
>
> Identify 4–7 primary ideas first.
>
> For each idea use a concise heading, one or two short notes or keywords, one meaningful drawing, and a connector only when necessary.
>
> Make every drawing explain the concept rather than decorate empty space.
>
> Preserve a readable visual path.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1632. `/guided-sketchnote` — Yönlendirilmiş Sketchnote

## 2026 araştırma bağlantısı

Guided doodle/sketchnote yaklaşımında öğrenciye tamamen boş sayfa vermek yerine bazı yapısal destekler sağlanabilir.

## Türkçe

> [KONU] için öğrencinin tamamlayacağı guided sketchnote şablonu oluştur.
>
> Sayfada:
>
> - ana başlıklar hazır,
> - 2–3 küçük başlangıç şekli,
> - bazı bağlantı çizgileri,
> - önemli boş alanlar
>
> bulunsun.
>
> Öğrencinin hâlâ kendi kelimelerini ve görsellerini üretebileceği alan bırak.

## English

> Create a guided sketchnote template for [TOPIC] with prepared main headings, 2–3 starter visual shapes, selected connectors, and generous blank areas.
>
> Leave enough space for the learner to generate their own wording and visuals.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1633. `/partial-sketchnote` — Yarı Tamamlanmış Görsel Not

## Eğitim

Drawing-to-learn araştırmalarındaki **cognitive load** sorununu azaltmak için.

## Türkçe

> [KONU]'nun karmaşık temel diyagramını önceden ver, ancak:
>
> - kritik etiketleri,
> - 2–3 bağlantıyı,
> - sonuç bölümünü
>
> öğrenciye bırak.
>
> Öğrenciyi sıfırdan detaylı çizim yapmak zorunda bırakma.

## English

> Provide the complex base diagram for [TOPIC] but leave critical labels, 2–3 relationships, and the conclusion for the learner to complete.
>
> Do not require the student to redraw a mechanically complex figure from scratch.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1634. `/sketchnote-linear` — Doğrusal Sketchnote

## Türkçe

> [SÜREÇ/KONU]'yu üstten alta veya soldan sağa açık sketchnote akışıyla göster.
>
> Her blok bir öncekinin devamı olsun.
>
> Timeline, süreç veya neden-sonuç konuları için uygundur.

## English

> Show [PROCESS/TOPIC] as a clear sketchnote sequence flowing top-to-bottom or left-to-right, with each block continuing from the previous one.
>
> Use this for timelines, processes, and causal explanations.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1635. `/sketchnote-radial` — Radyal Sketchnote

## Türkçe

> Tek merkez kavramdan 4–6 ana dala ayrılan radial sketchnote oluştur.
>
> Dallar eşit olmak zorunda değil.
>
> Yalnız gerçekten ilişkili alt kavramları aynı dala koy.

## English

> Create a radial sketchnote branching from one central concept into 4–6 primary branches.
>
> Branches need not be perfectly symmetrical.
>
> Group only genuinely related subtopics.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1636. `/sketchnote-path` — Yol / Rota Düzenli Sketchnote

## Türkçe

> [ÖĞRENME SÜRECİ/TARİHSEL SÜREÇ]'ni sayfa üzerinde takip edilebilen tek görsel yol boyunca sketchnote olarak göster.
>
> Yol dekoratif labirent olmasın; bilgi sırasını gerçekten anlatsın.

## English

> Turn [LEARNING PROCESS/HISTORICAL SEQUENCE] into a sketchnote arranged along one traceable visual path.
>
> Make the path encode real sequence rather than function as decorative maze.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1637. `/sketchnote-compare` — İki Kavramı Görsel Notla Karşılaştırma

## Türkçe

> [A] ve [B]'yi sayfanın iki tarafında matched sketchnote olarak karşılaştır.
>
> Aynı başlık kategorileri ve aynı görsel ölçek kullan.
>
> Ortak özellikleri merkezde küçük alanla göster.

## English

> Compare [A] and [B] using matched sketchnote structures on opposite sides of the page.
>
> Use the same categories and visual scale, with a small central area for shared features.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1638. `/sketchnote-legend` — Görsel Kelime Anahtarı

## Türkçe

> Sketchnote için 8–12 tekrar kullanılabilir küçük sembolün legend'ını oluştur.
>
> Örneğin:
>
> neden,
> sonuç,
> soru,
> örnek,
> uyarı,
> tarih,
> kişi,
> ana fikir.
>
> Semboller konu boyunca aynı anlamı taşısın.

## English

> Create a legend of 8–12 reusable symbols for the sketchnote, such as cause, effect, question, example, warning, date, person, and key idea.
>
> Keep meanings consistent throughout the notes.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1639. `/sketchnote-student` — Öğrenci Üretimi Görsel Not Hissi

## Türkçe

> Sayfayı profesyonel infographic gibi kusursuzlaştırma.
>
> Gerçek bir öğrencinin:
>
> - kısa kelime grupları,
> - birkaç düzeltme,
> - basit çizim,
> - sınırlı renk
>
> kullandığı düzenli ama doğal not sayfası gibi göster.
>
> Bilgi doğruluğu yine korunmalı.

## English

> Avoid polishing the page into a professional infographic.
>
> Make it feel like an organized but natural student note page using concise phrases, a few corrections, simple drawings, and limited color while preserving factual accuracy.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1640. `/sketchnote-slop-filter` — Sketchnote AI Slop Filtresi

Kaçınılması gerekenler:

- doodle = öğrenme sanmak,
- her başlığın yanına ampul,
- rastgele oklar,
- okunamayan handwritten text,
- her alanı doldurmak,
- çok fazla renk,
- görselin kavramla ilişkisiz olması,
- profesyonel infographic gridini “handdrawn” texture ile boyamak.

---

# 1641. `/visual-study-notes` — Görsel Çalışma Notları

## Ayrım

`visual learning whiteboard` daha açıklayıcı ders panosu olabilir.

`visual study notes` ise:

> **öğrencinin tekrar çalışması için kompakt öğrenme sayfası**

dır.

## Türkçe prompt

> [KONU]'yu sınav/tekrar için tek sayfalık visual study notes olarak düzenle.
>
> İçerik:
>
> - 5–8 temel terim,
> - 2–3 kritik ilişki,
> - 1 ana şema,
> - 1 karşılaştırma veya örnek,
> - 3 kısa kendini sınama sorusu.
>
> Sayfayı tam ders kitabı özetine dönüştürme.

## English

> Turn [TOPIC] into one-page visual study notes for revision.
>
> Include 5–8 essential terms, 2–3 critical relationships, one main diagram, one comparison or example, and three concise self-test questions.
>
> Do not compress the entire textbook chapter into one page.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1642. `/study-notes-core` — Çekirdek Bilgi Sayfası

## Türkçe

> [KONU]'nun yalnız sınav/öğrenme açısından gerçekten gerekli çekirdeğini göster.
>
> “İlginç bilgi” kutuları ve dekoratif yan bilgiler ekleme.
>
> Ana terimler ve ilişkiler önce gelsin.

## English

> Show only the learning-critical core of [TOPIC].
>
> Avoid decorative trivia and “fun fact” boxes.
>
> Prioritize key terms and relationships.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1643. `/study-notes-question-led` — Sorularla Düzenlenen Not

## Türkçe

> [KONU]'yu başlıklar yerine 5 ana soru etrafında düzenle.
>
> Her sorunun altında:
>
> - kısa cevap,
> - tek görsel,
> - gerekli örnek
>
> bulunsun.
>
> Sorular öğrencinin gerçekten cevaplaması gereken kavramsal sorular olsun.

## English

> Structure [TOPIC] around five primary questions rather than section headings.
>
> Under each question include a concise answer, one visual, and an example only where necessary.
>
> Use real conceptual questions rather than decorative prompts.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1644. `/study-notes-recall` — Recall Odaklı Görsel Not

## Türkçe

> Not sayfasının bir bölümünde bilgiyi doğrudan vermek yerine 4–6 küçük retrieval prompt bırak.
>
> Örneğin:
>
> “Bu ok neyi gösteriyor?”
> “İki farkı yaz.”
> “Bir sonraki aşama ne?”
>
> Cevaplar ayrı answer layer'da tutulabilir.

## English

> Reserve part of the study page for 4–6 retrieval prompts rather than displaying every answer directly, such as:
>
> “What does this arrow represent?”
> “Name two differences.”
> “What comes next?”
>
> Answers may live in a separate answer layer.

## Neye dikkat edilmeli?

Türkçe karakterleri (ğ, ş, ı, ç) harf harf kontrol edin; model el yazısında harf düşürür ve kelime uydurur. Yazı üç satırı geçecekse görseli değil not defterini kullanın.

---
# 1645. `/study-notes-slop-filter` — Görsel Ders Notu AI Slop Filtresi

Kaçınılması gerekenler:

- bir A4'e bütün konu,
- 50 minik ikon,
- her bilgi için renkli kutu,
- emoji,
- motivasyon sözü,
- konu dışı doodle,
- okunmayacak kadar küçük font,
- tekrar yerine pasif bakma sayfası.

---

# 1646. `/ingredient-breakdown` — İçerik Bileşenlerine Ayırma

## Başlangıç örneği

Başlangıç görselindeki:

> `labeled ingredient breakdown`

bu aileye aittir.

## Türkçe prompt

> [YEMEK/ÜRÜN]'ün fiziksel bileşenlerini final üründen ayrı ayrı göster.
>
> Ana ürün merkezde veya üstte kalsın.
>
> Çevresinde gerçek ingredient'lar:
>
> - ayrı,
> - kolay tanınır,
> - yaklaşık doğru oran ilişkisiyle
>
> yer alsın.
>
> Her bileşeni kısa isimle etiketle.
>
> Tarifte bulunmayan ingredient ekleme.

## English

> Show the physical ingredients of [FOOD/PRODUCT] separately from the finished item.
>
> Keep the final item central or above, with real ingredients arranged separately and recognizably at approximately meaningful proportions.
>
> Label each component concisely.
>
> Do not add ingredients absent from the recipe or source.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1647. `/ingredient-breakdown-topdown` — Tepeden İçerik Ayrımı

## Türkçe

> [YEMEK]'i merkezde, ingredient'ları çevresinde top-down düzende göster.
>
> Kap/kaşık/dekor yalnız gerçekten gerekli ise kullan.
>
> Ingredient'lar birbirine karışmasın.

## English

> Place [FOOD] in the center with its ingredients arranged around it in a top-down layout.
>
> Use bowls, spoons, and props only when genuinely necessary.
>
> Keep ingredients visually separated.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1648. `/ingredient-lineup` — İçerik Sıralaması

## Türkçe

> Ingredient'ları soldan sağa gerçek kullanım sırası veya miktar büyüklüğüne göre lineup olarak göster.
>
> Sıra neye göre yapıldıysa başlıkta belirt.
>
> Yalnız estetik renk geçişine göre sıralama yapma.

## English

> Arrange ingredients left-to-right according to actual use sequence or amount.
>
> State clearly what determines the order.
>
> Do not sort purely for decorative color progression.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1649. `/ingredient-to-result` — Bileşenden Sonuca

## Türkçe

> Sayfayı iki bölüme ayır:
>
> sol = ayrı ingredient'lar,
> sağ = final ürün.
>
> Arada yalnız gerekli transformation/process ilişkisini göster.
>
> Ingredient breakdown'u tarifin tüm adımlarıyla karıştırma.

## English

> Divide the page into:
>
> left = separate ingredients,
> right = finished result.
>
> Show only the necessary transformation relationship between them.
>
> Do not turn the ingredient breakdown into a full recipe procedure.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1650. `Ingredient Breakdown` ile `Exploded View` Aynı Şey Değildir

Bu ayrım rehberde açık tutulmalı.

### `/ingredient-breakdown`

Bir bütünü oluşturan **girdi/malzeme/içerikleri** gösterir.

Örnek:

> sandviç → ekmek, peynir, domates, yeşillik.

### `/exploded-view`

Bir fiziksel nesnenin **mekanik/parça ilişkisini** gösterir.

Örnek:

> bisiklet → tekerlek, kadro, zincir, pedal, fren.

### `/layer-breakdown`

Bir yapının üst üste gelen **katmanlarını** gösterir.

Örnek:

> Dünya → kabuk, manto, çekirdek.

### `/material-breakdown`

Bir ürünün hangi **malzemelerden** üretildiğini gösterir.

Örnek:

> ayakkabı → kauçuk, tekstil, köpük, bağcık.

Bu dört aileyi birbirine karıştırmak prompt sonucunu ciddi biçimde değiştirir.

---

# 1651. `/material-breakdown` — Malzeme Dağılımı

## Türkçe prompt

> [ÜRÜN/NESNE]'yi ana formuyla göster ve hangi fiziksel malzemelerin hangi bölümde kullanıldığını ayrı küçük samples/callouts ile açıkla.
>
> Örneğin:
>
> gövde → alüminyum,
> yüzey → tekstil,
> taban → kauçuk.
>
> Malzeme bilgisi gerçek kaynak verilmemişse tahmin olarak sunma.

## English

> Show [PRODUCT/OBJECT] as the main form and identify which physical materials belong to which parts using small samples or callouts.
>
> Do not present guessed material composition as fact when source information is missing.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1652. `/material-board` — Malzeme Panosu

## 2026 trend bağlantısı

Milan Design Week 2026 moodboard çalışmalarında materyal, renk ve yüzey tek tek dekor değil, **deneyim ve kimlik oluşturan ilişkili sistem** olarak ele alınıyor.

## Türkçe

> [ÜRÜN/MEKÂN] için 6–8 parçalık gerçek material board oluştur.
>
> Her örnek:
>
> - gerçek malzeme adı,
> - yakın yüzey görünümü,
> - kısa fiziksel özellik
>
> taşısın.
>
> Malzemeleri yalnız renk uyumuna göre seçme.

## English

> Create a real 6–8 sample material board for [PRODUCT/SPACE].
>
> Give each sample its actual material name, close surface view, and concise physical characteristic.
>
> Do not select materials only for color harmony.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1653. `/material-swatch` — Malzeme Swatch Kartı

## Türkçe

> Tek [MALZEME]'yi swatch card üzerinde:
>
> - tam yüzey,
> - macro,
> - kenar/kalınlık,
> - gerektiğinde işlenmiş yüzey
>
> olarak göster.
>
> Aynı malzemenin farklı görünümlerini başka materyallere dönüştürme.

## English

> Show one [MATERIAL] on a swatch card through full surface, macro, edge or thickness, and processed finish where relevant.
>
> Keep all views materially consistent.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1654. `/material-family` — Aynı Malzemenin İşlenmiş Hâlleri

## Türkçe

> Aynı malzemenin 4–6 gerçek finish'ini karşılaştır:
>
> örneğin metal için:
>
> brushed,
> polished,
> bead-blasted,
> anodized,
> patinated.
>
> Kamera ve ışık eşleşsin.
>
> Yalnız finish değişsin.

## English

> Compare 4–6 real finishes of the same material, such as brushed, polished, bead-blasted, anodized, or patinated metal.
>
> Keep camera and lighting matched and change only surface finish.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1655. `/material-aging-board` — Malzemenin Zamanla Yaşlanması

## Türkçe

> [MALZEME]'yi yeni, kısa kullanım, uzun kullanım ve bakım/onarım sonrası dört matched örnekte göster.
>
> Eskime gerçek malzeme fiziğine dayansın.
>
> Her materyale aynı çizik/grunge overlay uygulama.

## English

> Show [MATERIAL] in four matched states: new, lightly used, long-used, and maintained or repaired.
>
> Base aging on real material behavior.
>
> Avoid applying the same generic scratch or grunge overlay to every material.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1656. `/material-junction` — Malzeme Birleşim Detayı

## Türkçe

> [MALZEME A] ile [MALZEME B]'nin gerçek birleşim noktasını yakın teknik/detail görünümde göster.
>
> Vida, dikiş, yapıştırma, geçme, conta veya profil gibi bağlantı fiziksel olarak görünür olsun.
>
> İki malzemeyi sihirli biçimde kesintisiz birleştirme.

## English

> Show the real junction between [MATERIAL A] and [MATERIAL B] in a close technical detail.
>
> Make fastener, stitch, adhesive, interlock, gasket, or profile physically understandable.
>
> Avoid magically seamless joins.

## Neye dikkat edilmeli?

Parça adları ve sayıları gerçek ürünle eşleşsin; montaj ilişkisi §4 mantığıyla okunur kalsın.

---
# 1657. `/material-board-slop-filter` — Material Board AI Slop Filtresi

Kaçınılması gerekenler:

- yalnız renk swatch,
- her malzemeyi kusursuz CGI küp,
- “natural” = wood + stone + linen,
- malzeme adı uydurmak,
- aynı texture'ı farklı materyale yapıştırmak,
- kalınlık/kenar davranışını göstermemek,
- kullanım bağlamını yok saymak.

---

# 1658. `/specimen-board` — Numune / Örnek Panosu

## Genel aile

`specimen board`, biyolojiye özel değildir.

Kullanılabilir:

- botanik,
- jeoloji,
- malzeme,
- tekstil,
- baskı,
- renk,
- tipografi,
- ürün,
- arkeoloji.

## Türkçe prompt

> [NUMUNE GRUBU]'nu karşılaştırılabilir specimen board olarak düzenle.
>
> Her örnek:
>
> - ayrı alan,
> - kısa kimlik,
> - gerekiyorsa ölçü/ölçek,
> - aynı görüntüleme mantığı
>
> taşısın.
>
> Numuneleri estetik simetri uğruna yanlış boyut ilişkisine sokma.

## English

> Arrange [SPECIMEN GROUP] as a comparable specimen board.
>
> Give each specimen its own space, concise identity, scale where necessary, and one consistent viewing logic.
>
> Do not distort size relationships for decorative symmetry.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1659. `/specimen-grid` — Numune Grid'i

## Türkçe

> [N] numuneyi tutarlı grid üzerinde göster.
>
> Her hücrede yalnız numune, numara ve kısa ad olsun.
>
> Karşılaştırma için kamera/ışık/ölçek mümkün olduğunca eşleşsin.

## English

> Show [N] specimens on a consistent grid using only the specimen, number, and concise name in each cell.
>
> Match camera, lighting, and scale as closely as practical for comparison.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1660. `/specimen-scale` — Ölçekli Numune

## Türkçe

> Her numunenin yanında gerçek scale bar veya ölçü referansı göster.
>
> Numunelerin görsel olarak aynı boyuta normalize edilip edilmediğini açıkça belirt.
>
> Scale bar gerçek veri olmadan uydurulmasın.

## English

> Place a real scale bar or measurement reference beside each specimen.
>
> State clearly whether specimens are displayed at normalized visual size.
>
> Do not invent scale bars without measurement data.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1661. `/specimen-variation` — Aynı Tür/Ürünün Varyasyonu

## Türkçe

> Aynı [TÜR/MALZEME/ÜRÜN]'ün 6–12 gerçek varyasyonunu yan yana göster.
>
> Ortak yapı sabit, gerçek doğal/üretim varyasyonu görünür olsun.
>
> Her numuneyi başka kategoriye dönüştürme.

## English

> Show 6–12 real variations of the same [SPECIES/MATERIAL/PRODUCT] side by side.
>
> Preserve the common underlying structure while revealing natural or manufacturing variation.
>
> Do not turn each specimen into a separate category.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1662. `/specimen-outlier` — Aykırı Numuneyi Gösterme

## Türkçe

> Aynı specimen set içinde yalnız gerçekten farklı olan outlier'ı sınırlı bir işaretle vurgula.
>
> Diğer numunelerin görünümünü azaltarak farkı yapay biçimde büyütme.

## English

> Highlight a genuine outlier within the specimen set using one restrained marker.
>
> Do not artificially exaggerate the difference by visually suppressing the other specimens.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1663. `/specimen-provenance` — Numune Kaynak Bilgisi

## Türkçe

> Her specimen için varsa:
>
> - collection/site,
> - tarih,
> - catalog ID,
> - materyal/tür,
> - collector/source
>
> bilgilerini küçük katalog alanında göster.
>
> Eksik provenance bilgisini uydurma.

## English

> Where available, provide specimen provenance such as collection or site, date, catalog ID, material or species, and collector or source.
>
> Do not invent missing provenance.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1664. `/specimen-board-slop-filter` — Specimen Board AI Slop Filtresi

Kaçınılması gerekenler:

- her numuneyi eşit boyuta zorlamak,
- sahte bilimsel numara,
- uydurma Latin isim,
- dekoratif vintage kâğıt,
- her örneğin altında uzun paragraf,
- doğal varyasyonu kusur sanıp düzeltmek,
- doğrulanmamış scale bar.

---

# 1665. `/collection-sheet` — Koleksiyon Sayfası

## Ayrım

`specimen board`:

> karşılaştırma ve inceleme.

`collection sheet`:

> aynı ailedeki farklı parçaları bir bütün olarak gösterme.

## Türkçe prompt

> [KOLEKSİYON]'un 9–16 parçasını tek collection sheet üzerinde göster.
>
> Her öğe:
>
> - aynı genel görsel dil,
> - ayrı silhouette,
> - kısa isim/numara
>
> taşısın.
>
> Koleksiyonu her parçayı aynılaştıracak kadar standardize etme.

## English

> Show 9–16 items from [COLLECTION] on one collection sheet.
>
> Keep one shared visual language while preserving a distinct silhouette and concise name or number for each item.
>
> Do not standardize the series until all items look identical.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1666. `/collection-lineup` — Koleksiyon Sıralaması

## Türkçe

> Koleksiyonu fiziksel boyut, tarih, seri numarası veya başka gerçek bir değişkene göre soldan sağa sırala.
>
> Sıralama ölçütünü açıkça belirt.
>
> Yalnız renk gradient'i için sıralama yapma.

## English

> Arrange the collection left-to-right according to one real variable such as physical size, date, or series number.
>
> State the ordering rule explicitly.
>
> Avoid arranging only for a decorative color gradient.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1667. `/collection-completion` — Koleksiyonda Eksik Parça

## Türkçe

> Koleksiyonun sahip olunan ve eksik parçalarını aynı grid üzerinde göster.
>
> Mevcut parçalar tam, eksikler yalnız outline/placeholder olarak gösterilsin.
>
> Eksik parçaların gerçek görünümü bilinmiyorsa uydurma.

## English

> Show owned and missing items within one collection grid.
>
> Render existing pieces fully and missing pieces only as outline or placeholder when their real appearance is unknown.
>
> Do not invent missing items.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1668. `/collection-archive-card` — Koleksiyon Arşiv Kartı

## Türkçe

> Her koleksiyon öğesi için küçük archive card tasarla:
>
> - fotoğraf,
> - isim,
> - edinme tarihi,
> - kaynak,
> - kondisyon,
> - kısa kişisel not.
>
> Bilinmeyen tarih ve kaynakları doldurma.

## English

> Create a small archive card for each collection item containing photo, name, acquisition date, source, condition, and concise personal note.
>
> Leave unknown dates or sources blank rather than inventing them.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1669. `/museum-interpretation-panel` — Müze Yorumlama Paneli

## 2026 araştırma bağlantısı

2026 eye-tracking ve ziyaretçi araştırmaları, müze metninin yalnız bilgi vermediğini, izleyicinin **nereye ve nasıl baktığını** etkileyebildiğini gösteriyor.

Özellikle:

- doğrudan görülebilen ayrıntıya referans,
- teknik/yapım bilgisi,
- kısa ve erken verilen ana fikir

ziyaretçinin eserle ilişkisinde güçlü olabiliyor.

## Türkçe prompt

> [ESER/KONU] için kısa museum interpretation panel tasarla.
>
> Hiyerarşi:
>
> 1. tek cümle ana fikir,
> 2. ziyaretçinin eserde görebileceği somut bir ayrıntı,
> 3. kısa bağlam,
> 4. gerekirse tek soru.
>
> Metin eserin kendisini gözlemleme fırsatını elinden almasın.
>
> Akademik makale gibi uzun yazma.

## English

> Design a concise museum interpretation panel for [OBJECT/TOPIC].
>
> Use this hierarchy:
>
> 1. one-sentence main idea,
> 2. one concrete visible detail to look for,
> 3. concise context,
> 4. one optional question.
>
> Help visitors look more closely without replacing their own observation.
>
> Avoid academic-article length.

## Neye dikkat edilmeli?

Her nesneye ait etiket ve numara doğru nesneye bağlı olsun; vitrin ya da çekmece düzeninde aynı nesne iki farklı biçimde tekrarlanmasın.

---
# 1670. `/look-closer-label` — “Yakından Bak” Etiketi

## Türkçe

> [ESER]'de ziyaretçinin gerçekten görebileceği tek ayrıntıya dikkat çeken 30–60 kelimelik label oluştur.
>
> Önce ayrıntıyı tarif et, sonra neden önemli olduğunu açıkla.
>
> Görünmeyen veya belirsiz özelliği varmış gibi yazma.

## English

> Create a 30–60 word “look closer” label directing attention to one detail genuinely visible in [OBJECT].
>
> Describe what to look for first, then explain why it matters.
>
> Do not refer to invisible or uncertain features as established fact.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1671. `/technique-label` — Yapım Tekniği Etiketi

## Türkçe

> [ESER]'in tek önemli yapım tekniğini ziyaretçinin görebileceği iz üzerinden açıkla.
>
> Örneğin:
>
> fırça izi,
> dikiş,
> oyma,
> baskı,
> kalıp,
> birleşim.
>
> Teknik terimi kısa gündelik açıklamayla eşleştir.

## English

> Explain one important making technique of [OBJECT] through a trace the visitor can actually see, such as brushwork, stitching, carving, printing, molding, or joinery.
>
> Pair the technical term with a concise plain-language explanation.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1672. `/context-label` — Tarihsel / Sosyal Bağlam Etiketi

## Türkçe

> [ESER]'in anlaşılması için gerekli tek tarihsel/sosyal bağlamı 40–80 kelimede ver.
>
> Sanatçı biyografisini yalnız eserle ilişkiliyse kullan.
>
> Ziyaretçiyi bilgi bombardımanına tutma.

## English

> Provide one necessary historical or social context for [OBJECT] in roughly 40–80 words.
>
> Include artist biography only when directly relevant to the work.
>
> Avoid information overload.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1673. `/comparison-label` — İki Eseri Karşılaştırma Etiketi

## Türkçe

> Yan yana duran [ESER A] ve [ESER B] için ziyaretçinin doğrudan gözlemleyebileceği tek karşılaştırma sorusu üret.
>
> Örneğin:
>
> “Işığın kullanımında ne değişiyor?”
>
> Ardından yalnız kısa bir bağlam ver.
>
> Cevabı baştan tamamen açıklama.

## English

> Create one direct visual comparison prompt for [OBJECT A] and [OBJECT B] that visitors can answer by looking, such as:
>
> “How does the use of light differ?”
>
> Follow with only concise context.
>
> Do not fully answer the observation question in advance.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1674. `/child-museum-label` — Çocuklar İçin Müze Etiketi

## Türkçe

> [ESER]'i çocuklara anlatırken kavramı küçültme veya yanlışlaştırma.
>
> Bir gözlem sorusu, bir kısa gerçek ve bir “bulabilir misin?” ayrıntısı yeterli olsun.
>
> Emoji ve konuşan maskot zorunlu değil.

## English

> Interpret [OBJECT] for children without distorting or oversimplifying the concept.
>
> Use one observation question, one concise fact, and one “can you find?” detail.
>
> Emojis and talking mascots are not required.

## Neye dikkat edilmeli?

Ölçek çubuğu ve kaynak bilgisi her levhada olsun; varyasyon dizisinde aynı türün farklı bireyleri karışmasın.

---
# 1675. `/museum-label-length` — Etiket Uzunluğu Kontrolü

## 2026 araştırma notu

Müze label çalışmalarında okuma bırakma oranı metin uzadıkça artabiliyor; farklı ziyaretçiler farklı miktarda metin okuyor.

## Prompt kuralı

> En önemli bilgi ilk bölümde.
>
> İkinci paragraf = isteğe bağlı derinlik.
>
> Kritik ipucunu son cümleye saklama.

---

# 1676. `/museum-label-slop-filter` — Müze Etiketi AI Slop Filtresi

Kaçınılması gerekenler:

- “Bu büyüleyici eser...”
- reklam dili,
- 200 kelimelik biyografi,
- ziyaretçinin göremediği ayrıntı,
- “siz de fark ettiniz mi?” gibi yapay ton,
- her label'da soru,
- eser hakkında kesin olmayan yorumu gerçek gibi sunmak,
- akademik jargonu açıklamadan kullanmak.

---

# 1677. `/diorama` — Genel Diorama

## Genel kullanım

Diorama:

> küçük sahne + fiziksel ölçek + üç boyutlu mekân + hikâye/anlatım.

Sadece “miniature style” değildir.

## Türkçe prompt

> [SAHNE]'yi [ÖLÇEK] fiziksel diorama olarak oluştur.
>
> Açıkça:
>
> - taban,
> - arka/yan sınır,
> - fiziksel figürler,
> - gerçek model malzemeleri,
> - ölçeğe uygun detay
>
> göster.
>
> Sahneyi yalnız tilt-shift fotoğrafla minyatür gibi gösterme.

## English

> Build [SCENE] as a physical [SCALE] diorama with a visible base, bounded environment, physical figures, real model-making materials, and scale-appropriate detail.
>
> Do not simulate miniaturization only through tilt-shift blur.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1678. `/open-diorama` — Açık Ön Yüzlü Diorama

## Türkçe

> [SAHNE]'yi önü açık display-box diorama olarak göster.
>
> Kutunun fiziksel kenarları ve derinliği görünür olsun.
>
> Kamera diorama içine tamamen girmiş gibi davranmasın.

## English

> Present [SCENE] as an open-front display-box diorama with visible physical edges and depth.
>
> Keep the camera outside the miniature rather than pretending it is inside a full-scale world.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1679. `/museum-diorama` — Müze Eğitim Dioraması

## Türkçe

> [DOĞAL/TARİHSEL SAHNE]'yi müze eğitim diorama'sı olarak göster.
>
> Ana sahne gerçek araştırma/kanıta dayanmalı.
>
> Ön plandaki fiziksel modeller ile boyalı/printed background arasında kontrollü derinlik geçişi olsun.
>
> Bilinmeyen tarihsel ayrıntıları dekoratif olarak uydurma.

## English

> Present [NATURAL/HISTORICAL SCENE] as a museum educational diorama grounded in available evidence.
>
> Use a controlled transition between physical foreground models and painted or printed background.
>
> Do not invent unknown historical details for decoration.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1680. `/process-diorama` — Süreci Üç Boyutlu Gösterme

## Türkçe

> [SÜREÇ]'in farklı aşamalarını tek fiziksel diorama içinde soldan sağa veya katmanlı olarak göster.
>
> Her bölüm aynı ölçek mantığında olsun.
>
> Aşamaları aynı anda görülebilir ancak birbirine karışmayacak şekilde ayır.

## English

> Show stages of [PROCESS] within one physical diorama, arranged left-to-right or through layered sections.
>
> Keep scale logic consistent and separate stages clearly enough to compare.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1681. `/cutaway-diorama` — Kesit Diorama

## Türkçe

> [YAPI/DOĞAL ORTAM]'ı bir kenarı kesilmiş physical diorama olarak göster.
>
> Dış görünüm ile iç katmanlar aynı modelde birlikte okunabilsin.
>
> Kesit düzlemi temiz ve fiziksel model kesimi gibi olsun.

## English

> Show [STRUCTURE/ENVIRONMENT] as a physical diorama with one side cut away so exterior and internal layers can be read together.
>
> Keep the section plane clean and physically model-like.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1682. `/diorama-scale-cue` — Ölçek İpucu

## Türkçe

> Diorama'nın gerçek minyatür ölçeğini anlatmak için yalnız bir scale cue kullan:
>
> model tabanı,
> küçük insan figürü,
> cetvel,
> display-case kenarı
>
> gibi.
>
> Dev el veya dev gerçek nesne eklemeyi zorunlu kılma.

## English

> Use only one scale cue to communicate the physical miniature scale of the diorama, such as the model base, a scale figure, ruler, or display-case edge.
>
> Avoid forcing oversized hands or real objects into every miniature scene.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1683. `/diorama-slop-filter` — Diorama AI Slop Filtresi

Kaçınılması gerekenler:

- tilt-shift = diorama sanmak,
- model tabanı yok,
- gerçek ölçek belirsiz,
- her model kawaii,
- plastik CGI yüzey,
- minyatürde gerçek boyuttaki mikro detay,
- figürlerin farklı ölçeklerde olması,
- sahnenin “cute miniature café” klişesine dönüşmesi.

---

# 1684. `/editorial-illustration` — Editorial Illustration

## Kullanım

Soyut fikir, haber, makale, toplumsal kavram, psikoloji, ekonomi, teknoloji, eğitim.

## Türkçe prompt

> [MAKALE/KAVRAM]'ı tek güçlü editorial illustration fikriyle görselleştir.
>
> Önce yazının ana iddiasını tek cümlede belirle.
>
> Sonra bu iddiayı:
>
> - metafor,
> - karşıtlık,
> - ölçek değişimi,
> - nesne ilişkisi,
> - görsel paradoks
>
> yöntemlerinden yalnız biriyle anlat.
>
> Görsel makaleyi özetleyen infographic olmasın.
>
> Ampul, beyin, puzzle piece, merdiven, roket gibi otomatik stok metaforları kullanma.

## English

> Visualize [ARTICLE/CONCEPT] through one strong editorial-illustration idea.
>
> Define the article’s primary claim in one sentence, then express it using only one device such as metaphor, contrast, scale change, object relationship, or visual paradox.
>
> Do not turn the image into an infographic summary.
>
> Avoid automatic stock metaphors such as lightbulbs, brains, puzzle pieces, ladders, and rockets.

## Neye dikkat edilmeli?

Bilgi taşıyan her öğe §18 listesiyle kaynaktan doğrulanır; estetik kararlar (duvar dizimi, çocuk kitabı dili) içeriği sadeleştirebilir ama değiştiremez.

---
# 1685. `/editorial-metaphor` — Tek Metafor

## Türkçe

> [KAVRAM]'ı tek nesne ilişkisinden doğan görsel metaforla anlat.
>
> Metaforu açıklamak için ikinci, üçüncü sembol ekleme.
>
> İlk bakışta kavramın yönü sezilsin ama aşırı literal olmasın.

## English

> Express [CONCEPT] through one visual metaphor built from a single object relationship.
>
> Avoid adding second and third symbols to explain the first.
>
> Make the direction of the idea understandable without becoming completely literal.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1686. `/editorial-contrast` — Görsel Karşıtlık

## Türkçe

> [İKİ FİKİR/GÜÇ] arasındaki gerilimi tek kompozisyonda görsel contrast ile göster.
>
> Karşıtlığı:
>
> - scale,
> - material,
> - direction,
> - weight,
> - space
>
> seçeneklerinden biriyle kur.
>
> Sayfayı tam ortadan ikiye bölmek zorunda değilsin.

## English

> Show tension between [TWO IDEAS/FORCES] through one visual contrast using scale, material, direction, weight, or space.
>
> Do not default to splitting the page exactly in half.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1687. `/editorial-object-swap` — Nesne İşlev Değişimi

## Türkçe

> [KAVRAM]'ı anlatmak için tanınabilir bir nesnenin yalnız tek işlevsel parçasını başka anlam taşıyan parça ile değiştir.
>
> Geri kalan nesne normal kalsın.
>
> Dönüşüm tek fikir taşısın.

## English

> Explain [CONCEPT] by replacing only one functional part of a recognizable object with another meaningful element.
>
> Keep the rest of the object normal.
>
> Let the transformation carry one idea only.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1688. `/editorial-negative-space` — Negatif Alan Metaforu

## Türkçe

> [KONU]'yu ana figür ile negatif alanın birlikte ikinci bir anlam oluşturduğu sade editorial illustration olarak tasarla.
>
> İkinci anlam gerçekten silhouette/boşluk üzerinden okunmalı.
>
> Rastgele gizli yüz ekleme.

## English

> Design [TOPIC] as a restrained editorial illustration where the primary figure and negative space create a second meaning together.
>
> Make the secondary idea genuinely emerge from silhouette or empty space.
>
> Avoid arbitrary hidden faces.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1689. `/editorial-sequential` — İki/Üç Kare Editorial

## Türkçe

> [KAVRAM]'ın değişimini 2–3 matched panelde göster.
>
> Aynı ana nesne korunmalı.
>
> Her panel yalnız bir değişim eklesin.
>
> Comic-strip konuşma balonlarına dönüştürme.

## English

> Show the change in [CONCEPT] across 2–3 matched panels while preserving one primary object.
>
> Introduce only one change per panel.
>
> Avoid turning the sequence into a speech-bubble comic strip.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1690. `/editorial-illustration-slop-filter` — Editorial Illustration AI Slop Filtresi

Kaçınılması gerekenler:

- ampul = fikir,
- beyin = zihin,
- puzzle = çözüm,
- merdiven = başarı,
- roket = büyüme,
- labirent = karmaşıklık,
- kırık zincir = özgürlük,
- dev el + küçük insan,
- soyut yüz + bitki,
- her konuyu sürreal kolaj yapmak.

---

# 1691. `/visual-vocabulary-sheet` — Kişisel Görsel Kelime Dağarcığı

## Eğitim / sketchnote / illustration

## Türkçe

> [DERS/ALAN] için tekrar kullanılabilir 24 küçük görsel sembol oluştur.
>
> Her sembol:
>
> - tek kavram,
> - tek basit çizim,
> - kısa ad
>
> taşısın.
>
> Semboller öğrencinin/öğretmenin hızlı tekrar çizebileceği kadar sade olsun.

## English

> Create 24 reusable small visual symbols for [SUBJECT/FIELD].
>
> Give each one concept, one simple drawing, and one concise name.
>
> Keep symbols simple enough for a learner or teacher to redraw quickly.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1692. `/visual-translation` — Metni Görsele Çevirme Egzersizi

## 2026 öğrenme araştırmalarıyla ilişkili

Learner-generated explanation/drawing araştırmalarında önemli mekanizma, sözel ve görsel temsil arasında **translation** yapmaktır.

## Türkçe

> [CÜMLE/KAVRAM]'ı doğrudan ikonla değiştirmek yerine önce:
>
> 1. özne,
> 2. ilişki,
> 3. hareket/değişim,
> 4. sonuç
>
> olarak çözümle.
>
> Sonra bu ilişkileri görsel olarak temsil et.

## English

> Before turning [SENTENCE/CONCEPT] into an image, identify:
>
> 1. subject,
> 2. relationship,
> 3. action or change,
> 4. result.
>
> Then translate those relationships visually rather than substituting words with icons.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1693. `/notes-integration-check` — Görsel Not Entegrasyon Kontrolü

Bir sketchnote veya visual note için sor:

1. Çizim metindeki fikri gerçekten açıklıyor mu?
2. Metin çizimin eksik bilgisini tamamlıyor mu?
3. Aynı bilgi iki kez gereksiz tekrar mı ediliyor?
4. Oklar gerçek ilişki mi gösteriyor?
5. Görsel olmadan kritik anlam kayboluyor mu?
6. Görsel sadece dekor ise kaldırılabilir mi?

Bu kontrol özellikle:

> **dual coding ≠ duplicate coding**

ayrımını korur.

---

# 1694. Yeni üst aile: `Visual Notetaking`

Aile:

- `/handwritten`
- `/sketchnote`
- `/guided-sketchnote`
- `/partial-sketchnote`
- `/visual-study-notes`
- `/study-notes-recall`
- `/visual-vocabulary-sheet`
- `/visual-translation`

Ana kural:

> **çizim ve yazı birbirini tamamlar; birbirinin dekoratif kopyası olmaz.**

---

# 1695. Yeni üst aile: `Breakdown Grammar`

Rehberde “breakdown” kelimesinin dört farklı anlamı artık netleştirilebilir:

| Aile | Ne ayrılır? | Örnek |
|---|---|---|
| `/ingredient-breakdown` | içerik/girdi | yemek |
| `/material-breakdown` | malzeme | ayakkabı |
| `/exploded-view` | fiziksel parça | bisiklet |
| `/layer-breakdown` | üst üste katman | Dünya |
| `/process-breakdown` | zaman/adım | üretim |
| `/system-breakdown` | işlevsel alt sistem | makine/ağ |

Bu tablo, prompt seçimindeki en sık karışıklıklardan birini çözer.

---

# 1696. Yeni üst aile: `Specimen / Collection Grammar`

### Specimen

> tek tek örneklerin incelenmesi.

### Collection

> aynı ailedeki öğelerin birlikte görülmesi.

### Archive

> öğe + kayıt + tarih + kaynak.

### Museum display

> seçilmiş öğe + yorumlama + ziyaretçi.

### Inventory

> öğe + sayı + durum + takip.

Bu beş terim aynı görünse de **bilgi amacı farklıdır**.

---

# 1697. Yeni üst aile: `Interpretive Visual`

Müze, eğitim ve editorial alanlarının kesişimi.

Aile:

- `/museum-interpretation-panel`
- `/look-closer-label`
- `/technique-label`
- `/comparison-label`
- `/educational-story-scene`
- `/editorial-illustration`

Ortak kural:

> **görsel veya metin, izleyicinin nereye bakacağını destekler; ne düşünmesi gerektiğini tamamen dikte etmez.**

---

# 1698. `/material-vs-moodboard` — Material Board / Moodboard Ayrımı

## Material Board

Gerçek fiziksel seçim sorusu:

> hangi malzeme?

İçerir:

- yüzey,
- kalınlık,
- finish,
- birleşim,
- kullanım.

## Moodboard

Daha soyut yön sorusu:

> nasıl bir atmosfer/kimlik?

İçerir:

- renk,
- doku,
- fotoğraf,
- tipografi,
- çağrışım.

### Rehber kuralı

Moodboard'a malzeme konabilir.

Ama:

> **moodboard ≠ material specification.**

---

# 1699. `/material-moodboard-hybrid` — Materyal + Atmosfer Hibrit Panosu

## 2026 Milan Design Week sinyali

## Türkçe

> [MEKÂN/ÜRÜN] için board'u iki bölüme ayır:
>
> sol %60 = gerçek materyal swatch'ları,
> sağ %40 = bu malzemelerin oluşturacağı atmosferi anlatan 2–3 referans fotoğraf.
>
> Renk paleti swatch'lardan türesin.
>
> Atmosfer fotoğrafı gerçek material specification'ın yerine geçmesin.

## English

> Divide the board for [SPACE/PRODUCT] into:
>
> left 60% = real material swatches,
> right 40% = 2–3 reference images showing the resulting atmosphere.
>
> Derive the palette from the swatches.
>
> Do not let atmospheric imagery replace actual material specification.

## Neye dikkat edilmeli?

Ölçek tutarlılığı için tek bir insan-ölçekli referans nesne koyun; modelin devasa ya da ufak kaçan öğelerini bu referansla yakalayın.

---
# 1700. Bu turdaki slash-style indeks (aile-023)

| Kısayol | Aile |
|---|---|
| `/handwritten` | consistent handwritten annotation |
| `/handwritten-product` | product + handwritten callouts |
| `/handwritten-photo-notes` | source photo + marginal notes |
| `/handwritten-recipe` | kitchen-notebook layout |
| `/handwritten-map` | personal map annotations |
| `/sketchnote` | visual note-taking |
| `/guided-sketchnote` | scaffolded visual notes |
| `/partial-sketchnote` | partially completed learning visual |
| `/sketchnote-linear` | sequential visual notes |
| `/sketchnote-radial` | radial visual notes |
| `/sketchnote-path` | path-based notes |
| `/sketchnote-compare` | comparative notes |
| `/sketchnote-legend` | reusable visual vocabulary |
| `/sketchnote-student` | learner-made note aesthetic |
| `/visual-study-notes` | compact revision page |
| `/study-notes-core` | learning-critical core |
| `/study-notes-question-led` | question-organized study page |
| `/study-notes-recall` | retrieval-based study notes |
| `/ingredient-breakdown` | ingredients separated from final |
| `/ingredient-breakdown-topdown` | top-down ingredient layout |
| `/ingredient-lineup` | ordered ingredient comparison |
| `/ingredient-to-result` | ingredients → final product |
| `/material-breakdown` | object by physical material |
| `/material-board` | real material selection board |
| `/material-swatch` | one material study |
| `/material-family` | same material, multiple finishes |
| `/material-aging-board` | aging behavior comparison |
| `/material-junction` | material connection detail |
| `/specimen-board` | comparative specimen presentation |
| `/specimen-grid` | consistent specimen grid |
| `/specimen-scale` | measured specimen view |
| `/specimen-variation` | variation within one class |
| `/specimen-outlier` | controlled outlier emphasis |
| `/specimen-provenance` | specimen source record |
| `/collection-sheet` | coherent collection overview |
| `/collection-lineup` | ordered collection |
| `/collection-completion` | owned vs missing items |
| `/collection-archive-card` | collection metadata card |
| `/museum-interpretation-panel` | short interpretation panel |
| `/look-closer-label` | visual-detail museum label |
| `/technique-label` | making-technique label |
| `/context-label` | concise contextual label |
| `/comparison-label` | observation-based comparison |
| `/child-museum-label` | child-accessible interpretation |
| `/museum-label-length` | text-length hierarchy control |
| `/diorama` | physical miniature scene |
| `/open-diorama` | open-front display miniature |
| `/museum-diorama` | evidence-aware educational diorama |
| `/process-diorama` | process shown physically |
| `/cutaway-diorama` | sectioned physical miniature |
| `/diorama-scale-cue` | explicit miniature scale |
| `/editorial-illustration` | article/concept visual |
| `/editorial-metaphor` | one visual metaphor |
| `/editorial-contrast` | one controlled contrast |
| `/editorial-object-swap` | meaning through object substitution |
| `/editorial-negative-space` | negative-space concept |
| `/editorial-sequential` | short editorial sequence |
| `/visual-vocabulary-sheet` | reusable concept drawings |
| `/visual-translation` | verbal → visual relationship |
| `/notes-integration-check` | drawing/text integration audit |
| `/material-vs-moodboard` | clarify board purpose |
| `/material-moodboard-hybrid` | physical material + atmosphere |

---
