Eda Nur Işık</p>
ednurisk0@gmail.com


## Untitled-3 Çalıştırma Rehberi

Çalıştırma Adımları:

-Veri setinizi hazırlayın, projenin bulunduğu aynı klasöre koyun.

-Python Kodunu Çalıştırın:

-Pipeline içerisine (file_path parametresine) veri setinizin yolunu yazarak çalıştırabilirsiniz

<br> <br>

## Analysis Klasörü

🧹 Veri Temizleme ve Ön İşleme

🔧 Özellik Dönüşümleri

<br>


Cinsiyet:

Eksik değerler kontrol edildi.

Kadın ve Erkek kategorileri 0–1 binary encoding ile Cinsiyet_Binary sütununa dönüştürüldü.

<br>


Yaş:

Aykırı değerler incelendi.

YasGrubu adında yeni bir sütun oluşturuldu (örn. 0–18, 19–35, 36–50, 50+).

Yaş grubu kategorileri numerik kodlara dönüştürüldü.  

<br>


Kan Grubu:

Kan grubu verisi iki ayrı özellik haline getirildi:

KanGrubu_Tipi (A, B, AB, 0)

Rh_Tipi (+/-)

Böylece modelde ayrı ayrı kullanılabilir hale getirildi.

<br>


Uyruk:

Tekrarlayan değerler düzenlendi.

One-hot encoding uygulanarak her uyruk için ayrı bir sütun oluşturuldu.

<br>


Kategorik Kolonlar (KronikHastalik, Bolum, Alerji, Tanilar, TedaviAdi, UygulamaYerleri):

Veriler normalize edilerek standart hale getirildi (örneğin aynı hastalık farklı yazımlarda tekilleştirildi).

Listeleme yapılarak her satırda çoklu girişlerin düzgün biçimde tutulması sağlandı.

<br>


Uygulama Süresi:

Farklı formatlarda girilmiş değerler normalize edilerek tek bir zaman birimine çevrildi.

Gerekli görülen yerlerde min-max normalizasyon uygulandı.

<br>


📊 Keşifsel Veri Analizi (EDA)

Yaş, cinsiyet, kan grubu ve uyruk dağılımları görselleştirildi.

Kronik hastalıklar ve uygulama yerleri için en çok tekrar eden değerler listelendi.

Tedavi süreleri ve uygulama sürelerinin dağılımları incelendi.

Bölüm bazında hasta yoğunlukları ve tedavi süreleri karşılaştırıldı.
