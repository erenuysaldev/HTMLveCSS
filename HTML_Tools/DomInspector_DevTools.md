
Projelerinizde hata ayıklamak ve derlemek için DOM denetçisini ve devtools'u nasıl kullanıyorsunuz?

Projelerinizi oluştururken, programlarınızın beklendiği gibi çalışmadığı sorunlarla sık sık karşılaşırsınız.

Programcılar sorunları genellikle hata olarak adlandırır. Bu hataları bulma ve düzeltme süreci hata ayıklama olarak bilinir.

Kodunuzda hata ayıklamak için tarayıcınız tarafından sağlanan bazı araçları kullanmanız gerekecektir.

Kullanılacak iki önemli araç DOM denetçisi ve geliştirici araçlarıdır.

DOM denetçisi, bulunduğunuz sayfanın HTML yapısını incelemenizi sağlar.

DOM, Belge Nesne Modeli anlamına gelir. Bir sayfadaki öğeleri temsil eden ağaç benzeri bir yapıdır. Daha sonraki modüllerde DOM hakkında daha fazla bilgi edineceksiniz.

Geliştirici araçları, üzerinde bulunduğunuz sayfanın HTML, CSS ve JavaScript'ini incelemenize olanak tanır.

Şimdi anchor öğesinde küçük bir hata içeren bir HTML örneğine göz atalım:
```
<a href="https://www.freecodecamp.org/larn/">freeCodeCamp curriculum</a>
```
Bağlantıya tıkladığınızda bir 404 sayfasına yönlendirilirsiniz. 404 sayfası, bir kullanıcı sunucuda mevcut olmayan bir web sayfasına erişmeye çalıştığında görüntülenen bir hata sayfasıdır.

Bağlantının freeCodeCamp müfredatına yönlendirmesi amaçlanmıştır.

Sorunun ne olabileceğini görmek için geliştirici araçlarını kullanabilirsiniz.

Tarayıcınızda geliştirici araçlarını açmak için sayfaya sağ tıklayabilir ve İncele'yi seçebilirsiniz.

PC klavyenizde Control Shift I veya Mac klavyenizde Command Option I tuşlarını da kullanabilirsiniz.

Google Chrome'da geliştirici araçlarını açtığınızda, bir dizi sekme görürsünüz. İlk sekme Elements sekmesi olarak adlandırılır. Bu sekme size bulunduğunuz sayfanın HTML yapısını gösterir.

İkinci sekme Konsol sekmesi olarak adlandırılır. Bu sekme size sayfada meydana gelebilecek hataları gösterir.

Kırık bir bağlantınız olduğu durumda, bu kırık bağlantıya ilişkin hata mesajlarını görmek için konsolu kontrol edebilirsiniz. Bozuk bağlantı için görüntülenmeye devam eden ortak mesaj 404 hatasıdır. 404 hatası sayfanın bulunamadığını gösterir.

Bu bize sorunun anchor öğesindeki URL ile ilgili olduğunu bildirir. href değerini incelediğinizde bir yazım hatası olduğunu göreceksiniz.

Şu anda konsol mesajı 404'e karşı /larn gösteriyor, ancak doğru URL /learn olmalıdır. Bağlantı düzeltildiğinde, beklendiği gibi çalışacaktır.

Sertifika boyunca geliştirici araçlarıyla çalışma hakkında daha fazla bilgi edineceksiniz, ancak bu, kodunuzda hata ayıklamanıza nasıl yardımcı olabileceğine dair kısa bir örnektir.