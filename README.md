<div align="center">

# 🏨 InnJoy — Akıllı Otel Deneyimi

**Misafirlerinize unutulmaz bir konaklama deneyimi sunun.**

QR ile kapı açma, oda servisi, spa randevusu, etkinlik takibi ve çok daha fazlası — hepsi tek bir uygulamada.

[![Flutter](https://img.shields.io/badge/Flutter-3.10+-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Firestore](https://img.shields.io/badge/Cloud_Firestore-039BE5?style=for-the-badge&logo=firebase&logoColor=white)](https://firebase.google.com/products/firestore)


[🌐 Web Sitesi](https://berat-kaan-akcan.github.io/InnJoy_Website/) · [📲 APK İndir](https://berat-kaan-akcan.github.io/InnJoy_Website/InnJoy.apk) · [💬 Geri Bildirim](https://forms.gle/2sfGnK5VJ4hYPome7)

</div>

---

## 📖 Hakkında

**InnJoy**, oteller için geliştirilmiş kapsamlı bir mobil uygulama platformudur. Misafirlerin tüm otel hizmetlerine tek bir uygulama üzerinden erişmesini sağlarken, otel yöneticilerine güçlü bir admin paneli sunar.

Flutter ile geliştirilmiş olup tek bir kod tabanıyla **iOS** ve **Android** platformlarında çalışır.

---

## ✨ Özellikler

### 🧳 Misafir Tarafı

| Özellik | Açıklama |
|---------|----------|
| 🔑 **Hızlı Giriş** | PNR veya rezervasyon koduyla anında check-in |
| 🏨 **Otel Seçimi** | Listeden otel seçimi veya QR kod ile tanıma |
| 📊 **Akıllı Dashboard** | Otel duyuruları ve harcamalar tek ekranda |
| 🍽️ **Oda Servisi** | Zengin menüden seçim yaparak odaya sipariş |
| 🛀 **Spa & Wellness** | Spa randevusu alma ve takibi |
| 🍴 **Restoran Rezervasyonu** | Restoran menü görüntüleme ve rezervasyon |
| 🎉 **Etkinlik Takvimi** | Otel etkinliklerini görme ve hatırlatıcı ekleme |
| 🧹 **Housekeeping** | Havlu, temizlik, mini bar talepleri tek tıkla |
| 🚨 **Acil SOS** | Acil durumlarda anında otel görevlisiyle iletişim |
| 📅 **Planlarım** | Tüm rezervasyonlar ve etkinlikler tek ekranda |
| 👤 **Misafir Profili** | Tercih yönetimi ve konaklama geçmişi |
| 💰 **Harcama Takibi** | Tüm otel harcamalarını anlık izleme |
| 🗺️ **Harita & Yönlendirme** | OpenStreetMap ile konum ve acil çıkış yönlendirmesi |

### 🛠️ Admin Paneli

| Özellik | Açıklama |
|---------|----------|
| 📈 **Genel İzleme** | Doluluk oranları, giriş-çıkışlar ve günlük raporlar |
| 🚪 **Oda Yönetimi** | Oda listeleme, misafir atama ve durum takibi |
| 📂 **Kategori Yönetimi** | Menü, etkinlik, spa ve oda servisi düzenleme |
| 🚨 **Acil Durum Merkezi** | SOS alarmlarını anlık yönetme ve müdahale |
| 📋 **Talep Yönetimi** | Misafir taleplerini ve siparişlerini anlık takip |
| 🍽️ **Restoran Yönetimi** | Menü, rezervasyon ve ayarları tek panelden yönetme |

---

## 🛠️ Teknoloji Altyapısı

| Teknoloji | Kullanım Amacı |
|-----------|----------------|
| **Flutter** | iOS ve Android için tek kod tabanıyla cross-platform geliştirme |
| **Firebase Auth** | Kullanıcı kimlik doğrulama (E-posta, Google, Facebook) |
| **Cloud Firestore** | NoSQL veritabanı ile güvenli ve ölçeklenebilir veri yönetimi |
| **Firebase Storage** | Medya dosyaları ve görsellerin bulut depolaması |
| **flutter_map** | OpenStreetMap tabanlı harita entegrasyonu |
| **Google Fonts** | Modern tipografi desteği |
| **QR Flutter** | QR kod oluşturma ve kapı açma sistemi |
| **Geolocator** | Konum tabanlı hizmetler |
| **RxDart** | Reaktif programlama ve veri akış yönetimi |

---

## 📁 Proje Yapısı

```
InnJoy/
├── lib/
│   ├── main.dart                    # Uygulama giriş noktası
│   ├── firebase_options.dart        # Firebase yapılandırması
│   ├── models/                      # Veri modelleri
│   │   ├── user_model.dart
│   │   ├── menu_item_model.dart
│   │   ├── reservation_model.dart
│   │   └── location_model.dart
│   ├── screens/
│   │   ├── admin/                   # Admin paneli ve yönetim ekranları
│   │   │   ├── edit/                # Hizmet düzenleme
│   │   │   ├── restaurant/          # Restoran yönetimi
│   │   │   └── room_service/        # Oda servisi yönetimi
│   │   ├── auth/                    # Giriş, kayıt ve şifre sıfırlama
│   │   ├── customer/                # Müşteri ekranları
│   │   ├── dining/                  # Restoran ve menü ekranları
│   │   ├── emergency/               # Acil durum ekranları
│   │   ├── events_activities/       # Etkinlik yönetimi
│   │   ├── home/                    # Ana sayfa ve otel seçimi
│   │   ├── housekeeping/            # Kat hizmetleri
│   │   ├── legal/                   # Yasal bilgiler
│   │   ├── map/                     # Harita ekranı
│   │   ├── payment/                 # Harcama takibi
│   │   ├── profile/                 # Profil yönetimi
│   │   ├── requests/                # Talep ekranları
│   │   ├── room_service/            # Oda servisi
│   │   └── services/                # Hizmet ekranları
│   ├── services/                    # Firebase ve API servisleri
│   │   └── database/                # Veritabanı servisleri
│   ├── utils/                       # Yardımcı araçlar
│   │   ├── config/                  # Yapılandırma dosyaları
│   │   └── dialogs/                 # Dialog'lar
│   └── widgets/                     # Tekrar kullanılabilir bileşenler
│       ├── admin/                   # Admin widget'ları
│       └── common/                  # Ortak widget'lar
├── assets/
│   ├── images/                      # Uygulama görselleri
│   ├── avatars/                     # Kullanıcı avatarları
│   └── sounds/                      # Bildirim sesleri
├── android/                         # Android platform dosyaları
├── ios/                             # iOS platform dosyaları
└── pubspec.yaml                     # Bağımlılık yönetimi
```

---

## 🚀 Kurulum

### Gereksinimler

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (3.10+)
- [Dart SDK](https://dart.dev/get-dart) (Flutter ile birlikte gelir)
- Android Studio veya VS Code
- Firebase hesabı

### Adımlar

1. **Depoyu klonlayın:**
   ```bash
   git clone https://github.com/dogukandireksiz/InnJoy.git
   cd InnJoy
   ```

2. **Bağımlılıkları yükleyin:**
   ```bash
   flutter pub get
   ```

3. **Firebase yapılandırmasını ayarlayın:**
   - Firebase Console'dan yeni bir proje oluşturun
   - Android ve iOS uygulamalarını ekleyin
   - `firebase_options.dart` dosyasını projenize göre güncelleyin

4. **Uygulamayı çalıştırın:**
   ```bash
   flutter run
   ```

### 📱 APK ile Hızlı Test

Firebase kurulumu yapmadan uygulamayı denemek isterseniz:

1. [InnJoy.apk](https://berat-kaan-akcan.github.io/InnJoy_Website/InnJoy.apk) dosyasını indirin (57 MB)
2. Android cihazınızda **Ayarlar → Güvenlik → Bilinmeyen Uygulamalar → İzin Ver**
3. APK dosyasını açın ve yükleyin
4. Test hesabı ile giriş yaparak tüm özellikleri keşfedin

---

## 🔑 Test Hesabı

Uygulamayı tüm özellikleriyle deneyimlemek için demo hesabını kullanabilirsiniz:

| | |
|---|---|
| **📧 E-posta** | `appinnjoy@gmail.com` |
| **🔒 Şifre** | `123456` |

> ⚠️ **Uyarı:** Bu bir test hesabıdır. Gerçek kişisel bilgilerinizi paylaşmayın.

**✨ Deneyebileceğiniz özellikler:**
- 🔑 QR ile kapı açma ve dijital anahtar
- 🍽️ Oda servisi siparişi ve takibi
- 🛀 Spa randevusu alma
- 🍴 Restoran rezervasyonu ve menü
- 🎉 Etkinlik ve aktivite takibi
- 🚨 Acil durum ve çıkış yönlendirme
- 💰 Harcama takip ekranı
- 📊 Profil yönetimi ve bildirimler
- 📶 Wi-Fi bağlantı bilgileri
- 📅 Planlarım (rezervasyon & etkinlik takvimi)

---

## 👥 Ekip

<div align="center">

| | İsim | Rol | LinkedIn |
|:-:|------|------|----------|
| 👨‍💻 | **Berat Kaan Akcan** | Geliştirici | [Profil](https://www.linkedin.com/in/berat-kaan-akcan-224781285/) |
</div>

---

## 📬 İletişim

<div align="center">

[![Email](https://img.shields.io/badge/Email-innjoyapp@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:innjoyapp@gmail.com)
[![Instagram](https://img.shields.io/badge/Instagram-@innjoy__app-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/innjoy_app)
[![Website](https://img.shields.io/badge/Web_Sitesi-InnJoy-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white)](https://berat-kaan-akcan.github.io/InnJoy_Website/)
[![Feedback](https://img.shields.io/badge/Geri_Bildirim-Google_Form-34A853?style=for-the-badge&logo=google&logoColor=white)](https://forms.gle/2sfGnK5VJ4hYPome7)

</div>

---

<div align="center">

**⭐ Projeyi beğendiyseniz yıldız vermeyi unutmayın!**

© 2026 InnJoy — Akıllı Otel Deneyimi

</div>
