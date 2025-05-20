HTML ses ve video öğelerinin rolleri nelerdir ve nasıl çalışırlar?

Ses ve video öğeleri, HTML belgelerinize ses ve video içeriği eklemenizi sağlar. Ses öğesi mp3, wav ve ogg gibi popüler ses formatlarını destekler. Video öğesi mp4, ogg ve webm formatlarını destekler.

Web sayfanıza ses içeriği eklemek için, ses dosyanızın konumunu gösteren src özelliğine sahip ses öğesini kullanabilirsiniz:

```html
<audio src="CrystalizeThatInnerChild.mp3"></audio>
```
Bu örneği çalıştırmayı denerseniz, sayfada hiçbir şeyin görünmediğini göreceksiniz. Ancak, sayfayı geliştirici araçlarıyla incelerseniz, ses öğesinin gerçekten sayfada olduğunu göreceksiniz. Ses oynatıcısını sayfada görmek istiyorsanız, controls özelliğine sahip ses öğesini ekleyebilirsiniz:

```html
<audio src="CrystalizeThatInnerChild.mp3" controls></audio>
```
Controls özelliği, kullanıcıların ses çalmayı yönetmesine, ses seviyesini ayarlamasına ve çalmayı duraklatmasına veya devam ettirmesine olanak tanır. Controls özelliği, yerleşik çalma kontrollerini etkinleştirmek için bir öğeye eklenebilen bir boole özelliğidir. Atlanırsa, hiçbir kontrol gösterilmez.

src ve controls özelliklerinin yanı sıra, ses öğesinin işlevselliğini artıran birkaç başka özellik daha vardır. loop özelliği, sesin sürekli olarak yeniden çalınmasını sağlayan bir boole özelliğidir. İşte Quincy Larson'ın "Can't stay down" adlı şarkılarından birini çalmak için loop özelliğini kullanan bir örnek:

```html
<audio
  src="https://cdn.freecodecamp.org/curriculum/js-music-player/can't-stay-down.mp3"
  loop
  controls
></audio>
```
Şarkı sona erdiğinde, başa dönecek ve baştan tekrar çalacaktır. Kullanabileceğiniz başka bir özellik de muted özelliğidir. Ses öğesinde mevcut olduğunda, bu boole özelliği sesi sessiz durumda başlatacaktır. İşte muted özelliğini kullanan bir örnek:

```html
<audio
  src="https://cdn.freecodecamp.org/curriculum/js-music-player/can't-stay-down.mp3"
  loop
  controls
  muted
></audio>
```
Şarkıyı tarayıcıda başlattığınızda hiçbir şey duymayacaksınız. Müziği duymak için ses simgesine tıklamanız gerekecektir.

Ses dosyası türleri söz konusu olduğunda, tarayıcıların hangi türü desteklediği konusunda farklılıklar vardır. Bunu karşılamak için, ses öğesinin içinde kaynak öğelerini kullanabilirsiniz ve tarayıcı anladığı ilk kaynağı seçecektir. İşte bir ses öğesi için birden fazla kaynak öğesi kullanma örneği:

```html
<audio controls>
  <source src="audio.ogg" type="audio/ogg" />
  <source src="audio.wav" type="audio/wav" />
  <source src="audio.mp3" type="audio/mpeg" />
</audio>
```
Tarayıcı önce ogg türüyle başlayacak ve sesi çalamazsa listedeki bir sonraki türe geçecektir.

Şimdiye kadar öğrendiğimiz tüm özellikler video öğesinde de desteklenmektedir. İşte loop, controls ve muted özelliklerine sahip bir video öğesi kullanma örneği:

```html
<video
  src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
  loop
  controls
  muted
></video>
```
Src veya kaynak özelliği için archive.org'dan "Big Buck Bunny" adlı bir video kullanıyoruz. Video indirilirken bir resim görüntülemek isterseniz, poster özelliğini kullanabilirsiniz. Bu özellik ses öğeleri için mevcut değildir ve video öğesine özgüdür. İşte peach.blender.org tarafından sağlanan içerikle poster özelliğini kullanma örneği:

```html
<video
  src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
  loop
  controls
  muted
  poster="https://peach.blender.org/wp-content/uploads/title_anouncement.jpg?x11217"
  width="620"
></video>
```
Bu örnek ayrıca, videonun ekrana daha iyi sığması için genişliği 620 piksel olarak ayarlamak üzere width özelliğini de kullanıyor.

## freecodecamp