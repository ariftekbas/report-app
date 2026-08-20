<div align="center">

# 🏙️ Şehir İçi Şikayet ve Talep Yönetim Sistemi

### Vatandaş ↔ Belediye ↔ Saha Personeli arasında uçtan uca entegre akıllı şehir çözümü

**Backend & Web Admin Panel** · Laravel 10 REST API + Web Yönetim Paneli

<p>
  <img src="https://img.shields.io/badge/PHP-%5E8.1-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
  <img src="https://img.shields.io/badge/Laravel-10-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel" />
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Sanctum-Auth-EF3B2D?style=for-the-badge&logo=laravel&logoColor=white" alt="Sanctum" />
</p>
<p>
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" alt="MIT License" />
  <img src="https://img.shields.io/badge/Mobil-Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter" />
  <img src="https://img.shields.io/badge/RBAC-Spatie%20Permission-6C3483?style=for-the-badge" alt="Spatie Permission" />
</p>

[Özellikler](#-temel-özellikler) · [Ekran Görüntüleri](#-ekran-görüntüleri) · [Teknolojiler](#️-kullanılan-teknolojiler) · [Kurulum](#-backend-kurulumu) · [Reporlar](#-organizasyon-repoları)

</div>
<br>

## 🔗 Organizasyon Repoları

| Repo | Açıklama |
|---|---|
| 📱 [`sikayet_uygulamasi`](https://github.com/sikayet-app/sikayet_uygulamasi) | Mobil Uygulama (Flutter) |
| 🖥️ [`report-app-backend`](https://github.com/sikayet-app/report-app-backend) | Backend & Web Admin (Laravel) |

<br>

---

Vatandaşların şehir içi altyapı, çevre ve temizlik gibi sorunlarını yerel yönetimlere hızlıca iletebildiği; yetkililerin ise bu talepleri tek bir merkezden yönetip sahadaki personellere atayabildiği **uçtan uca entegre bir akıllı şehir çözümüdür.**

> Bu repo, projenin **Laravel tabanlı REST API ve Web Yönetim Paneli** bileşenini içerir. Mobil uygulama [ayrı bir repoda](https://github.com/sikayet-app/sikayet_uygulamasi) geliştirilmektedir.

<br>

## 📸 Ekran Görüntüleri

### 📱 Mobil Uygulama

<p align="center">
  <img src="https://github.com/user-attachments/assets/704e4bdf-b1df-427a-bddb-12cc64804a7c" width="270" alt="Ana Sayfa Harita" />
  <img src="https://github.com/user-attachments/assets/f98a3d75-fb77-474a-8e22-9f5067158946" width="270" alt="Şikayet Oluşturma" />
  <img src="https://github.com/user-attachments/assets/1076d0d1-87a8-4097-9cf7-3f9a3bfdd6e5" width="270" alt="Şikayet Detay" />
</p>

**Rol Bazlı Şikayet Yönetimi ve İstatistikler**

<p align="center">
  <img src="https://github.com/user-attachments/assets/42e292f7-8bd3-4636-8426-fa63da61d206" width="380" alt="Vatandaş Görünümü" />
  <img src="https://github.com/user-attachments/assets/019edf1a-9fd6-4c9d-9951-0d230c388c54" width="380" alt="Yönetici Görünümü" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/caa1293a-faee-43ef-b7dd-65984f6c6c04" width="380" alt="Yönetim" />
  <img src="https://github.com/user-attachments/assets/fe48860c-8eb6-4af1-86a4-71311f24a353" width="380" alt="Profil" />
</p>

### 🖥️ Web Yönetim Paneli (Admin Dashboard)

**İstatistikler**

<p align="center">
  <img src="https://github.com/user-attachments/assets/4ff9cf8b-17a5-4cb8-9021-3bb0d909c9a0" width="90%" />
</p>

**Şikayetler ve Detayları**

<p align="center">
  <img src="https://github.com/user-attachments/assets/7c93f37e-1278-4599-917a-ca076393ade7" width="48%" />
  <img src="https://github.com/user-attachments/assets/a4d8901c-57fe-498a-bed4-52f342ae9321" width="48%" />
</p>

**Şikayet Güncelleme ve Personel Atama**

<p align="center">
  <img src="https://github.com/user-attachments/assets/3ad612b5-f28c-4e74-ba33-0a33f10ddab4" width="48%" />
  <img src="https://github.com/user-attachments/assets/a6e3358d-200a-446f-8bff-4328185b312c" width="48%" />
</p>

**Kullanıcı ve Yetki Yönetimi**

<p align="center">
  <img src="https://github.com/user-attachments/assets/ad4657e5-0c15-4e6d-9ecb-dab5aa557951" width="48%" />
  <img src="https://github.com/user-attachments/assets/5a042393-dbc2-4c4c-9ba7-3b6c98dcbb02" width="48%" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/f0ad6d9f-7f74-4d91-a982-8fb44e511878" width="48%" />
  <img src="https://github.com/user-attachments/assets/0a825051-0de1-4ad2-902b-4ab54e5160ea" width="48%" />
</p>

<br>

## ✨ Temel Özellikler

Sistem, **4 farklı kullanıcı rolü** (`Vatandaş`, `Personel`, `Sorumlu`, `Sistem Yöneticisi`) üzerinden yetkilendirilmiş dinamik bir mimariye sahiptir.

### 🖥️ Web Yönetim Paneli (Admin & Managing)

Yetkililerin şehre dair tüm verileri kuşbakışı incelediği ve operasyonu yönettiği merkezdir.

| Özellik | Açıklama |
|---|---|
| 📊 **Merkezi Dashboard** | Şehir genelindeki şikayetlerin kategorilere ve aylara göre dağılımını gösteren detaylı istatistik paneli |
| 🧑‍🔧 **Görev Atama** | Bekleyen şikayetleri sahadaki uygun personellere atama ve süreç takibi |
| ✅ **Durum ve Çözüm Yönetimi** | Şikayetlerin durumlarını güncelleme ve vatandaşa gösterilecek "Çözüm Notları" ekleme |
| 🔐 **Kullanıcı ve Rol Yönetimi** | Vatandaş, personel ve yöneticilerin hesap/yetki kontrolleri (rol ve izin bazlı, granüler yetkilendirme) |

### 📱 Mobil Uygulama

Sahada veri girişini ve takibini kolaylaştırmak için tasarlanmıştır.

| Özellik | Açıklama |
|---|---|
| 📍 **Akıllı Konum Entegrasyonu** | İnteraktif harita üzerinden nokta atışı konum seçimi ve otomatik adres (ilçe/mahalle) tespiti |
| 📷 **Görsel Kanıt Yükleme** | Kamera veya galeri üzerinden çoklu fotoğraf yükleme (maksimum 3 adet) |
| 🔔 **Anlık Durum Takibi** | İletilen taleplerin durumlarını anlık olarak izleyebilme |
| 🛠️ **Mobil Yönetim Paneli** | Yöneticilerin bilgisayara ihtiyaç duymadan mobilden şikayetleri listeleyip durum güncelleyebildiği ve saha ataması yapabildiği özel arayüz |
| 📈 **Kişisel Dashboard** | Role göre özelleştirilmiş istatistik ekranı (Vatandaş için toplam talep, Personel için atanan işler) |
| 🌗 **Tema Desteği** | Karanlık (Dark) ve Aydınlık (Light) mod desteği |

<br>

## ⚙️ Kullanılan Teknolojiler

<table>
<tr>
<td valign="top" width="50%">

**Backend & Web**

| Katman | Teknoloji |
|---|---|
| Framework | Laravel 10 (PHP ^8.1) |
| Kimlik Doğrulama | Laravel Sanctum (API token) |
| Rol & Yetki Yönetimi | Spatie Laravel-Permission (RBAC) |
| Veritabanı | MySQL |
| Dosya Yönetimi | Laravel Filesystem (local / cloud disk) |
| HTTP Client | Guzzle |

</td>
<td valign="top" width="50%">

**Mobil Mimari**

| Katman | Teknoloji |
|---|---|
| Framework | Flutter |
| State Management | Riverpod |
| Ağ İstekleri & API | Dio (Interceptors & Token Management) |
| Harita ve Konum | flutter_map, geocoding, latlong2 |
| Form & Validasyon | mask_text_input_formatter |

</td>
</tr>
</table>

<br>

## 🚀 Backend Kurulumu

> **Gereksinimler:** PHP ^8.1, Composer, MySQL, Node.js (asset build için opsiyonel)

```bash
# 1. Repoyu klonlayın
git clone https://github.com/sikayet-app/report-app-backend.git
cd report-app-backend

# 2. Bağımlılıkları yükleyin
composer install

# 3. Ortam dosyasını oluşturun ve uygulama anahtarını üretin
cp .env.example .env
php artisan key:generate

# 4. .env dosyasında veritabanı bilgilerinizi düzenleyin

# 5. Veritabanı tablolarını oluşturun ve örnek verileri yükleyin
php artisan migrate --seed

# 6. Yüklenen görsellerin (şikayet fotoğrafları vb.) erişilebilir olması için
php artisan storage:link

# 7. Geliştirme sunucusunu başlatın
php artisan serve
```

Uygulama varsayılan olarak `http://127.0.0.1:8000` adresinde çalışır. API uç noktaları ve mobil uygulama bu adres üzerinden Sanctum token'ları ile kimlik doğrulaması yaparak haberleşir.


## 📄 Lisans

Bu proje [MIT lisansı](https://opensource.org/licenses/MIT) ile lisanslanmıştır.

<div align="center">

---

GBB Bilişim ile daha yaşanabilir şehirler

</div>
