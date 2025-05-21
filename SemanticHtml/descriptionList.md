
Açıklama listeleri nedir ve ne zaman kullanmalısınız?

Açıklama listeleri, terimleri ve tanımları düzenli ve okunması kolay bir biçimde sunmak için mükemmeldir; tıpkı bir sözlükte veya gerçek bir sözlükte olduğu gibi, kelimeleri karşılık gelen tanımlarıyla birlikte bulabilirsiniz.

Bu, HTML'de iki terim ve bunlara karşılık gelen ayrıntıları içeren bir açıklama listesi örneğidir:
```
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```
Bu durumda terimler HTML ve CSS kısaltmaları, ayrıntılar ise bunların açılımlarıdır. Ayrıntılar tanımlar veya terimlerle ilgili diğer bilgiler de olabilir.

Bir açıklama listesi tanımlamak için üç HTML öğesine ihtiyacınız olacaktır. Birincisi, tüm liste için kapsayıcı olan açıklama listesi öğesi, dl. Örnekte açıklama listesinin diğer tüm öğelerinin etrafını sardığını görebilirsiniz.

Ardından, her bir terim için bir açıklama terimi elemanı, dt. Bu durumda açıklama listesinin HTML ve CSS olmak üzere iki terimi vardır, dolayısıyla bu öğelerden iki tane vardır.

Ve son olarak, her terimden sonra, o terimle ilişkili açıklama veya ayrıntılar için bir açıklama ayrıntıları öğesi, dd, bulacaksınız. Bu örnekte bunlar Hypertext Markup Language ve Cascading Style Sheets'tir.

Tarayıcıda, her terimin ardından ilgili açıklamayı görürsünüz. Varsayılan olarak, açıklamalar görsel olarak ayırt edilebilmeleri için sağa doğru biraz daha girintilidir.

Ancak açıklama listeleri yalnızca terimler ve tanımlarla sınırlı değildir. Bundan çok daha çok yönlüdürler. Burada iki malzemeli bir tarifimiz var.
```
<dl>
  <dt>Flour</dt>
  <dd>2 cups</dd>
  <dt>Sugar</dt>
  <dd>1/2 cup</dd>
</dl>
```
Tüm açıklama listesi bir açıklama listesi öğesi içindedir. İlk bileşen olan Un, bir açıklama terimi öğesi içindedir. Ardından, bu malzemeden ne kadarına ihtiyacınız olacağını görebilirsiniz: 2 bardak. Bu, ilgili malzemelerden hemen sonra bir açıklama ayrıntıları öğesi içinde yer alır.

Ve aynı yapı Şeker için de tekrarlanır. Bu durumda tarifte yalnızca iki malzeme vardır, ancak daha fazla malzeme olsaydı aynı yapı açıklama listesi boyunca tekrarlanabilirdi.

Tarayıcıda, malzemeleri sola hizalanmış ve ölçümleri görsel olarak ayırmak için girintili olarak görürsünüz.

Açıklama listeleri için diğer kullanım alanları arasında ürün özellikleri, sıkça sorulan sorular, iletişim bilgileri ve meta veriler yer alır. Esasen, anahtar-değer çifti biçiminde, birinin etiket, yani anahtar, diğerinin ise ek ilgili bilgi, yani değer olarak işlev gördüğü iki ilgili bilgi parçasına sahip olduğunuzda bir açıklama listesi kullanabilirsiniz.
## FreeCodeCamp
