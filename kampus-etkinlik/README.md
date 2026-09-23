# Kampüs Etkinlikleri - Sprint 1

Bu proje, üniversite kampüsündeki etkinliklerin duyurulması, detaylarının incelenmesi ve yeni etkinliklerin eklenmesi için geliştirilen Kampüs Etkinlikleri web platformunun **Sprint 1 (HTML, Git ve Yayına Alma)** aşamasıdır.

## 🔗 Canlı Yayın (Vercel)
- **Vercel Canlı URL:** `https://web-tech-project-sprint1.vercel.app` *(veya Vercel üzerinde oluşturulan canlı adresiniz)*
- **GitHub Repository:** `https://github.com/MehmetKutlu32/web-tech-project`
- **Git Etiketi (Tag):** `sprint-01`

---

## 📁 Proje Klasör Yapısı
```text
kampus-etkinlik/
│
├── sprint1/
│   ├── index.html               # Ana Sayfa (Tanıtım, amaç, yaklaşan 2 etkinlik, linkler)
│   ├── etkinlikler.html         # Etkinlik Listesi (<table border="1"> tek hücreli kartlar + Ayın Programı)
│   ├── etkinlik-detay.html      # Etkinlik Detayı (Afiş, dl/dt/dd künye listesi, detaylı açıklama)
│   ├── etkinlik-ekle.html       # Etkinlik Ekleme Formu (Görünür label'lar, required doğrulaması)
│   ├── etkinlik-guncelle.html   # Güncelleme Formu (Önceden dolu value'lar + Güncelle butonu)
│   └── afis.jpg                 # Örnek etkinlik afişi görseli
│
├── .gitignore                   # İstenmeyen sistem/editör dosyalarını yok sayma listesi
└── README.md                    # Sprint 1 dokümantasyonu ve teslim bilgileri
```

---

## 📋 Sayfalar ve Semantik HTML Özellikleri

1. **`index.html` (Ana Sayfa)**:
   - Ortak `header`, `nav`, `main`, `footer` iskeleti.
   - Sayfada tek bir `<h1>` başlığı.
   - Uygulamanın amacı ve tanıtım metni.
   - Yaklaşan 2 etkinlik kartı (`<article>`, `<time>`).
   - Diğer sayfalara çalışan semantik bağlantılar.

2. **`etkinlikler.html` (Etkinlikler Listesi)**:
   - `<table border="1">` ve `<caption>Etkinlikler</caption>` ile çerçeveli tek sütunlu kart yapısı.
   - Her etkinlik `<tr><td>` tek bir hücre içerisinde ve elemanlar (`<h2>`, kategori/tarih/yer `<time>`, kısa açıklama, detay linki) birebir aynı sırada.
   - Altında `Ayın Programı` özet tablosu (`<th>`, `<tr>`, `<td>`).

3. **`etkinlik-detay.html` (Detay Sayfası)**:
   - `<h1>Kariyer Günleri 2026</h1>`
   - `<figure>`, `<img>` ve `<figcaption>` ile afiş görseli.
   - `<dl>`, `<dt>`, `<dd>` ve `<time>` etiketleriyle biçimlendirilmiş künye listesi (tarih, yer, kategori, kontenjan).
   - Detaylı açıklama paragrafları ve listeye dönüş linki.

4. **`etkinlik-ekle.html` (Etkinlik Ekleme)**:
   - Tüm form alanları için görünür `<label for="...">` etiketleri.
   - `input` (text, date, time, number), `select`, `textarea` elemanları.
   - Tüm alanlarda aktif `required` HTML5 doğrulaması.
   - `Kaydet` butonu.

5. **`etkinlik-guncelle.html` (Etkinlik Güncelleme)**:
   - Ekleme formuyla birebir aynı form alanları.
   - Tüm alanlar mevcut etkinlik bilgileriyle (`value="..."`) dolu.
   - `Güncelle` butonu.

---

## 🚀 Yerel Olarak Çalıştırma
Herhangi bir tarayıcıda doğrudan `sprint1/index.html` dosyasını açarak veya VS Code Live Server / basit bir HTTP sunucusu ile görüntüleyebilirsiniz:

```bash
# Tarayıcıda açmak için (Windows PowerShell):
Start-Process .\kampus-etkinlik\sprint1\index.html
```

---

## 👤 Geliştirici Bilgileri
- **Öğrenci Adı Soyadı:** Mehmet Kutlu
- **Öğrenci Numarası:** 2416501002
- **Tarih:** 2026
