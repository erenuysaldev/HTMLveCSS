Farklı düğme türleri nelerdir ve bunları ne zaman kullanmalısınız?

Düğme öğesi, etkinleştirildiğinde belirli bir eylemi gerçekleştirmek için kullanılır. Burada, düğme metni Start Game olan bir düğme öğesi örneği verilmiştir.
```
<button>Start Game</button>
```
Düğme öğesinin diğer kullanım örnekleri arasında bir formun gönderilmesi, bir modalın gösterilmesi veya bir yan menünün açılıp kapatılması yer alır. Düğme öğesi, etkinleştirildiğinde düğmenin davranışını kontrol eden bir type niteliğine sahiptir. type niteliği için ilk olası değer düğme türü olacaktır. Aşağıda, düğme öğesinin düğme türü ve Show Alert metni ile kullanımına bir örnek verilmiştir:
```
<button type="button">Show Alert</button>
```
Varsayılan olarak, düğme etkinleştirildiğinde hiçbir şey yapmayacaktır. Ancak, bu durumda bir uyarı göstermek gibi düğmeyi etkileşimli hale getirmek için bazı JavaScript kodları ekleyebilirsiniz. type niteliği için bir başka olası değer de submit değeridir. İşte submit türüne sahip bir düğme öğesinin kullanımına ilişkin bir örnek:
```
<form action="">
  <label for="email">Email address:</label>
  <input type="email" id="email" name="email" />
  <button type="submit">Submit form</button>
</form>
```
Bu form öğesinin içinde, kullanıcının e-posta adresi için bir etiket ve giriş öğesi vardır. Kullanıcı gönder düğmesine tıkladığında, verileri sunucuya gönderilecek ve işlenecektir. type niteliği için üçüncü olası değer sıfırlama değeridir. İşte sıfırlama ve gönderme düğmeleri içeren bir form öğesi örneği:
```
<form action="">
  <label for="email">Email address:</label>
  <input type="email" id="email" name="email" />
  <button type="reset">Reset form</button>
  <button type="submit">Submit form</button>
</form>
```
Bu değiştirilmiş örnekte, kullanıcının e-posta adresini toplamak için bir etiket ve giriş öğesi kullanılır. Kullanıcı sıfırlama düğmesine tıkladığında, tüm giriş verileri silinecektir. Sıfırlama düğmelerinin genellikle en iyi fikir olmadığına dikkat etmek önemlidir çünkü kullanıcıların verilerini yanlışlıkla sıfırlamasına neden olabilirler. Ayrıca, formunuzdaki birden fazla düğme kullanıcı arayüzünü karmaşıklaştırabilir.

HTML'de düğme oluşturmanın bir başka yolu da input öğesini kullanmaktır. Input öğesi ayrıca submit, reset ve button gibi olası değerleri olan bir type niteliğine sahiptir. Burada, türü düğme olarak ayarlanmış girdi öğesinin kullanımına bir örnek verilmiştir:
```
<input type="button" value="Show Alert" />
```
Düğme metnini göstermek için value niteliği kullanılır. Peki, input ve button öğelerini kullanmak arasındaki fark nedir? input öğeleri void öğelerdir, yani metin gibi alt düğümlere sahip olamazlar ve yalnızca bir başlangıç etiketine sahip olabilirler. Öte yandan, düğme öğesi daha fazla esneklik sunar çünkü içine metin, resim ve simge yerleştirebilirsiniz.