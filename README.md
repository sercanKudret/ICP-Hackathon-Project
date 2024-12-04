# LagaLuga

Bu proje, İngilizce kelimeleri ve Türkçe karşılıklarını kaydederek kendinizi test edebileceğiniz bir sistemdir.

---

### Nasıl Çalışır?

1. İngilizce ve Türkçe kelimeler eklenir.
2. Rastgele bir İngilizce kelime seçilir.
3. Kullanıcı, kelimenin Türkçe karşılığını tahmin eder ve doğruluğunu kontrol eder.

---

### Kullanılabilir Fonksiyonlar

- **AddWord(x, y)**  
  İngilizce (`x`) ve Türkçe (`y`) kelimeyi listeye ekler.
  
- **Question()**  
  Rastgele bir İngilizce kelime döner.
  
- **YourAnswer(answer)**  
  Verilen cevabın doğru olup olmadığını kontrol eder.

---

### Örnek Kullanım

```motoko
// 1. Kelime ekleyin
await LagaLuga.AddWord("apple", "elma");

// 2. Soru sorun
let question = await LagaLuga.Question();
// Örneğin: "apple"

// 3. Cevabınızı kontrol edin
let result = await LagaLuga.YourAnswer("elma");
// true (Doğru) veya false (Yanlış)
