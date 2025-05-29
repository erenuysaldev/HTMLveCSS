
``aria-hidden`` özniteliği nedir ve nasıl çalışır?

İçeriği görüntülerken aynı zamanda ekran okuyucular gibi yardımcı teknoloji kullanan kişilerden gizlemeniz gerekiyorsa, ``aria-hidden`` niteliğini kullanabilirsiniz.

Bunu gizlemek istediğiniz HTML öğesine eklemeniz ve değerini true olarak ayarlamanız yeterlidir, burada gördüğünüz gibi: ``aria-hidden="true"``.
Bu nitelik, öğeyi ve tüm alt öğelerini sayfada görünür tutarken erişilebilirlik ağacından gizler. Yaygın kullanım durumları şunları içerir:

Yalnızca dekoratif bir amacı olan simgeler ve resimler.
Çoğaltılmış içerik.
``aria-hidden`` özelliğinin içeriği yalnızca ekran okuyucular gibi yardımcı teknolojilerden gizlediğini unutmamak önemlidir. İçeriğin herkesten gizlenmesi gerekiyorsa, gizlemek için ``aria-hidden`` kullanmamalısınız. Örneğin, şu anda daraltılmış olan bir hamburger menü sadece ekran okuyucu kullanıcılarından değil, tüm klavye kullanıcılarından gizlenmelidir. Bu durumda, menü daraltıldığında DOM'dan kaldırmak için CSS görüntüleme özelliğini none olarak ayarlayabilirsiniz.
Klavye ile odaklanılabilen bir öğeyi gizlemek için asla aria-hidden kullanmamalısınız. ``aria-hidden`` niteliği yalnızca öğeyi erişilebilirlik ağacından kaldırır. DOM'dan kaldırmaz. Bu nedenle, ekran okuyucu kullanıcılarının öğeye sekmeleri mümkün olmaya devam edecektir, ancak ekran okuyucuları öğeyi duyurmayacak ve etkili bir şekilde "hiçbir şeye" odaklanmalarına neden olacaktır.

Burada, true değerine sahip`` aria-hidden`` niteliğini ekleyerek bir simgeyi erişilebilirlik ağacından gizlediğimiz bir örnek yer almaktadır.

Aynı amaç için hem bir simgeye hem de metne sahip olmanın gereksizliğinden kaynaklanabilecek herhangi bir karışıklığı önlemek için metni yalnızca yardımcı teknolojilere açık tutuyoruz.
```
<button>
  <i class="fa-solid fa-gear" aria-hidden="true"></i>
  <span class="label">Settings</span>
</button>
```
Şu durumlarda aria-hidden kullanmanıza gerek yoktur:

HTML öğesi zaten bir hidden niteliğine sahiptir.
Eleman veya elemanın atası zaten display: none ile gizlenmiştir.
Eleman veya elemanın atası zaten visibility: hidden ile gizlenmiştir.
Bu üç durumda, öğe zaten DOM'dan kaldırılmıştır ve dolayısıyla erişilebilirlik ağacından gizlenmiştir, bu nedenle aria-hidden niteliği gerekli değildir.
Tüm ARIA niteliklerini kullanırken olduğu gibi, bu gizli öğelerle bile kolay anlaşılır olduğundan emin olmak için her zaman yardımcı teknolojilerle test etmeli ve tercihen engelli kişilerin çalışmanızı test etmesini sağlamalısınız.

Ayrıca, aria-hidden özelliğinin false olarak ayarlanmasının, ebeveynlerinden herhangi birinde bu özellik true olarak ayarlanmışsa, öğeyi yardımcı teknolojilere maruz bırakmayacağını da bilmelisiniz.

aria-hidden niteliği, ekran okuyucu kullanıcıları gibi yardımcı teknoloji kullanan kişilerden öğeleri gizlemek için kullanılır.
Tamamen dekoratif unsurları ve yinelenen içeriği gizlemek için yararlı olsa da, erişilebilirliği engellememek için az kullanılmalıdır.

Genel olarak, sayfada bulunan tüm içerik ve işlevler yardımcı teknoloji kullanan kişiler tarafından da kullanılabilir olmalıdır. Aria-hidden'ın kullanım alanı çok dardır ve öncelikle tamamen dekoratif veya yinelenen bilgileri kaldırarak ekran okuyucu kullanıcıları için deneyimi daha temiz hale getirmekle sınırlı olmalıdır. Ekran okuyucu kullanıcılarının ilgilenmeyeceğini düşündüğünüz içerikleri gizlemek için aria-hidden kullanmayın. Ekran okuyucu kullanıcıları sayfadaki tüm bilgilere erişmeyi hak eder.

Bu en iyi uygulamaları izleyerek ve kullanıcı deneyimini test ederek herkes için kapsayıcı çevrimiçi deneyimler oluşturabilirsiniz.