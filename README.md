# Astral Düello

Windows için kart düellosu oyunu. Yapay zekâya karşı çevrimdışı veya oda kodu/rastgele eşleşmeyle çevrimiçi oynanabilir.

## Güncel oyun · v0.8.30 / Windows uygulaması · v0.8.28

Rastgele eşleşmede önce çevrimiçi oyuncu aranır. 20 saniye içinde eşleşme olmazsa veya arama bağlantısı kurulamazsa seçili karakterin seviyesine uygun rakip atanır: **1–4 Kolay, 5–9 Orta, 10+ Zor**. Rakip normal bir takma adla görünür; oyuncunun destesi korunur ve rakip farklı aileden seçilir. Oda koduyla eşleşme değişmez.

Bu maçlar **derecelidir**: galibiyet +25 RP, 150 gümüş ve 5 altın; yenilgi veya teslim −10 RP (en az 0) ve 50 gümüş verir. Karakter XP ve derece yükselme ödülleri mevcut kurallarla sürer; aynı maç ikinci kez ödül kazandırmaz. İptal veya menü değişimi aramayı kapatır, arka planda maç başlamaz. Rakip adı geçmişte de korunur.

Yapay zekâya karşı menüsünde Kolay/Orta/Zor seçimi ve teslimde ödül verilmemesi korunur. Kabus yeni kartlarla açılmak üzere kilitlidir.

586 oyun/kayıt ve 20 gerçek oyun arayüzü kontrolü geçti. **v0.8.28 Windows uygulaması bu imzalı oyun güncellemesini açılışta otomatik alır; yeniden kurulum gerekmez.** Çevrimiçi protokol astral-0825 ile uyumludur.

**Kullanıcı adı/şifre ile giriş ve üyelik eklendi.** Koleksiyon, altın/gümüş, derece, karakter seviyeleri, 32 deste yuvası, devam eden tek oyunculu düello ve maç geçmişi kişisel çevrimiçi hesaba kaydedilir.

Eski kaydın bulunduğu cihazda **Üye ol** ekranını açıp aktarım kutusunu seçili bırak. Her oyuncu kendi cihazında bu işlemi uygular. Başka bilgisayarda aynı hesaba giriş yapınca kayıt açılır. Üyelikte gösterilen kurtarma anahtarını sakla; şifreni unuttuğunda gereklidir. Çevrimiçi düello için giriş yapmak gerekir; misafir olarak tek oyunculu oynanabilir.

[Hesap servisi](https://astral-duello-hesap.fuzzyloon33.chatgpt.site) kalıcı veritabanında her oyuncunun kaydını ayrı tutar. İki cihazın ilerlemesi farklıysa kullanılacak kayıt seçilir. Derece para ödülleri, karakter seviyeleri ve koleksiyonda 5/destede 3 kopya sınırı korunur. Tekil kart sınırı 1; fazla T kopyası 30 altın verir.

**Geri tuşu ve Oyunu başlat düzeltmesini almak için v0.8.28 kurulumunu bir kez yükle veya yeni taşınabilir uygulamayı kullan.** Önce açık oyunu kapat. Oyun HTML güncellemesi eski EXE dosyasını değiştirmez. Kayıtlar aynı yerde korunur.

- [Kurulum ZIP dosyası](https://github.com/erenbaha/astral-duello/releases/download/v0.8.28/Astral-Duello-Kurulum-v0.8.28.zip)
- [Kurulumsuz uygulama ZIP dosyası](https://github.com/erenbaha/astral-duello/releases/download/v0.8.28/Astral-Duello-Uygulama-v0.8.28.zip)
- [Tek dosyalık HTML oyunu](https://github.com/erenbaha/astral-duello/releases/download/v0.8.30/Astral-Duello-v0.8.30.html)
- [Tüm sürümler ve güncelleme notları](https://github.com/erenbaha/astral-duello/releases)
- [v0.1–v0.8.17 arşivi](https://github.com/erenbaha/astral-duello/releases/tag/v0.8.17)

Kurulumsuz sürümün ZIP dosyasını tamamen çıkarıp `Astral-Duello/Astral-Duello.exe` dosyasını aç. Kurulum sürümünde ZIP içindeki kurulum EXE dosyasını çalıştır. Windows 10/11 64 bit içindir.

## Otomatik oyun güncellemeleri

v0.8.28 uygulaması her açılışta herkese açık şu adresi kontrol eder:

```text
https://github.com/erenbaha/astral-duello/releases/latest/download/latest.json
```

GitHub hesabı, giriş veya erişim anahtarı gerekmez. Windows ağ/proxy ayarları kullanılır. Geçici bağlantı hatasında bir kez yeniden denenir; ana bildirim erişilemiyorsa [herkese açık yedek bildirim](https://raw.githubusercontent.com/erenbaha/astral-duello/main/latest.json) kullanılır. Hata ayrıntısı ayarlarda gösterilir. Açılış kontrolü uzarsa **Oyunu başlat** ile mevcut sürüm açılabilir; aktif düello indirme bittiğinde yeniden yüklenmez.

Daha yeni bir oyun sürümü varsa boyutu, SHA-256 özeti ve Ed25519 imzası doğrulanarak indirilir. İnternet veya güncelleme hatasında mevcut oyunla devam edilir. Oyun kayıtları korunur. v0.8.17 uygulamasında aynı adres Ayarlar ekranına bir kez girilebilir.

Bu sistem kartları, görselleri, oyun kurallarını ve oyun arayüzünü günceller. Electron ve yerel uygulama kabuğu değişiklikleri için yeni uygulama/kurulum paketi gerekir. EXE dosyaları ticari Authenticode sertifikasıyla imzalanmamıştır; oyun içeriğinin imzası ayrıdır.

## Sürüm arşivi

Önceki 26 sürümün HTML ve kaynak ZIP dosyaları, v0.8.17 uygulama/kurulum/yayın paketleriyle birlikte arşiv yayınında tutulur. Numaralı dosyalar değiştirilmeyerek korunur. Gelecek sürümler kendi etiketleri altında bu depoya eklenir.

## Çevrimiçi bağlantı

Eşleşme ve oda kodu için iki oyuncunun uyumlu oyun sürümü kullanması gerekir. Bazı NAT/güvenlik duvarı koşullarında ek bir TURN hizmeti gerekebilir.

## Kaynak ve yayınlama

Oyun ve masaüstü kaynak ZIP dosyaları sürüm eklerinde bulunur. Yayınlama yöntemi [GUNCELLEME-YAYINLAMA.md](GUNCELLEME-YAYINLAMA.md) dosyasındadır. Özel imzalama anahtarı bu depoya eklenmez.
