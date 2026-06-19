# Konuşma & Süreç Kaydı

Bu repodaki HTML prototipleri, aşağıdaki istekler doğrultusunda Figma tasarımlarından
birebir üretildi. Her başlıkta **verilen prompt** (özet/aktarım) ve **yapılanlar** yer alır.

Tarih: 2026-06-18

---

## 1. Carte d'Or — Interactive Masthead

**Prompt (özet):**
> Figma'daki *Business — Projects 2024-2025* dosyasında, Mockup Pages altındaki Interactive
> Masthead'lerin en üstündekini birebir HTML'e dök. Bundle sayfası olacak (üstte Tümü / Gündem /
> Teknoloji vb. sekmeler), sayfa kaydırılabilir olacak; bir "test" butonuna basılınca tasarımdaki
> gibi ikinci görsel (sonuç) gelecek. Figma'daki öğeleri, fontları ve fotoğrafları **birebir**
> kullan. Dikkat: tasarım Figma'da görünenin altında devam ediyor; telefon ekranındaki içerik orada.
>
> (Ayrıca "Bundle Banner AI + HTML Vibe Coding Çalışması" brief'i paylaşıldı: tekrar eden reklam
> ailelerinde — push/advertorial, quiz, pop-up, carousel commerce, masthead, landing — AI destekli
> ilk mockup'ların üretilip üretilemeyeceğini test etmek; template-first yaklaşım.)

**Yapılanlar:**
- Figma MCP ile dosya tarandı; en üstteki **İnteraktive Masthead** (Carte d'Or) frame'i bulundu.
- İki telefonun aynı ekranın iki hâli olduğu tespit edildi: **soru durumu** ("Nasıl bir tarif
  istersiniz?" + 2 seçenek) ve **sonuç durumu** ("Carte d'Or Dondurmalı Cupcake" + "Tarifi gör").
- Renkler (`#975038`, `#2e1b05`…), metinler, sekmeler ve gerçek haber kartları (Apple Watch, roket,
  Meghan, yanardağ) Figma'dan alındı; logo ve cupcake görselleri indirildi.
- Tek sayfada telefon mockup'ı + kaydırılabilir feed + tıklayınca sonuca **kayan** masthead kuruldu.

## 2. Düzeltmeler + Bioderma

**Prompt (özet):**
> Bunu `cartedor_interactive_masthead` tarzı bir isimle klasöre kaydet. Hemen altındaki Bioderma'yı
> da yap. Düzenin **birebir** olmasını istiyorum: ilk sayfada masthead yanlardan boşluksuz (full)
> olmalı; ayrıca kendin uydurduğun "SPONSORLU" satırı gibi Figma'da olmayan öğeler ekleme.

**Yapılanlar:**
- Klasör yapısı kuruldu; Carte d'Or düzeltildi: masthead **full-bleed** yapıldı, uydurma "SPONSORLU"
  satırı kaldırıldı, sayfa sade telefon görünümüne indirildi.
- Bioderma masthead'i Figma'dan çıkarıldı: yeşil soru ekranı (`#89bd1e`, "Sivilce oluşumuna neden
  olan etkenler nelerdir?" + 2×2 şık) → açık temalı sonuç (BIODERMA logosu + "Sivilceler senin için
  sorun olmasın." + Sébium ürün görseli + "Satın al"). Feed'de GOSTERCO/Pixar "Soul" kartı.

## 3. Jolly — Dünya Kupası Quiz

**Prompt (özet):**
> (Yeni Figma dosyası — *Jolly · Dünya Kupası Quiz / Premium Bundle Studio*.) Buradaki akışı anlat ve
> birebir tasarla. Akış daha uzun ve karmaşık; **tam ekran** bir deneyim olacak ve **her şey
> çalışabilir** olacak. En sondaki "Rotanı Belirle" (sonuç) butonu
> `jollytur.com/yaz-firsatlari?...` adresine yönlendirsin.

**Yapılanlar:**
- 10 ekran incelendi; akış çözüldü: **Giriş → 4 soru → skora göre 5 sonuç (0/4–4/4)**.
- Tek sayfalık, viewport'a ölçeklenen tam ekran SPA kuruldu. Sorular: şıkka dokun → kısa bekleme →
  sonraki soru; skor tutulur. Tüm metin/emoji/CTA'lar (🏆⚽👏😊🏖️) Figma'dan birebir alındı.
- Arka plan görselleri (stadyum/kupa, havuz+aile+Jolly swoosh) ve Jolly logosu indirildi.
- Tüm sonuç tiplerinin CTA'sı `jollytur.com/yaz-firsatlari` adresine yönlendirir.

## 4. Quiz iyileştirmeleri

**Prompt (özet):**
> İki değişiklik: (1) yeni sorular **aşağı kayarak** gelsin; (2) yanlış cevapta — Figma'da olmayan
> ama istediğim davranış — **yanlış işaretlenen şık solgun**, **doğru şık kırmızı ve tikli** olsun.

**Yapılanlar:**
- Yeni soru geçişi yukarıdan aşağı kayan animasyona çevrildi.
- Yanlış seçimde: seçilen yanlış şık soluklaştırılır, doğru cevap kırmızı + tik ile gösterilir.

## 5. Carte d'Or / Bioderma ince ayarlar

**Prompt (özet):**
> Carte d'Or'da quizden sonraki (sonuç) sayfada yanlardan **biraz padding** var Figma'da; ilk (soru)
> sayfada padding yok — buna dikkat et. Bioderma'da ürün Figma'ya göre **çok sağda** kalmış; düzelt.

**Yapılanlar:**
- Carte d'Or: soru ekranı full-bleed kaldı; sonuç ekranı **içeri girintili** (yanlardan ~13px
  padding, yuvarlatılmış panel) yapıldı — Figma'daki `image256` ölçülerine göre.
- Bioderma: ürün tüpü sola çekildi (sağ kenardan ~40px), eğim 13°'ye ayarlandı.

## 6. Yayınlama

**Prompt (özet):**
> `business` klasörünü `seymakucuk0` hesabında **BusinessHTML** adıyla repoya push'la; bu sohbetteki
> promptları ve yapılanları da ekle. Katkıda yalnızca `seymakucuk0` görünsün. 3 HTML için
> paylaşılabilir 3 link oluştur.

**Yapılanlar:**
- `business/` git deposuna çevrildi, GitHub'da `seymakucuk0/BusinessHTML` (public) olarak yayınlandı.
- GitHub Pages açıldı; 3 proje için paylaşılabilir linkler oluşturuldu (bkz. [README.md](README.md)).
- Commit'ler yalnızca `seymakucuk0` adına yazıldı (ek katkı sahibi yok).

## 7. İş Bankası — Koşu Oyunu
İnteraktif Bundlestition (pixel koşu oyunu) Figma'dan birebir alındı: giriş → "Hızlan"a seri bas
(yol kayar, FINISH iner/karakter ilerler) → İstanbul Maratonu reklamı ("Hemen Kaydol"). Logo ve
karakterin gömülü beyaz kutuları temizlendi (şeffaf), pop-up ölçü/konumları düzeltildi, X gerçekten kapatır.

## 8. Dyson — Custom Masthead
"Kış Fırsatları" carousel'i. Önce yaklaşık ölçeklenmişti; geri bildirim üzerine Figma'nın **birebir
piksel değerleriyle** (panel 248, kart 202×250, başlık 34px…) yeniden kuruldu. 3 ürün **sonsuz
döngüyle** kayar (oklar + sürükle), ekstra ürün eklenmedi.

## 9. Knorr — İnteraktif Bundlestition
Tinder usulü yemek eşleştirme. Figma'daki 2 eşleşme 4 kart boyunca döner; 4 kart sonrası sonuç
(Acılı Ekşili Kış Çorbası). Geri bildirimlerle: ürün arkası şeffaflaştırıldı, pop-up ölçüsü/ortalaması
düzeltildi, logo–başlık mesafesi ayarlandı, arkadaki kart düz bırakıldı.

## 10. NIVEA — İnteraktif Masthead (responsive)
Veri toplayan full-bleed yatay banner: 4 etki → seçime göre farklı ürün ekranı + farklı Keşfet
yönlendirmesi. **Container-query** ile her ekrana ölçeklenir; iPhone 14 Pro / 15 Pro / 17 Pro Max /
Samsung S20 cihaz önizlemesi. Şıka basınca Figma'daki solgun seçili hâl; soru→sonuç yatay kayma geçişi.
Geri bildirim üzerine köşeler düz + tam genişlik (full-bleed) yapıldı.
