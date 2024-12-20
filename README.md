# 🔍 Terör Arananlar Yüz Tanıma Sistemi
Bu proje, Emniyet Genel Müdürlüğü'nün (EGM) [www.terorarananlar.pol.tr](http://www.terorarananlar.pol.tr) sitesindeki verileri kullanarak, kamera veya video üzerinden yüz tanıma yapabilen bir uygulamadır.

---

## 📋 İçerik
- [Özellikler](#%C3%B6zellikler)
- [Kurulum](#kurulum)
- [Kullanım](#kullan%C4%B1m)
- [Sistem Gereksinimleri](#sistem-gereksinimleri)
- [Proje Yapısı](#proje-yap%C4%B1s%C4%B1)
- [Özelleştirme](#%C3%B6zelle%C5%9ftirme)
- [Yasal Uyarı](#yasal-uyar%C4%B1)
- [Lisans](#lisans)
- [Sorun Giderme](#sorun-giderme)

---

## ✨ Özellikler
- **Otomatik Veri Toplama:** EGM'nin Terör Arananlar sitesinden otomatik veri çekme.
- **Gerçek Zamanlı Tespit:** Kamera üzerinden anlık yüz tanıma.
- **Video Analizi:** Video dosyalarından yüz tespiti ve tanıma.
- **Yüksek Doğruluk:** Gelişmiş yüz tanıma algoritmaları ile güvenilir sonuçlar.
- **Kategori Bazlı Filtreleme:** Aranan kişileri kategorilerine göre filtreleme imkânı.

---

## 🚀 Kurulum

1. **Projeyi Klonlayın:**
   ```bash
   git clone https://github.com/mehmetadiyaman/Goruntu_Tespiti_Teror_Arananlar.git
   cd Goruntu_Tespiti_Teror_Arananlar
   ```

2. **Gerekli Paketleri Yükleyin:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Projeyi Çalıştırın:**
   ```bash
   python main.py
   ```

---

## 💻 Kullanım

1. **Veri Çekme:**
   - `vericekme.py` dosyasını çalıştırarak güncel verileri çekin.
     ```bash
     python vericekme.py
     ```
   - İsteğe bağlı olarak kategori filtrelemesi yapabilirsiniz.

2. **Dosya İsimlerini Düzenleme:**
   - Türkçe karakterleri düzeltmek için `adlandirma.py` dosyasını çalıştırın.
     ```bash
     python adlandirma.py
     ```

3. **Uygulamayı Başlatma:**
   - Kamera ile tespit için:
     ```bash
     python main.py --mode camera
     ```
   - Video ile tespit için:
     ```bash
     python main.py --mode video --path video_dosyasi.mp4
     ```

---

## 💡 Sistem Gereksinimleri
- Python 3.7+
- OpenCV
- face_recognition
- numpy
- requests
- urllib3

---

## 📁 Proje Yapısı
```plaintext
Goruntu_Tespiti_Teror_Arananlar/
├── main.py              # Ana uygulama dosyası
├── vericekme.py         # Veri toplama modülü
├── adlandirma.py        # Dosya ismi düzenleme aracı
├── simple_facerec.py    # Yüz tanıma sınıfı
├── requirements.txt     # Gerekli kütüphaneler
├── images/              # Yüz görüntüleri klasörü
└── data.json            # Aranan kişiler veritabanı
```

---

## ⚙️ Özelleştirme

Proje farklı amaçlar için özelleştirilebilir:
- Farklı veri kaynakları kullanılabilir.
- Tanıma hassasiyeti ayarlanabilir.
- Yeni özellikler eklenebilir.
- Arayüz geliştirilebilir.

---

## ⚠️ Yasal Uyarı
Bu proje sadece yasal ve etik amaçlar için kullanılmalıdır. Projenin kötüye kullanımından doğacak sorumluluklar kullanıcıya aittir.

---

## 📝 Lisans
Bu proje [MIT Lisansı](LICENSE) altında lisanslanmıştır.

---

## 🔧 Sorun Giderme

1. **Kütüphane Kurulum Hataları:**
   - `face_recognition` kütüphanesi için dlib kurulumu gereklidir.
   - Windows için Visual Studio Build Tools gerekebilir.

2. **Veri Çekme Sorunları:**
   - İnternet bağlantınızı kontrol edin.
   - SSL sertifika hatalarında `verify=False` parametresini kullanın.

3. **Performans İyileştirmeleri:**
   - Frame boyutunu küçültebilirsiniz.
   - GPU desteği için CUDA kurulumu yapabilirsiniz.

