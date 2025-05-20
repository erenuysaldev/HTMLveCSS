Videoları iframe öğesini kullanarak sayfanıza nasıl eklersiniz?

Öncelikle, iframe öğesi tam olarak nedir? iframe, satır içi çerçeve anlamına gelir. Diğer HTML içeriğini doğrudan HTML sayfasına eklemek için kullanılan bir satır içi öğedir. Bu HTML içeriği bir video, harita, başka bir HTML öğesi ve hatta diğer web sayfaları olabilir. İşte iframe öğesinin sözdizimi şöyledir:

```html
<iframe
  src="video-url"
  width="genişlik-değeri"
  height="yükseklik-değeri"
  allowfullscreen
></iframe>
```
`src` özelliği, eklemek istediğiniz sayfanın URL'sini belirtir. `width` özelliği, iframe'in genişliğini belirtir. `height` özelliği, iframe'in yüksekliğini belirtir. `allowfullscreen` özelliği, kullanıcının iframe'i tam ekran modunda görüntülemesine olanak tanır. Erişilebilirlik için önemli olduğundan, iframe için bir `title` özelliği belirtmek de iyi bir uygulamadır.

Bir iframe içine video eklemek için, YouTube ve Vimeo gibi popüler video hizmetlerinden doğrudan kopyalayabilir veya o videonun URL'sini gösteren `src` özelliğiyle kendiniz tanımlayabilirsiniz. İşte YouTube'dan popüler bir freeCodeCamp kursunu ekleme örneği:

```html
<h1>iframe Öğesiyle Eklenmiş bir freeCodeCamp YouTube Videosu</h1>

<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/PkZNo7MFNFg?si=-UBVIUNM3csdeiWF"
  title="YouTube video oynatıcı"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  referrerpolicy="strict-origin-when-cross-origin"
  allowfullscreen
></iframe>
```
Ardından iframe'i ihtiyaçlarınıza göre özelleştirebilir veya YouTube videosunun bağlantısını kopyalayıp URL değeri olarak yapıştırarak kendinizinkini tanımlayabilirsiniz. Dikkat edilmesi gereken nokta, `https://youtu.be` adresini `https://youtube.com/embed/` ile değiştirmeniz gerektiğidir.

`youtu.be`, paylaşım bağlantısını kopyaladığınızda kullanılan alandır ve `youtube.com/embed/`, videoları iframe öğesiyle eklemek için gereken alandır. İşte bunun bir örneği:

```html
<iframe
  src="https://youtube.com/embed/gp5H0Vw39yw?si=Rb_2nDK6abv1iIAM"
  title="freeCodeCamp Typescript Kursu"
  width="500"
  height="285"
  allowfullscreen
></iframe>
```
Videonun herhangi bir yerden gelebileceğini unutmayın. YouTube ve Vimeo gibi video hizmetlerinden gelmek zorunda değildir. İşte iframe öğesiyle eklenmiş Pixabay'den bir video:

```html
<h1>iframe Öğesiyle Eklenmiş Pixabay'den Bir Video</h1>

<iframe
  src="https://cdn.pixabay.com/video/2022/07/24/125310-733046613_large.mp4"
  width="500"
  height="285"
></iframe>
```
iframe öğesi içine bir harita, başka bir web sayfası veya doğrudan HTML de ekleyebileceğinizi unutmayın. İşte iframe öğesiyle ekleyebildiğim bir harita:

```html
<h1>iframe Öğesiyle Eklenmiş Openstreetmap.org'dan Bir Harita</h1>

<iframe
  width="425"
  height="350"
  src="https://www.openstreetmap.org/export/embed.html?bbox=3.006134033203125%2C6.150112578753815%2C3.6357879638671875%2C6.749850810550778&amp;layer=mapnik"
  style="border: 1px solid black"
>
</iframe>
<br />
<small>
  <a href="https://www.openstreetmap.org/#map=11/6.4501/3.3210">
    Daha Büyük Haritayı Görüntüle
  </a>
</small>
```
iframe öğesi içine doğrudan HTML eklemek istiyorsanız, `src` yerine `srcdoc` özelliğini kullanmanız gerekir.
## freecodecamp