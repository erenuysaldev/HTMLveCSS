
HTML'de adresleri nasıl gösterirsiniz?

İletişim adresi öğesi, bir web sayfasındaki bir bölümün iletişim bilgilerini temsil etmek için kullanılır. Adres öğesi çok yönlüdür ve işletme sayfaları, yazar sayfaları, kişisel siteler ve daha fazlası için kullanılabilir.

Web sitenizin iletişim bölümlerini oluşturmak söz konusu olduğunda, div gibi genel bir öğe yerine semantik adres öğesini kullanmalısınız.

İşte bir şirket iletişim sayfası için adres öğesinin kullanımına ilişkin bir örnek:
```
<address>
  <h2>Company Name</h2>
  <p>
    1234 Elm Street<br />
    Springfield, IL 62701<br />
    United States
  </p>
  <p>Phone: <a href="tel:+15555555555">+1 (555) 555-5555</a></p>
  <p>Email: <a href="mailto:contact@company.com">contact@company.com</a></p>
</address>
```
Bu örnekte, şirket adı, fiziksel adres, telefon ve e-posta bilgileri bulunmaktadır. Fiziksel adres için, sokak adı, şehir ve ülke arasındaki bölünmeyi göstermek için br satır sonu öğesi kullanılır.

Telefon numarası için, href değeri telefon numaraları için ayarlanmış bir anchor elemanımız var. href niteliğinin içindeki tel:+ değeri, bunu destekleyen belirli cihazlarda bir telefon görüşmesi başlatmak için tıklanabilir bir bağlantı oluşturur.

E-posta adresi için, href değeri bir mailto bağlantısına ayarlanmış başka bir bağlantı öğesi kullanılır. mailto bağlantıları, HTML belgelerinde kullanıcıların tercih ettikleri e-posta istemcisinde yeni bir e-posta açmalarını sağlamak için kullanılır.

Bir mailto bağlantısı kullanmanın dezavantajlarından biri, kullanıcıların bunu genellikle spam olarak algılamasıdır. Ne yazık ki, birçok spam gönderici kullanıcılara e-posta göndermek için bu seçeneği kullanacaktır. Bu yüzden kullanırken bunu aklınızda bulundurun.