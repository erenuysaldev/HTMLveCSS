HTML formlarında istemci tarafı form doğrulaması nedir ve bazı örnekler nelerdir?

Bir kullanıcı web sitenizde bir form doldurduğunda, gerekli tüm bilgileri doğru biçimde doldurması önemlidir. HTML form kontrolleri, girişler gibi, geçersiz verileri kontrol etmek için kullanabileceğiniz birçok yerleşik doğrulamaya sahiptir. Bu, bilgiler gönderilmeden ve sunucu tarafından işlenmeden önce kullanıcının bu hataları düzeltmesini sağlamaya yardımcı olacaktır.

"İstemci tarafı" terimi, bir web sitesinin veya uygulamanın doğrudan etkileşimde bulunduğunuz kısmı gibi, kullanıcının bilgisayarında veya cihazında gerçekleşen her şeyi ifade eder. Buna düzen, tasarım ve tüm etkileşimli özellikler dahildir.

"Sunucu tarafı" terimi, web sitesini veya uygulamayı barındıran sunucuda, bilgisayarda veya sistemde gerçekleşen her şeyi ifade eder. Bu, verilerin işlenmesini, uygulamaların çalıştırılmasını ve kullanıcının cihazından gelen isteklerin ele alınmasını içerir.

İstemci tarafı doğrulama önemli olsa da, daha fazla güvenlik için sunucu tarafı doğrulamaya da ihtiyacınız vardır. Kötü niyetli kullanıcılar istemci tarafı kontrollerini atlayabilir, bu nedenle sağlam sunucu tarafı önlemleri çok önemlidir. Daha sonraki bir modülde bu konuda daha fazla bilgi edineceksiniz. Şimdilik, bazı istemci tarafı form doğrulama örneklerine bir göz atalım.

Yerleşik form doğrulamanın yaygın bir örneği, girdilerde required niteliğini kullanmaktır. required niteliği, kullanıcının gönderilmeden önce formun o bölümünü doldurması gerektiğini belirtir. İşte bir e-posta girdisinde required niteliğinin kullanımına bir örnek
```
<form action="">
  <label for="email">Email Address (Required field):</label>
  <input required type="email" name="email" id="email" />
  <button type="submit">Submit Form</button>
</form>
```
Kullanıcı bir e-posta adresi girmeden Formu Gönder düğmesine tıkladığında, alanın gerekli olduğu ve formun gönderilmeyeceği konusunda uyarılacaktır. Her tarayıcı bu uyarı mesajını göstermek için kendi stil setine sahip olacaktır. E-posta girdisini kullanmanın bir diğer avantajı, e-posta girdilerinin doğru biçimlendirilmiş e-posta adreslerini sağlamak için bazı temel doğrulamalara sahip olmasıdır. Tarayıcıların yalnızca standart e-posta adresleri için temel doğrulamayı kontrol ettiğini unutmamak önemlidir. Daha sonraki modüllerde öğreneceğiniz ek doğrulama katmanları eklemek size bağlıdır.

E-posta girdileri için diğer doğrulama biçimleri minlength ve maxlength niteliklerini kullanmaktır. İşte ekstra doğrulamayı kullanan bir örnek:
```
<form action="">
  <label for="email">Email Address (Required field):</label>
  <input
    required
    type="email"
    name="email"
    id="email"
    minlength="4"
    maxlength="64"
  />
  <button type="submit">Submit Form</button>
</form>
```
minlength ve maxlength nitelikleri, e-posta girişi için karakter cinsinden minimum ve maksimum uzunluğu ayarlamak için kullanılır. Minimum uzunluğu dahil etmezseniz veya maksimum karakter uzunluğunu aşarsanız, tarayıcı bir uyarı mesajı gösterecektir.