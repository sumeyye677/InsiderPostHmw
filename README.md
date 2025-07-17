# Modern Blog Sayfası – JSONPlaceholder ile Dinamik İçerik

## Web Live Link: https://mypostloading.netlify.app/

Bu proje, web programlamaya giriş seviyesinde olanlar için hazırlanmış bir blog arayüzü örneğidir. Sahte veri sağlayan bir API olan [JSONPlaceholder](https://jsonplaceholder.typicode.com/) üzerinden içerik çekilerek, modern tasarımlı, dinamik ve kullanıcı etkileşimli bir web sayfası oluşturulmuştur.

## Projenin Amacı

Bu çalışmanın amacı, bir web sayfasının dış veri kaynaklarından nasıl veri çekebileceğini, bu verileri nasıl dinamik şekilde gösterebileceğini ve kullanıcı deneyimini artırmak için neler yapılabileceğini öğrenmektir. Özellikle:

- AJAX çağrıları nasıl yapılır?
- Sayfa kaydırıldıkça içerik nasıl yüklenir? (infinite scroll)
- Kullanıcıya yükleme süreci ve hatalar nasıl gösterilir?
- Filtreleme, arama, modal pencere gibi özellikler nasıl eklenir?

## Kullanılan Teknolojiler

- **HTML5** – Sayfa yapısı için  
- **CSS3** – Görsel tasarım ve duyarlı (responsive) yapı için  
- **JavaScript & jQuery** – Etkileşim ve veri çekme işlemleri için  
- **JSONPlaceholder API** – Sahte veri kaynağı (post başlıkları, içerikler)

## Nasıl Çalışır?

1. Sayfa açıldığında, ilk 5 post verisi JSONPlaceholder API’den çekilir ve gösterilir.
2. Kullanıcı sayfanın sonuna doğru geldikçe yeni post’lar otomatik olarak yüklenir.
3. İsteğe bağlı olarak kullanıcı “Daha Fazla Yükle” butonuna da basabilir.
4. Her post için rastgele like ve yorum sayıları oluşturulur.
5. Arama kutusu ve filtreleme butonları ile içerikler daraltılabilir.
6. Post detayları, modal pencerede daha ayrıntılı görüntülenebilir.
7. Beğeni butonları ile interaktif kullanıcı deneyimi sağlanır.
8. Her AJAX çağrısı sırasında yükleme animasyonu görünür.
9. Eğer veri alınamazsa, kullanıcıya hata mesajı gösterilir.

## API Kullanımı

API üzerinden veri çekmek için aşağıdaki gibi bir istek yapılır:

```
https://jsonplaceholder.typicode.com/posts?_start=0&_limit=5
```

Burada:
- `_start` parametresi: Kaçıncı post’tan başlanacağını belirtir.
- `_limit` parametresi: Kaç adet post çekileceğini belirtir.

Her yeni yüklemede bu parametreler güncellenir.

## Özellik Listesi

- ✅ İlk 5 post otomatik olarak yüklenir  
- 🔄 Sonsuz kaydırma ile yeni içerik yüklenir  
- ⏳ Yükleme animasyonu  
- ❌ API hatası durumunda kullanıcıya uyarı  
- 🔍 Arama kutusu ile başlık ve içerikte arama  
- 🧲 Filtreler: Son Yazılar, Popüler  
- ❤️ Beğeni sistemi (kalp butonu)  
- 📊 Dinamik istatistik alanı: Toplam post, beğeni, yorum  
- 💬 Detayları modal pencerede gösterme  
- 🔝 Yukarı çıkma butonu (scroll top)

## Nasıl Çalıştırılır?

Projenin çalışması için sadece `index2.html` dosyasını herhangi bir modern tarayıcıda açmanız yeterlidir. Ek bir kurulum veya sunucu gerektirmez.

## Bonus Özellikler

Bu ödevin ana gereksinimlerinin dışında aşağıdaki isteğe bağlı (opsiyonel) detaylar da projeye eklenmiştir:

- **Yükleniyor Spinnerı**: İçerik alınırken kullanıcıya bekleme animasyonu gösterilir.
- **Hata Mesajı**: API isteği başarısız olursa kullanıcıya anlamlı bir hata bildirimi yapılır.
- **Beğeni Sayacı**: Kullanıcılar bir post’u beğendiğinde kalp ikonu değişir ve sayı artar.
- **Modal Pencere**: Post’un üzerine tıklanarak detaylı hali pop-up şeklinde gösterilir.
- **Mobil Duyarlılık**: Sayfa farklı ekran boyutlarına uygun olacak şekilde responsive tasarlandı.

## Ekran Görüntüsü (Opsiyonel)

<img width="1553" height="897" alt="aaaaaa" src="https://github.com/user-attachments/assets/b742964b-e400-439d-b4d9-ac5c92334824" />

