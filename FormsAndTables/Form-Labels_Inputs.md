HTML'de formlar, etiketler ve girişler nasıl çalışır?

HTML'deki form öğesi, adlar ve e-posta adresleri gibi kullanıcı bilgilerini toplamak için kullanılır. İşte bir form öğesi örneği:
```
<form action="url-goes-here">
  <!-- input elements go here -->
</form>
```
Action niteliği, form verilerinin gönderildikten sonra nereye gönderileceğini belirtir. Adlar ve e-posta adresleri gibi belirli bilgileri toplamak için input öğesini kullanırsınız. İşte bir girdi öğesi kullanma örneği:
```
<form action="">
  <input type="text" />
</form>
```
input elemanları void elemanlardır ve kapanış etiketleri yoktur. type niteliği kullanıcıdan beklenen veri türünü tanımlar. Bu durumda, veri düz metin olacaktır. Girdiye bir etiket eklemek için bir label öğesi kullanırsınız. Burada, Ad Soyad: metnini içeren bir etiket öğesi kullanımına örnek verilmiştir:
```
<form action="">
  <label>
    Full Name:
    <input type="text" />
  </label>
</form>
```
Bir girdiyi bir etiket öğesinin içine yerleştirerek, etiket ile girdi alanı arasında örtük bir ilişki oluşturursunuz. "Örtük" terimi, açıkça belirtilmesine veya ek nitelikler ya da öğelerle tanımlanmasına gerek kalmadan anlaşılan veya çıkarılan bir şeyi ifade eder. Bir etiketi bir girdiyle açıkça ilişkilendirmek için for niteliğini kullanabilirsiniz. İşte bir e-posta adresi etiketi için for niteliğinin kullanımına ilişkin bir örnek:
```
<form action="">
  <label for="email"> Email Address: </label>
  <input type="email" id="email" />
</form>
```
Açık bir ilişkilendirme kullanıldığında, for niteliği ve id değerlerinin aynı olması gerekir. Bu durumda, değerlerin her ikisi de email olarak ayarlanır. Girdideki e-posta türü, doğru biçimlendirilmiş e-posta adresleri için temel doğrulama sağlar. Kullanıcılara beklenen girdi hakkında ek ipuçları göstermek istiyorsanız, yer tutucu niteliğini kullanabilirsiniz. İşte e-posta girdisi içinde yer tutucu niteliğini kullanan bir örnek:
```
<form action="">
  <label for="email"> Email Address: </label>
  <input type="email" id="email" placeholder="Ex. example@email.com" />
</form>
```