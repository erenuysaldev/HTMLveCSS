
Ne zaman deyimsel metin öğesi yerine vurgu öğesini kullanmalısınız?

Bu öğeler sunumsal ve anlamsal HTML kavramlarıyla çok yakından ilişkilidir. Deyimsel metin öğesi, i, başlangıçta metni italik olarak görüntülemek için sunum amaçlı kullanılıyordu. Ancak şimdi, alternatif ses veya ruh halini, başka bir dilden deyimsel terimleri, teknik terimleri ve düşünceleri vurgulamak için sıklıkla kullanılmaktadır.

İşte resmi HTML spesifikasyonundan, Fransızca bir deyimsel ifadeyi göstermek için i öğesini kullanan örnek:
```
<p>There is a certain <i lang="fr">je ne sais quoi</i> in the air.</p>
```

Açık <i> etiketinin içindeki lang niteliği içeriğin dilini belirtmek için kullanılır. Bu durumda, dil Fransızca olacaktır. i öğesi metnin önemli olup olmadığını göstermez, sadece metnin çevresindeki metinden bir şekilde farklı olduğunu gösterir.

Metnin önemini vurgulamanız gerekiyorsa, vurgu öğesi olarak adlandırılan benzer bir anlamsal öğe olan em'yi kullanabilirsiniz. Bu genellikle daha fazla bağlam sağlamanız gerektiğinde önerilir. Bu öğeyi, metnin çevresindeki metne kıyasla özel bir vurgu gerektiren kısımları için kullanmalısınız. Genellikle yalnızca birkaç kelimeyle sınırlıdır, çünkü cümlenin anlamını değiştirebilir.

Bu, paragraf içindeki vurgu öğesine bir örnektir:
```
<p>
 <em>hayallerinizden</em> asla vazgeçmeyin.
</p>
```

Hayallerinizden asla vazgeçmeyin cümlesini görebilirsiniz. Bu öğenin içinde olduğu için your kelimesinin vurgulanacağına dikkat edin. Tarayıcıda, okuyuculara bunun cümledeki önemli bir kelime olduğunu söylemek için your kelimesinin italik olduğunu görürsünüz.

Metin deyimsel metin öğesinin içindeyken aynı görünse bile, anlamsal vurgu öğesi perde arkasında anlamını ve önemini aktarır.

Bu öğelerin yalnızca sunum amaçlı kullanılmaması gerektiğini bilmek önemlidir. Metni italik olarak görüntülemeniz gerekiyorsa, ancak metnin paragrafta özel bir amacı, stili veya anlamı yoksa, bunun yerine CSS kullanmalısınız.
## FreeCodeCamp
