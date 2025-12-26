# YAPILACAKLAR LİSTESİ - RAPOR DÜZELTMELERİ

## 🔴 YÜKSEK ÖNCELİK - MUTLAKA YAPILMALI

### 1. BM SÜRDÜRÜLEBİLİR KALKINMA HEDEFLERİ EKLENMELİ
   - **Konum**: Bölüm 1.1 (Proje Tanımı) veya Bölüm 1.2 (Benzer Ürünler ve Literatür İncelemesi)
   - **Eklenecek İçerik**: 
     - Projenin BM SKH Hedef 3: "Sağlıklı Yaşam ve Herkes İçin Refah" ile bağlantısı
     - Hedef 3.8: "Herkes için sağlık hizmetlerine evrensel erişim"
     - Projenin bu hedefe nasıl katkı sağladığı açıklanmalı
   - **Örnek Metin**: 
     ```
     Bu proje, Birleşmiş Milletler Sürdürülebilir Kalkınma Hedefleri'nden Hedef 3: 
     "Sağlıklı Yaşam ve Herkes İçin Refah" kapsamında, özellikle Hedef 3.8'in 
     "Herkes için sağlık hizmetlerine evrensel erişim" alt hedefine katkı sağlamaktadır. 
     Platform, kırsal bölgelerde ve gelişmekte olan ülkelerde yaşayan bireylerin 
     uzman doktorlara erişimini kolaylaştırarak, erken teşhis imkanı sunmakta ve 
     sağlık hizmetlerine erişilebilirliği artırmaktadır.
     ```

### 2. TEST SONUÇLARI TABLOLARI EKLENMELİ
   - **Konum**: Bölüm 3.1.2 (Model Doğruluk Testleri)
   - **Eklenecek Tablolar**:
     - **Tablo 3.1**: Model Doğruluk Sonuçları Tablosu
       - Sütunlar: Hastalık Türü, Model Mimarisi, Test Accuracy, Precision, Recall, F1 Score, Eğitim Veri Seti, Test Veri Seti
       - Satırlar: Deri Hastalıkları, Kemik Hastalıkları, Akciğer Hastalıkları
     - **Tablo 3.2**: Performans Test Sonuçları Tablosu
       - Sütunlar: Metrik, Hedef Değer, Gerçekleşen Değer, Durum
       - Satırlar: Görüntü Analizi Süresi, API Yanıt Süresi, Sayfa Yükleme Süresi, Eşzamanlı Kullanıcı Sayısı
     - **Tablo 3.3**: API Yanıt Süreleri Tablosu
       - Sütunlar: Endpoint, Ortalama Süre (ms), P95 Süre (ms), Durum
     - **Tablo 3.4**: Model Tahmin Süreleri Tablosu
       - Sütunlar: Hastalık Türü, Ortalama Süre (saniye), Min Süre, Max Süre
     - **Tablo 3.5**: Sayfa Yükleme Süreleri Tablosu
       - Sütunlar: Sayfa, FCP (saniye), LCP (saniye), TTI (saniye)
     - **Tablo 3.6**: Benzer Sistemlerle Karşılaştırma Tablosu
       - Sütunlar: Platform, Çoklu Hastalık, Tele-Tıp, Açık Kaynak, Maliyet, Model Doğruluğu
       - Satırlar: Bu Çalışma, Teladoc, Amwell, ISIC Platform, vb.

### 3. FONKSİYONEL OLMAYAN GEREKSİNİMLERİN TEST SONUÇLARI EKLENMELİ
   - **Konum**: Bölüm 3.1.3 (Performans Testleri) altına yeni alt bölüm
   - **Eklenecek İçerik**:
     - **3.1.3.1. Eşzamanlı Kullanıcı Testi**
       - Test yöntemi: Load testing (ör. Apache JMeter, Locust)
       - Sonuç: Sistem X eşzamanlı kullanıcıyı destekledi (hedef: 100)
       - Test ortamı: [belirtilmeli]
     - **3.1.3.2. Rate Limiting Testi**
       - Test yöntemi: [belirtilmeli]
       - Sonuç: Rate limiting başarıyla çalıştı, DDoS saldırıları engellendi
     - **3.1.3.3. Güvenilirlik Testi**
       - Uptime testi: [sonuç]
       - Veri kaybı testi: [sonuç]
     - **Tablo**: Fonksiyonel Olmayan Gereksinimler Test Sonuçları
       - Sütunlar: Gereksinim, Hedef, Gerçekleşen, Durum (✅/❌)

### 4. Dermascan → MediAnalytica DEĞİŞTİRİLMELİ
   - **Bulunan Yerler**:
     - RAPOR.txt satır 852: `'app_name': "DermaScan API"` → `'app_name': "MediAnalytica API"`
   - **Kontrol Edilmesi Gereken Dosyalar**:
     - RAPOR.txt (tüm dosya taranmalı)
     - Diğer tüm .md ve .txt dosyaları
   - **Yapılacak**: Tüm dosyalarda "DermaScan", "dermaScan", "DERMASCAN" → "MediAnalytica" olarak değiştirilmeli

### 5. MELİH KIZMAZ'IN GÖREVLERİNE EKSİK OLAN KISIM EKLENMELİ
   - **Konum**: Bölüm 2.1.1 (Melih Kızmaz'ın Görev Tanımı ve Kapsam)
   - **Eksik Olan**: Veri seti araştırması ve veri seti hazırlama
   - **Eklenecek İçerik**:
     ```
     Melih Kızmaz, projede yapay zeka modeli eğitimi ve optimizasyonu sorumluluğunu 
     üstlenmiştir. Derin öğrenme modellerinin geliştirilmesi, model mimarisi tasarımı, 
     **veri seti araştırması ve seçimi (ISIC, Mendeley, Kaggle), veri seti hazırlama 
     ve ön işleme**, veri ön işleme ve veri artırma tekniklerinin uygulanması, model 
     değerlendirme ve performans metriklerinin hesaplanması, Grad-CAM görselleştirme 
     tekniğinin implementasyonu bu görev kapsamındadır.
     ```
   - **Ayrıca Bölüm 2.1.2 (Tasarım) altına eklenmeli**:
     ```
     2.1.2.1. Veri Seti Araştırması ve Seçimi
     
     Proje kapsamında, açık kaynak tıbbi görüntü veri setleri araştırılmış ve 
     seçilmiştir. Deri hastalıkları için ISIC (International Skin Imaging 
     Collaboration) veri seti, kemik hastalıkları için Mendeley ve Kaggle 
     veri setleri, akciğer hastalıkları için Chest X-Ray veri setleri 
     kullanılmıştır. Her veri seti, sınıf dengesi, görüntü kalitesi ve 
     etiket doğruluğu açısından değerlendirilmiştir.
     
     2.1.2.2. Veri Seti Hazırlama ve Ön İşleme
     
     Seçilen veri setleri, model eğitimi için hazırlanmıştır. Veri seti 
     hazırlama süreci şu adımları içermektedir:
     - Veri seti indirme ve organizasyonu
     - Görüntü formatı standardizasyonu (JPEG, PNG)
     - Görüntü boyutlandırma ve normalizasyon
     - Train/Validation/Test split (örn: 70/15/15)
     - Sınıf dengesizliği kontrolü ve düzeltme
     - Veri kalitesi kontrolü (bozuk görüntülerin temizlenmesi)
     ```

---

## 🟡 ORTA ÖNCELİK - YAPILMASI ÖNERİLİR

### 6. KAYNAK TARİHLERİNİN DÜZELTİLMESİ
   - **Sorun**: Bazı kaynaklar "2024" tarihli (gelecek tarih)
   - **Yapılacak**: Tüm kaynak tarihleri kontrol edilmeli, 2023 veya uygun tarih olarak düzeltilmeli
   - **Kontrol Edilecek**: KAYNAKLAR bölümü

### 7. MELİH KIZMAZ'IN VERİ SETİ ÇALIŞMALARININ DETAYLANDIRILMASI
   - **Konum**: Bölüm 2.1.3 (Kullanılan Teknolojiler) altına eklenebilir
   - **Eklenecek**: Veri seti işleme kütüphaneleri (PIL/Pillow, OpenCV, pandas, numpy)

---

## 📋 YAPILACAKLAR ÖZETİ (SIRAYLA)

1. ✅ **BM SKH bağlantısını ekle** (Bölüm 1.1 veya 1.2)
2. ✅ **Test sonuçları tablolarını ekle** (Bölüm 3.1.2 - 6 tablo)
3. ✅ **Fonksiyonel olmayan gereksinimlerin test sonuçlarını ekle** (Bölüm 3.1.3)
4. ✅ **DermaScan → MediAnalytica değiştir** (Tüm dosyalarda)
5. ✅ **Melih Kızmaz'ın görevlerine veri seti araştırması ve hazırlama ekle** (Bölüm 2.1.1 ve 2.1.2)
6. ⚠️ **Kaynak tarihlerini düzelt** (KAYNAKLAR bölümü)
7. ⚠️ **Melih Kızmaz'ın veri seti çalışmalarını detaylandır** (Bölüm 2.1.3)

---

## 📝 NOTLAR

- Tüm değişiklikler yapıldıktan sonra raporun tutarlılığı kontrol edilmeli
- Tablolar ve şekiller eklendikten sonra içindekiler tablosu güncellenmeli
- Kaynak atıfları metin içinde kontrol edilmeli
- Sayfa numaraları kontrol edilmeli (eğer varsa)


