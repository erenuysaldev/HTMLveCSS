ARIA rolleri nelerdir?

ARIA, Erişilebilir Zengin İnternet Uygulamaları anlamına gelir.

ARIA rolleri, HTML öğelerinin semantik anlamını belirtir. Web içeriğini ekran okuyucular gibi yardımcı teknolojileri kullanan kişiler için erişilebilir kılmak için gereklidirler.

HTML, içerikleri hakkında anlam iletip iletmediklerine bağlı olarak semantik ve semantik olmayan öğelere sahiptir.
Birçok semantik HTML öğesi zaten varsayılan olarak atanmış bir ARIA rolüne sahiptir. Örneğin ``button``öğesinin varsayılan ARIA rolü ``button``'dur.
Ancak anlamsal olmayan öğelerin bir rolü yoktur. Örneğin, rolünü açıkça belirtmezseniz ekran okuyucular bir ``div``'in amacını nasıl yorumlayacaklarını bilemezler.
Bir öğenin ARIA rolünü belirtmek için, ``role`` özniteliğini eklemeniz yeterlidir, bu ``role="ARIA role"`` gibidir, burada value ARIA belirtimindeki bir rolün adıdır.
Bir öğe üzerinde bir rol belirtmenin tek bir işe yaradığını unutmamak önemlidir: Yardımcı teknolojiyi öğenin amacı hakkında bilgilendirir. Öğeye herhangi bir işlevsellik veya davranış eklemez. İnsanlar bir rolün belirli bir şekilde davranmasını bekliyorsa, beklenen davranışı eklemek geliştirici olarak size bağlıdır. Örneğin, bir div'e düğme rolü eklemek onu otomatik olarak fare ile tıklanabilir veya klavye ile kullanılabilir yapmaz. Div'in bir düğme gibi davranmasını sağlayan beklenen davranışı eklemek geliştiricinin sorumluluğundadır ve çoğu durumda düğme öğesini kullanmak daha iyidir.