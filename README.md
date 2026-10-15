# Suflör POS Güncellemeleri

Bu depo Suflör POS masaüstü uygulamasının derlenmiş Windows x64 güncelleme paketlerini barındırır. Kaynak kod, işletme veritabanı ve kişisel veriler bu depoda tutulmaz.

## İndirme

[Son sürüm ve kurulum paketi](https://github.com/TheEnginUnal/SuflorPos-Updates/releases/latest)

Kurulum için `SuflorPOS-VERSIYON-win-x64.zip` dosyasını kullanın. GitHub'ın otomatik oluşturduğu Source code dosyaları uygulama kurulum paketi değildir. Paket self-contained yayımlanır; ayrıca .NET kurulmaz. Windows x64 gerekir. Mevcut WebView2 gereksinimi devam eder.

## İlk geçiş

1. Mevcut veri yedeğini koruyun ve uygulamaları kapatın.
2. İlk kez 1.3.0'a geçerken tam paketi mevcut uygulama klasörüne çıkarın. `Updater` klasörü dahil tüm dosyaları taşıyın; işletme verilerini değiştirmeyin.
3. Önce ana bilgisayarı, ardından mutfak/bar cihazlarını açın. Ayrıntılar paketteki `Uygulama-Guncelleme-Kurulumu.md` dosyasındadır.

## Sonraki güncellemeler

Ana bilgisayarda yönetici oturumuyla **Ayarlar → Güncellemeler** üzerinden kontrol, indirme ve onaylı kurulum yapılır. Kurulum açık adisyonlar kapatıldıktan sonra servis dışında uygulanır. Mutfak/bar cihazları **Güncelleme** düğmesinden paketi ana bilgisayardan alır; bu cihazların internet erişimi gerekmez.

Güncellemeler kendiliğinden kurulmaz. Uygulama, yayıncı imzasını ve dosya bütünlüğünü doğrular. `update.json` sürüm bilgisi, `update.sig` yayıncı imzasıdır. İşletme veritabanı paketlere dahil değildir.
