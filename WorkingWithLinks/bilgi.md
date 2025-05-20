<!-- filepath: c:\Users\Eren\Desktop\html\WorkingWithLinks\bilgi.md -->
Farklı hedef (target) öznitelik türleri nelerdir ve nasıl çalışırlar?

Bağlantı etiketlerinde (anchor elements) veya linklerde hedef (target) özniteliğini görmüş olabilirsiniz. Bu önemli öznitelik, tarayıcıya bağlantı etiketinin URL'sini nerede açacağını söyler:

<a href="https://freecodecamp.org" target="_blank">freeCodeCamp'i Ziyaret Et</a>

Bu öznitelik için dört önemli olası değer vardır. Her değerin bir alt çizgi ile başladığını unutmayın.

İlk değer, varsayılan değer olan _self'tir. Bu, bağlantıyı geçerli göz atma bağlamında açar. Çoğu durumda, bu geçerli sekme veya pencere olacaktır.

İkinci değer, bağlantıyı yeni bir göz atma bağlamında açan _blank'tir. Tipik olarak, bu yeni bir sekmede açılır. Ancak bazı kullanıcılar tarayıcılarını bunun yerine yeni bir pencere açacak şekilde yapılandırabilir.

Üçüncü değer, bağlantıyı geçerli bağlamın üst öğesinde açan _parent'tır. Örneğin, web sitenizde bir iframe varsa, o iframe'deki bir _parent değeri, gömülü çerçevede değil, web sitenizin sekmesinde/penceresinde açılır.

Dördüncü değer, bağlantıyı en üstteki göz atma bağlamında açan _top'tur - "üst öğenin üst öğesi" gibi düşünün. Bu, _parent'a benzer, ancak bağlantı, iç içe gömülü çerçeveler için bile her zaman tam tarayıcı sekmesinde/penceresinde açılır.

Şu anda deneysel FencedFrame API'si için kullanılan _unfencedTop adlı beşinci bir değer vardır. Bu videonun çekildiği sırada, muhtemelen henüz bunu kullanmak için bir nedeniniz olmayacaktır.

Kullanıcılarınızın nereye gideceğini kontrol etmek için doğru hedef değerini seçmek, bir web sitesi oluştururken önemli bir husustur.

