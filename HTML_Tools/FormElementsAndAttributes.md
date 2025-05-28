HTML Form Öğeleri ve Nitelikleri
form öğesi: kullanıcı girişi için bir HTML formu oluşturmak için kullanılır.
action niteliği: form verilerinin gönderileceği URL'yi belirtmek için kullanılır.
method niteliği: form verilerini gönderirken kullanılacak HTTP yöntemini belirtmek için kullanılır. En yaygın yöntemler GET ve POST'tur.
```
<form method="value-goes-here" action="url-goes-here">
  <!-- inputs go inside here -->
</form>
```
input elemanı: kullanıcı girişi için bir giriş alanı oluşturmak için kullanılır.
type niteliği: giriş alanının türünü belirtmek için kullanılır. Örn. metin, e-posta, sayı, radyo, onay kutusu, vb.
placeholder niteliği: kullanıcıya giriş alanına ne gireceğini gösteren bir ipucu göstermek için kullanılır.
value niteliği: girişin değerini belirtmek için kullanılır. Girdinin bir düğme türü varsa, value niteliği düğme metnini ayarlamak için kullanılabilir.
size niteliği: kullanıcı girdiye yazarken görünür olması gereken karakter sayısını tanımlamak için kullanılır.
min niteliği: girdi alanında izin verilen minimum değeri belirtmek için sayı gibi girdi türleriyle kullanılabilir.
max niteliği: girdi alanında izin verilen maksimum değeri belirtmek için sayı gibi girdi türleriyle kullanılabilir.
minlength niteliği: bir girdi alanında gereken minimum karakter sayısını belirtmek için kullanılır.
maxlength niteliği: bir girdi alanında izin verilen maksimum karakter sayısını belirtmek için kullanılır.
required niteliği: formu göndermeden önce bir girdi alanının doldurulması gerektiğini belirtmek için kullanılır.
disabled niteliği: bir girdi alanının devre dışı bırakılması gerektiğini belirtmek için kullanılır.
readonly niteliği: bir girdi alanının salt okunur olduğunu belirtmek için kullanılır.
```
<!-- Text input -->
<input 
  type="text"
  id="name"
  name="name"
  placeholder="e.g. Quincy Larson" 
  size="20"
  minlength="5"
  maxlength="30"
  required
/>

<!-- Number input -->
<input
  type="number"
  id="quantity"
  name="quantity"
  min="2"
  max="10"
  disabled
/>

<!-- Button -->
<input type="button" value="Show Alert" />
```
label elemanı: bir girdi alanı için etiket oluşturmak için kullanılır.
for niteliği: etiketin hangi girdi alanı için olduğunu belirtmek için kullanılır.
Örtük form ilişkilendirmesi: girişler, giriş alanının etiket öğesinin içine sarılmasıyla etiketlerle ilişkilendirilebilir.