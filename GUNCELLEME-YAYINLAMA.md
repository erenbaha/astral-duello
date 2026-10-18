# GitHub üzerinden oyun güncellemesi yayımlama

Depo: https://github.com/erenbaha/astral-duello

Uygulamanın her açılışta kontrol ettiği sabit adres:

```text
https://github.com/erenbaha/astral-duello/releases/latest/download/latest.json
```

## Yeni sürüm

1. Yeni HTML'yi üret; numara önceki güncel sürümden yüksek olsun. v0.8.18'den sonraki sürüm v0.8.19'dur. Eski numaralı dosyaları değiştirme.
2. Aşağıdaki komutla HTML'yi imzala. `--url` mutlaka o sürüme ait doğrudan indirme adresi olmalı; `latest` adresini oyun dosyasının imzasında kullanma.

```text
node sign-update.cjs --html ../Astral-Duello-v0.8.19.html --version 0.8.19 --key C:/ozel/update-signing-private.pem --out ./yayin --url https://github.com/erenbaha/astral-duello/releases/download/v0.8.19/Astral-Duello-v0.8.19.html
```

3. GitHub'da `v0.8.19` etiketli bir taslak sürüm oluştur. İmzalanan HTML, `latest.json`, kaynak ZIP ve SHA-256 listesini ekle. Masaüstü kabuğu değişmişse yeni uygulama ve kurulum ZIP'lerini de ekle.
4. Dosyalar tamamen yüklendikten sonra sürümü yayımla ve en güncel sürüm olarak işaretle. Yeni sürümü ancak dosya ve imza kontrolleri geçtikten sonra yayımla.
5. Sabit `latest.json` adresinin yeni sürümü döndürdüğünü ve `url` alanındaki HTML'nin SHA-256/boyut değerlerini kontrol et. Eski sürümlerin dosyalarını silme.

## Anahtar ve kapsam

Özel anahtar yalnız bu bilgisayardaki `work/desktop-secrets/update-signing-private.pem` dosyasında tutulur. GitHub'a, yayın ZIP'ine, kaynak ZIP'ine veya uygulamaya eklenmez. Güvenli bir kişisel yedeği gerekir. Uygulamada yalnız `config/update-public.pem` bulunur.

İçerik güncelleyicisi kartları, görselleri, oyun kurallarını ve oyun arayüzünü yeniler. Electron veya yerel uygulama kabuğu değişikliklerinde yeni uygulama/kurulum paketi gerekir. Geçersiz imza, yanlış SHA-256, boyut uyuşmazlığı veya ağ hatasında mevcut oyun kullanılmaya devam eder.

v0.8.17 uygulamasını kullananlar bu adresi Ayarlar ekranına bir kez kaydedebilir veya GitHub adresi hazır gelen v0.8.18 uygulamasını kullanabilir. Önceki sürümde kaydedilmiş boş adres, v0.8.18'de ilk açılışta GitHub varsayılanına geçirilir; yeni sürümde adresi bilerek boş kaydetmek otomatik kontrolü kapatır.

## Geçmiş sürümler

v0.1–v0.8.17 dosyaları `v0.8.17` arşiv yayını altında, özgün dosya adlarıyla korunur. Gelecek sürümler kendi etiketleriyle yayımlanır.

## v0.8.22 ve sonraki yayınlar

İkinci herkese açık bildirim: https://raw.githubusercontent.com/erenbaha/astral-duello/main/latest.json . Release tamamen yayımlandıktan sonra deponun kökündeki latest.json dosyasını aynı imzalı içerikle güncelle. Böylece iki bildirim aynı sürümü gösterir; URL alanı sürüme özgü HTML dosyasına gider. Her iki bildirimi ve oyun indirmesini GitHub oturumu/erişim anahtarı olmadan kontrol et. İmza veya dosya bütünlüğü hatasında doğrulamayı atlama. Kök bildirimi, hedef dosyalar yayımlanmadan ileri sürüme taşıma.

Yerel uygulama v0.8.22 Chromium/Windows ağ ayarlarını kullanır, geçici hatalarda bir kez yeniden dener ve ana bildirim erişilemiyorsa yedek bildirime geçer. Hata ayrıntısı ayarlarda ve kullanıcı veri klasöründeki update-status.json içinde bulunur. Açılışta mevcut oyunla devam düğmesi vardır; indirilen yeni oyun, süren düelloyu yeniden yüklemez.

