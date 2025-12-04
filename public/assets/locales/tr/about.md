## NMS Optimizer Nedir?

NMS Optimizer, **No Man's Sky** oyunu için güçlü bir web tabanlı **hesaplayıcı**, **planlayıcı** ve **düzenleyici** aracıdır. Oyuncuların ekipmanları için en iyi modül yerleşimlerini tasarlamalarına yardımcı olur. Bu araç, **Uzay Gemisi düzenleri**, **Yük Gemileri (Freighter) düzenleri**, **Korvet düzenleri**, **Çok Amaçlı Alet (Multitool) yapıları**, **Exocraft düzenleri** ve **Exosuit yapılarını** destekler. Oyuncuların kritik oyun mekaniklerinden olan **bitişiklik bonuslarını** (benzer teknolojilerin gruplanmasından elde edilen) ve **süper şarjlı yuvalardan** gelen güçlü takviyeleri en üst düzeye çıkarmak için en iyi modül yerleşimini otomatik olarak hesaplar. Bu özelliklerin doğru kullanımı, maksimum performans elde etmek için kritik öneme sahiptir ve bu araç bu karmaşık süreci basitleştirir.  

## Nasıl Çalışır

> ~8,32 × 10⁸¹ olası kombinasyonu (82 basamaklı!) beş saniye içinde nasıl çözersiniz?

Tam bir ızgaradaki mutlak en iyi **modül yerleşimini** bulmak hiç de kolay değildir. Bu araç, deterministik desenler, makine öğrenimi ve Rust tabanlı simüle edilmiş tavlama (simulated annealing) yöntemlerini harmanlayarak yaklaşık beş saniyede en iyi **Uzay Gemisi**, **Yük Gemisi**, **Korvet**, **Çok Amaçlı Alet**, **Exocraft** ve **Exosuit** yapılarını sunar. Tüm faktörleri, **bitişiklik bonusları** ve **süper şarjlı yuvaların** stratejik kullanımını dikkate alır.

1.  **Desen Tabanlı Ön Çözüm:** Maksimum bitişiklik bonusu sağlayan, farklı ızgara tipleri için el ile test edilmiş yerleşim desenlerinden oluşan bir kütüphane ile başlar.  
2.  **Yapay Zeka Destekli Yerleştirme (ML Tahmini):** Eğer uygun bir yapı süper şarjlı yuvaları içeriyorsa, araç, optimal yerleşimi tahmin etmek için 16.000+ ızgara üzerinde eğitilmiş bir TensorFlow modelini devreye sokar.  
3.  **Simüle Edilmiş Tavlama (İyileştirme):** Yerleşimi rastgele değişimler ve modül kaydırmaları ile iyileştirir, bitişiklik puanını artırırken yerel maksimumlara takılmayı önler.  
4.  **Sonuç Sunumu:** En yüksek puanlı yapılandırmayı, puan dağılımları ve görsel yerleşim önerileri ile birlikte sunar: Uzay Gemileri, Yük Gemileri, Korvetler, Çok Amaçlı Aletler, Exocraft ve Exosuit’ler için.  

## Temel Özellikler

- **Kapsamlı Izgara Optimizasyonu:** Standart, **süper şarjlı** ve devre dışı yuvalar dahil tüm yuvaları destekleyerek gerçek optimal yerleşimi bulur.  
- **Stratejik Süper Şarjlı Yuvaların Kullanımı:** Süper şarjlı yuvaları sadece tanımakla kalmaz, hangi temel teknolojilerin veya en iyi yükseltmelerin bu yuvalara yerleştirileceğini hesaplar. Bu, hasar, menzil veya verimlilik gibi hedeflerinizi maksimize etmek için karmaşık takasları hesaplar. Uzman oyuncu stratejilerini taklit eder, ancak hesaplamayı kesin bir şekilde yapar.  
- **Makine Öğrenimi Tahmini:** 16.000+ geçmiş ızgara üzerinde eğitilmiş olup güçlü yerleşim desenlerini tanır.  
- **Gelişmiş Simüle Edilmiş Tavlama:** Her performans yüzdesinin optimize edilmesini sağlar.  

## Neden Bu Aracı Kullanmalı?

Modül yerleşimini tahmin etmeyi bırakın ve ekipmanınızın gerçek potansiyelini ortaya çıkarın! Maksimum hasar veren bir **Uzay Gemisi yapısı**, uzun menzilli bir **Yük Gemisi yapısı**, güçlü bir **Korvet yapısı**, mükemmel bir **Çok Amaçlı Alet yerleşimi**, optimize bir **Exocraft** veya sağlam bir **Exosuit** hedefliyorsanız, bu optimizer **bitişiklik bonusları** ve **süper şarjlı yuvaların** karmaşık etkileşimlerini anlaşılır bir şekilde sunar. Sınırlı süper şarjlı yuvalarınızı en verimli şekilde kullanmak istiyorsanız, bu **NMS hesaplayıcısı** size doğru cevabı verir.  

## Teknoloji Yığını (Tech Stack)

- **Frontend:** TypeScript, React, Zustand, Vite, Tailwind CSS, Radix UI  
- **Backend Çözücü:** Python, Flask, TensorFlow, NumPy, Rust tabanlı özel simüle edilmiş tavlama ve sezgisel puanlama implementasyonları  
- **Test:** Vitest, Python Unittest  
- **Dağıtım:** Heroku (Hosting), Cloudflare (DNS ve CDN), Docker  
- **Otomasyon:** GitHub Actions (CI/CD)  
- **Analitik:** Google Analytics  

## Depolar (Repositories)

- Web UI: [https://github.com/jbelew/nms_optimizer-web](https://github.com/jbelew/nms_optimizer-web)  
- Backend: [https://github.com/jbelew/nms_optimizer-service](https://github.com/jbelew/nms_optimizer-service)  

## Sıkça Sorulan Sorular

### No Man's Sky’de bitişiklik bonusu nedir?

Bitişiklik bonusu, uyumlu teknoloji modüllerini yan yana yerleştirdiğinizde elde edilen performans artışıdır. Aynı türden modülleri bir araya getirdikçe bonus güçlenir. NMS Optimizer, tüm teknolojileriniz için bu bonusları maksimize eden optimal yerleşimi hesaplar.  

### Süper şarjlı yuvalar nasıl çalışır?

Süper şarjlı yuvalar, yerleştirilen herhangi bir teknoloji modülüne yaklaşık %25-30 oranında büyük bir bonus sağlar. Çoğu platformda 4 yuva ile sınırlıdır ve stratejik olarak değerlidir. Optimizer, temel teknolojileri mi yoksa en iyi yükseltmeleri mi süper şarjlı yuvalara koymanız gerektiğini hesaplayarak performansı maksimize eder.  

### Hangi platformları destekliyor?

Optimizer, tüm önemli No Man’s Sky platformlarını destekler:  

- **Uzay Gemileri** (Standart, Egzotik, Sentinel, Solar, Yaşayam)  
- **Korvetler** (benzersiz reaktör ve kozmetik modül desteği ile)  
- **Çok Amaçlı Aletler** (Standart, Egzotik, Atlantid, Sentinel, Asalar)  
- **Exocraft** (Minotaur dahil tüm tipler)  
- **Exosuit**  
- **Yük Gemileri (Freighters)**  

### Optimizer ne kadar doğru?

Çok yüksek doğrulukta. Araç, kanıtlanmış desenler, 16.000+ yerleşim üzerinde eğitilmiş makine öğrenimi ve simüle edilmiş tavlama ile birlikte çalışır. Bitişiklik bonusları, süper şarjlı yuvalar ve modül yerleşim kısıtlamaları gibi tüm faktörleri dikkate alır ve belirli yapılandırmanız için matematiksel olarak optimal yerleşimi bulur.  

### Kullanımı ücretsiz mi?

Evet! NMS Optimizer tamamen ücretsiz, reklamsız ve açık kaynaklıdır. Kayıt veya ödeme gerektirmez.  

### Yapılarımı kaydedebilir ve paylaşabilir miyim?

Kesinlikle! Optimize edilmiş yerleşimlerinizi `.nms` dosyası olarak kaydedebilir, daha sonra tekrar yükleyebilir veya arkadaşlarınıza göndermek için paylaşılabilir bağlantılar oluşturabilirsiniz. Tüm yapılar bütünlük ve uyumluluk açısından doğrulanır.  

## Küçük Bir Tarihçe

İşte UI’nin **erken bir versiyonu**—fonksiyonel olarak sağlam ama görsel olarak minimal. Mevcut sürüm, tasarım, kullanılabilirlik ve netlik açısından büyük bir yükseltme sunar ve oyuncuların herhangi bir gemi veya araç için **en iyi yerleşimi** hızlıca bulmasını sağlar.  

![No Man's Sky yerleşim optimizer kullanıcı arayüzünün erken prototipi](/assets/img/screenshots/screenshot_v03.png)

