# Astral Düello

Windows için kart düellosu oyunu. Yapay zekâya karşı çevrimdışı veya oda kodu/rastgele eşleşmeyle çevrimiçi oynanabilir.

## Güncel oyun sürümü · v0.8.20

Çevrimiçi galibiyet +25 RP ve 5 altın kazandırır. 7 rütbe arasındaki 12 basamak yalnız gümüş ve altın verir; derece kart ödülleri kaldırıldı.

8 karakterin bağımsız seviyesi ve XP’si vardır. Yapay zekâ ve çevrimiçi galibiyet +100, yenilgi +50 XP verir. Her yeni seviyede karakterin kendi destesinden 1 kart, her 10. seviyede ana kartı kazanılır. Karakter panelinden veya **Derece → Karakter seviyeleri** yolundan gelişim ve sıradaki kartlar incelenebilir.

Koleksiyonda aynı karttan 5, destede 3 kopya bulunabilir. Tekil (T) sınırı 1’dir. Fazla kopya başına dönüşüm: **N 2 gümüş · R 5 gümüş · RR 10 gümüş · SR 1 altın · UR 2 altın · T 30 altın**. Eski kartlar, cüzdan, derece ve 32 deste yuvası korunur. Derece ve karakter gelişimi bu cihazdaki oyun kaydında tutulur.

Mevcut v0.8.18 Windows uygulamasını yeniden açarak v0.8.20 oyun içeriğini otomatik alabilirsin. Aşağıdaki Windows paketleri aynı güncellemeyi ilk açılışta alır.

- [Kurulum ZIP dosyası](https://github.com/erenbaha/astral-duello/releases/download/v0.8.18/Astral-Duello-Kurulum-v0.8.18.zip)
- [Kurulumsuz uygulama ZIP dosyası](https://github.com/erenbaha/astral-duello/releases/download/v0.8.18/Astral-Duello-Uygulama-v0.8.18.zip)
- [Tek dosyalık HTML oyunu](https://github.com/erenbaha/astral-duello/releases/download/v0.8.20/Astral-Duello-v0.8.20.html)
- [Tüm sürümler ve güncelleme notları](https://github.com/erenbaha/astral-duello/releases)
- [v0.1–v0.8.17 arşivi](https://github.com/erenbaha/astral-duello/releases/tag/v0.8.17)

Kurulumsuz sürümün ZIP dosyasını tamamen çıkarıp `Astral-Duello/Astral-Duello.exe` dosyasını aç. Kurulum sürümünde ZIP içindeki kurulum EXE dosyasını çalıştır. Windows 10/11 64 bit içindir.

## Otomatik oyun güncellemeleri

v0.8.18 uygulaması her açılışta şu adresi kontrol eder:

```text
https://github.com/erenbaha/astral-duello/releases/latest/download/latest.json
```

Daha yeni bir oyun sürümü varsa boyutu, SHA-256 özeti ve Ed25519 imzası doğrulanarak indirilir. İnternet veya güncelleme hatasında mevcut oyunla devam edilir. Oyun kayıtları korunur. v0.8.17 uygulamasında aynı adres Ayarlar ekranına bir kez girilebilir.

Bu sistem kartları, görselleri, oyun kurallarını ve oyun arayüzünü günceller. Electron ve yerel uygulama kabuğu değişiklikleri için yeni uygulama/kurulum paketi gerekir. EXE dosyaları ticari Authenticode sertifikasıyla imzalanmamıştır; oyun içeriğinin imzası ayrıdır.

## Sürüm arşivi

Önceki 26 sürümün HTML ve kaynak ZIP dosyaları, v0.8.17 uygulama/kurulum/yayın paketleriyle birlikte arşiv yayınında tutulur. Numaralı dosyalar değiştirilmeyerek korunur. Gelecek sürümler kendi etiketleri altında bu depoya eklenir.

## Çevrimiçi bağlantı

Eşleşme ve oda kodu için iki oyuncunun uyumlu oyun sürümü kullanması gerekir. Bazı NAT/güvenlik duvarı koşullarında ek bir TURN hizmeti gerekebilir.

## Kaynak ve yayınlama

Oyun ve masaüstü kaynak ZIP dosyaları sürüm eklerinde bulunur. Yayınlama yöntemi [GUNCELLEME-YAYINLAMA.md](GUNCELLEME-YAYINLAMA.md) dosyasındadır. Özel imzalama anahtarı bu depoya eklenmez.
