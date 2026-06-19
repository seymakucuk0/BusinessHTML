# BusinessHTML

Bundle reklam formatlarının **AI destekli HTML prototipleri**. Figma tasarımları, paylaşılabilir ve etkileşimli HTML mockup'lara birebir çevrildi.

Amaç: tekrar eden reklam ailelerinde (masthead, quiz, advertorial vb.) ilk mockup/prototip döngüsünü hızlandırmak — business ekibinin Figma'yı düzenlemeden inandırıcı, çalışan bir ilk versiyon üretip üretemeyeceğini test etmek.

## 🔗 Canlı Linkler (paylaşılabilir)

| Proje | Açıklama | Link |
| --- | --- | --- |
| **Ana sayfa** | 7 demoya açılan vitrin | https://seymakucuk0.github.io/BusinessHTML/ |
| **Carte d'Or — Interactive Masthead** | Soru → öneri kayan masthead | https://seymakucuk0.github.io/BusinessHTML/cartedor_interactive_masthead/ |
| **Bioderma — Interactive Masthead** | Yeşil soru → ürün öneri masthead | https://seymakucuk0.github.io/BusinessHTML/bioderma_interactive_masthead/ |
| **Jolly — Dünya Kupası Quiz** | Tam ekran, skor bazlı quiz akışı | https://seymakucuk0.github.io/BusinessHTML/jolly_worldcup_quiz/ |
| **İş Bankası — Koşu Oyunu** | Pixel koşu oyunu → İstanbul Maratonu | https://seymakucuk0.github.io/BusinessHTML/isbankasi_interactive_bundlestition/ |
| **Dyson — Custom Masthead** | Ürün carousel'i (sonsuz kaydırma) | https://seymakucuk0.github.io/BusinessHTML/dyson_custom_masthead/ |
| **Knorr — İnteraktif Bundlestition** | Tinder usulü eşleştirme → çorba | https://seymakucuk0.github.io/BusinessHTML/knorr_interactive_bundlestition/ |
| **NIVEA — İnteraktif Masthead** | Veri toplama → eşleşen ürün · responsive | https://seymakucuk0.github.io/BusinessHTML/nivea_interactive_masthead/ |

> Linkler GitHub Pages ile yayınlanır; push'tan ~1 dk sonra aktif olur.

## 📦 Projeler

### 1) `cartedor_interactive_masthead/`
Bundle haber feed'inin en üstünde **etkileşimli masthead**. İlk halde bir soru sorar
("Nasıl bir tarif istersiniz?"), bir seçeneğe dokununca **öneri tasarımına kayar**
(Carte d'Or Dondurmalı Cupcake + "Tarifi gör"). Üstte sekmeler (Tümü/Gündem/Teknoloji/Finans…),
altta gerçek haber kartları; feed kaydırılabilir.

### 2) `bioderma_interactive_masthead/`
Aynı masthead mantığı, **Bioderma** markası. Yeşil soru ekranı ("Sivilce oluşumuna neden olan
etkenler nelerdir?" — 2×2 şık) → açık temalı sonuç ("Sivilceler senin için sorun olmasın." +
BIODERMA logosu + Sébium ürün görseli + "Satın al").

### 3) `jolly_worldcup_quiz/`
**Tam ekran, tamamen çalışan** quiz deneyimi:
Giriş → 4 soru (şıkka dokun → doğruysa kırmızı+tik, yanlışsa yanlış şık solgun + doğru şık kırmızı+tik) →
skora göre 5 farklı sonuç (0/4 – 4/4). Sonuç CTA'sı **jollytur.com/yaz-firsatlari** adresine yönlendirir.

### 4) `isbankasi_interactive_bundlestition/`
**Türkiye İş Bankası** pixel koşu oyunu (İnteraktif Bundlestition). Giriş ("Ne kadar hızlı
koşabilirsin?") → "Hızlan" butonuna seri basarak karakteri yolda FINISH'e koşturma → **İstanbul
Maratonu** reklamı ("Hemen Kaydol"). Reklam X ile kapanıp altındaki Bundle feed'i gösterir.

### 5) `dyson_custom_masthead/`
**Dyson "Kış Fırsatları"** Custom Masthead. Sol tarafta buzlu cam panel (logo, başlık, rozetler),
sağda **sonsuz kayan ürün carousel'i** (3 ürün: V11 / Cyclone V10 / Cinetic — oklar + sürükle),
yeşil "Satın al". Figma'nın birebir piksel ölçüleriyle kuruldu.

### 6) `knorr_interactive_bundlestition/`
**Knorr** Tinder usulü eşleştirme. "Sence ne kadar yakışıyorlar?" — yemek kartlarını kaydır
(💔 / ❤️). 4 kart sonrası sonuç: **Acılı Ekşili Kış Çorbası** + "Satın AL". Pop-up X ile kapanır.

### 7) `nivea_interactive_masthead/`
**NIVEA** veri toplayan İnteraktif Masthead (full-bleed yatay banner). Cilt ihtiyacı sorusu (4 etki) →
seçime göre **farklı ürün ekranı** (Luminous630 / Skin Glow / Q10 / Derma Skin Clear), her birinin
**farklı Keşfet yönlendirmesi**. **Responsive** (container-query ile her ekrana ölçeklenir); ayrıca
iPhone 14 Pro / 15 Pro / 17 Pro Max / Samsung S20 cihaz önizlemesi.

## 🎨 Yöntem
- Tasarımlar Figma MCP ile incelendi; renkler, metinler, fontlar ve görseller **doğrudan Figma'dan** alındı.
- Markaların lisanslı fontları (Juana, Gilroy) yerine en yakın web karşılıkları (Playfair Display / Poppins) kullanıldı; geri kalan her şey orijinal tasarıma sadıktır.
- Her proje kendi `assets/` klasörüyle birlikte tek başına çalışır (bağımlılık yok, statik HTML/CSS/JS).

Konuşma akışı ve verilen promptlar için: [CONVERSATION.md](CONVERSATION.md)
