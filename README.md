# Satış Ligi

Eski satış ligi sayfasının yeni tasarımı. Firebase ayarları ve veri yapısı aynıdır, mevcut veriler olduğu gibi çalışır.

## Yayınlama

`badlucc7/larasatis` reposunda şu dosyaları değiştir/yükle:

- `index.html` (eskisinin yerine)
- `fonts/` ve `vendor/` klasörleri (repoda şu an yok; eksikse site bozuk açılır)
- `vince-mcmahon.gif` ve `here-comes-the-money.mp3` zaten repoda, aynı kalır

## Kullanım

- Kilit simgesi: PIN (4505) ile yönetimi açar. Açıkken satır başlarında + / − butonları ve dişli (yönetim paneli) görünür. Kilitliyken TV ekranı sade kalır. Eskiden PIN girmiş cihazlar açık kalır.
- Klavyede `A`: yönetim paneli.
- Hoparlör simgesi: tarayıcılar ses için bir kez dokunma ister; TV'de bir kez dokunursan sonraki kutlamalarda ses çalar.
- Tam ekran simgesi TV için.

## Eventler (yeni)

Eventlerdeki satışlar ayrı takip edilir ama **toplam ciroya dahildir**.

- Satış eklerken (+ butonu) üstte **Normal satış / Event satışı** seçilir. Event satışında hangi event olduğu seçilir ya da "Yeni event oluştur" ile adı yazılır (örn. "Londra · Kasım"). Aynı ad tekrar yazılırsa mevcut event kullanılır.
- **Ortak satış**: kutuyu işaretleyip ortağı seç, tutar iki kişiye eşit bölünür, her biri 0,5 satış sayılır. Eventte ve normalde kullanılabilir.
- Sıralamada **Toplam / Normal / Event** görünümleri var. Event görünümünde üstte event adı çipleri çıkar, tek bir event ya da "Tüm eventler" seçilir. Seçim bütün ekranlara yansır (TV dahil).
- Üst kartta ciro **Normal + Event** olarak ayrı gösterilir; hedef çubuğu iki renklidir. Toplam görünümünde her satırın çubuğunda event payı çizgili renkle görünür.
- Yönetim panelinde **Eventler** bölümü: event ekle, satış/ciro özetini gör, sil (satışları da silinir).
- Üstteki döngü simgesi **otomatik geçiş**: bu cihazda Toplam, Event, Normal görünümlerini 14 saniyede bir sırayla gösterir (TV için).
- Ay kapatılınca arşive eventler ve event cirosu da yazılır; CSV'de Normal / Event ciro sütunları vardır.
- Eski veriler olduğu gibi çalışır: event etiketi olmayan her satış "Normal" sayılır.

Event satışında ek kutlama: "EVENT SATIŞI" bandı, dönen ışık huzmeleri, kurdele ve yıldız yağmuru; ortak satışta iki temsilcinin avatarı birleşir. Her satışta tutar satırdan yukarı süzülür, sıra değişince ▲/▼ rozeti çıkar, yeni lider olunca taç düşer.

## Tasarım

Açık ve renkli tema. Üstte ciro kartı (3B altın kupa, etrafında dönen renkli toplar, hedef £1.000.000) ve 3B podyum, altında tüm temsilcilerin listesi (7+ kişide iki sütun). Her temsilcinin kendi rengi var. Arka planda renkli 3B şekiller süzülüyor, satış gelince hızlanıyor ve altın paralar yağıyor.

Cihaz zayıfsa arka plan kendini kapatır; "hareketi azalt" ayarı açık cihazlarda animasyonlar durur. Tek kutlama £1.000.000 hedefi aşılınca yapılır (eskiden 250K ve 500K de vardı).
