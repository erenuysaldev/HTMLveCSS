HTML'de Blok ve Satır İçi Alıntılar Nasıl Çalışır?
HTML'de alıntı öğeleri, alıntılanan metni çevresindeki içerikten ayırmak için kullanılır. Bu, alıntının kolayca fark edilebilmesini sağlar.

Blok Alıntı
Başka bir kaynaktan yapılan uzun alıntılar için blok alıntı (block quote) öğesi kullanılmalıdır. Bu öğe, özellikle uzun metinlerde tercih edilir. Eğer alıntının kaynağının bir adresi (URL) varsa, bunu cite niteliği ile belirtebilirsiniz. Bu niteliğin değeri geçerli bir URL olmalıdır.

Aşağıda bir blok alıntı örneği görebilirsiniz:
```
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
  "Başarılı bir geliştirici olduğunuzu hayal edebiliyor musunuz? İnsanların güvendiği yazılım sistemlerini inşa ettiğinizi?"
</blockquote>
```
Bu öğede bir cite niteliği vardır. Niteliğin değeri, alıntının kaynağının URL’sidir. Bu nitelik tarayıcıda görsel olarak bir değişiklik yapmaz; fakat ekran okuyucular ve arama motorları için faydalıdır. Tarayıcıda bu metin hafifçe girintili (indent) olarak görünür.

Alıntının başında ve sonunda tırnak işareti görünmesini istiyorsanız, bunları doğrudan metnin içine kendiniz yazmalısınız.

Eğer alıntı birden fazla paragraftan oluşuyorsa, her paragrafı ```<p> etiketine sararak aynı <blockquote>``` öğesi içinde tutabilirsiniz. Aşağıda dört paragraf içeren bir örnek vardır:
```
<div>
  <blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    Başarılı bir geliştirici olduğunuzu hayal edebiliyor musunuz? İnsanların güvendiği yazılım sistemlerini inşa ettiğinizi?
  </blockquote>
  <p>—Quincy Larson, <cite>How to Learn to Code and Get a Developer Job [Full Book]</cite></p>
</div>
```
Bu örnekte, blok alıntı belirli bir metni içerir. Altında ise bir paragraf ile yazar adı ve eserin başlığı görsel olarak belirtilmiştir.

Tarayıcıda bu kaynak kullanıcıya net şekilde gösterilir. Alıntının Quincy Larson tarafından yazılmış bir kitaptan alındığını anlayabiliriz. Kitabın adı ise How to Learn to Code and Get a Developer Job'dur.

Satır İçi (Inline) Alıntı
Uzun alıntılar için blok alıntılar kullanılır. Ancak bazı durumlarda, sadece birkaç kelimelik kısa alıntılar yapmanız gerekebilir.

Bu gibi durumlar için satır içi alıntı (inline quote) öğesi olan <q> kullanılır. Bu öğe, kısa alıntılar için mevcut paragrafın içinde kullanılır. Çoğu modern tarayıcı, bu öğeyi kullandığınızda alıntının etrafına otomatik olarak tırnak işaretleri ekler.
```
<p>
  Quincy Larson şöyle demişti:
  <q cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    Momentum her şeydir.
  </q>
</p>
```
Bu örnekte bir paragrafın içinde bir alıntı yapılmıştır. Alıntı <q> etiketi ile sarılmıştır ve kaynak yine cite niteliği ile belirtilmiştir. Tarayıcıda bu metin, tırnak işaretiyle birlikte görünür ve paragrafa dahil edilir.

Özet: Blok Alıntı vs Satır İçi Alıntı
Blok alıntı (<blockquote>): Uzun ve ayrı durması gereken alıntılar için kullanılır.

Satır içi alıntı (<q>): Paragraf içinde kısa alıntılar için kullanılır.
