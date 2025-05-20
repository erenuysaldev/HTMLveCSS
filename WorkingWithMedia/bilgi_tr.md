Değiştirilmiş öğe, içeriği CSS'in kendisi yerine harici bir kaynak tarafından belirlenen bir öğedir. CSS veya basamaklı stil sayfaları, bir web sayfasına stil eklemek için kullanılır. Değiştirilmiş öğelerin yaygın örnekleri arasında resim, iframe ve video öğeleri bulunur.

Değiştirilmiş öğelerle, bir öğenin konumunu veya düzenini kontrol edebilirsiniz. Ancak CSS'iniz o öğenin içeriğini doğrudan değiştiremez. Bunu bazı örneklerle açıklamak daha kolay olabilir. Web sayfanıza bir resim yerleştiren resim öğesini düşünün:

```html
<img src="ornek-resim-url" alt="Açıklayıcı metin buraya gelir">
```
Öğenin kendisi harici nesneyle değiştirilir: resim. CSS'iniz resmin konumu gibi şeyleri kontrol edebilir veya ona bir filtre uygulayabilir, ancak resmin kendisini değiştiremezsiniz. Daha sağlam bir örnek, web sayfanıza harici bir site yerleştiren iframe öğesi olabilir:

```html
<iframe src="https://www.example.com" title="Örnek Site"></iframe>
```
iframe öğesini kullanmanın yaygın örnekleri, Haritalar veya YouTube videolarını sayfaya yerleştirmek olabilir. Öğenin kendisi harici nesneyle değiştirilir: site. CSS'iniz yerleştirilmiş sitenin konumunu değiştirebilir, ancak sitenin içeriğini değiştiremezsiniz. Biraz daha derine inecek olursak, yerleştirilmiş sitenin bir h1 öğesi varsa, CSS'iniz o h1 öğesini biçimlendiremez. Boyutunu, yazı tipi rengini vb. değiştiremezsiniz.

Video ve embed gibi başka değiştirilmiş öğeler de vardır. Ve bazı öğeler belirli durumlarda değiştirilmiş öğeler gibi davranır. İşte type özelliği image olarak ayarlanmış bir input öğesi örneği:

```html
<input type="image" alt="Açıklayıcı metin buraya gelir" src="ornek-resim-url">
```
Bu tür bir giriş, değiştirilmiş bir öğe olarak kabul edilir, ancak metin veya e-posta gibi diğer giriş türleri değiştirilmiş öğeler değildir.

## freecodecamp