```markdown
![npm version](https://img.shields.io/npm/v/chatgpt-prompt-engineering)
![downloads](https://img.shields.io/npm/dm/chatgpt-prompt-engineering)
![license](https://img.shields.io/npm/l/chatgpt-prompt-engineering)
![build](https://img.shields.io/github/actions/workflow/status/turkcoode/chatgpt-prompt-engineering/ci.yml)

## Table of Contents

- [Giri](#giri)
- [Neden Bu Ara](#neden-bu-ara)
- [zellikler](#zellikler)
- [Kurulum](#kurulum)
- [Hzl Balang](#hzl-balang)
- [API Referans](#api-referans)
- [CLI Kullanm](#cli-kullanm)
- [Konfigrasyon](#konfigrasyon)
- [Mimari ve Tasarm Kararlar](#mimari-ve-tasarm-kararlar)
- [Performans ve Optimizasyon](#performans-ve-optimizasyon)
- [Gerek Dnya Kullanm Senaryolar](#gerek-dnya-kullanm-senaryolar)
- [SSS ve Sorun Giderme](#sss-ve-sorun-giderme)
- [Katkda Bulunma](#katkda-bulunma)
- [Dokmantasyon](#dokmantasyon)
- [Lisans](#lisans)

## Giriş

Günümüzde yapay zeka uygulamaları, özellikle de dil modelleri, birçok sektörde devrim yaratma potansiyeline sahiptir. Ancak, bu modellerin etkili bir şekilde kullanılabilmesi için doğru "prompt" yani talimatları sağlamak kritik bir önem taşır. 10.000 kullanıcıya sahip bir SaaS projesinde, kullanıcıların doğru sonuçlar alabilmesi için sadece doğru verilerin sağlanması yeterli değildir; aynı zamanda bu verilerin nasıl sunulduğu da büyük bir rol oynamaktadır. Yanlış ya da yetersiz prompt'lar, kullanıcıların beklentilerini karşılamayabilir ve bu da müşteri kaybına yol açabilir. İşte bu noktada "ChatGPT Prompt Engineering Toolkit" devreye giriyor.

ChatGPT Prompt Engineering Toolkit, ChatGPT ve GPT-4 ile etkileşimde bulunmak için gelişmiş bir prompt mühendisliği çerçevesidir. Bu araç, kullanıcıların etkili ve optimize edilmiş prompt'lar oluşturmasına yardımcı olmak için çeşitli şablonlar, düşünce zinciri kalıpları ve otomatik prompt optimizasyonu gibi özellikler sunar. Yapay zeka ile etkileşim kurarken en iyi sonuçları elde etmek, doğru araç ve yöntemler kullanmayı gerektirir. Bu araç, hem yeni başlayanlar hem de deneyimli kullanıcılar için ideal bir çözümdür. Eğer yapay zeka projelerinizde başarı elde etmek istiyorsanız, bu araç tam da ihtiyacınız olan şey olabilir. Özellikle dil işleme, metin analizi veya yaratıcı yazma gibi alanlarda çalışan profesyonellerin bu aracı kullanarak verimliliklerini artırmaları mümkündür.

## Neden Bu Araç?

Bu araç, mevcut benzer araçlardan birkaç önemli özellik ile ayrılmaktadır. Örneğin, birçok popüler prompt mühendisliği kütüphanesi, kullanıcıların sadece basit prompt'lar oluşturmasına izin verirken, ChatGPT Prompt Engineering Toolkit, kullanıcıların düşünce zinciri kalıpları oluşturmasına ve otomatik optimizasyon yapmasına olanak tanır. Bu özellik, kullanıcıların daha karmaşık ve etkili prompt'lar oluşturmasına yardımcı olur.

Ayrıca, mevcut birçok alternatif, Türkçe gibi dillerde yeterli destek sunmamaktadır. Bu nedenle, Türkçe dil desteği ile kullanıcıların bu araçtan daha fazla faydalanabilmesi sağlanmaktadır. Aşağıdaki tabloda ChatGPT Prompt Engineering Toolkit ile bazı popüler alternatiflerin karşılaştırmasını görebilirsiniz:

| Özellik                               | ChatGPT Prompt Engineering Toolkit | Alternatif 1 (dzhng/llamaflow) |
|---------------------------------------|-----------------------------------|----------------------------------|
| Türkçe Desteği                        | ✅                                 | ❌                                |
| Otomatik Prompt Optimizasyonu         | ✅                                 | ❌                                |
| Düşünce Zinciri Kalıpları            | ✅                                 | ✅                                |
| Hata Yönetimi                         | ✅                                 | ✅                                |
| CLI Desteği                           | ✅                                 | ❌                                |
| Docker Entegrasyonu                   | ✅                                 | ❌                                |

Bu tabloda görüldüğü üzere, ChatGPT Prompt Engineering Toolkit, hem teknik özellikleri hem de kullanıcı ihtiyaçlarını karşılaması açısından rakiplerinden bir adım öndedir. Kullanıcıların daha etkili ve optimize edilmiş sonuçlar elde etmesine yardımcı olurken, aynı zamanda geniş bir kullanıcı kitlesine hitap etme yeteneği sunmaktadır. Özellikle, projelerinizde deneyimlediğiniz zorlukları aşmanıza yardımcı olacak esnek bir yapı sunması, bu aracı tercih etmenizi sağlayabilir.

## Özellikler

ChatGPT Prompt Engineering Toolkit, kullanıcı deneyimini geliştirmek için birçok özellik sunmaktadır. İşte bu araçtaki bazı temel özellikler:

- **Otomatik Prompt Optimizasyonu**: Kullanıcıların sağladığı temel prompt'ları analiz ederek en iyi sonuçları elde etmek için otomatik olarak optimize eder. Bu, kullanıcıların daha az çaba harcayarak daha iyi sonuçlar almasını sağlar. Ayrıca, kullanıcıların zamanını alacak tekrar eden görevleri otomatikleştirerek, verimlilik artışı sağlamaktadır.

- **Düşünce Zinciri Kalıpları**: Kullanıcıların karmaşık düşünce süreçlerini daha iyi yansıtabilmesi için önceden tanımlanmış düşünce zinciri kalıpları sunar. Bu kalıplar, kullanıcıların problem çözme yeteneklerini geliştirmesine yardımcı olur ve yaratıcı düşünme süreçlerini destekler.

- **CLI Desteği**: Komut satırı arayüzü ile kullanıcıların hızlı ve etkili bir şekilde prompt'lar oluşturmasına ve test etmesine olanak tanır. CLI kullanımı, özellikle geliştiriciler için büyük bir avantaj sağlar; komut satırını kullanarak hızlı bir şekilde denemeler yapabilir ve sonuçları görebilirler.

- **Hata Yönetimi**: API çağrıları sırasında oluşabilecek hataları etkili bir şekilde yönetir. Örneğin, oran sınırlama hataları için otomatik geri çekilme (exponential backoff) stratejisi uygular. Kullanıcıların karşılaşabileceği sorunları minimize ederek, sorunsuz bir deneyim sunar.

- **Türkçe Desteği**: Türkçe gibi dillerde yeterli destek sunarak, yerel kullanıcıların ihtiyaçlarını karşılar. Bu, Türkçe konuşan geliştiricilerin ve kullanıcıların bu araçtan daha fazla faydalanabilmesine olanak tanır ve projelerinin yerel pazarda daha etkili olmasını sağlar.

- **Docker Entegrasyonu**: Araç, Docker ile entegre çalışabilmesi için gerekli yapılandırmaları içerir. Bu, kullanıcıların kendi uygulamalarında kolayca kullanabilmesine ve dağıtım süreçlerini hızlandırabilmesine olanak tanır.

Bu özellikler, ChatGPT Prompt Engineering Toolkit'i rakiplerinden ayıran ve kullanıcıların projelerinde başarı elde etmesine yardımcı olan faktörlerdir. Kullanıcıların ihtiyaç duyduğu çeşitli senaryolar için esnek bir çözüm sunması, bu aracı daha da cazip kılmaktadır.

## Kurulum

ChatGPT Prompt Engineering Toolkit'i projelerinizde kullanmaya başlamak oldukça kolaydır. Aşağıda, npm, yarn ve pnpm kullanarak nasıl kurulum yapacağınızı bulabilirsiniz.

### npm ile Kurulum

```bash
npm install chatgpt-prompt-engineering
```

### Yarn ile Kurulum

```bash
yarn add chatgpt-prompt-engineering
```

### pnpm ile Kurulum

```bash
pnpm add chatgpt-prompt-engineering
```

Kurulum işlemi tamamlandıktan sonra, projelerinizde bu aracı kullanmaya başlayabilirsiniz. Aşağıda, bu aracın nasıl kullanılacağı hakkında kısa bir bilgi verilecektir. Kurulum adımlarının basitliği, bu aracı projelerde hızlı bir şekilde devreye almanıza olanak tanır.

## Hızlı Başlangıç

ChatGPT Prompt Engineering Toolkit'i kullanmaya başlamak için aşağıdaki adımları takip edebilirsiniz. İlk olarak, aracı içe aktarın ve ardından basit bir örnekle başlayın.

### Örnek 1: Basit Prompt Oluşturma

```javascript
const { ChatGPT } = require('chatgpt-prompt-engineering');

const chatgpt = new ChatGPT();

const prompt = "Bana yapay zeka hakkında kısa bir bilgi ver.";
chatgpt.send(prompt).then(response => {
    console.log(response);
});
```

### Örnek 2: Düşünce Zinciri Kullanma

```javascript
const { ChatGPT, ChainOfThought } = require('chatgpt-prompt-engineering');

const chatgpt = new ChatGPT();
const chain = new ChainOfThought();

const prompt = "Bir problem çözme sürecini açıkla.";
chain.addStep(prompt);

chain.execute(chatgpt).then(response => {
    console.log(response);
});
```

### Örnek 3: Otomatik Optimizasyon

```javascript
const { ChatGPT } = require('chatgpt-prompt-engineering');

const chatgpt = new ChatGPT();

const prompt = "Yapay zeka nedir?";
chatgpt.optimizePrompt(prompt).then(optimizedPrompt => {
    return chatgpt.send(optimizedPrompt);
}).then(response => {
    console.log(response);
});
```

Bu örnekler, ChatGPT Prompt Engineering Toolkit'i kullanarak nasıl etkili ve optimize edilmiş prompt'lar oluşturabileceğinizi göstermektedir. Kullanım kolaylığı ve pratikliği sayesinde, projelerinizde hızlı bir şekilde uygulamaya başlayabilirsiniz. Ayrıca, bu örnekler üzerinde kendi deneyimlerinizi yaparak, daha karmaşık senaryolar oluşturabilirsiniz.

## API Referansı

ChatGPT Prompt Engineering Toolkit'in sunduğu API, kullanıcıların bu aracı etkili bir şekilde kullanabilmesi için tasarlanmıştır. Aşağıda, API'nin temel fonksiyon imzaları ve parametreleri yer almaktadır.

### Fonksiyonlar

- `send(prompt: string): Promise<string>`
  - **Açıklama**: Verilen prompt'u ChatGPT'ye gönderir ve yanıtı döner.
  - **Parametreler**:
    - `prompt`: Gönderilecek metin.
  - **Dönüş Değeri**: ChatGPT'den alınan yanıt.

- `optimizePrompt(prompt: string): Promise<string>`
  - **Açıklama**: Verilen prompt'u optimize eder.
  - **Parametreler**:
    - `prompt`: Optimize edilecek metin.
  - **Dönüş Değeri**: Optimize edilmiş prompt.

- `addChainStep(step: string): void`
  - **Açıklama**: Düşünce zincirine yeni bir adım ekler.
  - **Parametreler**:
    - `step`: Eklenecek adım.

- `execute(chain: ChainOfThought): Promise<string>`
  - **Açıklama**: Düşünce zincirini çalıştırır ve sonuç döner.
  - **Parametreler**:
    - `chain`: Çalıştırılacak düşünce zinciri.
  - **Dönüş Değeri**: Düşünce zincirinin sonucu.

### Örnek Kullanım

```javascript
const { ChatGPT, ChainOfThought } = require('chatgpt-prompt-engineering');

const chatgpt = new ChatGPT();
const chain = new ChainOfThought();

chain.addChainStep("Bir problem çözme sürecini açıkla.");
chain.addChainStep("Bu sürecin avantajları nelerdir?");

chain.execute(chatgpt).then(response => {
    console.log(response);
});
```

Bu API, kullanıcıların ChatGPT ile etkileşimde bulunmalarını kolaylaştırmak için tasarlanmıştır. Genişletilebilir yapısı sayesinde, gelecekte daha fazla fonksiyon eklenmesi mümkündür. API'nin sağladığı esneklik, geliştiricilerin projelerinde ihtiyaç duydukları özellikleri hızlı bir şekilde eklemelerine olanak tanır.

## CLI Kullanımı

ChatGPT Prompt Engineering Toolkit, kullanıcıların komut satırı arayüzü (CLI) üzerinden de kullanımına olanak tanır. CLI, kullanıcıların hızlı ve etkili bir şekilde prompt oluşturmalarını sağlar. Aşağıda, CLI kullanımına ilişkin bazı temel komutlar ve flag'ler bulunmaktadır.

### Temel Komutlar

- `chatgpt --prompt "<prompt_metin>"`
  - **Açıklama**: Verilen prompt'u ChatGPT'ye gönderir.
  - **Örnek**: 
    ```bash
    chatgpt --prompt "Yapay zeka nedir?"
    ```

- `chatgpt --optimize "<prompt_metin>"`
  - **Açıklama**: Verilen prompt'u optimize eder.
  - **Örnek**:
    ```bash
    chatgpt --optimize "Yapay zeka nedir?"
    ```

### Flag'ler

- `--lang <dil>`
  - **Açıklama**: Kullanılacak dilin belirtildiği flag.
  - **Örnek**: 
    ```bash
    chatgpt --prompt "Yapay zeka nedir?" --lang "tr"
    ```

- `--output <dosya_yolu>`
  - **Açıklama**: Çıktının kaydedileceği dosya yolu.
  - **Örnek**: 
    ```bash
    chatgpt --prompt "Yapay zeka nedir?" --output "sonuc.txt"
    ```

CLI kullanımı, geliştiricilerin hızlı bir şekilde test yapmalarını ve sonuçları görmelerini sağlar. Bu, özellikle geliştirme aşamasında büyük bir avantaj sunmaktadır. Kullanıcılar, CLI aracılığıyla farklı senaryoları kolayca deneyebilir ve geri bildirim alabilir.

## Konfigürasyon

ChatGPT Prompt Engineering Toolkit, kullanıcıların projelerine kolayca entegre olabilmesi için çeşitli konfigürasyon seçenekleri sunmaktadır. Aşağıda, konfigürasyon dosyası ve çevresel değişkenler hakkında daha fazla bilgi bulabilirsiniz.

### Konfigürasyon Dosyası

Kullanıcılar, `config.json` adında bir konfigürasyon dosyası oluşturarak çeşitli ayarları özelleştirebilirler. Aşağıda örnek bir konfigürasyon dosyası verilmiştir.

```json
{
  "apiKey": "YOUR_API_KEY",
  "defaultLang": "tr",
  "outputFormat": "text"
}
```

### Çevresel Değişkenler

Ayrıca, çevresel değişkenler kullanarak da ayarları değiştirebilirsiniz. Aşağıdaki değişkenler desteklenmektedir:

- `CHATGPT_API_KEY`: API anahtarı.
- `CHATGPT_DEFAULT_LANG`: Varsayılan dil.
- `CHATGPT_OUTPUT_FORMAT`: Çıktı formatı (ör. "text", "json").

Bu yöntemler, kullanıcıların ihtiyaçlarına göre aracı özelleştirmelerine olanak tanır. Kullanıcılar, projelerinin gereksinimlerine göre bu ayarları kolayca değiştirebilirler.

## Mimari ve Tasarım Kararları

ChatGPT Prompt Engineering Toolkit, modüler bir mimari ile tasarlanmıştır. Bu yaklaşım, kullanıcıların ihtiyaçları doğrultusunda aracı özelleştirmesine olanak tanırken, aynı zamanda gelecekteki geliştirmeler için de sağlam bir temel sağlar. Aşağıda bu mimari yaklaşımın getirdiği bazı avantajlar ve trade-off'lar bulunmaktadır.

### Avantajlar

- **Modülerlik**: Her bir bileşen bağımsız olarak geliştirilebilir ve güncellenebilir. Bu, bakım ve geliştirme süreçlerini kolaylaştırır. Ayrıca, bu modüler yapı, kullanıcıların kendi ihtiyaçlarına uygun özel bileşenler geliştirmelerine olanak tanır.

- **Genişletilebilirlik**: Kullanıcılar, ihtiyaç duydukları yeni özellikleri eklemek için mevcut bileşenleri genişletebilirler. Örneğin, yeni bir düşünce zinciri kalıbı eklemek oldukça basittir ve bu, kullanıcıların daha karmaşık senaryoları yönetmesine yardımcı olur.

- **Performans**: API çağrıları sırasında oluşabilecek hataların etkili bir şekilde yönetilmesi, kullanıcı deneyimini artırır. Örneğin, oran sınırlama hataları için otomatik geri çekilme (exponential backoff) stratejisi uygulanmaktadır. Bu, kullanıcıların daha stabil bir deneyim yaşamasını sağlar.

### Trade-off'lar

- **Karmaşıklık**: Modüler yapı, bazı kullanıcılar için karmaşık bir kurulum süreci anlamına gelebilir. Ancak, bu karmaşıklık genellikle sağlanan esneklik ile telafi edilmektedir. Kullanıcılar, daha fazla özelleştirme seçeneği ile projelerini daha verimli hale getirebilirler.

- **Bağımlılıklar**: Araç, bazı harici kütüphanelere bağımlılık göstermektedir. Bu, kullanıcıların ek kurulumlar yapması gerektiği anlamına gelebilir. Ancak, bu bağımlılıklar genellikle yaygın olarak kullanılan ve güvenilir kütüphanelerdir, bu yüzden kullanıcılar herhangi bir sorun yaşamadan projelerinde bu araçları kullanabilirler.

Bu tasarım kararları, ChatGPT Prompt Engineering Toolkit'in hem kullanıcıların ihtiyaçlarına hem de geliştirme sürecinin gerekliliklerine uygun bir şekilde şekillenmesini sağlamaktadır.

## Performans ve Optimizasyon

ChatGPT Prompt Engineering Toolkit, performans odaklı bir yaklaşım ile tasarlanmıştır. Kullanıcıların elde ettiği sonuçların kalitesini artırmak için çeşitli optimizasyon teknikleri uygulanmaktadır. Bu teknikler, hem sistem kaynaklarının verimli kullanımı hem de kullanıcı deneyimini iyileştirmek için kritik öneme sahiptir.

### Performans İyileştirmeleri

Araç, API çağrıları sırasında oluşabilecek gecikmeleri minimize etmek amacıyla asenkron işlemler kullanmaktadır. Bu, kullanıcıların birden fazla prompt'u aynı anda göndermesine ve sonuçları beklerken diğer işlemlerini sürdürebilmesine olanak tanır. Ayrıca, hata yönetimi mekanizmaları sayesinde, sistem sorunları oluştuğunda kullanıcıların deneyimlerini olumsuz etkilememek için otomatik geri çekilme yöntemleri uygulanmaktadır.

### Optimizasyon Stratejileri

Kullanıcıların sağladığı prompt'ların analizi, araç içinde yer alan otomatik optimizasyon özellikleri ile desteklenmektedir. Bu özellik, kullanıcıların daha önce denediği prompt'ları öğrenir ve benzer durumlar için en iyi yanıtı almak üzere önerilerde bulunur. Ayrıca, kullanıcıların tercihlerini ve alışkanlıklarını anlamak için makine öğrenimi yöntemleri kullanılmaktadır. Bu sayede, kullanıcıların en etkili sonuçları elde etmelerine yardımcı olunmaktadır.

Sonuç olarak, performans ve optimizasyon konusundaki bu yaklaşımlar, kullanıcıların daha verimli çalışmasını sağlar. Bu durum, özellikle yüksek trafikli uygulamalarda ve sistemlerin sürekli güncellenmesi gereken durumlarda büyük bir avantaj sunar.

## Gerçek Dünya Kullanım Senaryoları

ChatGPT Prompt Engineering Toolkit, farklı sektörlerde ve uygulama alanlarında geniş bir kullanım yelpazesine sahiptir. İşte bu aracın gerçek dünya senaryolarında nasıl kullanılabileceğine dair bazı örnekler:

### Eğitim Sektörü

Eğitimde, ChatGPT Prompt Engineering Toolkit, öğrencilere bireysel öğrenme deneyimlerini geliştirmek için kullanılabilir. Öğrenciler, belirli bir konu hakkında detaylı bilgi almak ya da karmaşık bir problemi çözmek için bu aracı kullanarak etkili prompt'lar oluşturabilirler. Örneğin, bir öğrenci "Kuantum fiziği nedir?" gibi bir soruyu sorarak, bu alandaki temel kavramları öğrenebilir. Bu tür bir kullanım, eğitim materyallerinin oluşturulmasında da önemli bir rol oynayabilir.

### İçerik Üretimi

İçerik üreticileri, blog yazıları veya sosyal medya gönderileri oluştururken ChatGPT Prompt Engineering Toolkit'ten yararlanabilirler. Yaratıcı yazma süreçlerinde, kullanıcılar belirli temalar veya konular hakkında ilham almak için bu aracı kullanabilir. Örneğin, bir içerik üreticisi "Yapay zeka ile ilgili en son trendler nelerdir?" şeklinde bir prompt oluşturarak, güncel bilgiler ve öneriler alabilir.

### Müşteri Destek Sistemleri

Müşteri destek ekipleri, sıkça sorulan soruların yanıtlarını hazırlamak için bu aracı kullanabilirler. Müşterilerin sorunlarını daha hızlı bir şekilde çözmek amacıyla, önceden tanımlanmış prompt'lar kullanılarak yanıtlar otomatikleştirilebilir. Örneğin, bir müşteri destek temsilcisi "Üyelik iptal süreci nasıl işler?" sorusuna karşılık olarak, hızlı ve doğru bir yanıt oluşturmak için bu aracı kullanabilir.

Bu kullanım senaryoları, ChatGPT Prompt Engineering Toolkit'in çok yönlülüğünü ve çeşitli alanlarda sağladığı faydaları göstermektedir. Kullanıcılar, bu aracı kendi ihtiyaçlarına göre özelleştirerek daha etkili sonuçlar elde edebilirler.

## SSS ve Sorun Giderme

### 1. Bu aracı nasıl kurabilirim?

Araç, npm, yarn veya pnpm ile kolayca kurulabilir. Kurulum adımları için yukarıdaki "Kurulum" bölümüne bakabilirsiniz.

### 2. Türkçe dil desteği var mı?

Evet, ChatGPT Prompt Engineering Toolkit, Türkçe dil desteği sunmaktadır. Bu, Türkçe konuşan kullanıcıların aracı daha etkin bir şekilde kullanmalarına olanak tanır.

### 3. Hangi ortamda kullanılabilir?

Araç, Node.js ortamında çalışmaktadır. Geliştiriciler, bu aracı kendi projelerinde kolayca entegre edebilirler.

### 4. Hata yönetimi nasıl çalışıyor?

Araç, API çağrıları sırasında oluşabilecek hataları etkili bir şekilde yönetir. Örneğin, oran sınırlama hataları için otomatik geri çekilme (exponential backoff) stratejisi uygular.

### 5. CLI kullanımı nasıl yapılır?

CLI kullanımı, yukarıdaki "CLI Kullanımı" bölümünde detaylı olarak açıklanmıştır. Komutlar ve flag'ler hakkında bilgi bulabilirsiniz.

### 6. Docker ile nasıl kullanabilirim?

Docker ile kullanım için yukarıdaki "Docker ile Kullanım" bölümünde bir Dockerfile örneği verilmiştir. Bu, uygulamaların kolayca dağıtımını sağlar.

### 7. Otomatik optimizasyon nasıl çalışıyor?

Otomatik optimizasyon, kullanıcıların sağladığı temel prompt'ları analiz eder ve en iyi sonuçları elde etmek için optimize eder. Kullanıcıların deneyimlerine göre sürekli gelişir.

### 8. Düşünce zinciri kalıplarını nasıl ekleyebilirim?

Düşünce zinciri kalıplarını eklemek için `addChainStep()` fonksiyonunu kullanarak yeni adımlar ekleyebilirsiniz. Daha fazla bilgi için API Referansı bölümüne göz atabilirsiniz.

### 9. API anahtarımı nasıl alabilirim?

API anahtarınızı, OpenAI'nin resmi web sitesinden kaydolduktan sonra alabilirsiniz. Bu anahtarı `config.json` dosyanıza ekleyerek kullanabilirsiniz.

### 10. Hangi özellikler gelecekte eklenebilir?

Gelecekte eklenebilecek özellikler arasında daha fazla optimizasyon stratejisi, yeni dil desteği ve daha fazla hata yönetimi mekanizması bulunabilir. Kullanıcı geri bildirimleri doğrultusunda yeni özellikler geliştirilecektir.

## Katkıda Bulunma

Bu projeye katkıda bulunmak isterseniz, lütfen GitHub üzerindeki [repo](https://github.com/turkcoode/chatgpt-prompt-engineering) üzerinden katkı yapabilirsiniz. Her türlü öneri ve geri bildirim değerlidir. Açık kaynak topluluğunun bir parçası olmak, hem sizin hem de diğer kullanıcılar için büyük fayda sağlayacaktır.



## 📚 Dokümantasyon

- [Ana Sayfa](docs/Home.md)
- [Kurulum Rehberi](docs/Kurulum.md)
- [API Dokümantasyonu](docs/API-Docs.md)
- [SSS](docs/SSS.md)
- [Örnekler](docs/Örnekler.md)

## Lisans

MIT Lisansı altında lisanslanmıştır.

ChatGPT Prompt Engineering Toolkit, TurkCode tarafından geliştirilmiştir. Daha fazla bilgi için [TurkCode](https://turkcode.net) sayfasını ziyaret edebilirsiniz. Ayrıca, [TurkCode Blog](https://turkcode.net/blog) üzerinden güncel haberleri takip edebilirsiniz. Diğer araçlar hakkında bilgi almak için [Daha fazla araç](https://turkcode.net) sayfasını ziyaret edebilirsiniz.
```