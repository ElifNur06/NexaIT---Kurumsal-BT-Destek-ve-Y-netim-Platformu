# NexaIT - Kurumsal BT Destek ve Yönetim Platformu 🚀

NexaIT, kurumsal seviyede biletleme (ticketing) ve BT yönetim süreçlerini otomatize etmek için geliştirilmiş, yüksek performanslı bir **Full-Stack** çözümdür. Sistem; güçlü bir **FastAPI** backend çekirdeği, dinamik **Jinja2** web arayüzü ve modern bir **Flutter** mobil uygulamasından oluşur.

## 🛠 Teknik Mimari ve Teknoloji Yığını

### 1. Backend & API (Merkezi Çekirdek)
Sistemin beyni, yüksek hız ve asenkron operasyonlar için optimize edilmiş Python tabanlı bir yapıdır.
* **Framework:** FastAPI (Asenkron destekli yüksek performanslı API).
* **Template Engine:** Jinja2 (Dinamik sunucu taraflı rendering).
* **Validasyon:** Pydantic (Tip güvenli veri doğrulama).
* **Dokümantasyon:** Swagger UI ve Redoc (Canlı API spesifikasyonları).

### 2. Mobile (Flutter İstemcisi)
Modern bir kullanıcı deneyimi sunan, hibrit mobil uygulama katmanıdır.
* **Dil:** Dart.
* **Tasarım:** Material 3 standartlarında Deep Purple teması.
* **Mimari:** StatefulWidget mimarisi ile gerçek zamanlı UI güncellemeleri.
* **Tema Yönetimi:** `MyApp` sınıfı üzerinden merkezi global navigasyon ve görsel kimlik kontrolü.

## 📂 Öne Çıkan Özellikler

### 🌐 Web & Yönetim Paneli
* **Rol Tabanlı Erişim (RBAC):** Admin, Teknisyen ve Müşteri rolleri için özelleştirilmiş dashboardlar.
* **Dinamik Harita Entegrasyonu:** `Leaflet.js` ile yerinde (On-site) destek talepleri için konum seçimi.
* **Veri Görselleştirme:** Açık, Atanmış ve Çözülmüş bilet sayılarını gösteren canlı istatistik kartları.
* **SLA & Paket Yönetimi:** Basic, Standard, Premium ve 24/7 Corporate plan takibi.

### 📱 Mobil Uygulama Yetenekleri
* **Anlık Bilet Takibi:** Teknik destek taleplerinin mobil cihazlar üzerinden yönetimi.
* **Modern UI:** Material 3 standartlarında yüksek tepkiselliğe sahip kullanıcı arayüzü.
* **Gerçek Zamanlı Veri:** Backend API ile tam entegre, dinamik veri akışı.

## 📋 API Spesifikasyonları
Sistem, aşağıdaki uç noktalar üzerinden tam entegrasyon sağlar:
* `POST /api/login/{role}`: Yetkilendirme simülasyonu.
* `POST /api/logout`: Güvenli oturum kapatma.
* `GET /api/tickets`: Merkezi bilet listesi.
* `GET /api/ticket/{id}`: Bilet detayları ve teknik geçmiş.

## Görseller

<img width="921" height="515" alt="image" src="https://github.com/user-attachments/assets/d928f1d8-fdf0-411f-aa95-a7fc43af0c9b" />
<img width="921" height="521" alt="image" src="https://github.com/user-attachments/assets/88be2bb1-d435-4481-8730-654d5c2c5302" />
<img width="918" height="519" alt="image" src="https://github.com/user-attachments/assets/47341b47-ada6-4952-b252-080a502c49f9" />
<img width="922" height="516" alt="image" src="https://github.com/user-attachments/assets/7d249096-bcf3-4209-a51d-9432b9620529" />
<img width="921" height="516" alt="image" src="https://github.com/user-attachments/assets/6d8b0963-c48d-431e-b7e5-eafb744b0f45" />
<img width="921" height="517" alt="image" src="https://github.com/user-attachments/assets/ac6417c6-e868-487f-af7e-af0c1aa5f152" />
<img width="921" height="517" alt="image" src="https://github.com/user-attachments/assets/10c4cab2-09f6-44d3-93bb-18be3a503fe7" />
<img width="918" height="514" alt="image" src="https://github.com/user-attachments/assets/b2db0621-8655-486f-af70-d741a77a17d5" />
<img width="921" height="518" alt="image" src="https://github.com/user-attachments/assets/e1c9e614-5902-4e71-948a-e0ab90587bc5" />
<img width="919" height="518" alt="image" src="https://github.com/user-attachments/assets/511dd7fc-5dc8-4cf4-941d-aa742a8b9e06" />
<img width="923" height="517" alt="image" src="https://github.com/user-attachments/assets/a67fa3c9-4cae-41e0-a75f-05b4ca65deee" />
<img width="907" height="507" alt="image" src="https://github.com/user-attachments/assets/d2cc8af9-020c-4a01-92e1-ffe8658e885b" />

## 🚀 Kurulum ve Çalıştırma

### 1. Backend Hazırlığı
```bash
cd backend
pip install fastapi uvicorn jinja2
python main.py

