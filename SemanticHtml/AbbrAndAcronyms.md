HTML'de Kısaltmalar ve Akronimler Nasıl Gösterilir?
Kısaltma, bir kelimenin kısaltılmış hali anlamına gelir. Örneğin, "Dr." kelimesi, "Doctor" (doktor) kelimesinin kısaltmasıdır.

Akronim ise, bir ifadenin kelimelerinin baş harflerinden oluşan bir kelimedir. Örneğin, HTML bir akronimdir. Bu, HyperText Markup Language (Hipermetin İşaretleme Dili) ifadesinin baş harflerinden oluşur.

Her kelimenin ilk harflerini alarak (H, T, M, L) HTML akronimini elde ederiz. Kısaltmalar ve akronimler, özellikle bağlamda iyi biliniyor ve kolay anlaşılıyorsa, daha kısa ve öz metinler yazmak için çok faydalıdır.

HTML'de kısaltmaları ve akronimleri göstermek için <abbr> (abbreviation) etiketi tam aradığınız şeydir. Kısaltmaları veya akronimleri ilk kullandığınızda, bunların tam anlamını mutlaka açıklamalısınız. Sonrasında ise <abbr> etiketiyle onları vurgulayabilir ve daha fazla bilgi sağlayabilirsiniz.

Aşağıda, içinde "HTML web’in temelidir." cümlesi bulunan bir paragraf örneği var:
```
<p><abbr>HTML</abbr> web’in temelidir.</p>
```
Bu örnekte HTML akronimi  ```<abbr>``` etiketi içine alınmıştır. Tarayıcıda bu metin normal metin gibi görünür, yani görünürde bir değişiklik olmaz. ```<abbr>``` etiketi arka planda kullanıcıya ve teknolojiye yardımcı olacak ek bağlam sağlar.

Eğer kullanıcıların bu akronimin ne anlama geldiğini anlamalarına yardımcı olmak isterseniz, tam anlamını title niteliğiyle gösterebilirsiniz.

title niteliği opsiyoneldir, ancak eklerseniz, bu niteliğin değeri kısaltmanın veya akronimin insan tarafından okunabilir tam açıklaması olmalıdır.

Yukarıdaki örneği alalım ve title niteliğini ekleyelim. Böylece tam hali "HyperText Markup Language" olur:
```
<p><abbr title="HyperText Markup Language">HTML</abbr> web’in temelidir.</p>
```
Genellikle title niteliği eklenince ```<abbr>``` etiketinin görünümü değişir. Bu değişiklik tarayıcıya bağlıdır. Bazı tarayıcılar altını noktalı çizgiyle çizer, bazıları içeriği küçük büyük harf (small caps) olarak gösterebilir ya da farklı varsayılan stiller uygulayabilir. Kullanıcı fareyi bu kısaltmanın üzerine getirdiğinde, tam hali araç ipucu (tooltip) olarak görünür.

Her kısaltma ya da akronim için mutlaka ```<abbr>``` kullanmak zorunda değilsiniz, ancak anlamı belirsiz veya ek bağlam gerektirenler için kullanmanız önerilir.

Metnin gereksiz kalabalık olmaması ve aynı zamanda açık ve öz olması için dengeyi iyi kurmanız gerekir.
