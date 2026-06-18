# BusinessHTML

Bundle reklam formatlarının **AI destekli HTML prototipleri**. Figma tasarımları, paylaşılabilir ve etkileşimli HTML mockup'lara birebir çevrildi.

Amaç: tekrar eden reklam ailelerinde (masthead, quiz, advertorial vb.) ilk mockup/prototip döngüsünü hızlandırmak — business ekibinin Figma'yı düzenlemeden inandırıcı, çalışan bir ilk versiyon üretip üretemeyeceğini test etmek.

## 🔗 Canlı Linkler (paylaşılabilir)

| Proje | Açıklama | Link |
| --- | --- | --- |
| **Ana sayfa** | 3 demoya açılan vitrin | https://seymakucuk0.github.io/BusinessHTML/ |
| **Carte d'Or — Interactive Masthead** | Soru → öneri kayan masthead | https://seymakucuk0.github.io/BusinessHTML/cartedor_interactive_masthead/ |
| **Bioderma — Interactive Masthead** | Yeşil soru → ürün öneri masthead | https://seymakucuk0.github.io/BusinessHTML/bioderma_interactive_masthead/ |
| **Jolly — Dünya Kupası Quiz** | Tam ekran, skor bazlı quiz akışı | https://seymakucuk0.github.io/BusinessHTML/jolly_worldcup_quiz/ |

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

## 🎨 Yöntem
- Tasarımlar Figma MCP ile incelendi; renkler, metinler, fontlar ve görseller **doğrudan Figma'dan** alındı.
- Markaların lisanslı fontları (Juana, Gilroy) yerine en yakın web karşılıkları (Playfair Display / Poppins) kullanıldı; geri kalan her şey orijinal tasarıma sadıktır.
- Her proje kendi `assets/` klasörüyle birlikte tek başına çalışır (bağımlılık yok, statik HTML/CSS/JS).

Konuşma akışı ve verilen promptlar için: [CONVERSATION.md](CONVERSATION.md)
