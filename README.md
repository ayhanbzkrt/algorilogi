# algorilogi
Algori ve Logi Kitabındakihikayemizin öğrenme portalı.
# Algori & Logi — Python Öğrenme Portalı (Pyodide + 3D Kristaller)

Çocuklar için oyunlaştırılmış, tek dosya (single-file) bir **Python öğrenme portalı**.  
Ders → pratik → quiz → **6 taş parçası** toplama → **sertifika** akışıyla çalışır.  
Python kodları tarayıcı içinde **Pyodide (gerçek Python)** ile çalıştırılır; Pyodide yüklenemezse **Mini-Python fallback** devreye girer.

---

## Özellikler
- ✅ 6 derslik ilerleme sistemi (kilitli ders akışı)
- ✅ Pyodide ile tarayıcıda gerçek Python çalıştırma
- ✅ 3D taş/kristal sistemi (Three.js)
- ✅ Quiz ile ders tamamlama ve taş kazanma
- ✅ Sertifika ekranı + isim girişi
- ✅ İlerleme kaydı: `localStorage`

---

## Kurulum (GitHub Pages)
1. Repoya **`index.html`** dosyası olarak bu tek HTML dosyasını ekleyin (tamamını kopyalayın).
2. GitHub → **Settings → Pages**
3. Source: **Deploy from a branch**
4. Branch: **main** / folder: **/(root)**
5. Save → Sayfanız birkaç dakika içinde yayında olur.

> Not: Dosya tek parça olduğu için en sorunsuz yöntem adı `index.html` yapmaktır.

---

## Yerel Çalıştırma
Bu proje CDN kullandığı için doğrudan çift tıkla da açılabilir; fakat bazı tarayıcılarda güvenlik kısıtları olabilir.  
Öneri (en temiz yöntem):
- VS Code → **Live Server** eklentisi ile açın  
veya
- Basit bir HTTP server ile servis edin.

---

## Bağımlılıklar (CDN)
HTML içinde zaten ekli:
- **Pyodide v0.25.1**
- **Three.js r128**
- Google Fonts + Font Awesome

---

## Veri Kaydı (LocalStorage Keys)
Tarayıcıda ilerleme ve isim şu anahtarlarla saklanır:
- `algori_logi_progress_v8` (tamamlanan dersler)
- `algori_logi_student_name_v8` (öğrenci adı)
- `algori_logi_crystals_v8` (toplanan taşlar)

Sıfırlamak için tarayıcı depolamasını temizleyebilirsiniz:
- DevTools → Application → Local Storage → ilgili domain → delete keys

---

## Bilinen Notlar
- `input()` bu portalda **bilinçli olarak kapalıdır** (çocuk dostu akış + güvenlik).  
  Kodlarda `input()` kullanılırsa Pyodide “kullanılmıyor” hatası verir.
- Sertifika “PNG/PDF indir” butonları şu an demo akışında **gerçek dosya üretmez**.  
  (İstersen gerçekten PNG/PDF üreten sürümü de ekleyebilirim: `html2canvas` + `jspdf` ile, yine single-file uyumlu.)

---

## Lisans
İstediğin lisansı koyabilirsin:
- MIT önerilir (açık kaynak)
- veya “All Rights Reserved” (telifli)

---

## Kredi / İmza
**AI'Han Academy — Algori & Logi**
