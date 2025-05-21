HTML'de saat ve tarihleri nasıl gösterirsiniz?

time elementi, belirli bir anı temsil etmek için kullanılır.

İşte, time elementi kullanarak yirmi yüz saat yani akşam sekiz'i temsil eden bir örnek:

<p>Rezervasyonlar <time datetime="20:00">20:00</time> içindir.</p>

datetime özniteliği, tarih ve saat bilgisini makine tarafından okunabilir formata çevirmek için kullanılır. Bu, arama motoru sonuçları ve tarayıcının tarih ile saat bilgisini daha etkili biçimde işlemesine yardımcı olur.

datetime özniteliğinin değeri; geçerli bir yıl, geçerli bir ay, geçerli bir saat, yerel tarih, global tarih veya geçerli bir süre dizesi olmalıdır.

Belirli bir tarihi temsil etmek için time elementinin başka bir örneği:

<p>
    Mezuniyet <time datetime="2024-06-15T15:00">15 Haziran</time> tarihinde gerçekleşecek.
</p>

datetime özniteliğinin değeri ISO 8601 formatındadır. ISO 8601, tarih ve saatleri temsil etmek için uluslararası bir standarttır. Bu değerin ilk kısmı yıl, ay ve günü belirtir. Değer içindeki büyük T, tarih ile saat arasında bir ayırıcıdır.

15:00, öğleden sonra üçü ifade eder.

Etkinlikleri, yayın tarihlerini veya randevuları temsil etmek gerektiğinde, time elementini kullanmak en iyisidir.
