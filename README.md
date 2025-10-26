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
  - Daire çizimi
  - İşaretçi ekleme
- **Düzenleme**: Çizilen şekilleri düzenleme ve silme
- **Export Formatları**:
  - GeoJSON (.geojson)
  - KML (.kml)
  - WKT (.wkt)
- **Import**: Mevcut GeoJSON dosyalarını yükleme ve görüntüleme

## Kullanım

1. `index.html` dosyasını bir web tarayıcısında açın
2. Sağ üst köşedeki katman seçiciden istediğiniz altlık haritayı seçin
3. Harita sağ üstteki çizim araçlarını kullanarak şekiller çizin
4. Çizimlerinizi istediğiniz formatta indirin:
   - **GeoJSON İndir**: Standart GeoJSON formatında
   - **KML İndir**: Google Earth uyumlu KML formatında
   - **WKT İndir**: Well-Known Text formatında
5. **GeoJSON Yükle** butonu ile mevcut GeoJSON dosyalarınızı haritaya yükleyebilirsiniz
6. **Tümünü Temizle** butonu ile tüm çizimleri silebilirsiniz

## Teknolojiler

- [Leaflet.js](https://leafletjs.com/) - Harita kütüphanesi
- [Leaflet.draw](https://github.com/Leaflet/Leaflet.draw) - Çizim araçları
- [OpenStreetMap](https://www.openstreetmap.org/) - Harita verileri
- [Esri ArcGIS](https://www.arcgis.com/) - Uydu ve sokak harita katmanları
- [CartoDB](https://carto.com/) - Özelleştirilmiş harita stilleri

## Koordinatlar

Uygulama Balıkesir merkez koordinatlarına (39.6484° K, 27.8826° D) odaklanmıştır.

## Mevcut Dosyalar

Depo içerisinde örnek GeoJSON dosyaları bulunmaktadır:
- `planlar.geojson`
- `weekly.geojson`
- `07052025.geojson`
- `fgfdg345refd6_65.geojson`

Bu dosyaları "GeoJSON Yükle" butonu ile haritaya yükleyebilirsiniz.
