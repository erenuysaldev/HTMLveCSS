HTML tabloları ne için kullanılır ve ne için kullanılmamalıdır?

HTML tabloları bugünlerde eskiden olduğu kadar çok kullanılmıyor. Ancak, bir ön uç geliştiricisi olarak, yine de onlara aşina olmalısınız. Tablolar, 1990'larda geliştiricilerin tarayıcıda veri görüntülemek için kullandıkları en eski yöntemlerden biriydi.

İşte ABD Çalışma İstatistikleri Bürosu'ndan bir tablo oluşturmak için kullanılan bir kod örneği:
```
<table id="quickfacts">
  <thead>
    <tr>
      <th colspan="2">Quick Facts: Software Developers, Quality Assurance Analysts, and Testers</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2023 Median Pay</th>
      <td>
        $130,160 per year
        <br>$62.58 per hour
      </td>
    </tr>
    <tr>
      <th>Typical Entry-Level Education</th>
      <td>Bachelor's degree</td>
    </tr>
    <tr>
      <th>Work Experience in a Related Occupation</th>
      <td>None</td>
    </tr>
    <tr>
      <th>On-the-job Training</th>
      <td>None</td>
    </tr>
    <tr>
      <th>Number of Jobs, 2022</th>
      <td>1,795,300</td>
    </tr>
    <tr>
      <th>Job Outlook, 2022-32</th>
      <td>25% (Much faster than average)</td>
    </tr>
    <tr>
      <th>Employment Change, 2022-32</th>
      <td>451,200</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <th>If this table had a footer it would be here.</th>
    </tr>
  </tfoot>
</table>
```
Gördüğünüz gibi, kimliği quickfacts olarak ayarlanmış bir ana tablo öğesi var. Tablonun içinde bir tablo başı öğesi, thead, tablo gövdesi öğesi, tbody ve bir tablo ayağı öğesi, tfoot vardır.

Tablo başlığı, gövdesi ve ayağı öğelerinin her biri belirli sayıda tablo satırı içerebilir, tr. Ve her tablo satırı, o satırdaki verileri etiketleyen bir tablo başlığı içerebilir. Ayrıca, tablo verileri (td) olarak adlandırılan belirli sayıda ayrı veri hücresi de içerebilir.

Şimdi, bu çok fazla HTML öğesi. Ancak gözünüz korkmasın - bunlar basit bir hiyerarşi izler.

İşte tüm bu öğeleri içeren oluşturabileceğimiz en basit tablo:
```
<table>
  <thead>
    <tr>
      <th>The title of this table</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>First Row</th>
      <td>
        First Data Cell
      </td>
    </tr>
    <tr>
      <th>Second Row</th>
      <td>
        Second Data Cell
      </td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <th>The footer of this table, which might contain date of publication, author credits, or other meta information.</th>
    </tr>
  </tfoot>
</table>
```
Gördüğünüz gibi, verinin kendisi her zaman bir tr öğesinin içindedir - ve bu tr öğesinin içinde bir başlık içeren bir th öğesi ve veri içeren bir td öğesi bulunur.

Bazı web siteleri, daha uygun olan tablo öğesini kullanmak yerine kendi tablolarını oluşturmak için div'leri kullanmayı tercih eder.

Genel div öğelerini kullanarak tablo şeklindeki verileri görüntülemek mümkün olsa da, bunun yerine tablo öğesini kullanmak daha iyidir.

Yıllar önce, geliştiriciler bir web sayfasındaki veri olmayan öğeleri konumlandırmak için bir tablo kullanabilirdi. Bu hiçbir zaman en iyi uygulama olarak görülmedi. Ancak tabloların hala bu şekilde kullanıldığı bazı kod tabanlarına rastlayabilirsiniz.

Günümüzde geliştiriciler tasarımlarını düzenlemek için CSS flexbox ve grid kullanmaktadır. freeCodeCamp bu araçları daha sonra derinlemesine ele alacaktır.

Şimdilik HTML tablolarını asıl amaçları için kullanın: tablo şeklindeki verileri görüntülemek.