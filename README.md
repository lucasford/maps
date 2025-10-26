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
  - 📝 **Text Etiketi**: Harita üzerine yazı ekleme
    - Font seçimi (Arial, Times New Roman, Courier, vb.)
    - Boyut ayarlama (12-72px)
    - Renk seçimi
    - Sürüklenebilir
    - Tıklayarak metin değiştirebilme
- **Düzenleme**: Çizilen şekilleri düzenleme ve silme
- **Export Formatları**:
  - GeoJSON (.geojson)
  - KML (.kml) - Google Earth uyumlu
  - WKT (.wkt) - Well-Known Text
  - 📄 **PDF** - Haritanın yüksek kaliteli PDF çıktısı (A4 landscape)
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
   - **📝 Yazı butonu**: Text etiketi ekle
     - Yazınızı girin
     - Font, boyut ve renk seçin
     - Haritaya tıklayın
     - Yazıyı sürükleyerek taşıyabilirsiniz
     - Yazıya tıklayarak metni değiştirebilirsiniz
4. Çizimlerinizi istediğiniz formatta indirin:
   - **GeoJSON İndir**: Standart GeoJSON formatında
   - **KML İndir**: Google Earth uyumlu KML formatında
   - **WKT İndir**: Well-Known Text formatında
   - **📄 PDF İndir**: Haritanın tam görüntüsünü PDF olarak kaydedin
5. **GeoJSON Yükle** butonu ile mevcut GeoJSON dosyalarınızı haritaya yükleyebilirsiniz
6. **Tümünü Temizle** butonu ile tüm çizimleri silebilirsiniz

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

### 📊 Otomatik Hesaplamalar
- Poligonlar için alan hesaplama (hektar)
- Daireler için yarıçap ve alan bilgisi
- Çizgiler için uzunluk hesaplama (km)

### 📤 Çoklu Export Formatları
- **GeoJSON**: Web uygulamaları için
- **KML**: Google Earth için
- **WKT**: GIS yazılımları için
- **PDF**: Baskı ve sunum için

## Koordinatlar

Uygulama Balıkesir merkez koordinatlarına (39.6484° K, 27.8826° D) odaklanmıştır.

## Mevcut Dosyalar

Depo içerisinde örnek GeoJSON dosyaları bulunmaktadır:
- `planlar.geojson`
- `weekly.geojson`
- `07052025.geojson`
- `fgfdg345refd6_65.geojson`

Bu dosyaları "GeoJSON Yükle" butonu ile haritaya yükleyebilirsiniz.
