Satır içi, dahili ve harici CSS nedir ve her birini ne zaman kullanmalısınız?

CSS bir web sayfasına üç ana şekilde uygulanabilir: satır içi, dahili veya harici.

Her yöntemin kendine özgü kullanım durumu, avantajları ve sınırlamaları vardır ve her birini ne zaman kullanacağınızı bilmek temiz, verimli ve sürdürülebilir kod yazmak için önemlidir.

Üç CSS türünü ve bunları ne zaman kullanmanız gerektiğini inceleyelim.

Satır içi CSS, style niteliği kullanılarak doğrudan bir HTML öğesinin içine yazılır. Belirli bir öğeye stiller uygular.

Satır içi CSS kullanan bir örnek:
```
<p style="color: red;">This is an inline-styled paragraph.</p>
```
Bu örnekte, paragraf metnini kırmızıya ayarlamak için style niteliğini kullanıyoruz.

Satır içi CSS genellikle hızlı, tek seferlik stiller için veya belirli bir öğe için diğer stilleri geçersiz kılmak için kullanılır.

Ancak, çoğu durumda kaçınılmalıdır çünkü HTML'yi karıştırabilir ve kodun bakımını zorlaştırabilir.

Çoğu zaman, stillerinizi düzenli ve bakımı kolay tutmak için dahili veya harici CSS kullanmak daha iyidir.

Dahili CSS, bir HTML belgesinin başlık bölümündeki style etiketlerinin içine yazılır. Stilleri tüm sayfaya uygular ve tek bir belgeyi biçimlendirmeniz gerektiğinde kullanışlıdır.

İşte dahili CSS'ye bir örnek:
```
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
<body>
  <p>This paragraph is styled using internal CSS.</p>
</body>
```
