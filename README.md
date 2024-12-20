# 🔍 Terör Arananlar Yüz Tanıma Sistemi
Bu proje, Emniyet Genel Müdürlüğü'nün (EGM) www.terorarananlar.pol.tr sitesindeki verileri kullanarak, kamera veya video üzerinden yüz tanıma yapabilen bir uygulamadır.
## 📋 İçerik
- [Özellikler](#özellikler)
 [Kurulum](#kurulum)
 [Kullanım](#kullanım)
 [Sistem Gereksinimleri](#sistem-gereksinimleri)
 [Proje Yapısı](#proje-yapısı)
 [Katkıda Bulunma](#katkıda-bulunma)
## ✨ Özellikler
- **Otomatik Veri Toplama:** EGM'nin Terör Arananlar sitesinden otomatik veri çekme
 **Gerçek Zamanlı Tespit:** Kamera üzerinden anlık yüz tanıma
 **Video Analizi:** Video dosyalarından yüz tespiti ve tanıma
 **Yüksek Doğruluk:** Gelişmiş yüz tanıma algoritmaları ile güvenilir sonuçlar
 **Kategori Bazlı Filtreleme:** Aranan kişileri kategorilerine göre filtreleme imkanı
## 🚀 Kurulum
1. Projeyi klonlayın:
2. Gerekli paketleri yükleyin:
3. Projeyi çalıştırın:

## 💻 Kullanım

1. **Veri Çekme:**
   - `vericekme.py` dosyasını çalıştırarak güncel verileri çekin
   - İsteğe bağlı olarak kategori filtrelemesi yapabilirsiniz

2. **Dosya İsimlerini Düzenleme:**
   - Türkçe karakterleri düzeltmek için `adlandirma.py` dosyasını çalıştırın

3. **Uygulamayı Başlatma:**
   - Kamera ile tespit için:
   ```bash
   python main.py --mode camera
   ```
   - Video ile tespit için:
   ```bash
   python main.py --mode video --path video_dosyasi.mp4
   ```

## 💡 Sistem Gereksinimleri

- Python 3.7+
- OpenCV
- face_recognition
- numpy
- requests
- urllib3

## 📁 Proje Yapısı
baştan çok güzel bir readme dosyası yazmak istiyorum projemi iyi analiz edip readme dosyasını kullanıcılar için türkçe  yaz

Size projeniz için daha detaylı ve profesyonel bir README dosyası hazırlayacağım.
bash
git clone https://github.com/kullaniciadi/teror-arananlar-yuz-tanima.git
bash
pip install -r requirements.txt
bash:README.md
python vericekme.py
├── main.py # Ana uygulama dosyası
bash
git clone https://github.com/kullaniciadi/teror-arananlar-yuz-tanima.git
bash
pip install -r requirements.txt
bash
python vericekme.py
├── main.py # Ana uygulama dosyası
├── vericekme.py # Veri toplama modülü
├── adlandirma.py # Dosya ismi düzenleme aracı
├── simple_facerec.py # Yüz tanıma sınıfı
├── requirements.txt # Gerekli kütüphaneler
├── images/ # Yüz görüntüleri klasörü
└── data.json # Aranan kişiler veritabanı

## ⚙️ Özelleştirme

Proje farklı amaçlar için özelleştirilebilir:
- Farklı veri kaynakları kullanılabilir
- Tanıma hassasiyeti ayarlanabilir
- Yeni özellikler eklenebilir
- Arayüz geliştirilebilir

## 🤝 Katkıda Bulunma

1. Bu projeyi fork edin
2. Yeni bir branch oluşturun (`git checkout -b feature/yeniOzellik`)
3. Değişikliklerinizi commit edin (`git commit -am 'Yeni özellik eklendi'`)
4. Branch'inizi push edin (`git push origin feature/yeniOzellik`)
5. Pull Request oluşturun

## ⚠️ Yasal Uyarı

Bu proje sadece yasal ve etik amaçlar için kullanılmalıdır. Kötüye kullanımdan doğacak sorumluluklar kullanıcıya aittir.

## 📝 Lisans

Bu proje [MIT Lisansı](LICENSE) altında lisanslanmıştır.

## 🔧 Sorun Giderme

Sık karşılaşılan sorunlar ve çözümleri:

1. **Kütüphane Kurulum Hataları:**
   - face_recognition kütüphanesi için dlib kurulumu gereklidir
   - Windows için Visual Studio Build Tools gerekebilir

2. **Veri Çekme Sorunları:**
   - İnternet bağlantınızı kontrol edin
   - SSL sertifika hatalarında verify=False parametresini kullanın

3. **Performans İyileştirmeleri:**
   - Frame boyutunu küçültebilirsiniz
   - GPU desteği için CUDA kurulumu yapabilirsiniz


