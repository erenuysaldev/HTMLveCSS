HTML Temelleri  
HTML’in Rolü: HTML, web sayfasının içeriğini ve yapısını temsil eder.  

HTML Öğeleri: Öğeler, bir HTML belgesinin yapı taşlarıdır. Başlıkları, paragrafları, bağlantıları, resimleri ve daha fazlasını temsil ederler. Çoğu HTML öğesi, bir açılış etiketi (<elementName>) ve bir kapanış etiketi (</elementName>) içerir.  

İşte temel sözdizimi:

<elementName>İçerik buraya gelecek</elementName>

Boş Öğeler: Boş öğeler hiçbir içerik taşımaz ve yalnızca başlangıç etiketi bulunur. Örnekler arasında img ve meta öğeleri yer alır.  

<img>  
<meta>  

Bazı kod tabanlarında boş öğeler içinde eğik çizgi (/) kullanılması da yaygındır. Her iki kullanım da doğrudur:

<img>  
<img/>

Öznitelikler: Bir öznitelik, bir HTML öğesinin açılış etiketinin içine yerleştirilen bir değerdir. Öznitelikler, öğe hakkında ek bilgiler sağlar veya öğenin nasıl davranması gerektiğini belirtir. İşte bir öznitelik için temel sözdizimi:

<element attribute="değer"></element>

Boolean (Mantıksal) Öznitelik: Boolean öznitelik, bir HTML etiketinde var olup olmamasına göre doğru veya yanlış değeri alan özniteliktir. Varlığında true, yokluğunda false kabul edilir. Örnek boolean öznitelikler arasında disabled, readonly ve required bulunur.

Yorumlar: Yorumlar, kodunuzda kendiniz veya diğer geliştiriciler için not bırakmak amacıyla kullanılır. HTML'de yorum yazmanın sözdizimi şöyledir:

<!--Bu bir HTML yorumudur.-->

Yaygın HTML Öğeleri

Başlık Öğeleri: HTML'de altı adet başlık öğesi vardır. h1'den h6'ya kadar olan başlık öğeleri, altlarındaki içeriğin önemini belirtmek için kullanılır. Numara ne kadar düşükse, o kadar yüksek önem taşır; bu yüzden h2 öğeleri h1 öğelerinden daha az önemlidir.
<h1>en önemli başlık öğesi</h1>
<h2>ikinci en önemli başlık öğesi</h2>
<h3>üçüncü en önemli başlık öğesi</h3>
<h4>dördüncü en önemli başlık öğesi</h4>
<h5>beşinci en önemli başlık öğesi</h5>
<h6>en az önemli başlık öğesi</h6>

Paragraf Öğeleri: Bu öğe, bir web sayfasındaki paragraflar için kullanılır.
<p>Bu bir paragraf öğesidir.</p>

img Öğeleri: img öğesi, web sayfasına resim eklemek için kullanılır. Resmin konumunu belirtmek için src özniteliği kullanılır. Resim öğelerinde, alt özniteliğini eklemek iyi bir uygulamadır. İşte src ve alt öznitelikleriyle bir img öğesi örneği:
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="Bir tabağın üzerindeki bir dilim lazanya.">

body Öğesi: Bu öğe, HTML belgesinin içeriğini temsil etmek için kullanılır.
<body>
    <h1>CatPhotoApp</h1>
    <p>Bu bir paragraf öğesidir.</p>
</body>    

section Öğeleri: Bu öğe, içeriği daha küçük bölümlere ayırmak için kullanılır.
<section>
    <h2>Hakkımda</h2>
    <p>Merhaba, ben Jane Doe ve bir web geliştiricisiyim.</p>
</section>

div Öğeleri: Bu öğe, belirli anlam taşımayan genel bir HTML öğesidir. Diğer HTML öğelerini barındıran genel bir kapsayıcı olarak kullanılır.
<div>
    <h1>Ben bir başlıkım</h1>
    <p>Ben bir paragrafım</p>
</div>

Bağlantı (a) Öğeleri: Bu öğeler, web sayfasına bağlantılar eklemek için kullanılır. href özniteliği, kullanıcının tıkladığında bağlantının nereye gideceğini belirtir.
<a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">sevimli kediler</a>

Sırasız (ul) ve Sıralı (ol) Liste Öğeleri: Öğelerin madde işaretli listesini oluşturmak için ul öğesi, içine bir veya daha fazla li öğesi yerleştirilerek kullanılır:
<ul>
    <li>kedi otu</li>
    <li>lazer işaretleyiciler</li>
    <li>lazanya</li>
</ul>
Sıralı liste oluşturmak için ol öğesi kullanılır:

<ol>
    <li>parazit tedavisi</li>
    <li>gök gürültüsü</li>
    <li>diğer kediler</li>
</ol>

Vurgu (em) Öğesi: Bir metne vurgu yapmak için kullanılır.
<p>Kediler <em>lazanyayı</em> sever.</p>  

Güçlü Önem (strong) Öğesi: Bu öğe, metinde aciliyet ve ciddiyeti belirtmek için güçlü vurgu yapar.
<p>
    <strong>Önemli:</strong> Devam etmeden önce lütfen koruyucu gözlüklerinizi takın. 
</p>

figure ve figcaption Öğeleri: figure öğesi, resimler ve diyagramlar gibi içerikleri gruplandırmak için kullanılır. figcaption öğesi, bu içeriğe ait açıklamayı temsil eder.
<figure>
    <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Bir tarlada etrafa bakan beş kedi.">
    <figcaption>Kediler <strong>diğer kedilerden nefret eder.</strong></figcaption>  
</figure>

main Öğesi: Bu öğe, bir web sayfasının ana içeriğini temsil etmek için kullanılır.

footer Öğesi: Bu öğe, HTML belgesinin en altında yer alır ve genellikle telif hakkı bilgileri ve diğer önemli sayfa bağlantılarını içerir.
<footer>
    <p>
        Telif Hakkı Yok - <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>
    </p>
</footer>

Tanımlayıcılar ve Gruplama

ID'ler: HTML öğeleri için benzersiz tanımlayıcılardır. ID isimleri her HTML belgesinde yalnızca bir kez kullanılmalıdır.
<h1 id="title">Film İnceleme Sayfası</h1>
ID isimlerinde boşluk olmamalıdır. Eğer ID'niz birden fazla kelime içeriyorsa, kelimeler arasına tire (-) koyabilirsiniz:

<div id="red-box"></div>

Sınıflar: Sınıflar, stil ve davranış için öğeleri gruplamak amacıyla kullanılır.
<div class="box"></div>

ID'lerin aksine, HTML belgesinde aynı sınıf adını birden fazla kez kullanabilirsiniz. Sınıf değeri aynı zamanda şu şekilde boşluk içerebilir:

<div class="box red-box"></div>
<div class="box blue-box"></div>

Özel Karakterler ve Bağlantı

HTML Varlıkları: Bir HTML varlığı veya karakter referansı, HTML'de ayrılmış bir karakteri temsil etmek için kullanılan karakter kümesidir. Örnekler arasında ampersand (&amp;) sembolü ve küçük olan (<) sembolü bulunur.
<p>Bu bir <img /> öğesidir</p>

link Öğesi: Bu öğe, stil sayfaları ve site simgeleri gibi harici kaynaklara bağlantı kurmak için kullanılır. İşte harici bir CSS dosyası için link öğesinin temel sözdizimi:
<link rel="stylesheet" href="./styles.css" />

rel özniteliği, bağlantılı kaynak ile HTML belgesi arasındaki ilişkiyi belirtir. href özniteliği ise harici kaynağın URL konumunu belirtir.

script Öğesi: Bu öğe, çalıştırılabilir kod gömmek için kullanılır.
<body>
    <script>
        alert("freeCodeCamp'e hoş geldiniz");
    </script>
</body>
Script öğesinde tüm JavaScript kodunu yazmak teknik olarak mümkün olsa da, en iyi uygulama kodu harici bir JavaScript dosyasına bağlamaktır. İşte harici bir JavaScript dosyasına bağlanmak için script öğesi örneği:

<script src="javascript-dosya-yolu.js"></script>

Temel Yapı ve Kodlama

HTML Temel Yapısı: Bu, her HTML belgesinde bulunması gereken temel yapı ve önemli öğeleri içerir.
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>freeCodeCamp</title>
        <link rel="stylesheet" href="./styles.css" />
    </head>
    <body>
        <!--Başlıklar, paragraflar, resimler, vb. buraya gelecek-->
    </body>
</html>

DOCTYPE: Bu, tarayıcılara hangi HTML sürümünü kullandığınızı belirtir.

html Öğesi: Bu, bir HTML belgesinin en üst düzey veya kök öğesidir. Belgenin dilini belirtmek için lang özniteliğini kullanmalısınız.

head Öğesi: head bölümü, tarayıcılar ve arama motorları için gerekli olan meta verileri içerir.

meta Öğeleri: Bu öğeler, sitenizin meta verilerini temsil eder. Karakter kodlaması, Twitter gibi hizmetler için sayfa önizlemesi ve diğer bilgileri içerir.

title Öğesi: Bu öğe, tarayıcı sekmesi veya pencerede görünen metni ayarlamak için kullanılır.

UTF-8 Karakter Kodlaması: UTF-8 ya da UCS Transformation Format 8, webde yaygın olarak kullanılan standart bir karakter kodlamasıdır. Bilgisayarların karakterleri veriye dönüştürme yöntemidir. charset özniteliği, bir meta öğesi içinde karakter kodlamasını UTF-8 olarak ayarlamak için kullanılır.

SEO ve Sosyal Paylaşım

SEO: Arama Motoru Optimizasyonu, web sayfalarının daha görünür hale gelmesi ve arama motorlarında daha üst sıralara yerleşmesi için yapılan uygulamalardır.

Meta (description) Öğesi: Bu öğe, web sayfası için kısa bir açıklama sağlar ve SEO'ya etki eder.
<meta
    name="description"
    content="Küçük alanlarda bahçıvanlık için uzman ipuçları ve teknikleri keşfedin, doğru bitkileri seçin ve gelişen bir bahçe oluşturun."
/>

Open Graph Etiketleri: Open Graph protokolü, web sitenizin içeriğinin Facebook, LinkedIn gibi sosyal medya platformlarında nasıl görüneceğini kontrol etmenizi sağlar. Bu özellikleri, HTML head bölümünüzdeki bir dizi meta öğesiyle ayarlayabilirsiniz.

og:title Özelliği: Sosyal medya gönderilerinde görünen başlığı ayarlamak için kullanılır.
<meta content="freeCodeCamp.org" property="og:title" />

og:type Özelliği: Bu özellik, sosyal medyada paylaşılan içeriğin türünü temsil eder. Örnek içerikler arasında makaleler, web siteleri, videolar veya müzik bulunur.
<meta property="og:type" content="website" />

og:image Özelliği: Sosyal medya gönderilerinde gösterilecek resmi ayarlamak için kullanılır.
<meta
    content="https://cdn.freecodecamp.org/platform/universal/fcc_meta_1920X1080-indigo.png"
    property="og:image"
/>

og:url Özelliği: Sosyal medya gönderilerinde kullanıcıların tıklayacağı URL'yi ayarlamak için kullanılır.
<meta property="og:url" content="https://www.freecodecamp.org" />

Medya Öğeleri ve Optimizasyon

Değiştirilmiş Öğeler: İçeriği CSS tarafından belirlenmek yerine harici bir kaynaktan alınan öğelerdir. Örneğin bir iframe öğesi. iframe, inline frame’in kısaltmasıdır. HTML sayfası içinde başka HTML içeriği yerleştirmek için kullanılır.
<iframe src="https://www.example.com" title="Örnek Site"></iframe>
allowfullscreen özniteliğini ekleyerek kullanıcının iframe’i tam ekran olarak görüntülemesine izin verebilirsiniz.

<iframe
    src="video-url"
    width="genişlik-değeri"
    height="yükseklik-değeri"
    allowfullscreen
></iframe>

YouTube veya Vimeo gibi popüler video servislerinden kopyalayarak veya src özniteliğini video URL’sine işaret ettirerek iframe ile video yerleştirebilirsiniz. İşte YouTube üzerinden freeCodeCamp kursunu gömmenin örneği:

<h1>iframe Öğesi ile Gömülü FreeCodeCamp YouTube Videosu</h1>

<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/PkZNo7MFNFg?si=-UBVIUNM3csdeiWF"
    title="YouTube video oynatıcı"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen
></iframe>

Bazı diğer değiştirilmiş öğeler, video ve embed gibi öğelerdir. Belirli durumlarda bazı öğeler de değiştirilmiş öğe olarak davranır. İşte type özniteliği "image" olan bir input öğesi örneği:

<input type="image" alt="Buraya açıklayıcı metin gelecek" src="örnek-resim-url">

Medya Optimizasyonu: Web sayfalarında resimler gibi medya öğelerini kullanırken boyut, format ve sıkıştırma olmak üzere üç aracı göz önünde bulundurmalısınız. Sıkıştırma algoritması, dosya veya verinin boyutunu azaltmak için kullanılır.

Resim Formatları: En yaygın dosya formatlarından ikisi PNG ve JPG'dir, ancak bunlar artık resim sunumu için en ideal formatlar değildir. Eski tarayıcı desteğine ihtiyaç yoksa, WEBP veya AVIF gibi daha optimize formatlar kullanmayı düşünmelisiniz.

Resim Lisansları: Kamu malı olan bir resmin üzerinde telif hakkı bulunmaz ve kısıtlama olmadan kullanılabilir. Creative Commons 0 lisansı altındaki resimler kamu malı sayılır. Bazı resimler, freeCodeCamp'in kullandığı BSD lisansı veya daha esnek Creative Commons lisansı altında yayınlanmış olabilir.

SVG'ler: Ölçeklenebilir Vektör Grafikler, noktalar, çizgiler ve eğriler çizmek için yollar ve denklemler kullanır. Bu, bir SVG'nin herhangi bir boyuta ölçeklenebileceği, ancak kalitesinden ödün vermeyeceği anlamına gelir.

Multimedya Entegrasyonu

audio ve video Öğeleri: audio ve video öğeleri, HTML belgelerinize ses ve video içeriği eklemenizi sağlar. audio öğesi mp3, wav ve ogg gibi popüler ses formatlarını destekler. video öğesi ise mp4, ogg ve webm formatlarını destekler.
<audio src="CrystalizeThatInnerChild.mp3"></audio>
Ses çaların görünmesi için controls özniteliği eklenebilir:

<audio src="CrystalizeThatInnerChild.mp3" controls></audio>

controls özniteliği, kullanıcının sesi boyutlandırma, duraklatma veya devam ettirme gibi işlemleri yapmasını sağlar. Bu öznitelik varsa yerleşik oynatma kontrolleri görüntülenir, yoksa görüntülenmez.

loop Özniteliği: loop özniteliği, sesin sürekli tekrar etmesini sağlar.
<audio
    src="https://cdn.freecodecamp.org/curriculum/js-music-player/can't-stay-down.mp3"
    loop
    controls
></audio>

muted Özniteliği: Ses öğesinde mevcutsa, ses başlangıçta sessiz (muted) olur.
<audio
    src="https://cdn.freecodecamp.org/curriculum/js-music-player/can't-stay-down.mp3"
    loop
    controls
    muted
></audio>

source Öğesi: Ses dosyası türleri arasında tarayıcıların hangi tipleri desteklediğinde farklar vardır. Bunu telafi etmek için, audio öğesi içinde birden fazla source öğesi kullanabilirsiniz. İşte çoklu source öğeleri kullanma örneği:
<audio controls>
    <source src="audio.ogg" type="audio/ogg" />
    <source src="audio.wav" type="audio/wav" />
    <source src="audio.mp3" type="audio/mpeg" />
</audio>

Tüm bu öznitelikler video öğesi tarafından da desteklenir. İşte loop, controls ve muted özniteliklerine sahip bir video öğesi örneği:

<video
    src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
    loop
    controls
    muted
></video>

poster Özniteliği: Video indirilirken görüntülenecek bir resim göstermek isterseniz, video öğesinde poster özniteliğini kullanabilirsiniz. Bu öznitelik yalnızca video öğesine özgüdür, audio öğesinde kullanılmaz.
<video
    src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
    loop
    controls
    muted
    poster="https://peach.blender.org/wp-content/uploads/title_anouncement.jpg?x11217"
    width="620"
></video>

Hedef Öznitelik Türleri

target Özniteliği: Bu öznitelik, tarayıcıya bir bağlantının URL'sini nereye açacağını söyler. Bu öznitelik için dört önemli değer vardır: _self, _blank, _parent ve _top. Deneysel FencedFrame API için kullanılan _unfencedTop değeri de vardır, fakat şu anda kullanımı genel değildir.

_self Değeri: Bu, varsayılan değerdir. Bağlantıyı mevcut tarama bağlamında açar; çoğu durumda bu, mevcut sekme veya pencere olacaktır.
<a href="https://freecodecamp.org" target="_self">freeCodeCamp'u ziyaret et</a>

_blank Değeri: Bu, bağlantıyı yeni bir tarama bağlamında açar. Genellikle yeni sekmede açılır, ancak bazı kullanıcılar tarayıcı ayarlarına bağlı olarak yeni pencere de açabilir.
<a href="https://freecodecamp.org" target="_blank">freeCodeCamp'u ziyaret et</a>

_parent Değeri: Bu, bağlantıyı mevcut bağlamın ebeveyninde açar. Örneğin, sitenizde bir iframe varsa, iframe içindeki _parent değeri, bağlantıyı sitenizin sekmesi/penceresinde açar.
<a href="https://freecodecamp.org" target="_parent">freeCodeCamp'u ziyaret et</a>

_top Değeri: Bu, bağlantıyı en üst düzey tarama bağlamında, yani "ebeveynin ebeyni" şeklinde açar. _parent'e benzer, ancak bağlantı her durumda tam tarayıcı sekmesinde/penceresinde açılır, gömülü çerçevelerde bile.
<a href="https://freecodecamp.org" target="_top">freeCodeCamp'u ziyaret et</a>

Mutlak ve Göreceli Yollar

Yol Tanımı: Bir yol, dosya veya dizinin konumunu belirten bir karakter dizisidir. Web geliştirmede yollar, resimler, stil dosyaları, scriptler ve diğer web sayfaları gibi kaynaklara bağlantı kurmak için kullanılır.

Yol Sözdizimi: Bilmeniz gereken üç temel sözdizimi vardır. İlk olarak, işletim sisteminize bağlı olarak ters eğik çizgi (\) veya eğik çizgi (/) kullanılan bölücü. İkinci, tek nokta (.) ve son olarak çift nokta (..). Eğik çizgi, klasör veya dosya isimleri arasında ayrım sağlar. Tek nokta mevcut dizini, çift nokta ise üst dizini temsil eder.
public/index.html  
./favicon.ico  
../src/index.css

Mutlak Yol: Mutlak yol, bir kaynağa tam bağlantı sağlar. Kök dizinden başlar, tüm alt dizinleri içerir ve dosya adı ile uzantısını belirtir. "Kök dizin", hiyerarşideki en üst düzey dizini ifade eder. Mutlak yol ayrıca protokol (http, https, file) ve kaynak web üzerinde ise alan adını da içerir. İşte freeCodeCamp logosuna bağlantı veren mutlak yol örneği:
<a href="https://design-style-guide.freecodecamp.org/img/fcc_secondary_small.svg">
    freeCodeCamp Logosu'nu Görüntüle
</a>

Göreceli Yol: Göreceli yol, dosyanın mevcut dosyaya göre konumunu belirtir. Protokol veya alan adı içermez, bu yüzden dahili bağlantılar için daha kısa ve esnektir. İşte contact.html sayfasından aynı klasörde bulunan about.html sayfasına bağlantı örneği:
<p>
    Daha fazlası için,
    <a href="about.html">Hakkında Sayfasını</a> ziyaret edin.
</p>

Bağlantı Durumları

:link: Bu varsayılan durumdur. Henüz ziyaret edilmemiş, tıklanmamış veya etkileşimde bulunulmamış bir bağlantıyı temsil eder. Diğer durumlar bu temel üzerine inşa edilir.  
:visited: Kullanıcının bağlantı verilen sayfayı zaten ziyaret ettiği durumlarda geçerli olur. Varsayılan olarak bağlantıyı mor renge çevirir; ancak CSS ile farklı bir stil uygulanabilir.  
:hover: Kullanıcı fareyi bağlantının üzerine getirdiğinde geçerli olur. Bağlantıya ekstra dikkat çekmek için kullanılır.  
:focus: Bağlantı odaklandığında (klavye navigasyonu gibi) geçerlidir.  
:active: Kullanıcı bağlantıya tıkladığında veya bağlantı etkinleştirildiğinde geçerli olan durumdur.  