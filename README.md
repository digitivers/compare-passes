# /compare-passes – prototip

Istanbul Tourist Pass karşılaştırma sayfasının iç inceleme prototipi. `noindex` ve `robots.txt` ile arama motorlarına kapalı.

## Yayınlama (GitHub Pages)

1. Yeni bir repo açın ve bu klasördeki dosyaları köke yükleyin (`index.html`, `robots.txt`, `.nojekyll`, `README.md`).
2. Settings → Pages → Source: `main` / `root`.
3. Link: `https://<kullanıcı-veya-org>.github.io/<repo>/`
   Karar modunda açmak için sonuna `#approved` ekleyin.

## Sayfadaki prototip kontrolleri (üstteki koyu bar)

- **Today:** yalnızca bugün doğru olan satırlar. Rakibin önde olduğu 11 konu gizli.
- **If decisions are approved:** karar raporundaki 11 karar uygulanırsa tablo (turuncu "Decision N" etiketli satırlar).
- **Review notes:** sarı notlar; yayından önce doğrulanacak noktalar.

## Yayından önce

- Koyu prototip barını ve tüm `.note` öğelerini kaldırın.
- `<meta name="robots" content="noindex, nofollow">` satırını silin, `<link rel="canonical" href="https://istanbultouristpass.com/compare-passes">` ekleyin. `robots.txt` yalnızca bu prototip repo içindir.
- Hukuk onayı: karşılaştırmalı reklam (Ticari Reklam ve Haksız Ticari Uygulamalar Yönetmeliği) ve rakibi çağrıştıran renkler. Rakip sayfalarının tarihli ekran görüntülerini arşivleyin.
- Doğrulanacak veriler: turların kendi rehberlerimizle yapıldığı, güncel Trustpilot puanı, %1 iade oranının tanımı, 2–7 günlük çocuk fiyatları.
- "Decision" satırları ancak ilgili karar uygulandıktan sonra açılmalı.
- JSON-LD: WebPage, BreadcrumbList, TravelAgency, Product (AggregateOffer €149–299), FAQPage. Üçüncü taraf puanlarından `aggregateRating` eklenmedi.

Kaynaklar sayfanın "Sources and how we compared" bölümünde. Her iddianın birebir metin kanıtı ayrı bir iç dosyada tutuluyor (repo dışında).
