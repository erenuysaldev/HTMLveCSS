
Link Durumları Nelerdir ve Neden Önemlidir?

Bir web sayfasındaki bir bağlantıya tıkladıktan sonra bağlantının mor renge döndüğünü görmüş olabilirsiniz. Bunun nedeni, bağlantının durumunun değişmiş olmasıdır; dolayısıyla farklı stiller uygulanır. Bir bağlantının sahip olabileceği beş farklı durum bulunmaktadır.

İlk durum, varsayılan durum olan :link'tir. Bu durum, kullanıcının henüz ziyaret etmediği, tıklamadığı veya etkileşime girmediği bağlantıyı temsil eder. Bu durumu, sayfanızdaki tüm bağlantılar için temel stilleri sağlayan bir yapı olarak düşünebilirsiniz. Diğer durumlar buna eklenir.

İkinci durum, kullanıcının daha önce bağlantısının işaret ettiği sayfayı ziyaret etmesinden sonra uygulanan :visited durumudur. Varsayılan olarak, bu durum bağlantıyı mor renge çevirir; ancak CSS kullanarak kullanıcıya farklı bir görsel gösterim sağlayabilirsiniz. Bu, kullanıcının belgelerinizin bir bölümünü zaten okuduğunu veya siteyi daha önce kullandığı için güvenebileceğini göstermeye yardımcı olur.

Üçüncü durum, :hover durumudur. Bu durum, kullanıcının imlecini bir bağlantı üzerinde gezdirdiğinde uygulanır. :hover durumu, bir bağlantıya fazladan dikkat çekmek ve kullanıcının gerçekten tıklamak istediğinden emin olmak için faydalıdır.

Daha sonra :focus durumu gelir. Bu durum, bir bağlantıya odaklanıldığında uygulanır.

Ve son olarak :active durumu vardır. Bu durum, kullanıcının etkinleştirdiği bağlantılar için geçerlidir. Genellikle, bu birincil fare düğmesi (sol tıklama) ile bağlantıya tıklamak anlamına gelir. Bu durum, kullanıcının tıkladığı öğenin etkileşimli olduğunu göstermek için yardımcı olabilir.

Bu durumları kullanarak bağlantılarınızı stillendirdiğinizde, CSS'inizi yazarken belirli bir sıra izlemelisiniz: link, visited, hover, focus ve ardından active.

Artık, sayfanızdaki bağlantılara kendi kişisel dokunuşunuzu katarken, kullanıcıya her bağlantının durumuyla ilgili gerekli bilgiyi sağlamayı biliyorsunuz.