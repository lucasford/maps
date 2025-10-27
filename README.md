# Balıkesir Harita Uygulaması

Balıkesir bölgesini gösteren interaktif bir web harita uygulaması. Bu uygulama ile harita üzerinde poligonlar ve çizgiler çizebilir, bunları çeşitli formatlarda dışa aktarabilirsiniz.

## Özellikler

- **İnteraktif Harita**: Balıkesir merkezli harita, 7 farklı altlık harita seçeneği
  - 🛰️ Uydu Görünümü (varsayılan) - Yüksek çözünürlüklü uydu görüntüleri
  - 🌍 Hibrit - Uydu görünümü + etiketler
  - 🗺️ OpenStreetMap - Klasik harita görünümü
  - 🏙️ Esri World Street - Detaylı sokak haritası
  - 🎨 CartoDB Voyager - Renkli ve modern tasarım
  - ⚪ CartoDB Positron - Temiz, minimal beyaz tema
  - ⚫ CartoDB Dark Matter - Koyu tema
- **Çizim Araçları**:
  - Poligon (Kapalı alan) çizimi
  - Çizgi (Polyline) çizimi
  - Dikdörtgen çizimi
  - Daire çizimi (standart)
  - İşaretçi ekleme
- **Gelişmiş Çizim Araçları**:
  - 🔵 **Özel Yarıçaplı Daire**: Kullanıcının belirlediği yarıçapta (metre) daire çizimi
    - Renk seçimi
    - Mouse ile sürüklenebilir
    - Alan ve yarıçap bilgisi
  - 🚶 **İnsan Simgesi**: Harita üzerine insan emoji simgesi ekleme
    - Boyut ayarlama (20-100px)
    - Sürüklenebilir
    - Tıklayarak boyut değiştirebilme
  - 📝 **Text Etiketi**: Harita üzerine çok satırlı yazı ekleme
    - Font seçimi (Arial, Times New Roman, Courier, vb.)
    - Boyut ayarlama (12-72px)
    - Renk seçimi
    - **Çok satırlı metin desteği** (Enter ile satır atlama)
    - Sürüklenebilir
    - Tıklayarak metin değiştirebilme
- **Katman Yönetimi (Layer Panel)**:
  - 📋 Sağ tarafta açılır/kapanır katman paneli
  - Tüm çizimleri listeler
  - Her katman için:
    - 👁️ Görünürlük açma/kapama
    - 🎨 Renk değiştirme (poligon, çizgi, daire için)
    - 🗑️ Tek tek silme
  - Katman ismi ve türü gösterimi
- **Düzenleme**: Çizilen şekilleri düzenleme ve silme
- **Export Formatları**:
  - GeoJSON (.geojson)
  - KML (.kml) - Google Earth uyumlu
  - WKT (.wkt) - Well-Known Text
  - 📄 **PDF** - Gelişmiş PDF export:
    - Önizleme özelliği
    - Özel başlık girişi
    - Logo ekleme (opsiyonel)
    - A4 landscape format
    - Otomatik tarih ekleme
- **Import**: Mevcut GeoJSON dosyalarını yükleme ve görüntüleme

## Kullanım

1. `index.html` dosyasını bir web tarayıcısında açın
2. Sağ üst köşedeki katman seçiciden istediğiniz altlık haritayı seçin
3. Çizim yapın:
   - **Sağ üstteki çizim araçları**: Standart poligon, çizgi, dikdörtgen, daire çizimi
   - **🔵 Daire butonu**: Özel yarıçap ile daire çiz
     - Yarıçapı metre cinsinden belirleyin
     - Renk seçin
     - Haritaya tıklayın
     - Çizilen daireyi sürükleyerek taşıyabilirsiniz
   - **🚶 İnsan butonu**: İnsan simgesi ekle
     - Boyutu ayarlayın
     - Haritaya tıklayın
     - Simgeyi sürükleyerek taşıyabilirsiniz
     - Simgeye tıklayarak boyutunu değiştirebilirsiniz
   - **📝 Yazı butonu**: Çok satırlı text etiketi ekle
     - Yazınızı girin (Enter ile yeni satır ekleyebilirsiniz)
     - Font, boyut ve renk seçin
     - Haritaya tıklayın
     - Yazıyı sürükleyerek taşıyabilirsiniz
     - Yazıya tıklayarak metni değiştirebilirsiniz
4. **Katman Panelini** kullanın (sağ taraftaki 📋 butonu):
   - Tüm katmanları görüntüleyin
   - Katmanların görünürlüğünü açıp kapatın
   - Katman renklerini değiştirin
   - Tek tek silin
5. Çizimlerinizi istediğiniz formatta indirin:
   - **GeoJSON İndir**: Standart GeoJSON formatında
   - **KML İndir**: Google Earth uyumlu KML formatında
   - **WKT İndir**: Well-Known Text formatında
   - **📄 PDF İndir**: Gelişmiş PDF export
     - Başlık girin
     - Logo ekleyin (opsiyonel)
     - Önizleme oluştur butonuna tıklayın
     - Önizlemeyi kontrol edin
     - PDF İndir butonuna tıklayın
6. **GeoJSON Yükle** butonu ile mevcut GeoJSON dosyalarınızı haritaya yükleyebilirsiniz
7. **Tümünü Temizle** butonu ile tüm çizimleri silebilirsiniz

## Teknolojiler

- [Leaflet.js](https://leafletjs.com/) - Harita kütüphanesi
- [Leaflet.draw](https://github.com/Leaflet/Leaflet.draw) - Çizim araçları
- [OpenStreetMap](https://www.openstreetmap.org/) - Harita verileri
- [Esri ArcGIS](https://www.arcgis.com/) - Uydu ve sokak harita katmanları
- [CartoDB](https://carto.com/) - Özelleştirilmiş harita stilleri
- [jsPDF](https://github.com/parallax/jsPDF) - PDF oluşturma
- [html2canvas](https://html2canvas.hertzen.com/) - Harita görüntüsü yakalama

## Öne Çıkan Özellikler

### 🎯 Sürüklenebilir Öğeler
- Tüm daireler mouse ile sürüklenebilir
- İnsan simgeleri sürüklenebilir
- Text etiketleri sürüklenebilir

### 🎨 Özelleştirilebilir Araçlar
- Daire yarıçapını ve rengini seçebilirsiniz
- İnsan simgesi boyutunu ayarlayabilirsiniz
- Text için font, boyut ve renk seçenekleri
- **Çok satırlı text** desteği (Enter ile satır atlama)

### 📋 Katman Yönetimi
- **Katman Paneli**: Sağ taraftaki panel ile tüm katmanları yönetin
- **Görünürlük Kontrolü**: Her katmanı ayrı ayrı göster/gizle
- **Renk Değiştirme**: Katman renklerini dinamik olarak değiştirin
- **Tek Tek Silme**: İstenmeyen katmanları panelden silin

### 📊 Otomatik Hesaplamalar
- Poligonlar için alan hesaplama (hektar)
- Daireler için yarıçap ve alan bilgisi
- Çizgiler için uzunluk hesaplama (km)

### 📤 Gelişmiş PDF Export
- **Önizleme**: PDF'i indirmeden önce görün
- **Özel Başlık**: Kendi başlığınızı yazın
- **Logo Ekleme**: Kurumsal logonuzu ekleyin
- **A4 Format**: Standart A4 landscape boyutunda
- **Otomatik Tarih**: Export tarihi otomatik eklenir

### 📥 Çoklu Export Formatları
- **GeoJSON**: Web uygulamaları için
- **KML**: Google Earth için
- **WKT**: GIS yazılımları için
- **PDF**: Profesyonel baskı ve sunum için

## Koordinatlar

Uygulama Balıkesir merkez koordinatlarına (39.6484° K, 27.8826° D) odaklanmıştır.

## Mevcut Dosyalar

Depo içerisinde örnek GeoJSON dosyaları bulunmaktadır:
- `planlar.geojson`
- `weekly.geojson`
- `07052025.geojson`
- `fgfdg345refd6_65.geojson`

Bu dosyaları "GeoJSON Yükle" butonu ile haritaya yükleyebilirsiniz.
