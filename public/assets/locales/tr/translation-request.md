## NMS Optimizer'ın Çevirisinde Yardımcı Olun

Analitikler, dünyanın dört bir yanından ziyaretçiler olduğunu gösteriyor ve uygulamayı global No Man's Sky topluluğu için daha erişilebilir hâle getirmek istiyorum — işte burada siz devreye giriyorsunuz.

## Nasıl Yardımcı Olabilirsiniz

Uygulamayı çevirmeye yardımcı olacak iki dilli oyuncular arıyorum — özellikle **AI tarafından üretilmiş Fransızca, Almanca ve İspanyolca çevirileri düzenlemek ve düzeltmek**, veya güçlü NMS oyuncu topluluklarına sahip diğer diller üzerinde çalışmak için.

Profesyonel bir çevirmen olmanıza gerek yok — sadece dili akıcı konuşabilmek, oyunla aşina olmak ve yardım etmeye istekli olmak yeterlidir. Kesinlikle bu ChatGPT karmaşasından daha iyi olacaktır! Katkınız için isimle anılacaksınız (veya anonim kalmayı tercih ederseniz gizli kalabilirsiniz).

Metinlerin çoğu kısa kullanıcı arayüzü etiketleri, ipuçları veya eğlenceli durum mesajlarından ibaret.

Çeviriler [`i18next`](https://www.i18next.com/) kullanılarak yönetiliyor ve basit JSON ve Markdown dosyalarıyla yapılmaktadır. Ayrıca **Crowdin** kullanarak toplu çeviri katkılarını yönetiyoruz.

## Crowdin Kullanımı (Önerilen)

Katkıda bulunmanın en kolay yolu:

1. [https://crowdin.com](https://crowdin.com/project/nms-optimizer) adresinden **Crowdin’e kaydolun** ve NMS Optimizer projesine erişim talep edin.  
2. Onaylandıktan sonra, **web UI üzerinden mevcut çevirileri doğrudan düzenleyebilir** veya kendi çevirilerinizi yükleyebilirsiniz.  
3. Crowdin farklı dilleri yönetir ve güncellemelerinizin uygulama ile otomatik senkronize olmasını sağlar.  
4. Mevcut çevirileri düzeltmeye veya kendi dilinizde yeni çeviriler eklemeye odaklanabilirsiniz.

> Crowdin, standart [ISO dil kodları](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) kullanır: Fransızca için `fr`, Almanca için `de`, İspanyolca için `es` vb.

GitHub’a aşina değilseniz veya değişikliklerin uygulamada hemen görünmesini istiyorsanız, bu yöntem önerilen yaklaşımdır.

## GitHub ile Rahat Çalışıyorsanız

**Depoyu Forklayın:**  
[github.com/jbelew/nms_optimizer-web](https://github.com/jbelew/nms_optimizer-web)

**Çeviri Dosyalarını Güncelleyin veya Oluşturun:**

- Uygulama UI etiketleri `/src/i18n/locales/[language_code]/translation.json` dizininde bulunur.  
- Daha büyük diyalog kutusu içerikleri `/public/locales/[language_code]/` dizininde saf Markdown dosyaları olarak saklanır.

Mevcut dosyaları güncelleyebilir veya diliniz için [ISO 639-1 kodunu](https://en.wikipedia.org/wiki/List_of-ISO_639-1-codes) kullanarak yeni bir klasör oluşturabilirsiniz (örn. `de` Almanca için). İlgili Markdown ve JSON dosyalarını bu klasöre kopyalayın ve içeriği güncelleyin.

> _Örnek:_ Diyalog içeriği için `/public/locales/de/about.md` ve UI etiketleri için `/src/i18n/locales/de/translation.json` oluşturun.

**İşiniz bittiğinde bir pull request gönderin.**

## Pull Request Yapmak İstemiyor Musunuz?

Sorun değil — sadece [GitHub Discussions sayfasına](https://github.com/jbelew/nms_optimizer-web/discussions) gidin ve yeni bir konu başlatın.

Çevirilerinizi buraya yapıştırabilir veya nereden başlayacağınızdan emin değilseniz sorular sorabilirsiniz. Ben devamını hallederim.

## Notlar

`randomMessages`, isminden de anlaşılacağı gibi — optimizasyon birkaç saniyeden uzun sürerse gösterilen rastgele mesajlar listesidir. Hepsini çevirmek zorunda değilsiniz; dilinizde anlamlı birkaç tane yeterlidir.

Herkes için No Man's Sky Teknoloji Yerleşim Optimizer’ı daha iyi hâle getirmeye yardımcı olduğunuz için teşekkürler! Herhangi bir sorunuz olursa bana bildirin — memnuniyetle yardımcı olurum.

