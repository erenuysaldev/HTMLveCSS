
aria-label ve aria-labelledby niteliklerinin rolleri nelerdir?

Engelli kullanıcılar da dahil olmak üzere tüm kullanıcıların web sitelerine sorunsuz bir şekilde erişebilmelerini sağlamak önemlidir.

Ekran okuyucu kullanan kişiler için aria-label ve aria-labelledby öznitelikleri, belirsiz veya görünmez olabilecek sayfa öğeleri hakkında önemli bilgiler sağlar.

Şimdi aria-label ve aria-labelledby niteliklerinin ne olduğuna ve web'i görme engelli ve ilgili engelleri olan kişiler için erişilebilir hale getirmede oynadıkları rollere bakalım.

Hem aria-label hem de aria-labelledby'nin başına aria eklendiğini fark edeceksiniz. Peki bu ne anlama geliyor? ARIA, Erişilebilir Zengin İnternet Uygulamaları anlamına gelir. Geliştiricilerin yardımcı teknolojilere öğelerin amacını iletmesini sağlayan, ön eki aria- olan bir dizi özniteliktir. aria-label niteliği, etkileşimli öğeler için görünmez bir etikettir. Bir öğeye ekran okuyucuların okuyabileceği bir metin etiketi ekler.
aria-label özellikle görünür metni olmayan ancak yine de ekran okuyucular tarafından tanımlanması gereken öğeler için kullanışlıdır. Örneğin, yalnızca simge içeren düğmelerin amaçlarını iletmek için genellikle aria-label'e ihtiyaçları vardır.

İşte bir örnek:
```
<input type="text" aria-labelledby="search-btn">
<button type="button" id="search-btn">Search</button>
```
Bu durumda, düğme metni arama girişi için etiket olarak kullanılmaktadır. Ekran okuyucular girişi Ara, düzenle gibi bir şekilde duyuracaktır. Daha sonra düğme metnini Bul olarak değiştirmek istediğinize karar verirseniz, düğme metnini referans aldığı için girdinin etiketi otomatik olarak yeni metinle güncellenecektir. Birden fazla id değerini tek bir aria-labelledby öznitelik değerinde birleştirmek de mümkündür. Bunun nasıl çalıştığı aşağıda açıklanmıştır:
```
  <span id="volume-label">Volume</span>
  <span id="volume-details">Adjust the volume level</span>
  <input
    type="range"
    min="0"
    max="100"
    value="30"
    aria-labelledby="volume-label volume-details">
</div>
```
Kaydırıcı için ekran okuyucu volume-label ve volume-details öğelerinin içeriğine bakacak ve Volume Adjust the volume level (Ses seviyesini ayarla) diyecektir.

Hem aria-label hem de aria-labelledby niteliklerinin ekran okuyucuların öğelerin ne işe yaradığını anlamasına yardımcı olduğunu gördünüz. Peki, hangisini kullanmalısınız? Her ikisi de aynı işlevi sağladığından, ikisi de kullanılabilir, ancak aria-labelledby'yi aria-label'a göre kullanmanın birkaç avantajı olabilir:
Birisi sayfanızdaki içeriği çevirmek için bir çeviri hizmeti kullanıyorsa, aria-label özniteliğindeki metin her zaman çevrilmeyebilir.
Görünür metnin güncellenmesi görünmez etiketi de otomatik olarak güncelleyeceğinden, aria-labelledby kullanımı ekran okuyucu kullanıcıları için görünür etiket metni ile görünmez etiket arasındaki uyumsuzluğu önlemeye de yardımcı olabilir.
aria-labelledby birden fazla metin kaynağından oluşan karmaşık görünmez etiketleri programlı olarak oluşturmayı çok daha kolay hale getirebilir.
Son bir not, aria-label ve aria-labelledby öğelerini bir öğe üzerinde aynı anda kullanmayın. Bu durumda, ekran okuyucular için görünmez etiket her zaman aria-labelledby tarafından belirlenecek ve aria-label tamamen göz ardı edilecektir.