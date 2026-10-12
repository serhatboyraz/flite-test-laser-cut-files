# Flite Test Lazer Kesim Dosyaları

[English](README.md) · **Türkçe**

[Flite Test](https://www.flitetest.com/) köpük levha RC uçaklarından üçü için lazer kesim dosyaları: **FT Corsair**, **FT Explorer** ve **FT P-51 Mustang**. Her model klasöründe orijinal Flite Test yapım planı (PDF) ve lazere gönderilmek üzere hazırlanmış kesim dosyaları vardır.

Köpük parçalar **1000 × 700 mm** fotoblok levhalara göre yerleştirilmiştir. Ahşap parçalar ayrıdır; bu levhalardan kesilmez.

Bunlar yeni uçak tasarımları değildir. Uçaklar, teknik veriler ve plan PDF’leri Flite Test’e aittir. CDR ve DXF dosyaları, parçaların lazerde kesilebilmesi için yerleşim hâline getirilmiştir.

## Modeller

### FT Corsair

Dört kanallı warbird (gaz, aileron, elevator, rudder), sürüm 1.0 (9 Mart 2019).

| | |
| --- | --- |
| Tasarım | John Overstreet, Flite Test ile birlikte |
| Çizim | Dan Sponholz |
| Uzunluk | 30,75 inç (781 mm) |
| Kanat açıklığı | 46,00 inç (1168 mm) |
| Kanat alanı | 355,5 inç² (22,9 dm²) |
| Kanal | 4 |

Plandaki önerilen kurulum: 2218B 1080 kv motor, 10×4,7 pervane, en az 35 A ESC, dört adet 9 g servo, 2200–2800 mAh 3S veya 4S batarya. Ağırlık merkezi, planda işaretlendiği gibi hücum kenarından 2,00 inç (50,8 mm) geridedir.

### FT Explorer

3 kanallı trainer kanat veya 4 kanallı sport kanat olarak kurulabilen eğitim uçağı.

| | |
| --- | --- |
| Tasarım | Josh Bixler |
| Çizim | Dan Sponholz |
| Uzunluk | 36,5 inç (927 mm) |
| Kanat açıklığı | 57 inç (1448 mm) |
| Kanat alanı | 460 inç² (29,7 dm²) |
| Kanal | 3 (trainer) veya 4 (sport) |

Plandaki önerilen kurulum: Park 370–425 motor, en az 1000 kv, 20–30 A ESC, en az 2200 mAh 3S batarya, 9 g servo (trainer için iki, sport için dört), 8×4,5 slow-fly veya 9×6 pervane. Ağırlık merkezi hücum kenarından 2,25 inç (57 mm) geridedir.

Plan, köpük levhanın yanında kontrplak da ister: 3/32 inç (2,4 mm) firewall ve 1/16 inç (1,5 mm) kontrol boynuzları. Ahşap parçalar `wood.cdr` ve `wood.dxf` dosyalarındadır.

### FT P-51 Mustang

Flite Test Master Series warbird, dört kanallı (gaz, aileron, elevator, rudder), sürüm 1.0 (26 Mayıs 2020).

| | |
| --- | --- |
| Tasarım | John Overstreet |
| Çizim | Dan Sponholz |
| Uzunluk | 41,0 inç (1042 mm) |
| Kanat açıklığı | 48,25 inç (1225 mm) |
| Kanat alanı | 400 inç² (26 dm²) |
| Kanal | 4 |

Plandaki önerilen kurulum: 2218B 1080 kv motor, 10×4,7 pervane, en az 35 A ESC, dört adet 9 g servo, 2250–3000 mAh 4S batarya. Ağırlık merkezi hücum kenarından 3,0 inç (76 mm) geridedir. Plan 12° atış ve %30 expo yazar.

Plandaki ahşap plaka 3/32 inç (2,4 mm) kontrplaktır. Bu parçalar `woods.cdr` ve `woods.dxf` dosyalarındadır.

## Klasör yapısı

```
flite/
├── ft-corsair/
│   ├── ft-corsair-1.cdr      Lazer parçaları, 1. plaka (CorelDRAW)
│   ├── ft-corsair-2.cdr      Lazer parçaları, 2. plaka (CorelDRAW)
│   ├── wood.cdr              Ahşap parçalar (CorelDRAW)
│   └── ft-corsair.pdf        Flite Test tümleşik plan
├── ft-explorer/
│   ├── 3ch-explorer-parts-1.cdr / .dxf   3 kanal parçalar, 1. plaka
│   ├── 3ch-explorer-parts-2.cdr / .dxf   3 kanal parçalar, 2. plaka
│   ├── 4ch-explorer-parts-1.cdr / .dxf   4 kanal parçalar, 1. plaka
│   ├── 4ch-explorer-parts-2.cdr / .dxf   4 kanal parçalar, 2. plaka
│   ├── wood.cdr / wood.dxf               Ahşap parçalar
│   └── ft-explorer.pdf                   Flite Test tam boy plan
└── ft-p51/
    ├── p51-parts-1.cdr                   Lazer parçaları, 1. plaka (CorelDRAW)
    ├── p51-parts-2.cdr                   Lazer parçaları, 2. plaka (CorelDRAW)
    ├── p51-parts-3.cdr                   Lazer parçaları, 3. plaka (CorelDRAW)
    ├── p51-parts-4.cdr                   Lazer parçaları, 4. plaka (CorelDRAW)
    ├── woods.cdr / woods.dxf             Ahşap parçalar
    └── P51.pdf                           Flite Test tam boy plan
```

Explorer için **bir** varyant seçin. `3ch` aileronsuz trainer’dır. `4ch` aileronlu sport kanattır. Her varyant iki plakaya bölünmüştür.

## Dosya biçimleri

| Uzantı | Kullanım |
| --- | --- |
| `.dxf` | Lazere giden dosya. LightBurn, RDWorks, LaserGRBL, Inkscape ve çoğu kesim programında açılır. AutoCAD DXF R2018. |
| `.cdr` | CorelDRAW kaynağı. Corsair köpük plakaları ve P-51 köpük plakaları yalnızca CDR’dir; kesim programı CDR açmıyorsa CorelDRAW’dan DXF verin. P-51 ahşap parçalarının DXF’i hazırdır (`woods.dxf`). |
| `.pdf` | Orijinal Flite Test planı. Uçağı bununla kurun: parça adları, kat yerleri, iz açma, pah ve elektronik. |

Kesmeden önce çizimin **1:1** olduğunu kontrol edin. Ölçekli içe aktarma gövdeye uymaz.

Explorer DXF dosyaları tek katman geometridir. Plandaki PDF; kesim, iz, kat ve pah çizgilerini ayırır. Her çizgiyi kesmeyin. Köpük levhadaki iz ve kat çizgileri iz olarak kalmalıdır.

## Yapım notları

- Köpük parçalar **1000 × 700 mm** fotoblok levhalara göre yerleştirilmiştir. Plaka yerleşimini ve parça adlarını PDF’den izleyin.
- Ahşap parçalar (kiriş, firewall, kontrol boynuzu) `wood` dosyalarındadır (P-51 klasöründe `woods`). Kalınlığı planda yazan ölçüyle eşleştirin.
- Elektronik, atış açıları ve expo plan sayfalarındadır. Bu değerler başlangıç ayarıdır; her güç sistemi için garanti değildir.
- Yapım videoları ve güncel planlar [flitetest.com](https://www.flitetest.com/) adresindedir.

## Atıf ve kullanım

FT Corsair, FT Explorer ve FT P-51 Mustang tasarımları ile bu depodaki plan PDF’leri **Flite Test, LLC**’ye aittir.

Corsair planında şu uyarı vardır:

> © 2019 FliteTest, LLC. Plans provided free of charge. Copies allowed for personal use only. Not for commercial use.

P-51 planında şu uyarı vardır:

> © 2020 FliteTest, LLC. Plans provided free of charge. Copies allowed for personal use only. Not for commercial use.

Bu dosyaları kendi yapımınız için kullanın. Planları, kesim dosyalarını veya bunlardan üretilmiş kitleri satmayın.

- FT Corsair: John Overstreet ve Flite Test tasarımı, Dan Sponholz çizimi, sürüm 1.0 (2019).
- FT Explorer: Josh Bixler tasarımı, Dan Sponholz çizimi.
- FT P-51 Mustang: John Overstreet tasarımı, Dan Sponholz çizimi, sürüm 1.0 (2020).
