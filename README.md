# İller ve İlçeler (Provinces and Districts of Turkey)

Bu Flutter projesi, Türkiye'nin illerini ve ilçelerini listeleyen basit bir uygulama sağlar. Kullanıcılar, illeri genişleterek o ile bağlı ilçeleri görebilirler.

## Özellikler

* İller alfabetik sırayla listelenir.
* Her ilin yanında plaka kodu gösterilir.
* İllere tıklandığında, o ile bağlı ilçeler açılır liste şeklinde gösterilir.
* İl isimleri mavi renkte vurgulanır.

## Kullanılan Teknolojiler

* Flutter
* Dart
* `dart:convert` (JSON verilerini ayrıştırmak için)
* `flutter/services.dart` (asset dosyalarına erişmek için)

## Veri Kaynağı

Proje, `assets/iller_ilceler.json` dosyasından iller ve ilçeler hakkındaki verileri alır. Bu dosyanın formatı şu şekildedir:

```json
{
  "01": {
    "name": "Adana",
    "districts": {
      "01_01": {
        "name": "Aladağ"
      },
      "01_02": {
        "name": "Ceyhan"
      },
      "01_03": {
        "name": "Çukurova"
      },
