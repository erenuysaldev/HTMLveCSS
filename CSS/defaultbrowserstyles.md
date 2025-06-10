HTML'ye uygulanan bazı varsayılan tarayıcı stilleri nelerdir?

HTML ve CSS ile çalışmaya başladığınızda, herhangi bir CSS yazmadan önce bile bazı stillerin web sayfalarınıza uygulandığını fark edeceksiniz. Bu stillere "varsayılan tarayıcı stilleri" veya "kullanıcı aracısı stilleri" denir.

Bu varsayılan tarayıcı stilleri, HTML öğelerinin tüm tarayıcılarda okunabilir bir şekilde görüntülenmesini sağlamak için temel biçimlendirme sağlar.

Ancak, bu stiller bir tarayıcıdan diğerine biraz farklılık gösterebilir, bu nedenle web siteniz için tutarlı bir görünüm tasarlarken bunları anlamak önemlidir.

Çeşitli HTML öğelerine uygulanan bazı yaygın varsayılan tarayıcı stillerine bir göz atalım.

Başlıklar en yaygın kullanılan HTML öğelerinden biridir ve varsayılan olarak farklı boyutlara ve ağırlıklara sahip olacak şekilde biçimlendirilir.

Örneğin, h1 (en üst düzey başlık) genellikle kalın ve h2, h3 vb. gibi daha düşük düzey başlıklara kıyasla daha büyük yazı tipi boyutundadır.

Bu başlık etiketleri içeriğinizin hiyerarşisini ve yapısını tanımlamaya yardımcı olur.

Aşağıdaki örnek h1'den h6'ya kadar olan altı başlık öğesinin tamamını göstermektedir.
```
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```
Varsayılan stillere sahip bir diğer öğe, genellikle içerik bölümlerini görsel olarak ayırmak için kullanılan yatay bir kural oluşturan hr öğesidir. Tarayıcılar genellikle bu öğeye basit bir çizgi stili uygular.

Daha iyi anlamak için şu kod örneğine bakalım:
```
<p>Paragraph 1</p>
<p>Paragraph 2</p>
<hr>
<p>Paragraph 3</p>
<p>Paragraph 4</p>
```
Yatay kural, içerik bölümlerini ayırt etmek için metnin üstünde ve altında boşluk bulunan ince bir çizgi olarak görünür.

Şimdi, alıntı bloğu öğesine bakacağız.

Alıntı blokları, başka bir kaynaktan alıntı olan bir metin bölümünü belirtmek için kullanılır. Tarayıcılar genellikle girinti ekler ve bazen metni italik yapar.

Girinti, alıntı bloğunu metnin geri kalanından ayırmaya yardımcı olur ve bu içeriğin başka bir kaynaktan alıntılandığını açıkça belirtir.

Şu kod örneğine bir göz atalım:
```
<p>Paragraph 1</p>
<p>Paragraph 2</p>
<blockquote>I think, therefore I am. (Rene Descartes)</blockquote>
<p>Paragraph 3</p>
<p>Paragraph 4</p>
```
