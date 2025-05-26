Farklı form durumları nelerdir ve neden önemlidirler?

HTML'de form kontrolleri, girişler gibi, odaklanmış durum, salt okunur durum veya devre dışı durum gibi farklı aşamalarda veya koşullarda olabilir.

İlk durum varsayılan durum olarak kabul edilir. Bir e-posta adresi girdisinin varsayılan durumu boş bir girdidir. E-posta girişi sayfada ilk kez oluşturulduğunda böyle görünür. Bu noktada, kullanıcı herhangi bir bilgi girmemiştir.

Kullanıcı bir form kontrolünü tıkladığında veya klavyenin sekme tuşuyla seçtiğinde, bu kontrol odaklanmış durumda demektir. Bir girdi odaklanmış durumdayken, çoğu tarayıcı girdinin etrafında mavi vurgulu bir kenarlık gösterecektir. Ancak CSS'de ek stiller eklemeyi seçebilirsiniz.

Bir başka form durumu da devre dışı durumudur. Bu durum, kullanıcılara bir girdinin odaklanamadığını veya etkinleştirilemediğini gösterir. Bir girdiyi devre dışı bırakmak için elemana şu şekilde disabled boolean niteliğini ekleyebilirsiniz:
```
<input disabled type="email" name="email" id="email" />
```
Kullanıcı girişe tıklamaya çalışırsa odak etkinleştirilmez. Odaklanmış duruma benzer şekilde, CSS kullanarak devre dışı bırakılmış durum için ek stiller eklemeyi seçebilirsiniz.

Başka bir form durumu türü de salt okunur durumudur. Bu, girdi gibi bir form denetiminin kullanıcı tarafından düzenlenemediği durumdur. İşte bir e-posta girdisini salt okunur olarak ayarlamanın bir örneği:
```
<input
  readonly
  type="email"
  name="email"
  id="email"
  value="example@email.com"
/>
```
Değer niteliği, giriş alanının içinde gösterilen değeri ayarlamak için kullanılır. Girdiye tıklamaya çalışırsanız, mevcut değeri düzenleyemezsiniz.

Devre dışı bırakılmış durum ile salt okunur durum arasındaki temel fark, salt okunur duruma odaklanılabilirken devre dışı bırakılmış duruma odaklanılamamasıdır.

Farklı form durumlarını anlamak önemlidir çünkü hataları ele alırken net geri bildirim ve rehberlik sağlayarak sorunsuz bir kullanıcı deneyimi sunarlar.