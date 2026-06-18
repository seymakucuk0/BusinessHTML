# Bundle Banner AI + HTML Vibe Coding Çalışması

Tarih: 2026-06-18

Figma kaynağı: [Business Projects 2024 2025](https://www.figma.com/design/tJveFEiRvvEkYcHuzO6gH0/Business---Projects-2024-2025?node-id=1271-117&m=dev&t=Ul3qsh8g674i5tmf-1)

## Görev Tanımı

Bu projenin amacı, Bundle için business ekibiyle hazırlanan banner ve reklam mockup tasarımlarının AI destekli HTML prototipleriyle hızlandırılıp hızlandırılamayacağını test etmektir.

Bugünkü süreç genelde reklam veren brief'i, business ekibi, tasarımcı ve yazılımcı arasında ilerliyor. Bu akış özel ve yüksek prodüksiyonlu işler için gerekli; fakat push destekli advertorial, quizli reklam, pop-up/interstitial, carousel commerce, masthead ve landing page uzantısı gibi tekrar eden formatlarda ilk mockup döngüsünü yavaşlatabiliyor.

Ana soru:

Business ekibi, AI yardımıyla güvenilir bir ilk tasarım/prototip seviyesine ulaşabilir mi? Ulaşabilirse tasarımcı ve yazılımcı daha çok kalite kontrol, polish, özel etkileşim, animasyon, entegrasyon ve production güvenliği için mi devreye girmeli?

İlk hipotez: Evet, ama yalnızca şablonlaşabilen reklam ailelerinde. Hedef tasarımcıyı veya developer'ı süreçten çıkarmak değil; tekrarlı işleri hızlandırmak, ilk fikir/mockup üretimini business tarafına yaklaştırmak ve hangi senaryoların production'a gitmeden önce hızlıca denenebileceğini görmek.

## Mevcut Kaynaklar

Bu ilk incelemede kullanılan kaynaklar:

- Figma içinde `Template` sayfası ve `Mockup Pages` bölümü.
- Figma sayfasında tespit edilen 259 adet üst seviye 1280x720 mockup frame'i.
- Figma mockup alanından alınmış 7 ekran görüntüsü.
- Masthead, studio, survey, commerce, bülten, push, içerik paketi ve AI odaklı format etiketleri.

Görsel referanslar:

![Masthead, Custom Masthead, Video Masthead](assets/mockups/01-masthead-custom-video.png)

![Custom Videostition, Premium Studio, Video Premium Studio](assets/mockups/02-videostition-premium-studio.png)

![Morning Bundle, Bundle Studio, Audience Ad](assets/mockups/03-morning-bundle-studio-audience.png)

![Wordle Brandle, Interaktif Bundlestition, In App Push](assets/mockups/04-wordle-interactive-inapp.png)

![Bundle AI Studio, Survey, ECOM](assets/mockups/05-ai-studio-survey-ecom.png)

![Bülten, Carstition, İçerik Paketi, AI Bülten](assets/mockups/06-bulten-carstition-content-ai.png)

![Masthead Retarget, LP, Reviews, Lines](assets/mockups/07-retarget-lp-reviews-lines.png)

## Mockup Tip Envanteri

`Mockup Pages` satırında görünen ana tipler:

- Interactive Masthead
- Custom Masthead
- Video Masthead
- Custom Videositition
- Premium Studio
- Video Premium Studio
- Morning Bundle
- Bundle Studio
- Audience Ad
- Wordle Brandle
- Interaktif Bundlestition
- In App Push
- Bundle AI Studio
- Survey
- ECOM Bülten / ECOM AI
- Bülten
- Carstition
- İçerik Paketi
- AI Bülten
- Push Kategori
- Masthead + Retarget
- Masthead + LP
- Bundle AI Reviews
- Bundle Lines
- Bundle AI Summary Ads
- Premium Bundle AI

Figma isimlendirme notu: Dosyada bazı etiketlerin farklı yazımları var. Örneğin `Interactive/İnteraktive`, `Videostition/Videositition`, `Bundlestition` gibi varyasyonlar görünüyor. HTML tarafında bunları stabil template ID'lerine normalize etmek gerekir.

## Stil Aileleri

| Aile | Örnekler | Temel davranış | HTML uygulanabilirliği | Business ekibi uygunluğu |
| --- | --- | --- | --- | --- |
| Push + advertorial | Morning Bundle, Audience Ad, Premium Bülten, AI Bülten, İçerik Paketi | Push notification kullanıcıyı makale/reklam içeriğine taşır. Genelde sponsor etiketi, hero görsel, metin ve CTA vardır. | Yüksek | Yüksek |
| In-app push / pop-up | In App Push, Push Kategori | Bundle feed veya makale üzerinde floating CTA / alt popup görünür. | Yüksek | Yüksek |
| Survey / quiz | Survey, Interaktif Bundlestition | Interstitial soru, seçenekler, seçili state, sonuç ekranı veya retargeting push. | Orta-yüksek | Form tabanlı editörle orta-yüksek |
| Commerce carousel | ECOM, ECOM mobil, ECOM web, Carstition, Productstition, Bundle Lines | Ürün/haber kartları, yatay kaydırma, görsel kartlar, fiyat veya CTA, landing page. | Orta-yüksek | Orta-yüksek |
| Masthead | Interactive Masthead, Custom Masthead, Video Masthead | Feed üstünde takeover alanı, markalı hero, bazen soru/video/countdown. | Orta | Orta |
| Masthead + journey | Masthead + Retarget, Masthead + LP, Custom Masthead + LP | Banner sonrası push retargeting veya landing page devamı. | Orta | Orta |
| Studio / editorial derin içerik | Premium Studio, Video Premium Studio, Bundle Studio | Markalı uzun hikaye/makale deneyimi, özel story sayfaları, bazen video. | Orta | Orta-düşük |
| AI odaklı içerik | Bundle AI Studio, Bundle AI Reviews, Bundle AI Summary Ads, Premium Bundle AI | AI chat, review, özet veya öneri hissi veren arayüzler. | Orta | Statik mock data ile orta |
| Oyunlaştırılmış formatlar | Wordle Brandle, Crossup Brandle | Oyun mekaniği, klavye/grid/score/result state'leri. | Orta-düşük | Düşük |
| Ağır animasyon/video | Custom Video Masthead, Video Premium Studio | Zamanlama, motion, video, geçiş ve state yönetimi önemlidir. | Düşük-orta | Düşük |

## Görsel Sistem Gözlemleri

Mockupların çoğunda ortak bir sunum dili var:

- Sol tarafta koyu panel: `Example Case`, format açıklaması, push badge ve marka logosu.
- Sağ tarafta açık panel: telefonlar, landing page, makale sayfası veya web preview.
- Mobil formatlarda ana canvas olarak iPhone mockup'ları kullanılıyor.
- Push akışını anlatmak için yeşil kıvrımlı oklar yer alıyor.
- Her mockup ailesinin üstünde beyaz, yuvarlatılmış bölüm etiketi var.
- Reklamın içinde marka rengi baskın; Bundle UI ise tanınabilir kalıyor.
- CTA metinleri kısa ve aksiyon odaklı: `Hemen Keşfet`, `Satın Al`, `Keşfet`, `Devam Et` gibi.
- Çoğu format daha küçük bileşenlere ayrılabilir: push card, telefon frame'i, makale kartı, hero image, quiz option, product card, CTA button, sponsor chip, carousel track.

HTML replikasyonunda Figma'daki sunum panosundan çok reklam deneyiminin kendisi önemli. Yani üretilecek HTML; mobil ekranı, makale/landing sayfasını, push overlay'i, carousel'i, quiz state'ini ve CTA davranışını canlandırmalı.

## İlk Uygulanabilirlik Değerlendirmesi

Business tarafında AI destekli üretime en uygun adaylar, yapısı öngörülebilir ve özel logic ihtiyacı düşük olan formatlar:

1. In App Push + Landing/Article
2. Morning Bundle / Audience Ad / Premium Bülten
3. Survey / Quiz Interstitial
4. ECOM Carousel / Product Cards
5. Basit/statik Custom Masthead + LP

İlk aşamada tasarımcı/developer ağırlıklı kalması daha doğru olan formatlar:

- Wordle Brandle ve gerçek oyun mekaniği içeren formatlar.
- Video Masthead, özellikle timing, motion ve video edit kalitesi önemliyse.
- Çok art-directed Premium Studio sayfaları.
- Gerçek canlı AI davranışı gerektiren AI chat/review formatları.
- Sıkı marka/legal review veya standart dışı interaction gerektiren kampanyalar.

## Önerilen Pilot Template'ler

İlk HTML replikasyon fazında 3-4 stili seçmek mantıklı:

1. `push-advertorial`
   - Morning Bundle, Audience Ad, Premium Bülten, AI Bülten ve İçerik Paketi formatlarını kapsar.
   - Business input: sponsor, push metni, başlık, hero görsel, gövde metni, CTA, destination URL.
   - Neden ilk pilot: tekrar oranı yüksek, teknik riski düşük.

2. `survey-quiz`
   - Survey ve daha basit Interaktif Bundlestition akışlarını kapsar.
   - Business input: soru, seçenekler, marka renkleri, ürün görseli, sonuç metni, retarget push metni.
   - Neden pilot: interaktif değeri yüksek, JSON config ile yönetilebilir.

3. `ecom-carousel`
   - ECOM, ECOM mobil/web, Carstition/Productstition ve Bundle Lines formatlarını kapsar.
   - Business input: ürün kartları, görseller, fiyat veya makale başlıkları, CTA label, tracking/deeplink.
   - Neden pilot: kart/carousel mantığı tekrar kullanılabilir.

4. `custom-masthead-lp`
   - Custom Masthead, Interactive Masthead, Masthead + LP ve Masthead + Retarget formatlarını kapsar.
   - Business input: marka hero'su, headline, CTA, makale kartları, opsiyonel soru, opsiyonel LP bloğu.
   - Neden pilot: ticari olarak önemli; fakat ilk aşamada motion'sız/statik denenmeli.

## HTML Replikasyon Yaklaşımı

HTML sistemi serbest tasarım üretiminden önce template-first ilerlemeli.

Önerilen yapı:

- `templates/`: Her reklam ailesi için bir HTML/CSS/JS implementasyonu.
- `configs/`: Business ekibinin doldurduğu veya AI'ın ürettiği campaign JSON dosyaları.
- `assets/`: Reklam veren görselleri, ürün görselleri, logolar ve preview screenshot'ları.
- `preview/`: Kampanya ve viewport seçmek için basit bir index sayfası.

Örnek config:

```json
{
  "template": "survey-quiz",
  "brand": {
    "name": "Vodafone",
    "logo": "assets/vodafone.svg",
    "primaryColor": "#e60000",
    "secondaryColor": "#ffffff"
  },
  "copy": {
    "headline": "Vodafone kullanıcısı mısın?",
    "body": "Kısa bir soruyu cevapla, sana uygun teklifi görelim.",
    "cta": "Devam Et"
  },
  "interaction": {
    "question": "Vodafone kullanıcısı mısın?",
    "options": ["Evet", "Değilim", "Değişim"],
    "retargetPush": "Vodafone FLEX'in avantajları seni bekliyor."
  },
  "assets": {
    "heroImage": "assets/campaign/hero.png"
  }
}
```

AI'ın rolü, brief'i bu kontrollü config yapısına çevirmek ve birkaç copy/layout varyasyonu önermek olmalı. Bu, AI'a her seferinde tamamen serbest layout ürettirmekten daha güvenli ve sürdürülebilir.

## Business Akışı Önerisi

1. Business kullanıcısı reklam ailesini seçer.
2. Advertiser brief'i, brand asset'leri, zorunlu metinleri, ürün görsellerini ve hedef aksiyonu girer.
3. AI bir campaign config'i ve 2-3 copy/layout varyasyonu önerir.
4. HTML preview mobil ve gerekiyorsa desktop/web görünümünde render edilir.
5. Business ekibi yön seçer.
6. Tasarımcı görsel kalite, marka uyumu ve polish kontrolü yapar.
7. Developer yalnızca production entegrasyonu, advanced interaction, animasyon, tracking ve özel ihtiyaçlarda devreye girer.

Bu akış business ekibini hızlandırır; fakat kompleks reklamların son production sorumluluğunu business tarafına bırakmaz.

## Başarı Kriterleri

Pilot şu soruları cevaplamalı:

- Business kullanıcısı Figma edit etmeden inandırıcı bir ilk mockup çıkarabiliyor mu?
- Aynı template farklı markalarda yalnızca config ve asset değiştirerek çalışıyor mu?
- HTML preview tasarımcı/developer clarification döngüsünü azaltıyor mu?
- Hangi formatlar animasyon, marka karmaşıklığı, legal copy veya özel logic yüzünden kırılıyor?
- Figma MCP, HTML output'u mevcut mockup ile karşılaştırmak için yeterince iyi referans sağlayabiliyor mu?

## Sonraki Adım

Bir sonraki aşamada 3-4 pilot stil seçilip HTML replikasyonlarına başlanmalı. Önerilen sıra:

1. In App Push / push-advertorial
2. Survey / quiz
3. ECOM carousel
4. Custom Masthead + LP

Her pilot için Figma MCP ile seçilen referans frame incelenmeli, ölçü/screenshot alınmalı ve lokal HTML versiyonu Figma mockup'ı ile görsel olarak karşılaştırılmalı.
