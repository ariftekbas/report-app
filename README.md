# Şehir İçi Şikayet ve Talep Yönetim Sistemi

Vatandaşların şehir içi altyapı, çevre ve temizlik gibi sorunlarını yerel yönetimlere hızlıca iletebildiği; yetkililerin ise bu talepleri tek bir merkezden yönetip sahadaki personellere atayabildiği **uçtan uca entegre bir akıllı şehir çözümüdür.**

Bu organizasyon, projenin birbirine entegre çalışan iki temel bileşenini barındırmaktadır:
1. **Mobil Uygulama**
2. **Web Yönetim Paneli ve REST API**

---

## Ekran Görüntüleri

### Mobil Uygulama
<p align="center">
  <img src="https://github.com/user-attachments/assets/704e4bdf-b1df-427a-bddb-12cc64804a7c" width="270" alt="Ana Sayfa Harita" />
  <img src="https://github.com/user-attachments/assets/f98a3d75-fb77-474a-8e22-9f5067158946" width="270" alt="Şikayet Oluşturma" />
  <img src="https://github.com/user-attachments/assets/1076d0d1-87a8-4097-9cf7-3f9a3bfdd6e5" width="270" alt="Şikayet Detay" />
</p>

#### Rol Bazlı Şikayet Yönetimi ve İstatistikler
<p align="center">
  <img src="https://github.com/user-attachments/assets/42e292f7-8bd3-4636-8426-fa63da61d206" width="380" alt="Vatandaş Görünümü" />
  <img src="https://github.com/user-attachments/assets/019edf1a-9fd6-4c9d-9951-0d230c388c54" width="380" alt="Yönetici Görünümü" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/caa1293a-faee-43ef-b7dd-65984f6c6c04" width="380" alt="Yönetim" />
  <img src="https://github.com/user-attachments/assets/fe48860c-8eb6-4af1-86a4-71311f24a353" width="380" alt="Profil" />
</p>

### Web Yönetim Paneli (Admin Dashboard)
<p align="center">
  <img src="[WEB_DASHBOARD_RESIM_LINKI]" width="800" alt="Web Admin Dashboard" />
</p>
<p align="center">
  <img src="[WEB_SIKAYET_LISTESI_LINKI]" width="400" alt="Web Şikayet Listesi" />
  <img src="[WEB_DETAY_VEYA_ATAMA_LINKI]" width="400" alt="Web Görev Atama" />
</p>

---

## Temel Özellikler

Sistem, 4 farklı kullanıcı rolü (`Vatandaş`, `Personel`, `Sorumlu`, `Sistem Yöneticisi`) üzerinden yetkilendirilmiş dinamik bir mimariye sahiptir.

### Mobil Uygulama
Mobil uygulama, sahada veri girişini ve takibini kolaylaştırmak için tasarlanmıştır.
* **Akıllı Konum Entegrasyonu:** Şikayet oluştururken interaktif harita üzerinden nokta atışı konum seçimi ve otomatik adres (ilçe/mahalle) tespiti.
* **Görsel Kanıt Yükleme:** Kamera veya galeri üzerinden çoklu fotoğraf yükleme (maksimum 3 adet).
* **Anlık Durum Takibi:** İletilen taleplerin durumlarını anlık olarak izleyebilme.
* **Mobil Yönetim Paneli**: Yöneticilerin bilgisayara ihtiyaç duymadan mobilden şikayetleri listeleyebildiği, durum güncelleyebildiği ve sahada görev ataması yapabildiği özel yönetim arayüzü.
* **Kişisel Dashboard:** Kullanıcının rolüne göre (Vatandaş için toplam talep, Personel için atanan işler) özelleştirilmiş istatistik ekranı.
* **Tema Desteği:** Kullanıcı tercihine göre Karanlık (Dark) ve Aydınlık (Light) mod desteği.

### Web Yönetim Paneli (Admin & Managing)
Yetkililerin şehre dair tüm verileri kuşbakışı incelediği ve operasyonu yönettiği merkezdir.
* **Merkezi Dashboard:** Şehir genelindeki şikayetlerin kategorilere ve aylara göre dağılımını gösteren detaylı istatistik paneli.
* **Görev Atama:** Bekleyen şikayetleri sahadaki uygun personellere atama ve süreç takibi.
* **Durum ve Çözüm Yönetimi:** Şikayetlerin durumlarını güncelleme ve vatandaşa gösterilecek "Çözüm Notları" ekleme.
* **Kullanıcı ve Rol Yönetimi:** Sistemdeki vatandaş, personel ve yöneticilerin hesap/yetki kontrolleri.

---

## Kullanılan Teknolojiler

**Mobil Mimari**
* **Framework:** Flutter
* **State Management:** Riverpod
* **Ağ İstekleri & API:** Dio (Interceptors & Token Management)
* **Harita ve Konum:** flutter_map, geocoding, latlong2
* **Form & Validasyon:** mask_text_input_formatter, form validation

**Backend & Web Mimari**
* **Framework:** Laravel (RESTful API mimarisi)
* **Veritabanı:** PostgreSQL / MySQL
* **Kimlik Doğrulama:** JWT (JSON Web Tokens) ile Role-Based Access Control (RBAC)
* **Dosya Yönetimi:** Lokal Storage / Cloud Image Upload

---

## Organizasyon Repoları

Sistemin kaynak kodlarına aşağıdaki bağlantılardan ulaşabilirsiniz:

* **[Mobil Uygulama Reposu (Flutter)](https://github.com/sikayet-app/sikayet_uygulamasi)** 
* **[Backend & Web Admin Reposu (Laravel)](https://github.com/sikayet-app/report-app-backend)**

---
