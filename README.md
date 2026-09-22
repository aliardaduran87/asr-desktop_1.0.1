# 🪐 ASR — Personal Intelligence System
### Kurumsal Seviyede Yerel, Hibrit Zekâlı Kişisel Zaman ve Verimlilik Ekosistemi

> *«Asra yemin olsun ki; insan mutlaka bir hüsrandadır. Ancak iman edip salih amel işleyenler, birbirlerine hakkı ve sabrı tavsiye edenler müstesna.»*  
> — **Asr Sûresi**

---

[✨ Temel Özellikler](#-öne-çıkan-temel-yetenekler) • [🏛️ Mimari Tasarım](#️-mimari-tasarım-clean-architecture--ddd) • [🧠 Muvakkit AI & STT](#4--muvakkit-ai--sesli-komut-stt-motoru) • [🔒 Güvenlik & Kasa](#7--sıfır-sızıntılı-gizli-görev-kasası-secret-task-vault) • [⌨️ Kısayollar](#️-kısayol-tuşları-rehberi) • [🚀 Kurulum](#-başlangıç-ve-kurulum) • [📊 Kalite & Testler](#-kalite-güvencesi-ve-test-metrikleri)

---

## 🌌 Vizyon ve Felsefe

**ASR Desktop**, modern insanın en kıymetli hazinesi olan zamanı zayi etmeden, yüksek şuur, intizam ve dinginlikle yönetmesi için tasarlanmış kurumsal seviyede bir masaüstü zekâ sistemidir.

Adını köklü zaman bilincinden ve asrın sorumluluğundan alan sistem; Osmanlı saraylarında ve rasathanelerinde vakti ve gök cisimlerini milimetrik bir hassasiyetle tanzim eden **"Muvakkit"** geleneğini, 21. yüzyılın üretken yapay zekâ (LLM) teknolojileri ve modern Qt6 mimarisiyle yeniden inşa eder.

Bulut tabanlı servislerin veri gizliliği açıklarına ve dikkat dağıtıcı arayüzlerine karşı; tamamen yerel (**local-first**), fiziksel veri izolasyonlu ve donanım seviyesinde şifreli bir odaklanma mabedi sunar.

---

## ✨ Öne Çıkan Temel Yetenekler

### 1. 📅 42 Hücreli Dinamik Takvim & Ajanda Motoru
* **Gelişmiş Matris Hesaplama:** Ayın ilk gününe göre dinamik pazartesi hizalaması, önceki ve sonraki aylardan taşan günlerin görsel ayrımı.
* **Akıllı Hafta Sonu & Tatil Sistemi:** Hafta sonları ve 2026-2100 yılları arasındaki resmi ve dini tatilleri otomatik algılayan renkli vurgulama motoru.
* **Hızlı Gün Detayı:** Herhangi bir güne tıklandığında görevleri, saatlik randevuları ve günlük notları listeleyen modal diyalog.
* **Hızlı Tarih Atlama:** Ay/Yıl seçici ile istenen tarihe tek tıkla geçiş; "Bugün" butonu ile anında güncel güne dönüş.

### 2. 🎯 Görev ve Kategori İntizamı
* **Öncelik Seviyeleri:** Düşük, Orta, Yüksek ve Acil öncelik bayrakları ile renk kodlamalı ayırt edilebilirlik.
* **Bitiş Tarihi ve Alarm Uyarısı (Due Alert):** Süresi yaklaşan veya geçen görevler için görsel ve sesli ikaz pencereleri.
* **300ms Debounce Canlı Arama:** Bellek içi indeksleme sayesinde binlerce görev arasında yazıldığı anda anında filtreleme.
* **Geri Alma (Undo Engine - Ctrl+Z):** İstem dışı silinen veya tamamlanan görev/kategori eylemlerini geçmiş yığından geri getirme.

### 3. 🔁 Görev Şablonları & Saatlik Rutin Planlayıcı (Scheduler)
* **Haftalık Rutin Şablonları:** Pazartesi'den Pazar'a kadar haftanın günlerine veya "Her Gün" periyoduna özel şablon tanımlama.
* **Toplu Takvime Aktarım:** Seçilen tarih aralığına (≤365 gün) şablonları saniyeler içinde otomatik görev olarak yerleştirme.
* **Geçmiş Gün Emniyet Kilidi:** Yanlışlıkla geçmiş tarihlere görev eklenmesini önleyen kullanıcı onay koruması.
* **İdempotent Çakışma Önleme:** Aynı görevin aynı güne mükerrer basılmasını engelleyen veri bütünlüğü kuralı.

### 4. 🧠 Muvakkit AI & Sesli Komut (STT) Motoru
* **Çoklu Sağlayıcı Desteği (Hybrid LLM):** OpenAI (GPT-4o), Google Gemini 1.5/2.0, DeepSeek V3/R1, Nvidia NIM ve tamamen çevrimdışı/yerel çalışan Ollama (Llama 3, Mistral, Qwen) entegrasyonu.
* **Doğal Dil Niyet Ayrıştırma (Intent Parsing):** *"Yarın saat 14:00'te Ahmet ile toplantı yap Yüksek öncelikli"* dendiğinde başlığı, tarihi ve önceliği otomatik olarak ayrıştıran parser.
* **Sesli Görev Oluşturma (Speech-to-Text):** Qt6 Audio altyapısı ve Whisper/Deepgram sürücüleri ile mikrofondan konuşarak eller serbest görev ve not girişi.
* **Gün Sonu Değerlendirmesi & Koçluk:** Yapılan ve ertelenen işleri analiz ederek kullanıcıya kişiselleştirilmiş üretkenlik tavsiyeleri sunan asistan.

### 5. ⏳ Odaklanma Sayacı (Pomodoro) & Alışkanlık Takibi
* **25/5 & 50/10 Odaklanma Döngüleri:** Kesintisiz çalışma seansları, mola uyarıları ve seans tamamlama sayaçları.
* **Alışkanlık Zinciri Takibi (Streak Tracker):** *"Zinciri kırma"* prensibiyle günlük alışkanlıkların süreklilik yüzdeleri ve başarı rozetleri.

### 6. 📈 Çok Katmanlı Analitik & Rapor Merkezi (Trophy Road)
* **Görsel Grafikler:** Günlük Bar, Aylık Dağılım, Kategori Pasta Grafiği ve Alan Verimlilik Trendleri.
* **Dışa Aktarım Motoru:** CSV, JSON ve detaylı Markdown raporları formatında veri dışa aktarımı.
* **Kupa Yolu (Trophy Road):** Tamamlanan görev puanlarıyla seviye atlama, verimlilik rozetleri ve gamification ödülleri.

### 7. 🔒 Sıfır Sızıntılı Gizli Görev Kasası (Secret Task Vault)
* **Donanım Destekli Güvenlik:** API anahtarları Windows Credential Manager (DPAPI / Keyring) üzerinde izole edilir; asla düz metin dosyalarda saklanmaz.
* **PBKDF2-HMAC-SHA256:** Master şifre 100.000 iterasyon ve kriptografik tuz (salt) ile özetlenir.
* **Otomatik Kilit:** Boşta kalma süresi sonunda ve `Ctrl+G` kısayolu ile anında görünmez hale gelerek kendini kilitler.

### 8. 🛡️ Fiziksel Çok Kullanıcılı Mimari (Multi-Tenant Physical Isolation)
* Kullanıcı verileri tek bir büyük tabloda karışık tutulmaz.
* Her hesap için bağımsız `data/users/user_{id}.db` fiziksel SQLite veritabanı tahsis edilir.
* SQLite WAL (Write-Ahead Logging) modu ile okuma ve yazma işlemlerinde maksimum eşzamanlılık ve sıfır kilitlenme garantilenir.

---

## 🏛️ Mimari Tasarım (Clean Architecture & DDD)

ASR Desktop, kurumsal ölçekte test edilebilirlik, gevşek bağlılık (loose-coupling) ve yüksek sürdürülebilirlik sağlayan Temiz Mimari (Clean Architecture) prensipleriyle geliştirilmiştir:

```text
┌────────────────────────────────────────┐
│      Presentation Layer (PySide6)      │
│   Views, ViewModels, Dialogs, Theme    │
└───────────────────┬────────────────────┘
                    │ (Depends on)
                    ▼
┌────────────────────────────────────────┐
│      Application Layer (Use Cases)     │
│   DTOs, UseCase Interactors, Ports     │
└───────────────────┬────────────────────┘
                    │ (Depends on)
                    ▼
┌────────────────────────────────────────┐
│          Domain Layer (Core)           │
│  Entities, Value Objects, Domain Enums │
└───────────────────▲────────────────────┘
                    │ (Implements Ports)
┌───────────────────┴────────────────────┐
│      Infrastructure Layer (Adapters)   │
│   SQLAlchemy ORM, Keyring, LLM, Audio  │
└───────────────────┬────────────────────┘
                    │
                    ▼
┌────────────────────────────────────────┐
│      Composition Layer (Root DI)       │
│   Container, Service Factory, Wires    │
└────────────────────────────────────────┘
```

### Modüler Dizin Düzeni

```text
ASR-Desktop/
├── app/
│   ├── domain/               # Saf Python iş nesneleri, Entity'ler, Invariant kuralları
│   │   ├── entities/         # Task, Category, Habit, User, DailyNote, TaskTemplate
│   │   └── value_objects/    # Tarih aralıkları, renk kodları, takvim hücreleri
│   ├── application/          # Uygulama mantığı ve kullanım senaryoları
│   │   ├── dto/              # Veri aktarım nesneleri (Data Transfer Objects)
│   │   ├── ports/            # Repository arayüzleri ve servis kontratları
│   │   └── use_cases/        # 40+ saf kullanım senaryosu (Task, Category, AI, Vault...)
│   ├── infrastructure/       # Dış dünya adaptörleri ve kütüphane bağlayıcıları
│   │   ├── database/         # SQLAlchemy 2.0 ORM modelleri, WAL SQLite bağlantıları
│   │   ├── security/         # PBKDF2 Hasher, OS Keyring Vault, Password Policy
│   │   ├── ai/               # OpenAI, Gemini, DeepSeek, Ollama, Nvidia LLM sürücüleri
│   │   └── audio/            # Qt6 QAudioSource, STT adaptörleri
│   ├── presentation/         # Qt6 / PySide6 Grafik Arayüzü (MVVM)
│   │   ├── viewmodels/       # Reaktif View Modelleri (QObject sinyalleri)
│   │   ├── views/            # Sol, Orta, Sağ Panel bileşenleri ve Özel Widget'lar
│   │   ├── dialogs/          # 25+ Modal yönetim ve analitik penceresi
│   │   └── themes/           # Koyu tema (#121212), QSS stilleri, High-DPI kontrolü
│   └── composition/          # Bağımlılık Enjeksiyonu (Dependency Injection Container)
├── docs/                     # Sistem mimarisi, tasarım kılavuzu ve teknik raporlar
├── tests/                    # 228 adet Unit, Integration, UI ve Benchmark testleri
├── asr.spec                  # PyInstaller bağımsız dağıtım yapılandırması
├── inno_setup.iss            # Windows Setup Wizard (Installer) derleme betiği
├── pyrefly.toml              # Pyrefly Static Type Checker kuralları
└── pyrightconfig.json        # Pyright LSP yapılandırması
```

---

## ⌨️ Kısayol Tuşları Rehberi

| Kısayol | Kapsam | Fonksiyon |
| :--- | :--- | :--- |
| **F1** | Genel | İnteraktif Kullanım Kılavuzu & Yardım Kütüphanesini açar |
| **Ctrl + G** | Güvenlik | Gizli Görev Kasası (Secret Task Vault) kilit açma / kapama |
| **Ctrl + Z** | Global | Son yapılan Görev / Kategori silme veya tamamlama eylemini geri al (Undo) |
| **Ctrl + S** | Ajanda | Seçili günün notunu ve değişikliklerini hızlı kaydeder |
| **Ctrl + A** | Listeler | Görev veya Şablon listesindeki tüm öğeleri toplu seçer |
| **Ctrl + D** | Listeler | Seçili görev veya şablonları toplu silme onay diyalogunu çağırır |
| **Del** | Görevler | Vurgulanan görevi anında siler |
| **Space** | Görevler | Vurgulanan görevin tamamlanma durumunu değiştirir |
| **Esc** | Pencereler | Açık olan modal diyalogları ve form düzenleme modunu güvenle kapatır |

---

## 📊 Kalite Güvencesi ve Test Metrikleri

ASR Desktop, kurumsal güvenilirlik standartlarını sağlamak için kapsamlı bir otomatik test piramidiyle korunur:

| Test Kategorisi | Test Sayısı | Durum | Kapsam / Ortalama Süre |
| :--- | :---: | :---: | :--- |
| **Unit Tests** | 182 | ✅ Geçti | UseCases, Entities, Domain Invariants (~4.8 sn) |
| **Security & Vault Tests** | 14 | ✅ Geçti | PBKDF2, Keyring, SQL Injection, Parola Politikası (~1.2 sn) |
| **Database & WAL Tests** | 8 | ✅ Geçti | SQLite Multi-Tenant & Eşzamanlılık (~2.1 sn) |
| **UI & Dialog Tests** | 12 | ✅ Geçti | PySide6 QtBot Otomasyonu (~7.2 sn) |
| **10K Tasks Stress Benchmark** | 1 | ✅ Geçti | 10.000 görev altındaki anlık filtreleme (<150 ms) |
| **TOPLAM** | **228** | **%100 BAŞARILI** | **~22 saniye** |

* **Pyrefly & Pyright LSP:** 0 Type Diagnostics (Tam statik tip denetimi).
* **Ruff Linter:** 0 Hata, 0 Uyarı (PEP 8 ve Clean Code standartları).

---

## 🚀 Başlangıç ve Kurulum

### Sistem Gereksinimleri
* **İşletim Sistemi:** Windows 10 veya Windows 11 (64-bit)
* **Python Sürümü:** Python 3.13+ (Önerilen)
* **Bellek (RAM):** Minimum 4 GB (Önerilen 8 GB)
* **Ekran Çözünürlüğü:** 1366x768 ve üzeri (4K Ultra-HD PassThrough desteklenir)

### 1. Depoyu Klonlama & Sanal Ortam Kurulumu
```bash
# Depoyu klonlayın
git clone https://github.com/aliardaduran87/yakin-desktop_1.1.git
cd yakin-desktop_1.1

# Sanal ortam oluşturun ve aktif edin
python -m venv .venv
.venv\Scripts\activate

# Bağımlılıkları yükleyin
pip install -r requirements.txt
```

### 2. Uygulamayı Geliştirme Modunda Başlatma
```bash
python main.py
```

### 3. Test Paketini Çalıştırma
```bash
python run_tests.py
```

### 4. Tek Dosya (.exe) Üretimi
PyInstaller kullanarak harici Python kurulumuna ihtiyaç duymayan optimize edilmiş tek dosya yürütülebilir paket oluşturmak için:
```bash
python -m PyInstaller asr.spec
```
Üretilen binary dosyası `./dist/ASR.exe` dizininde hazır hale gelir.

### 5. Windows Kurulum Sihirbazı (Installer) Oluşturma
[Inno Setup Compiler](https://jrsoftware.org/isinfo.php) ile `inno_setup.iss` derlendiğinde:
```bash
iscc inno_setup.iss
```
Bu işlem `dist_installer/ASR_Desktop_v1.0_Setup.exe` kurulum paketini otomatik olarak üretir.

---

## 🛡️ Gizlilik ve Veri Güvenliği Taahhüdü

* **Sıfır Telemetri:** ASR Desktop, kullanıcının izni olmadan arka planda hiçbir analitik, telemetri veya kullanım verisi toplamaz.
* **Tamamen Yerel:** Görevleriniz, notlarınız, takvim kayıtlarınız ve alışkanlıklarınız yalnızca sizin bilgisayarınızdaki `data/` klasöründe fiziksel veritabanlarında tutulur.
* **Bağımsız API Kontrolü:** Yapay zekâ entegrasyonlarında kullanılan API anahtarları yalnızca kullanıcının kendi belirlediği sağlayıcılara (OpenAI, Google, DeepSeek vb.) doğrudan istek göndermek için kullanılır; hiçbir aracı sunucu bulunmaz.

---

## 📄 Lisans ve Telif Hakkı

Telif Hakkı © 2026 Ali Arda Duran / ASR Systems. Tüm Hakları Saklıdır.  
Detaylı yasal şartlar ve kullanım lisansı için lütfen `LICENSE.txt` belgesini inceleyiniz.
