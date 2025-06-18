# 🎓 Moodle Tabanlı Performans ve Yük Testi

Bu proje, **Bilecik Şeyh Edebali Üniversitesi** kapsamında hazırlanmış bir çalışmadır. Projenin amacı, Moodle platformunun yüksek kullanıcı yükü altındaki performansını ölçmek ve analiz etmektir. Apache JMeter kullanılarak sistemin tepkileri detaylı şekilde incelenmiştir.

## 📌 Proje Amacı

- Moodle sisteminde **yük testi ve performans ölçümü** yapmak  
- Gerçek kullanıcı ve kurs verileriyle **senaryo bazlı testler** uygulamak  
- Sistemin kararlılığını ve yanıt süresini ölçmek  

## 🔧 Kullanılan Teknolojiler

- ✅ **Moodle LMS** (Açık kaynak kodlu eğitim yönetim sistemi)  
- ✅ **Apache JMeter** (Performans testi ve yük simülasyon aracı)  
- ✅ **PHP / MySQL / Apache** (Web sunucusu altyapısı)  
- ✅ **CSV** (Toplu kullanıcı ve kurs verisi yükleme)

## 🧪 Uygulanan Testler

### 1. Kullanıcı Giriş Testi
- 100 eş zamanlı kullanıcı /login/index.php adresine yönlendirildi  
- Ortalama yanıt süresi: **30 ms**  
- Maksimum: 52 ms – Minimum: 19 ms  
- Hata oranı: **%0**

### 2. Sınav (Quiz) Testi
- /mod/quiz/attempt.php üzerinden HTTP istekleri gönderildi  
- Sınav sırasındaki sistem davranışları gözlemlendi

### 3. Dosya Yükleme / İndirme Testi
- Ödev etkinliği oluşturuldu  
- /mod/assign/view.php ve yükleme endpointleri test edildi

### 4. Forum Kullanımı ve Mesajlaşma
- /mod/forum/post.php ve /message/index.php yollarıyla  
- Forum mesajlaşma, okuma ve cevaplama testleri yapıldı

## 📊 Sonuçlar

- Ortalama Yanıt Süresi: **30 ms**
- Hata Oranı: **%0**
- Verimlilik: **3.4 istek/saniye**
- Alınan veri: **92.66 KB/s**
- Gönderilen veri: **0.88 KB/s**

## 📂 Proje Dosyaları

| Dosya Adı                          | Açıklama                             |
|-----------------------------------|--------------------------------------|
| `bulut3.pdf`                      | Detaylı proje raporu                 |
| `İbrahim Akçal Enes Baş.pdf`      | Projenin sunumu / görsel özeti       |
| *(İsteğe bağlı)* `test_plan.jmx`  | JMeter senaryo dosyası               |
| *(İsteğe bağlı)* `users.csv`      | Kullanıcı veri dosyası               |
| *(İsteğe bağlı)* `courses.csv`    | Kurs veri dosyası                    |

## 👨‍💻 Hazırlayanlar

- **İbrahim Akçal** – 11203786592  
- **Enes Baş** – 10124322308

## 🔗 Kaynaklar

- [📘 Moodle Belgeleri](https://docs.moodle.org/)
- [🧪 Apache JMeter](https://jmeter.apache.org/)
- [📦 PHP Resmi Dokümantasyonu](https://www.php.net/manual/en/)
- [🛠 Apache HTTP Server](https://httpd.apache.org/)
- [💾 MySQL Dokümantasyonu](https://dev.mysql.com/doc/)

---

**Not:** Bu proje, bir eğitim ortamında yapılan test senaryosunu temsil etmektedir ve üretim sistemlerinde kullanılmadan önce özelleştirme ve güvenlik kontrolleri yapılmalıdır.
