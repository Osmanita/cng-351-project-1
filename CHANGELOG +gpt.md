# CNG 351 Assignment 1 - +gpt değişiklik günlüğü

**Durum:** Son kullanıcı onayına göre K1 ve R1-R5 uygulandı. O1 ve O3 uygulanmadı. O2 değiştirilmedi. Rapor 16 sayfa; sekiz diyagram 1684 × 1191 pt ve vektör.

## Dosyalar ve kaynak koruması

- Çıktılar CNG351_Assignment1_Chen +gpt.drawio ve CNG351_Assignment1_Report +gpt.pdf adlarıyla güncellendi.
- Orijinal, +claude ve copy 2 dosyaları değiştirilmedi. Altı korunan kaynağın SHA-256 değerleri işlem öncesi/sonrası karşılaştırıldı.
- Önceki teknik +gpt sürümü çalışma klasöründe ayrı bir before kopyası olarak korundu.
- CHECKS_BEFORE +gpt.json ve SVG_CHECKS_BEFORE +gpt.json ilk +claude devralmasının tarihçesidir; güncel ölçü ve sonuçlar CHECKS_AFTER +gpt.json içindedir. İlk istekteki 2245 × 1587 değeri son kullanıcı talimatıyla 1684 × 1191 pt olarak düzeltildi.

## Sayfa bazında uygulanan İngilizce metin değişiklikleri

### R3 - Sayfa 4 - UC1 assumptions 4

Dosya: CNG351_Assignment1_Report +gpt.pdf

**Eski metin:**

The mandatory first question is checked when participation is completed. Temporary pre-answer workflow states are outside the stored completed-play model.

**Yeni metin:**

Every recorded contestant has been asked at least one question, so Contestant participates totally in HasAttempt.

### R5 - Sayfa 8 - UC2 rules 1

Dosya: CNG351_Assignment1_Report +gpt.pdf

**Eski metin:**

Machine.Type is standard or industrial. Dormitory.Level is undergraduate or graduate. Student.Username is unique in addition to StudentID. CampusZone and Student.Age are stored attributes.

**Yeni metin:**

Machine.Type is standard or industrial. Dormitory.Level is undergraduate or graduate. Student.Username is unique in addition to StudentID. Student.Age is a stored attribute because no birth date is given.

### R4 - Sayfa 8 - UC2 rules 2

Dosya: CNG351_Assignment1_Report +gpt.pdf

**Eski metin:**

Each machine has exactly one current model and one current laundry room. MinLoad must not exceed MaxLoad; the model records its supported program names.

**Yeni metin:**

Each machine is based on exactly one model and is located in exactly one laundry room. MinLoad must not exceed MaxLoad; the model records its supported program names.

### R4 - Sayfa 8 - UC2 rules 3

Dosya: CNG351_Assignment1_Report +gpt.pdf

**Eski metin:**

Each Machine-Dormitory pair has at most one current allocation, with its own UsageRank and FreeCreditAmount. IsLeadingDorm is true exactly when UsageRank = 1 for that machine.

**Yeni metin:**

Each Machine-Dormitory pair has at most one allocation, with its own UsageRank and FreeCreditAmount. IsLeadingDorm is true exactly when UsageRank = 1 for that machine.

### R5 - Sayfa 9 - UC2A / text_1

Dosya: CNG351_Assignment1_Chen +gpt.drawio

**Eski metin:**

Chen ERD | Allocation attributes belong to the Machine-Dormitory pair. CampusZone is stored as supplied.

**Yeni metin:**

Chen ERD | Allocation attributes belong to the Machine-Dormitory pair.

### R1 - Sayfa 13 - UC3 assumptions 3

Dosya: CNG351_Assignment1_Report +gpt.pdf

**Eski metin:**

Bookings take place within one calendar date, with StartTime earlier than EndTime. The stated start-slot uniqueness rule is enforced; a broader interval-overlap prohibition is not inferred from it.

**Yeni metin:**

A booking starts and ends on the same date, with StartTime earlier than EndTime. The key (RoomNumber, BookingDate, StartTime) prevents two bookings for the same room from starting on the same date at the same time.

### R2 - Sayfa 13 - UC3 assumptions 4

Dosya: CNG351_Assignment1_Report +gpt.pdf

**Eski metin:**

An investor may invest in the same company more than once. InvestmentID distinguishes those dated transactions. Investor email is not assumed to be unique.

**Yeni metin:**

An investor may invest in the same company more than once. InvestmentID distinguishes those dated transactions. Investor email is not assumed to be unique. An investor may be registered before making any investment, so Investor participates partially in ProvidedBy.

### K1 - Sayfa 13 - UC3 assumptions 5

Dosya: CNG351_Assignment1_Report +gpt.pdf

**Eski metin:**

(new paragraph)

**Yeni metin:**

A company that has left KALTEV stays in the system so that its past rentals remain linked to it. The ongoing-rental rule applies only to companies currently operating in the building.

### K1 - Sayfa 13 - UC3 rules 3

Dosya: CNG351_Assignment1_Report +gpt.pdf

**Eski metin:**

Each Rental links one company to one office with its dates and MonthlyRent. Every company has at least one active rental now. Historical rentals are retained and an office may be empty. Rental intervals for the same office cannot overlap.

**Yeni metin:**

Each Rental links one company to one office and records StartDate, EndDate and MonthlyRent. A rental is ongoing when StartDate is on or before today and EndDate is NULL or later than today. Every company currently operating in KALTEV has at least one ongoing rental. Ended rentals are kept as history, and an office may have no ongoing rental. Rental periods of the same office cannot overlap.

### K1 - Sayfa 14 - UC3A / text_3

Dosya: CNG351_Assignment1_Chen +gpt.drawio

**Eski metin:**

Each company must have at least one active rental now. Rental intervals for the same office cannot overlap.

**Yeni metin:**

Every company currently operating in KALTEV has at least one ongoing rental. Rental periods of the same office cannot overlap.

## Teknik PDF değişiklikleri

| Sayfa | Görünüm | Değişiklik |
|---|---|---|
| 5 | UC1A | Güncel +gpt.drawio kaynağından yeniden native vektör export; 2245 × 1587 pt → 1684 × 1191 pt. `5 of 16` footer korundu. |
| 6 | UC1B | Güncel +gpt.drawio kaynağından yeniden native vektör export; 2245 × 1587 pt → 1684 × 1191 pt. `6 of 16` footer korundu. |
| 9 | UC2A | Güncel +gpt.drawio kaynağından yeniden native vektör export; 2245 × 1587 pt → 1684 × 1191 pt. `9 of 16` footer korundu. UC2A alt başlığı R5 ile güncellendi. |
| 10 | UC2B | Güncel +gpt.drawio kaynağından yeniden native vektör export; 2245 × 1587 pt → 1684 × 1191 pt. `10 of 16` footer korundu. |
| 11 | UC2C | Güncel +gpt.drawio kaynağından yeniden native vektör export; 2245 × 1587 pt → 1684 × 1191 pt. `11 of 16` footer korundu. |
| 14 | UC3A | Güncel +gpt.drawio kaynağından yeniden native vektör export; 2245 × 1587 pt → 1684 × 1191 pt. `14 of 16` footer korundu. UC3A kira notu K1 ile güncellendi. |
| 15 | UC3B | Güncel +gpt.drawio kaynağından yeniden native vektör export; 2245 × 1587 pt → 1684 × 1191 pt. `15 of 16` footer korundu. |
| 16 | UC3C | Güncel +gpt.drawio kaynağından yeniden native vektör export; 2245 × 1587 pt → 1684 × 1191 pt. `16 of 16` footer korundu. |

- Diyagramların oranları korundu; PNG kullanılmadı. Sekiz diyagram sayfasının her birinde 0 raster görüntü var.
- Kapak, legend ve entity identities sayfaları (1, 2, 3, 7, 12) içerik akışı, ölçü ve 2000 px render bakımından kaynakla birebir aynı.
- 4, 8 ve 13. metin sayfaları onaylanan içerikle yeniden oluşturuldu. Times-Roman 11.5 pt, 15 pt leading ve önceki paragraf/başlık aralıkları korundu; font küçültülmedi.
- Kapak aynen korundu: Team / Group ID 8; Osman Caner Cakmak 2584829; Bedri Can Guneser 2585032. İki öğrenci numarası da x=350 pt sütununda Times-Roman 12 pt.
- Kapakta footer yok; 2-16. sayfalarda sayfaya uygun `x of 16` footer tam bir kez var. Yeni footer Times-Roman 10 pt, yatay ortalı, alt taban çizgisi 24 pt.

## Korunan çizim ve model tercihleri

- Bu onay aşamasında draw.io’da yalnızca UC2A text_1 ve UC3A text_3 değerleri değişti. Hiçbir koordinat, stil, entity/attribute adı, ilişki ucu veya cardinality değeri değişmedi.
- Önceki teknik aşamadaki UC1B edge_13_0 (JokerUse → UsedAt) çıkış noktası düzeltmesi korundu: exitX=1;exitY=0.2;exitDx=0;exitDy=0. Böylece UsedAt, UsedFor çift çizgisini kesmiyor.
- Claude yerleşimleri korundu: UC3B Employee/Intern sırası; UC3A Represents sol/sağ köşe bağlantıları ve HoldsRental üst girişi; UC2C ContractAmount sağ konumu; UC3C ReceivedBy sağ bağlantısı.
- shape=link;width=8, labelBackgroundColor=none, ellipsePerimeter/rhombusPerimeter ve none arrow ayarları korundu.
- Altı partial-key alt çizgisi ve bunların koordinatları değişmedi.
- O1 uygulanmadı: Aynı sorunun aynı yarışmacıya tekrar sorulabilmesi varsayımı ve mevcut QuestionAttempt anahtarı korundu.
- O2 değişmedi: IsCorrect düz oval/saklanan değer; GivenAnswer ile Question.CorrectChoice karşılaştırmasına uyması kuralı korundu. UC1B recorded/checked notu da değişmedi.
- O3 uygulanmadı: s.2 legend içindeki Booking cümlesi ve draw.io export cümlesi korundu.
- UsageSession–UsedByDorm (0,1), LaundryRoom, Rental, Investment, Stay ve InternsAt seçimleri korundu.

## Bölüm 6 - kontrol listesinin bütün maddeleri

| Kontrol | Sonuç | Kanıt |
|---|---|---|
| Her ilişki çizgisi iki şekle de değiyor | GEÇTİ | Sekiz son vektör PDF görünümü tek tek görsel incelendi. |
| Kopukluk, çentik, ok ucu veya crow’s-foot benzeri işaret yok | GEÇTİ | Son görsel inceleme; XML’de bütün kenarların startArrow/endArrow ayarları none. |
| Her (min,max) kendi kenarında; attribute çizgisinin üstünde değil | GEÇTİ | 66 kenar etiketi, labelBackgroundColor=none; native SVG yollarında 0 etiket–başka çizgi çakışması. |
| min≥1 çift, min=0 tek çizgi | GEÇTİ | 66 uç değer/stil eşleşmesi; çift çizgiler shape=link;width=8. |
| Kesişen çizgi yok | GEÇTİ | Native SVG yollarında 0 kesişme; ortak şekil üzerindeki geçerli uç temasları hariç. Son PDF görsel olarak da incelendi. |
| Entity/attribute adları, ilişki uçları ve (min,max) anlamı korunmuş | GEÇTİ | Önceki +gpt ile doğrudan XML karşılaştırması; bu aşamada yalnızca iki onaylı not değişti. |
| Entity identities anahtarları ve kurallardaki adlar diyagramlarda mevcut | GEÇTİ | Kimlik tabloları değişmedi; EmployeeCount*, TotalInvestmentReceived, IsLeadingDorm, Duration, CompanyAge raporda mevcut; node değerleri kaynakla aynı. |
| Değişen kuralın ilgili draw.io notu güncel | GEÇTİ | K1 → UC3A text_3; R5 → UC2A text_1. Diğer aynı bilgiyi taşıyan notlar korunmuş ve uyumlu. |
| Kapak bilgileri ve ödev adı/numarası doğru | GEÇTİ | Verilen takım/üye/numara değerleri kaynaktaki kapakta aynen korundu. |
| Form alanı yok; öğrenci numaraları aynı sütun ve fontta | GEÇTİ | 0 field, 0 widget; iki numara x=350, Times-Roman 12 pt. |
| PDF 16 sayfa, sıra doğru | GEÇTİ | Diyagram sayfaları 5, 6, 9, 10, 11, 14, 15, 16. |
| Sayfa 2-16 footer x of 16; kapakta footer yok | GEÇTİ | Her sayfanın metniyle doğrulandı; footer tekil. |
| Diyagramlar 1684×1191 pt ve vektör | GEÇTİ | Sekiz mediabox değeri tam eşit; 0 raster görüntü. |
| Tek PDF, İngilizce, sade akademik biçim | GEÇTİ | Plain cover/body korundu; değişen metinlerin font ve aralıkları aynı. |
| Bütün ilişkiler binary, yalnızca Chen | GEÇTİ | 33 ilişki elması; her birine tam iki entity rolü bağlı; n-ary yok. |

### Görünüm bazında son görsel ve geometri kontrolleri

| Görünüm | Sayfa | Uçlar/işaretler | Etiketler | Participation | Kesişme |
|---|---|---|---|---|---|
| UC1A | 5 | GEÇTİ | GEÇTİ | GEÇTİ | GEÇTİ |
| UC1B | 6 | GEÇTİ | GEÇTİ | GEÇTİ | GEÇTİ |
| UC2A | 9 | GEÇTİ | GEÇTİ | GEÇTİ | GEÇTİ |
| UC2B | 10 | GEÇTİ | GEÇTİ | GEÇTİ | GEÇTİ |
| UC2C | 11 | GEÇTİ | GEÇTİ | GEÇTİ | GEÇTİ |
| UC3A | 14 | GEÇTİ | GEÇTİ | GEÇTİ | GEÇTİ |
| UC3B | 15 | GEÇTİ | GEÇTİ | GEÇTİ | GEÇTİ |
| UC3C | 16 | GEÇTİ | GEÇTİ | GEÇTİ | GEÇTİ |

## Yöntem ve kalan sınırlamalar

- Diyagramlar yerel resmî draw.io Desktop 32.5.5 motoruyla dışa aktarıldı. ReportLab yalnızca üç metin sayfası/footer için, pypdf birleştirme için kullanıldı.
- Sekiz diyagram ve üç değişen metin sayfası ayrı ayrı incelendi. Korunan beş sayfa hem temas sayfasında incelendi hem kaynakla piksel düzeyinde eşit bulundu.
- SVG etiket geometrisi Arial Bold 27 px ölçümünü kullanır; görsel PDF incelemesiyle desteklenmiştir. Ortak entity sınırındaki geçerli birleşimler kesişme sayılmaz.
- Poppler, kaynaktan korunan Symbol ve ArialUnicode kaynakları için fallback-font uyarıları verdi. Korunan sayfalar kaynakla aynı render edildi; eksik karakter görülmedi.
- 0 sayfa dışına taşan karakter ve 0 raster diyagram bulundu.
- Onaylanan K1 ve R1-R5 kapsamında yapılmamış iş veya açık içerik onayı kalmadı. O1/O3 bilinçli olarak uygulanmadı; IsCorrect tercihi bilinçli olarak korundu.
- Sonuçlar istenen dosya/notasyon kontrollerini kapsar; öğretmenin vereceği nota ilişkin bir garanti değildir.

## İnceleme paketi

ZIP, güncel +gpt PDF/draw.io dosyalarını, bu günlüğü, tam eski → yeni metin kayıtlarını, güncel içerik JSON’unu, önce/sonra kontrol JSON’larını ve SHA-256 manifestini içerir.
