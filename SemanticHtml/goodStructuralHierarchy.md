İyi bir yapısal hiyerarşiye sahip olmak neden önemlidir?

Yapısal bir hiyerarşi oluşturmanın en önemli yönü başlık öğelerinin doğru kullanılmasıdır. Başlık öğeleri h1, h2, h3 ve benzeri şekilde numaralandırılır. Bu numaralar o öğe için başlık düzeyini temsil eder.

Tıpkı bir metin belgesinde olduğu gibi, başlık düzeylerini yanlış sırada kullanmak istemezsiniz. h1 öğeniz en üst düzey başlığınızdır. Bir sayfada nadiren birden fazla bulunur ve genellikle tüm içeriğinizden önce gelmelidir.

h2 öğeniz alt başlığınızdır. Her zaman h1'den sonra gelmelidir ve bazı giriş metinlerinden sonra gelebilir. Bir h1 öğesinin aksine, sayfanızda birden fazla h2 öğesi olabilir. Bunu genellikle içeriğin farklı bölümlerini tanımlamak için yaparsınız.

Kalıbı izleyerek, h3 öğeniz her zaman bir h2 öğesinden sonra gelmelidir. Yani, asla doğrudan h1'den h3'e atlamamalısınız. Bununla birlikte, aynı seviyede birden fazla başlık öğesine sahip olabilirsiniz. Örneğin, bu kod doğrudur:
```
<div>
  <section>
    <h1>freeCodeCamp</h1>
    <h2>Learn Front-End Development</h2>
    <h2>Learn Back-End Development</h2>
  </section>
</div>
```
Ancak bu kod doğru olmayacaktır çünkü h3, h2'den önce gelir:
```
<div>
  <section>
    <h1>freeCodeCamp</h1>
    <h3>Learn Front-End Development</h3>
    <h2>Learn Back-End Development</h2>
  </section>
</div>
```
Stilinden dolayı belirli bir başlık öğesini kullanmak cazip gelebilir, örneğin büyük metin için h1 gibi:
```
<article>
  <p>
    Here is some
    <h1>Large Text</h1>
  </p>
</article>
```
Bunun yerine, belge yapınız için uygun öğeyi seçmeli ve istediğiniz stili elde etmek için CSS kullanmalısınız.

Doğru hiyerarşiyi kullanmak erişilebilirlik açısından önemlidir. Ekran okuyucular gibi yardımcı teknolojiler, bir web sayfasını nasıl ayrıştıracaklarını ve kullanıcıya nasıl duyuracaklarını belirlemek için o web sayfasının yapısına güvenir. Bir h1 öğesinden sonra bir h3 öğesi kullanmak, ekran okuyucu kullanıcısının h2 öğesinin olmaması nedeniyle yanlışlıkla önemli içeriğin üzerinden atladığını düşünmesine neden olabilir.

Doğru yapı SEO için de önemlidir. Arama motorları, web sayfanızın içeriğini ayrıştırmak ve sonuçlarda ne zaman ve nerede görünmesi gerektiğini belirlemek için otomasyonu kullanır. Yapınız hatalıysa, arama motorları sizi ilgili arama sonuçlarında çok iyi sıralayamayabilir.

Son olarak, yapınızın ne kadar hatalı olduğuna bağlı olarak, HTML'niz teknik olarak geçerli bile olmayabilir. Bu durumda, web tarayıcısı ne yapmak istediğinizi etkili bir şekilde tahmin etmek zorunda kalır. Ve tahmin ettiği şey sizin istediğiniz şey bile olmayabilir.

Bugün öğrendiğiniz gibi, sayfanız için uygun yapısal hiyerarşiyi kullanmak için birçok neden vardır. Yeni projeler oluştururken bunu aklınızda tutun.

