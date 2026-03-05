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

# Algori & Logi — Python Learning Portal (Pyodide + 3D Crystals)

A kid-friendly, gamified **Python learning portal** built as a **single-file (single HTML)** project.  
Flow: Lessons → Practice → Quiz → Collect **6 crystal stones** → **Certificate**.  
Python runs in the browser using **Pyodide (real Python)**; if Pyodide fails to load, a **Mini-Python fallback** is used.

---

## Features
- ✅ 6-lesson progression system (locked lesson flow)
- ✅ Run real Python in the browser with Pyodide
- ✅ 3D crystal/stone system (Three.js)
- ✅ Quizzes to complete lessons and earn stones
- ✅ Certificate page + name input
- ✅ Progress saved with `localStorage`

---

## Setup (GitHub Pages)
1. Add the full HTML as **`index.html`** in your repo (paste the entire file).
2. GitHub → **Settings → Pages**
3. Source: **Deploy from a branch**
4. Branch: **main** / folder: **/(root)**
5. Save → Your site will be live shortly.

> Tip: Using the filename `index.html` avoids routing issues on Pages.

---

## Run Locally
Since the project uses CDNs, it may work by opening the file directly, but some browsers apply restrictions.  
Recommended:
- VS Code → **Live Server** extension  
or
- Any simple HTTP server.

---

## Dependencies (CDN)
Already included inside the HTML:
- **Pyodide v0.25.1**
- **Three.js r128**
- Google Fonts + Font Awesome

---

## Saved Data (LocalStorage Keys)
The portal stores progress and name using:
- `algori_logi_progress_v8` (completed lessons)
- `algori_logi_student_name_v8` (student name)
- `algori_logi_crystals_v8` (collected stones)

To reset:
- DevTools → Application → Local Storage → your domain → delete these keys

---

## Known Notes
- `input()` is **intentionally disabled** (kid-safe flow + predictable UX).  
  If user code calls `input()`, Pyodide throws a “not supported in this portal” error.
- Certificate “Download PNG/PDF” buttons are currently a **demo flow** and do **not** generate real files.  
  (If you want real PNG/PDF export, it can be added using `html2canvas` + `jsPDF` while keeping it single-file friendly.)

---

## License
Choose what you prefer:
- MIT (recommended for open source)
- or “All Rights Reserved”

---

## Credit
**AI'Han Academy — Algori & Logi**
