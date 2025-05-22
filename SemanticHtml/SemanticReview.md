Semantik HTML'in Önemi  
Başlık öğeleri için yapısal hiyerarşi: İçeriğin yapısal hiyerarşisini korumak için doğru başlık öğesini kullanmak önemlidir. h1 öğesi en yüksek düzeyde başlık, h6 öğesi ise en düşük düzeyde başlıktır.

Görsel HTML öğeleri: İçeriğin görünümünü tanımlayan öğeler. Örn. kullanım dışı kalmış center, big ve font öğeleri.

Semantik HTML öğeleri: Anlam ve yapı barındıran öğeler. Örn. header, nav, figure.

Semantik HTML Öğeleri

Header öğesi: Bir belgenin veya bölümün başlığını tanımlamak için kullanılır.

Main öğesi: Web sayfasının ana içeriğini barındırmak için kullanılır.

Navigasyon Bölümü (nav) öğesi: Navigasyon bağlantılarının bulunduğu bir bölümü temsil eder.

Figure öğesi: İllüstrasyonlar ve diyagramları içermek için kullanılır.

Vurgu (em) öğesi: Vurgu yapılmış metni belirtir.  
Örnek Kod
<p>
    Asla <em>hayallerinizden</em> vazgeçmeyin.
</p>

İdiomatik Metin (i) öğesi: Alternatif bir ses tonu veya ruh halini, başka bir dilden gelen deyimleri, teknik terimleri ve düşünceleri vurgulamak için kullanılır.  
Örnek Kod
<p>
    Havada belli bir <i lang="fr">je ne sais quoi</i> var.
</p>
Açılı i etiketindeki lang özniteliği, içeriğin dilini belirtmek için kullanılır. Bu durumda dil Fransızcadır. i öğesi, metnin önemli olup olmadığını göstermez; sadece çevresindeki metinden farklı olduğunu belirtir.

Güçlü Vurgu (strong) öğesi: Güçlü vurgu yapılan metni belirtir.  
Örnek Kod
<p>
    <strong>Uyarı:</strong> Bu ürün alerjik reaksiyonlara neden olabilir.
</p>

Dikkat Çekme (b) öğesi: İçeriğin anlamı ile doğrudan ilgili olmayan metne dikkat çekmek için kullanılır. Genellikle özetlerde anahtar kelimeleri veya incelemelerde ürün isimlerini vurgulamak için tercih edilir.  
Örnek Kod
<p>
    Birkaç ürün test ettik, bunlar arasında ses kalitesi için <b>SuperSound 3000</b>, hızlı şarj için <b>QuickCharge Pro</b> ve temizlik için <b>Ecoclean Vacuum</b> vardı. İlk ikisi iyi performans gösterdi, ancak <b>Ecoclean Vacuum</b> beklentileri karşılamadı.
</p>

Açıklama Listesi (dl) öğesi: Terim ve açıklama gruplarını temsil etmek için kullanılır.  
Açıklama Terimi (dt) öğesi: Tanımlanan terimi belirtir.  
Açıklama Detayları (dd) öğesi: Terimin açıklamasını belirtir.  
Örnek Kod
<dl>
    <dt>HTML</dt>
    <dd>HiperMetin İşaretleme Dili</dd>
    <dt>CSS</dt>
    <dd>Basamaklı Stil Sayfaları</dd>
</dl>

Blok Alıntı (blockquote) öğesi: Başka bir kaynaktan alıntılanmış bir bölümü temsil eder. Bu öğenin cite özniteliği vardır; cite özniteliğinin değeri kaynağın URL'sidir.  
Örnek Kod
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    "Başarılı bir geliştirici olmanın nasıl bir şey olacağını hayal edebiliyor musunuz? İnsanların güvendiği yazılım sistemlerini inşa etmek nasıl bir şey olurdu?"
</blockquote>

Atıf (cite) öğesi: Referans çalışmanın kaynağını görsel olarak belirtmek için kullanılır ve referansın başlığını işaretler.  
Örnek Kod
<div>
    <blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
        "Başarılı bir geliştirici olmanın nasıl bir şey olacağını hayal edebiliyor musunuz? İnsanların güvendiği yazılım sistemlerini inşa etmek nasıl bir şey olurdu?"
    </blockquote>
    <p>
        -Quincy Larson, <cite>How to learn to Code and Get a Developer Job [Tam Kitap].</cite>
    </p>
</div>

Satır İçi Alıntı (q) öğesi: Kısa bir satır içi alıntıyı temsil etmek için kullanılır.  
Örnek Kod
<p>
    Quincy Larson'ın dediği gibi,
    <q cite="https://www.freecodecamp.org/news/learn-to-code-book/">
        Momentum her şeydir.
    </q>
</p>

Kısaltma (abbr) öğesi: Bir kısaltma veya akronimi temsil etmek için kullanılır. Kullanıcılara kısaltmanın tam formunu ya da okunabilir açıklamasını title özniteliği ile gösterebilirsiniz.  
Örnek Kod
<p>
    <abbr title="HiperMetin İşaretleme Dili">HTML</abbr> webin temelidir.
</p>

İletişim Adresi (address) öğesi: İletişim bilgilerini temsil etmek için kullanılır.

(Zaman) (time) öğesi: Bir tarih ve/veya zamanı temsil etmek için kullanılır. datetime özniteliği, tarihleri ve zamanları makine tarafından okunabilir formata çevirmek için kullanılır.  
Örnek Kod
<p>
    Rezervasyonlar <time datetime="20:00">20:00 </time> için yapılmıştır.
</p>

ISO 8601 Tarih (datetime) özniteliği: Tarih ve zamanları makine tarafından okunabilir formda temsil etmek için kullanılır. Standart format YYYY-MM-DDThh:mm:ss şeklindedir; burada büyük T, tarih ve zaman arasındaki ayırıcıdır.

Üst Simge (sup) öğesi: Üst simge metni temsil etmek için kullanılır. Sup öğesinin yaygın kullanım alanları arasında üstel ifadeler, üst harfler ve sıralama numaraları bulunur.  
Örnek Kod
<p>
    2<sup>2</sup> (2'nin karesi) eşittir 4.
</p>

Alt Simge (sub) öğesi: Alt simge metni temsil etmek için kullanılır. Alt simge öğesinin yaygın kullanım alanları arasında kimyasal formüller, dipnotlar ve değişken alt simgeleri sayılabilir.  
Örnek Kod
<p>
    CO<sub>2</sub>
</p>

Satır İçi Kod (code) öğesi: Bir bilgisayar kodu parçasını temsil etmek için kullanılır.

Önceden Biçimlendirilmiş Metin (pre) öğesi: Önceden biçimlendirilmiş metni temsil eder.  
Örnek Kod
<pre>
    <code>
        body {
            color: red;
        }
    </code>
</pre>

Belirtilmemiş Açıklama (u) öğesi: Metnin belirli bölümlerini, metin dışı açıklamalar olduğunu gösterecek şekilde vurgulamak için kullanılır.  
Örnek Kod
<p>
    Aşağıdaki gibi belirgin olmayan hataları vurgulamak için
    <u>yanlış</u> <u>yazılmış</u> <u>hataları</u> kullanabilirsiniz.
</p>

Ruby Açıklama (ruby) öğesi: Metni telaffuz veya anlam açıklamaları ile anotasyonlamak için kullanılır. Bu, Doğu Asya tipografisi için örnek bir kullanımdır.  
Ruby yedek parantez (rp) öğesi: Ruby açıklamalarını görüntülemekte desteklenmeyen tarayıcılar için yedek olarak kullanılır.  
Ruby Metni (rt) öğesi: Ruby açıklaması için metni belirtir; genellikle telaffuz veya çeviri detayları için kullanılır.  
Örnek Kod
<ruby>
    明日 <rp>(</rp><rt>Ashita</rt><rp>)</rp>
</ruby>

Üstü Çizili (s) öğesi: Artık doğru veya geçerli olmayan içeriği temsil etmek için kullanılır.  
Örnek Kod
<p>
    <s>Yarınki yürüyüş öğle saatinde buluşulacaktı.</s>
</p>
<p>
    Öngörülemeyen hava koşulları nedeniyle yürüyüş iptal edilmiştir.
</p>
