# Öğrenci Bilgi Sistemi (OBS) Uygulaması

Bu proje, Mobil Programlama dersi kapsamında İstanbul Medeniyet Üniversitesi adına **Flutter** kullanılarak geliştirilen temel bir **Öğrenci Bilgi Sistemi (OBS)** mobil uygulamasıdır. Uygulama, üniversite öğrencileri için ders bilgilerini, haftalık ders programlarını, yapılacak görevlerini ve mezuniyet bilgilerini kolayca görüntüleyebilmelerini sağlar. Aynı zamanda giriş yapan kullanıcıya özel kişiselleştirilmiş bir deneyim sunar.

## Özellikler

- **Kullanıcı Girişi:**  
  Kullanıcı adı ve şifre ile giriş yapılır, JSON dosyasından doğrulama gerçekleştirilir.
  
- **Profil Yönetimi:**  
  Giriş yapan kullanıcının ad-soyad ve e-posta bilgileri otomatik olarak görüntülenir.
  
- **Yapılacaklar Listesi:**  
  Kullanıcı, anasayfada yapılacak görevlerini ekleyebilir, silebilir ve düzenleyebilir. Veriler, uygulama yeniden başlatıldığında da saklanır.
  
- **Ders Bilgileri:**  
  Öğrencinin aldığı dersler ve derslerin öğretim üyeleri listelenir.
  
- **Haftalık Ders Programı:**  
  Haftalık ders programı günlere göre görüntülenebilir.
  
- **Mezuniyet Bilgileri:**  
  Tamamlanan kredi, kalan kredi ve dönem bilgileri görüntülenir.
  
- **Çıkış Yapma:**  
  Kullanıcı, menüden çıkış yaparak uygulamayı sonlandırabilir.

## Ekran Görüntüleri
  |
| **Giriş Ekranı**                     | **Anasayfa**                       |
|--------------------------------------|-----------------------------------|
|  ![giriş](https://github.com/user-attachments/assets/2cca1697-24e9-45ed-8e2c-9fdb7453658f)
  | ![anasayfa](https://github.com/user-attachments/assets/f93571da-7218-468c-af8b-fc7a82f47e8f)
   |

| **Menü Çubuğu**                   | **Profil Sayfası**                 |
|--------------------------------------|-----------------------------------|
| ![menü_çubuğu](https://github.com/user-attachments/assets/214810e7-8810-4fe8-b0a6-cf6072470025)      | ![profil](https://github.com/user-attachments/assets/1a43f769-0d81-4f35-b0ab-a17fc4bcec41)    | 
## Teknolojiler

- **Flutter:**  
  Uygulamanın geliştirilmesi için kullanıldı.
- **Dart:**  
  Uygulama kodlama dili olarak kullanıldı.
- **JSON:**  
  Kullanıcı verilerinin saklanması ve doğrulaması için kullanıldı.
- **Shared Preferences:**  
  Kullanıcı görevlerinin kalıcı olarak saklanması sağlandı.

## Kurulum

1. **Proje deposunu klonlayın:**

   ```bash
   git clone https://github.com/fatmazeyrek/OBS_app.git

2. **Gerekli bağımlılıkları yükleyin:**
   ```bash
   flutter pub get

3. **Projeyi çalıştırın:**
   ```bash
   flutter run
**Klasör Yapısı:**
   ```bash
OBS_app/
├── lib/
│   ├── home_screen.dart          # Anasayfa kodları
│   ├── login_screen.dart         # Giriş ekranı kodları
│   ├── profile_screen.dart       # Profil ekranı kodları
│   ├── courses_screen.dart       # Ders bilgileri ekranı kodları
│   ├── schedule_screen.dart      # Ders programı ekranı kodları
│   ├── custom_drawer.dart        # Menü çubuğu kodları
│   └── globals.dart              # Global değişkenler
├── assets/
│   ├── users.json                # Kullanıcı verileri
│   ├── imu_logo.png              # Uygulama logosu
│   └── 200x200.png               # Giriş ekranı görseli
└── pubspec.yaml                  # Bağımlılık dosyası
