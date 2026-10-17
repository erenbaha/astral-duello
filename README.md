# Astral Düello

Windows için kart düellosu oyunu. Yapay zekâya karşı çevrimdışı veya oda kodu/rastgele eşleşmeyle çevrimiçi oynanabilir.

## Güncel oyun sürümü · v0.8.21

**Kullanıcı adı/şifre ile giriş ve üyelik eklendi.** Koleksiyon, altın/gümüş, derece, karakter seviyeleri, 32 deste yuvası, devam eden tek oyunculu düello ve maç geçmişi kişisel çevrimiçi hesaba kaydedilir.

Eski kaydın bulunduğu cihazda **Üye ol** ekranını açıp aktarım kutusunu seçili bırak. Her oyuncu kendi cihazında bu işlemi uygular. Başka bilgisayarda aynı hesaba giriş yapınca kayıt açılır. Üyelikte gösterilen kurtarma anahtarını sakla; şifreni unuttuğunda gereklidir. Çevrimiçi düello için giriş yapmak gerekir; misafir olarak tek oyunculu oynanabilir.

[Hesap servisi](https://astral-duello-hesap.fuzzyloon33.chatgpt.site) kalıcı veritabanında her oyuncunun kaydını ayrı tutar. İki cihazın ilerlemesi farklıysa kullanılacak kayıt seçilir. Derece para ödülleri, karakter seviyeleri ve koleksiyonda 5/destede 3 kopya sınırı korunur. Tekil kart sınırı 1; fazla T kopyası 30 altın verir.

Mevcut v0.8.18 Windows uygulamasını yeniden açarak v0.8.21 oyun içeriğini otomatik alabilirsin. Aşağıdaki Windows paketleri aynı güncellemeyi ilk açılışta alır.

- [Kurulum ZIP dosyası](https://github.com/erenbaha/astral-duello/releases/download/v0.8.18/Astral-Duello-Kurulum-v0.8.18.zip)
- [Kurulumsuz uygulama ZIP dosyası](https://github.com/erenbaha/astral-duello/releases/download/v0.8.18/Astral-Duello-Uygulama-v0.8.18.zip)
- [Tek dosyalık HTML oyunu](https://github.com/erenbaha/astral-duello/releases/download/v0.8.21/Astral-Duello-v0.8.21.html)
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
