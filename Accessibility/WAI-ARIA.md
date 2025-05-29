WAI-ARIA'nın amacı nedir ve nasıl çalışır?

Statik içeriği erişilebilir hale getirmek nispeten kolay olabilir, ancak dinamik içerik daha zor olabilir. İşte WAI-ARIA burada devreye giriyor.

Şimdi WAI-ARIA'nın ne olduğuna, amacına, nasıl çalıştığına ve bazı örneklere bakalım.

WAI-ARIA, Web Erişilebilirlik İnisiyatifi - Erişilebilir Zengin İnternet Uygulamaları anlamına gelir. Dinamik içerik ve UI (Kullanıcı Arayüzü) bileşenleri için erişilebilirliği geliştiren bir spesifikasyondur.

WCAG ve WAI-ARIA'nın aynı olmadığını unutmayın. WCAG web erişilebilirliği için genel kurallar sağlarken, WAI-ARIA dinamik ve etkileşimli içeriği yardımcı teknolojilerin kullanıcıları için erişilebilir hale getirmek için özel kurallar sunar.

Bu nedenle, WAI-ARIA'nın birincil amacı, yerel HTML eşdeğerleri olmayan dinamik içerik ve UI bileşenleri için erişilebilirliği iyileştirmektir.

WAI-ARIA, ek anlamsal bilgiler sağlamak için HTML öğelerine ekleyebileceğiniz bir dizi öznitelik sunarak çalışır. Bu nitelikler roller, durumlar ve özellikler olarak kategorize edilir.

ARIA rolü, bir web sitesi veya web uygulaması içindeki bir öğenin amacını tanımlar. İşte bir div öğesi için rolün düğme olarak ayarlanmasına ilişkin bir örnek.
```
<div role="button">Click Me</div>
```
Bunu yaparak yardımcı teknolojiye öğenin bir düğme olduğunu belirtmiş olursunuz. Ancak roller herhangi bir işlevsellik sağlamaz. Bu ``div``'e yalnızca düğme rolü vermek, düğme gibi davranmasını sağlamaz. Bir düğme gibi görünmesini ve davranmasını sağlamak için CSS ve JavaScript kullanarak istediğiniz sonucu elde etmeniz gerekir. Bunun yerine type="button" ile yerel düğme veya giriş öğesini kullanmak her zaman daha iyidir.

HTML tek başına sekmeli gezinme (sekme listesi) gibi özel UI bileşenlerini erişilebilir kılmak için bir yol sağlamadığından, ARIA rolleri çok yardımcı olabilir.

İşte bir sekme listesinin rol niteliği ile nasıl görünebileceği:
```
<div role="tablist" aria-label="Football Match Dashboard">
   <button
     role="tab"
     aria-selected="true"
     aria-controls="match-info-panel"
     id="match-info-tab">
       Match Info
   </button>

   <button
     role="tab"
     aria-selected="false"
     aria-controls="player-stats-panel"
     id="player-stats-tab">
     Player Stats
   </button>
</div>
```
Sekme listesindeki her sekme, sekmesi seçildiğinde görüntülenecek ilişkili bir sekme paneline sahip olacaktır. Her sekme paneli tabpanel rolüne sahip olacaktır.

İşte bu sekme panellerinin her biri nasıl görünebilir:
```
<div 
  role="tabpanel"
  id="match-info-panel" 
  aria-labelledby="match-info-tab"
>
   <p>
     Details about the match, including date,
     time, venue, and current score.
   </p>
</div>

<div
   role="tabpanel"
   id="player-stats-panel"
   aria-labelledby="player-stats-tab"
   hidden
>
   <p>
     Individual player statistics such as goals,
     assists, and minutes played.
   </p>
</div>
```
ARIA state, kullanıcı etkileşimlerine bağlı olarak değişebilen bir öğenin mevcut durumunu tanımlar. Katlanabilir bölümler için ``aria-expanded`` niteliği buna bir örnektir:
```
<button aria-expanded="false" aria-controls="more-info">
  More Info
</button>

<div id="more-info" hidden>
   <p>This is additional information.</p>
</div>
```
Yine, bu yalnızca durumu tanımlar, herhangi bir işlevsellik sağlamaz. Kullanıcı düğmeyi tıkladığında niteliğin durumunu değiştirmek için JavaScript kullanmanız gerekir.

ARIA özellikleri öğeler hakkında ek ayrıntılar sağlar. Örneğin, aria-labelledby özelliği bir öğeyi belirli bir etikete bağlamanızı sağlar:
```
<h2 id="header-id">About freeCodeCamp</h2>
<button id="button-id" aria-labelledby="header-id button-id">Learn More</button>
```
Bu, öğeleri yardımcı teknoloji kullanıcıları için anlaşılabilir ve gezilebilir hale getirecektir.

WAI-ARIA'dan en iyi şekilde yararlanmak için mümkün olduğunca yerel HTML'ye bağlı kalmaya çalışın, çünkü genellikle kutudan çıkar çıkmaz daha fazla erişilebilirlik sağlar.

WAI-ARIA'yı yalnızca HTML yetersiz kaldığında kullanın ve ekran okuyucular gibi yardımcı teknolojilerle test etmeyi veya engelli kişilerin çalışmanızı test etmesini sağlamayı unutmayın. Ayrıca, WAI-ARIA durumlarınızın ve özelliklerinizin içerikle birlikte gerçek zamanlı olarak güncellendiğinden emin olun. Çoğu zaman kafa karıştırıcı olabileceğinden ARIA'yı aşırı kullanmaktan kaçının.