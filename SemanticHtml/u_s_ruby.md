
u, s ve ruby öğeleri ne için kullanılır ve nasıl çalışır?

Açıklamasız ek açıklama öğesi veya kısaca u öğesi, metin dışı ek açıklama uygulanmış satır içi metni temsil etmek için kullanılır.

Burada, çeşitli yazım hatalarını vurgulamak için u öğesinin kullanımına bir örnek verilmiştir:
```
<p>
  You can use the unarticulated annotation element to highlight
  <u>inccccort</u> <u>spling</u> <u>issses</u>.
</p>
```
Örnekte, ```incorrect```, ```spelling``` ve ```issues``` kelimeleri yanlış yazılmıştır. u öğesi için varsayılan stil, metnin altında siyah bir alt çizgidir.

HTML4'te u öğesi biçimlendirme amacıyla kullanılırdı. Ancak HTML5'te, u öğesi yalnızca metne metin dışı ek açıklama uygulandığını belirtmek için kullanılmalıdır.

Bir metin parçasını alt çizgi ile biçimlendirmek istiyorsanız, HTML yerine CSS kullanmalısınız.

Üstü çizili öğe veya kısaca s öğesi, metnin artık doğru veya alakalı olmadığını göstermek için kullanılmalıdır. İşte bir etkinliğin iptal edildiğini göstermek için s öğesinin kullanımına bir örnek:
```
<p><s>Tomorrow's hike will be meeting at noon.</s></p>

<p>Due to unforeseen weather conditions, the hike has been cancelled.</p>
```
Bu örnekte, ilk cümlenin üzeri çizilmiştir çünkü yürüyüş hava koşulları nedeniyle iptal edilmiştir.

s öğesi asla sadece bir belgedeki değişiklikleri göstermek için kullanılmamalıdır. Bu durumda daha uygun öğeler silinen metin öğesi ve eklenen metin öğesi olacaktır.

Ruby öğesi, ana metnin üstünde veya altında gösterilen küçük metni temsil eder. Genellikle Doğu Asya karakterlerinin telaffuzunu göstermek için kullanılır. İşte MDN web dokümanları sayfasından ruby öğesi örneği:
```
<ruby> 明日 <rp>(</rp><rt>Ashita</rt><rp>)</rp> </ruby>
```
rp öğesi veya ruby fallback parantez öğesi, ruby ek açıklamalarını görüntüleme desteği olmayan tarayıcılar için bir yedek olarak kullanılır.

rt öğesi veya ruby metin öğesi, ruby ek açıklamasının metnini belirtmek için kullanılır. Bu metin genellikle Doğu Asya tipografisinde telaffuz veya çeviri ayrıntıları için kullanılır.

Ruby öğesi diğer ek açıklama türleri için kullanılabilse de, en yaygın kullanım alanı Doğu Asya tipografisidir.