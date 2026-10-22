# benGpT — gerçek yapay zekâ sürümü

Bu klasör Safari uyumlu sohbet arayüzünü, iPhone ana ekranına ekleme dosyalarını ve Vercel üzerinde çalışan güvenli API sunucu fonksiyonunu içerir.

## Önemli
- Bu ZIP tek başına internette yayınlanmış bir uygulama değildir.
- Gerçek AI cevapları için Vercel'e yayınlanması ve `OPENAI_API_KEY` ortam değişkeninin eklenmesi gerekir.
- API anahtarını `index.html` içine yazmayın ve kimseyle paylaşmayın.
- OpenAI API kullanımı, ChatGPT aboneliğinden ayrı ücretlendirilebilir. API hesabında faturalandırma/limit ayarı gerekir.

## Yayınlama özeti
1. ZIP'i açın ve içindeki dosyaları bir GitHub deposuna yükleyin (depo Public ise asla API anahtarı koymayın).
2. Vercel'de GitHub deposunu içe aktararak yeni proje oluşturun.
3. Vercel proje ayarlarında **Environment Variables** bölümüne `OPENAI_API_KEY` adında değişken ekleyin; değer alanına API anahtarınızı girin. İsteğe bağlı `OPENAI_MODEL` = `gpt-4.1-mini` ekleyebilirsiniz.
4. Deploy edin. Vercel'in verdiği HTTPS adresini Safari'de açın.
5. Bir mesaj göndererek test edin. Çalışmıyorsa Vercel proje loglarını ve API faturalandırma/limit ayarlarını kontrol edin.

## iPhone ana ekranına ekleme
1. Yayınlanmış HTTPS adresini Safari'de açın.
2. Paylaş düğmesine dokunun.
3. **Ana Ekrana Ekle** seçeneğini seçin.
4. Adı `benGpT` bırakıp **Ekle**'ye dokunun.

## Güvenlik ve ilk sürüm sınırları
- API anahtarı sunucu ortam değişkeninde tutulur, tarayıcıya gönderilmez.
- Sohbet geçmişi bu ilk sürümde sunucu veritabanına kaydedilmez; sayfayı yenileyince arayüz geçmişi sıfırlanabilir.
- Bu temel sürümde kullanıcı hesabı, ücretli üyelik ve kötüye kullanım kotası yoktur. Herkese açık yayın öncesi istek limiti/koruma eklenmesi önerilir.
