# Balıkesir Harita Uygulaması

Balıkesir bölgesini gösteren interaktif bir web harita uygulaması. Bu uygulama ile harita üzerinde poligonlar ve çizgiler çizebilir, bunları çeşitli formatlarda dışa aktarabilirsiniz.

## Özellikler

- **İnteraktif Harita**: OpenStreetMap tabanlı, Balıkesir merkezli harita
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
2. Harita sağ üstteki çizim araçlarını kullanarak şekiller çizin
3. Çizimlerinizi istediğiniz formatta indirin:
   - **GeoJSON İndir**: Standart GeoJSON formatında
   - **KML İndir**: Google Earth uyumlu KML formatında
   - **WKT İndir**: Well-Known Text formatında
4. **GeoJSON Yükle** butonu ile mevcut GeoJSON dosyalarınızı haritaya yükleyebilirsiniz
5. **Tümünü Temizle** butonu ile tüm çizimleri silebilirsiniz

## Teknolojiler

- [Leaflet.js](https://leafletjs.com/) - Harita kütüphanesi
- [Leaflet.draw](https://github.com/Leaflet/Leaflet.draw) - Çizim araçları
- [OpenStreetMap](https://www.openstreetmap.org/) - Harita verileri

## Koordinatlar

Uygulama Balıkesir merkez koordinatlarına (39.6484° K, 27.8826° D) odaklanmıştır.

## Mevcut Dosyalar

Depo içerisinde örnek GeoJSON dosyaları bulunmaktadır:
- `planlar.geojson`
- `weekly.geojson`
- `07052025.geojson`
- `fgfdg345refd6_65.geojson`

Bu dosyaları "GeoJSON Yükle" butonu ile haritaya yükleyebilirsiniz.
