Tablolar ve erişilebilirlik için en iyi uygulamalar nelerdir?

Bir tablo gördüğümüzde, hemen veriler ve başlıklar arasında görsel ilişkilendirmeler yapmaya başlarız.

Örneğin, evcil hayvanlarımızı temsil eden bir tablomuz olduğunu varsayalım. İki köpeğimiz ve iki kedimiz var ve tablo bize onların isimlerini ve yaşlarını gösteriyor. Gören bir kişi bu tablodaki ilişkileri anlayabilirken, değerler ve başlıklar arasındaki bağlantıları kurmak, ekran okuyucu kullanan kişilerin tabloda gezinmesi için çok daha zordur.

Bir web geliştiricisi olarak, bu ilişkileri oluşturmaktan ve HTML işaretlemenizi ekran okuyucu kullanıcılarının da yorumlayabileceği şekilde yapılandırmaktan siz sorumlusunuz.

Şimdi herkesin anlayabileceği erişilebilir tabloları nasıl oluşturabileceğinizi görelim. Ele alacağımız ilk en iyi uygulama tablo başlığı kullanmaktır. Başlık öğesi ile bir tablonun başlığını (veya başlığını) yazabilirsiniz, böylece kullanıcılar, özellikle de yardımcı teknolojileri kullananlar, tablonun amacını ve içeriğini hızlı bir şekilde anlayabilir. Başlık öğesini tablo öğesinin açılış etiketinden hemen sonra yerleştirmelisiniz. Bu şekilde, ekran okuyucular ve diğer yardımcı teknolojiler içeriği okumadan önce başlığı duyurarak daha fazla bağlam sağlayabilir.
```
<table>
  <caption>Our Pets</caption>
  <!-- Table Rows and Columns -->
</table>
```
Şimdi satır ve sütun başlıklarından bahsedelim. Başlıklar, genellikle bir satırın veya sütunun başında bulunan ve satırda veya sütunda depolanan verilerin türünü açıklayan özel hücrelerdir. Tablo başlığı öğesi ``th`` ile bir satır veya sütun başlığı tanımlayabilirsiniz.

Örneğin, aşağıdaki kod iki evcil hayvan için bir tablo oluşturur. Her satırın bir satır başlığı (evcil hayvanın adı) ve her sütunun, sütundaki verilerin neyi temsil ettiğini (yaş ve tür) açıklayan bir sütun başlığı vardır.
```
<table>
  <caption>Our Pets</caption>
  <thead>
    <tr>
      <!-- Column Headers -->
      <th>Name</th>
      <th>Age</th>
      <th>Type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Nora</th> <!-- Row Header -->
      <td>5</td>
      <td>Dog</td>
    </tr>
    <tr>
      <th>Gino</th> <!-- Row Header -->
      <td>2</td>
      <td>Cat</td>
    </tr>
  </tbody>
</table>
```
Yukarıdaki kodun açılış tablosu öğesinden hemen sonra bir başlık öğesine sahip olduğuna dikkat edin. Ardından, tablo başlığı (thead) öğesinin içinde sütun başlıkları (Ad, Yaş ve Tür) bulunur. İkinci ve üçüncü satırlarda, tablo gövdesi (tbody) öğesinin içinde, evcil hayvanlarımızın her biri için verileri buluruz. Evcil hayvanların adları satır başlıklarıdır çünkü tablo başlığı öğelerinin (th) içindedirler.
Veri hücrelerini ilgili başlıklarla ilişkilendirmek de ekran okuyucular için çok önemlidir. Kapsam niteliği, bir başlığın satır başlığı mı yoksa sütun başlığı mı olduğunu belirler. Ekran okuyucular bunu tablonun yapısından doğru tahmin edebilir, ancak netliği sağlamak için genellikle kapsamın açıkça belirtilmesi önerilir.

Kapsam niteliğinin dört olası değeri vardır. En sık kullanacağınız iki değer sütun için col ve satır için row'dur. Aşağıdaki kodda, scope niteliğini sütun ve satır başlıklarına eklediğimizi görebilirsiniz. Üç sütun başlığı (Name, Age ve Type) col, column kapsamına sahiptir.

İki satır başlığı (Nora ve Gino) satır kapsamına sahiptir.
```
<table>
  <caption>Our Pets</caption>
  <thead>
    <tr>
      <!-- Now they have scope -->
      <th scope="col">Name</th>
      <th scope="col">Age</th>
      <th scope="col">Type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">Nora</th>
      <td>5</td>
      <td>Dog</td>
    </tr>
    <tr>
      <th scope="row">Gino</th>
      <td>2</td>
      <td>Cat</td>
    </tr>
  </tbody>
</table>
```
Bir sütun veya satır başlığı birden fazla hücreye yayılıyorsa, kapsam hücrelerin her birine ayrı ayrı uygulanır. İşte buna bir örnek:
```
<table>
  <tbody>
    <tr>
      <td></td>
      <th scope="col">Name</th>
      <th scope="col">Age</th>
    </tr>
    <tr>
      <th rowspan="2" scope="row">Dogs</th>
      <th scope="row">Nora</th>
      <td>5</td>
    </tr>
    <tr>
      <th scope="row">Gino</th>
      <td>2</td>
    </tr>
    <tr>
      <th rowspan="2" scope="row">Cats</th>
      <th scope="row">Lulu</th>
      <td>10</td>
    </tr>
    <tr>
      <th scope="row">Elizabeth</th>
      <td>6</td>
    </tr>
  </tbody>
</table>
<p>In this table, the cell with <code>Nora</code>'s age (<code>5</code>) will have one column header (<code>Age</code>) and two row headers (<code>Dogs</code> and <code>Nora</code>). <code>Gino</code>'s age (<code>2</code>) will also have one column header (<code>Age</code>) and two row headers (<code>Dogs</code> and <code>Gino</code>).</p>
```
Bununla birlikte, bazı ekran okuyucular karmaşık yapılara sahip tabloları yorumlayamayabilir, bu nedenle birden fazla hücreye yayılan satır ve sütun başlıklarından kaçınmak için tabloyu mümkün olduğunca düzleştirmeye çalışmalısınız.

Amacınız her zaman, ekran okuyucuları karmaşık tablo yapılarını işleyebilse bile kullanıcıların bu bilgilere erişebilmesini sağlamak olmalıdır.

Şimdi, hücre genişliği için sabit değerler kullanmaktan kaçınmanız önerilir. Bunun yerine yüzde gibi göreli değerler kullanmalısınız. Ayrıca, hücre yüksekliğini tanımlamaktan kaçının. Bu, kullanıcıların metin boyutunu kendi ihtiyaçlarına göre ayarlamalarına olanak tanıyacaktır.

Ve son olarak, yatay kaydırma ihtiyacını azaltmak için mümkün olduğunda tablo genişliğini tarayıcının belirlemesine izin vermelisiniz.

HTML tabloları, yapılandırılmış verilerin erişilebilir ve anlaşılabilir bir biçimde sunulması için gereklidir. Bu erişilebilirlik yönergelerini izleyerek herkes için anlaşılması kolay tablolar oluşturabilirsiniz.
