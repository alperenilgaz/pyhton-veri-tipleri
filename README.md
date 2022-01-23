# pyhton-veri-tipleri
##matematik operatörleri : 
--------------------------
tamsayı bölmesi (//): Bu operatör, bir sayının başka bir sayıya bölümünden ortaya çıkan bölüm sonucunu vermektedir.
örnek : 13//4 = 3 sonucunu veririr.
kalanı bulma (%) : Bu operatör de , bir sayının başka bir sayıya bölümünden kalan sonucunu bulmamızı sağlar.
örnek : 13 % 4 = 1 sonucunu veririr.
üs bulma (**) : Bu operatör de , bir sayının başka bir sayıya bölümünden kalan sonucunu bulmamızı sağlar.**
örnek : 16**0.5 = 4 sonucunu verir.**
##string oluşturma 
-------------------
--->Şimdi  bir tane string veri tipinde değişken oluşturalım. Stringler de bir veri tipi oldukları için bunlardan değişken oluşturup kullanabiliriz.
örnek : a="alperen"
        a
       konsol bize alperen yazısını bastırır.
       
## String Indeksleme ve Parçalama 
----------------------------------
--->Stringler birer karakter dizileri oldukları için her bir karakterin aslında string içinde bir yeri vardır. Örnek olarak "ali" stringinde a,l ve i karakterlerinin yerleri indeks olarak adlandırılır.Pythonda ve genellikle çoğu programlama dilinde (Octave hariç) stringlerin indekslenmesi "0" dan başlamaktadır. Şimdi isterseniz bir string içindeki karakterlere indeks yoluyla nasıl ulaşacağımıza bakalım.bunun için birkaç örnek çözelim.

1)0. elemana  ulaşalım . Bunun için [] operatörünü kullanacağız.
a="oğuz"
a[0]                                //  **eğer 1 yazarsak ğ harfini 2 yazarsak u harfini 3 yazarasak z harfini bastırır.**
konsol: o harfini bastırır.

2 )Pythonda stringler baştan olduğu gibi sondan da indekslenebilirler. Sondan başlayarak -1,-2 ... şeklinde indekslenirler
örnek : a="atay"
        a[-1] ** eğer -2 yazarsak a harfini -3 yazarsak t harfini -4 yazarasak a harfini bastırır.**
        konsol : y harfini gösterir.
        
3)Peki uzun bir string'in sadece belirli bir kısmını elde etmek için ne yapacağız ? Bunun için indeksleri, : ve [] işaretini kullanacağız. Formülümüz şu şekilde ;
-------------------------------------------------------
| [başlama indeksi : bitiş indeksi : atlama değeri]   |
-------------------------------------------------------
İsterseniz örneklerimize bakalım.
     1.örnek :4.indeksten başla 10.indekse kadar(10 dahil değil) 
        a="tehlikeli oyunlar"
        a[4:10] -------->**bunun anlamı 4. indeksten 10.indekse kadar(10 dahil değil) yazdır ayrıca aradaki boşluğuda bir karakter 
                           olarak alır.**
         konsol : bize 'ikeli ' yazısını verir.
        
     2.örnek : Başlangıç değeri belirtilmemişse en baştan başlayarak alır. 
       a="tehlikeli oyunlar"   
       a[:10] 
       konsol : 'tehlikeli ' yazısını gösterir
    
    3.örnek : Başlangıç değeri belirtilmemişse en baştan başlayarak alır.
     a="tehlikeli oyunlar"   
     a[4:] 
     konsol : 'ikeli oyunlar'  yazısını gösterir   
        
     4.örnek : İki değer de belirtilmemişse tüm stringi al.   
       a="tehlikeli oyunlar"   
       a[:] 
       konsol : 'tehlikeli oyunlar ' yazısını gösterir.
    
     5.örnek : son karaktere kadar al.
        
       a="tehlikeli oyunlar"   
       a[:-1]
       konsol : 'tehlikeli oyunla ' yazısını gösterir.
        
        
        
       6.örnek : Baştan sona 2 değer atlaya atlaya stringi al.
        
       a="tehlikeli oyunlar"   
       a[::2]
       konsol : 'thieioulr' yazısını gösterir.
       
       
        
        
       
       7.örnek : 4.indeksten 12'nci indekse 3'er atlayarak stringi al.
        
       a="tehlikeli oyunlar"   
       a[4:12:3]
       konsol : 'ilo'  yazısını gösterir.
       
        
        
       
       8.örnek :Baştan sona -1 atlayarak stringi al. (String'i ters çevirme)
        
       a="tehlikeli oyunlar"   
       a[::-1] ---->     **kelimeyi tersten yazma kodu**
       konsol : 'ralnuyo ilekilhet'  yazısını gösterir.
       
 ## String Özellikleri
 ----------------------
Bir string'in uzunluğunu nasıl buluruz ? Bunun için Python'da len() fonksiyonu bulunmaktadır.
örnek: 
string="nazım hikmet"
len (string) ----> **boşluğuda bir karakter sayar**
konsol : 12 sayısını bize verir.

Peki, Pythonda stringler toplanabiliyor mu ? Python'da bunu yapmak mümkündür.    
1.örnek : 
"python"*3
konsol : bize 'pythonpythonpython' yazısını verir.

2.örnek: Stringleri toplayalım yani birbirine ekleyelim.
a="necip "
b="fazil "
c="kisakürek "
a+b+c
konsol : 'necip fazil kisakürek' yazisini gösterir
        
        
3.örnek :         
a="oğuz atay "
a+="tutunamayanlar"
a
konsol : oğuz atay tutunamayanlar yazisini gösterir.

=> Bir string ile bir sayıyı da çarpabiliriz.
örnek : 
a="alp=
a*3
konsol :'alpalpalp' yazısını verir.
-----------------------------------------------------------------------------------------------------------------------------------
## Veri tipi dönüşümleri     
------------------------
### 1)Tamsayıyı Ondalıklı Sayıya Çevirme :
------------------------------------
=>Bir string'i bir tamsayıya çevirmek istediğimiz zaman int() fonksiyonunu kullanabiliriz. Ancak biraz dikkatli olmamızda fayda var. Dönüştürme işlemini yaparken stringin herbir karakterinin bir rakam olduğundan emin olmalıyız. Örneklere bakalım.

 örnek  :  a="01235847"
           b=int (a)
           b
           konsol : '01235847' cevabını verir.
        
### 2)Stringleri Ondalıklı Sayıya Çevirme : 
-----------------------------------------
 => Bir string'i bir ondalıklı sayıya çevirmek istediğimiz zaman float() fonksiyonunu kullanabiliriz. Ancak biraz dikkatli olmamızda fayda var. Dönüştürme işlemini yaparken stringin ondalıklı sayı formatına uygun olduğundan emin olmalıyız. Örneklere bakalım.
  
  örnek :  a="1.235847"
           b=float(a)
           b
           konsol : '1.235847' cevabını verir.
        
 ### 3) Sayıları Stringlere Çevirme       
------------------------------------
 => Bir sayıyı string'e çevirmek için str() fonksiyonunu kullanabiliriz.Sayıyı oluşturan tüm rakamlar veya noktalar birer karaktere dönüşecek. Örneklerimize bakacak olursak ;
 
 1.örnek:
 a="32324324"
 b=str(a)
 len(b)
 konsol : '8' cevabının gösterir
        
 2.örnek :
 a=str(3.14) // noktayı da dahil ederek sayar//
 len (a)
 konsol : '4'cevabını verir.
-----------------------------------------------------------------------------------------------------------------------------------
## Print fonksiyonu ve formatlama :(bu kısım çoooooook önemli)
--------------------------------
Bu bölümde ekrana veri tiplerini yazdırmak için kullandığımız print() fonksiyonunu ve formatlama yöntemlerini öğreneceğiz.
 
### 1) Print() Fonksiyonu :
----------------------------
Kodlarımızı dosyalara yazdığımızda, eğer ekrana bir değer bastırmak istersek print fonksiyonunu kullanırız. Kullanımı oldukça basittir ve değişik özelliklere sahiptir. Örneklerimize bakalım.

örnek 1 : 
a=4
b=5
print(a+b)
konsol = 9 cevabını bize verir.

Buradaki işlemde  gördüğümüz gibi biz print fonksiyonunun içine bastırmak istediğimiz değeri veriyoruz ve bu fonksiyon da ekrana değerimizi bastırıyor. Peki aynı satırda birkaç değer bastırmak istersek ne yapıyoruz? Bunun için değerlerimizin arasına , karakterini atıyoruz. Örnek yapacak olursak

1.örnek :
print(3.14+2)
konsol = 5.14 cevabını veirir.

2.örnek :
print("alperen ılgaz")
konsol bize alperen ılgaz yazısını aynen gösterir.

Peki aynı satırda birkaç değer bastırmak istersek ne yapıyoruz? Bunun için değerlerimizin arasına , karakterini atıyoruz.

örnekler :
----------
1)print("alperen",5,12,39)
  konsol  bize ' alperen 5 12 39 'yazısını gösterir(eğere hepsi tırnak içinde olsaydı alperen ,5,12,39 şeklinde bastırırdı.)
  
 2)print("necip","fazil","kısakürek")         
   konsol= necip fazil kısakürek yazısını gösterir. 

## Stringlerdeki Özel Karakterler
----------------------------------------
Pythonda stringlerde kullanılan özel karakterler mevcuttur ve kullanıldıkları yerler de işlerimizi kolaylaştırır. En çok kullanılan 2 tanesi şunlardır;

 ### 1) \n karakteri
--------------------
Eğer print() fonksiyonu stringlerde böyle bir karakterle karşılaşırsa alt satırdan ekrana yazdırma işlemine devam eder. Hemen örneklerimize bakalım.
örnekler

1)print("alperen\nılgaz\nsoftware")
  konsol = 
  alperen
  ılgaz
  software
yazısını bize gösterir.

 ### 2) \t karakteri
--------------------
Eğer print() fonksiyonu stringlerde böyle bir karakterle karşılaşırsa bir tab boşluk bırakarak ekrana yazdırma işlemine devam eder. Hemen örneklerimize bakalım.
örnekler : 

1) print("Ocak\tMart\tŞubat")
   konsol: ocak   mart   şubat
   
## type() fonksiyonu
--------------------
print() fonksiyonundan bahsetmişken type() fonksiyonunu öğrenmekte fayda var. type() fonksiyonu içine gönderilen değerin hangi veri tipinden olduğunu söyler.

1) Integer (Tamsayı) türü
a=65
print(type(a))
konsol = <class 'int'> yazısını verir.
 
2)Float (Ondalıklı Sayı) türü
  a=5.87
  konsol = <class 'float'>  yazısını verir.

3)String (Karakter Dizisi) türü 
  a = "alperen"
  print(type(a)) 
   konsol =  <class 'str'> yazısını verir.
   
## Print() Fonksiyonunun Özellikleri
---------------------------------------
Ekrana yazdırma işlemlerimiz sırasında print() fonksiyonunun faydalı özelliklerini kullanırsak yazdığımız kodu daha verimli kılabiliriz. Bunun için burada 2 tane özellikten bahsedeceğiz.

### 1) sep parametresi
------------------------
=> print() fonksiyonunda kullanılabilen sep parametresi yazdırdığımız değerlerin arasına istediğimiz karakterlerin yerleştirilmesini sağlar. Eğer bu parametreyi kullanmazsak değerlerin arasına varsayılan olarak boşluk yerleştirildiğini biliyoruz.Örneklere bakalım.

örnekler

1)print(3,4,5,6,7,8,9)
  konsol = 3 4 5 6 7 8 9

2)sep parametresi sayesinde değerlerin arasına nokta konuyor.
  print(3,4,5,6,7,8,9,sep = ".")
   konsol = 3.4.5.6.7.8.9
 
3)Değerlerin arasında "/" sembolü yerleştiriliyor.
  print("06","04","2015",sep = "/")
     konsol = 06/04/2015

### 2) Yıldızlı Parametreler
----------------------------
=>Eğer bir stringin başına * işareti koyup, print fonksiyonuna gönderirsek bu string karakterlerine ayrılacak ve her bir karakter ayrı birer string olarak davranılarak ekrana basılacaktır.
örnekler
1) Varsayılan olarak karakterlerin arasına boşluk konuluyor.
   print(*"Python")
   konsol = P y t h o n

2)print(*"Python",sep = "\n")
     konsol =P
             y
             t
             h
             o
             n 


## Formatlama
-------------
=>Programlama yaparken bazı yerlerde bir stringin içinde daha önceden tanımlı string,float, int vs. değerleri yerleştirmek isteyebiliriz. Böyle durumlar için Pythonda format() fonksiyonu bulunmaktadır. Örneğin, programımızda 3 tane tamsayı değerimiz var ve biz bunları bir string içinde ekrana basmak istiyoruz. Bunun için format() fonksiyonunu kullanabiliriz. format() fonksiyonunun çok fazla özelliği olduğu için, ben burada sadece en çok kullandığımız özelliğini göstereceğim.

örnekler :

1)Burada 3 tane süslü parantezimiz ({}) var ve bunların yerine sırasıyla format fonksiyonun içindeki değerler geçiyor.
  "{} {} {}".format(3.1423,5.324,7.324324)
       konsol = '3.1423 5.324 7.324324' 

2)a = 3
  b = 4
  print("{} + {} 'nin toplamı {} 'dır".format(a,b,a+b))
  konsol =  3 + 4 'nin toplamı 7 'dır

3) Süslü parantezlerin içindeki sayılar format fonksiyonun içinden hangi sıradaki değerin geleceğini söylüyor.

   "{1} {0} {2} ".format(20,"alperen","yaşında")
     konsol = 'alperen 20 yaşında '

4)üslü parantezlerin içindeki kullanım ondalıklı kısmın sadece 2 basamağına kadar almak istediğimiz söylüyor.
  
  "{:.2},{:.3},{:.4}".format(3.85687,7.98754,1.1212) //ondalıktan sonra :.x basamağa kadar x.indeks dahil değil//
   konsol = '3.9,7.99,1.121'
   
--------------------------------------------------------------------------------------------------------------------------------   ## Listeler :
---------------------
  Şimdi de yeni bir veritipimiz olan listeleri öğrenmeye çalışalım. Listeler yapıları gereği stringlere oldukça benzerler ve kullanıldıkları yerler de çok yararlı olan bir veritipidir. Tıpkı stringler gibi ,indekslenirler,parçalanırlar ve üzerinde değişik işlemler yapabildiğimiz metodlar bulunur. Ancak listelerin stringlerden önemli farkları da bulunmaktadır. Stringler konusundan bildiğimiz kadarıyla stringler değiştirilemez bir veri tipidir. Ancak, listelerimiz değiştirilebilir bir veritipidir.

Bir listede her veritipinden elemanı saklayabiliriz. Bu anlamda sıralı bir diziye benzer. Peki bu konuda ne öğreneceğiz?

       1.Liste oluşturma
       2.Indeksleme ve Parçalama
       3.Temel Liste Metodları ve İşlemleri
       4.İç içe Listeler                                             
   
   ### 1) Liste Oluşturma :
   ---------------------
   Listeler bir [] köşeli parantez içine veriler veya değerler konarak oluşturulabilir.
   
   örnekler;
   
   1)liste değişkeni. Değişik veri tiplerinden değerleri saklayabiliyoruz.
     liste =  [3,4,5,6,"Elma",3.14,5.324]
     liste
     konsol = [3, 4, 5, 6, 'Elma', 3.14, 5.324]   
   
   2) Boş liste
      bos_liste = []
      bos_liste
      konsol = []
   
   3)len fonksiyonu listeler üzerinde de kullanılabilir.
     liste3 = [3,4,5,6,6,7,8,9,0,0,0]
     len(liste3)
     konsol = 11
   
   !!önemli not!! : Bir string list() fonksiyonu yardımıyla listeye dönüştürülebilir.
   örneğin;
   
   s =  "Merhaba"
   lst =  list(s)
   lst
   konsol = ['M', 'e', 'r', 'h', 'a', 'b', 'a']
   
   
  ## Listeleri Indeksleme ve Parçalama
----------------------------------------
 Listeleri indeksleme ve parçalama stringlerle birebir olarak aynıdır.
 örneğin bir liste tanımlayıp ona değer verip sonrasında [x] şeklinde indeksliyip (stringlerdeki gibi sıfırdan başlar saymaya)
 x değerine göre listeyi parçalayabiliriz.
 
 örnekler:
 ---------
  1) liste = [3,4,5,6,7,8,9,10]
     liste
     konsol = [3, 4, 5, 6, 7, 8, 9, 10]
   
   2)5.eleman
     liste[4]
     konsol = 7
   
   3)Sonuncu Eleman
     liste[len(liste)-1] // bunu liste[-1] şeklinde de bastırabiliriz. //
     konsol = 10
   
   4)İlk Eleman
     liste[-len(liste)]
     konsol: 3
   
## Temel Liste Metodları ve İşlemleri   
  Bu kısımda da listelerde yapabileceğimiz temel işlemleri ve bazı temel metodları öğreneceğiz. Listelerin daha bir çok metodunu kursun ileriki kısımlarında görüyor olacağız.

Bir listeyi birbirine toplama işlemini stringlerdeki gibi yapabiliriz. 
   
   örneğin;
   1)liste1 =  [1,2,3,4,5]
     liste2 =  [6,7,8,9,10]
     liste1 + liste2
     konsol=  [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
   
   !Bir listeye bir tane eleman eklemek içinse aşağıdaki işlemi uygulayabiliriz.
   
   liste = [1,2,3,4]
   liste =  liste + ["alperen"]
   liste
   konsol = [1, 2, 3, 4, 'alperen']
   
   not => Listeler direk olarak değiştirilebilirler.
   örneğin;
   liste[0] = 10
   liste
   [10, 2, 3, 4, 'alperen']
   
  ** Şöyle bir kullanım da mümkündür.
   liste[:2] = [40,50] // 3.elemandan sonra 40,50 elamanı koy ve geri kalan elemanları yaz//
   liste
   konsol : [40, 50, 3, 4, 'alperen']
   
  ** Bir listeyi bir tamsayıyla da çarpabiliriz.

   liste = [1,2,3,4,5]
   liste * 3
   konsol = [1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5]
   
   
  * Bir listeyi bir tamsayıyla da çarpabiliriz. //ama listemiz yine değişmez//
   liste = [1,2,3,4,5]
   liste * 3
   konsol = [1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5]
   
   !!!Şimdi de isterseniz temel bazı liste metodlarına bakalım. Listeler, diğer programlama dillerindeki arraylere göre oldukça esnektir. Belli bir boyutları yoktur ve ekleme, çıkarma yapmak oldukça kolaydır.
   
## append(ekleme) metodu
----------------
append metodu, verdiğimiz değeri listeye eklememizi sağlar
örneğin;
liste = [3,4,5,6]
liste.append(7)
liste

konsol = [3, 4, 5, 6, 7]

liste.append("alperen")
liste
konsol = [3, 4, 5, 6, 7, 'alperen']

## pop metodu
--------------
Bu metod, içine değer vermezsek listenin son indeksindeki elemanı, değer verirsek verdiğimiz değere karşılık gelen      indeksteki elemanı listeden atar ve attığı elemanı ekrana basar.
örneğin;
liste = [1,2,3,4,5] 
liste.pop()//eğer pop'un içine değer verilmemişse sondaki elemanı atar ve listeyi son haliyle bastırır.//
liste
konsol=1,2,3,4 

##sort(çeşit) metodu
--------------------
=>sort metodu listenin elemanlarını sıralamamızı sağlar. Hemen kullanımına bakalım.
1)

liste = [34,1,56,334,23,2,3,19]
liste.sort()  //Küçükten büyüğe sıralar.//
liste

2)liste.sort(reverse = True) // Büyükten küçüğe sıralar.//


3)liste = ["Elma","Armut","Muz","Kiraz"]
liste.sort() //Alfabetic olarak küçükten büyüğe//
liste

4)liste = ["Elma","Armut","Muz","Kiraz"]
liste.sort(reverse = True) //Alfabetic olarak büyükten küçüğe// 
liste

## İç içe Listeler
=> Bir listenin içinde başka bir liste bulundurmak mümkündür. Bunlara Pythonda içiçe listeler denmektedir. Bu tip bir özellik, Pythonda ağaç yapılarında veya matris yapılarında oldukça kullanışlı olmaktadır.


** 3 Tane liste oluşturalım.

liste1 = [1,2,3]
liste2 = [4,5,6]
liste3 = [7,8,9]

yeniliste = [liste1,liste2,liste3]
yeniliste
Şimdi, 2. listenin ilk elemanına nasıl ulaşacağımıza bakalım.

** 1.elemanın 0.elemanı
yeniliste[1][0]

## Demetler (Tuplelar)
-----------------------
Demetler veya İngilizce ismiyle tuplelar listelere oldukça benzer ancak farkları demetlerin değiştirilemez oluşudur. Bu yüzden programlarımızda değiştirilmesini istemediğimiz değerleri bir demet içinde depolayabiliriz. İsterseniz konumuza demetlerin oluşturulmasıyla başlayalım.

### Demet Oluşturma
---------------------
Demet elemanları parantez içine alınarak demet oluşturulabilir.
demet = (1,2,3,4,5,6,7,8,9)
demet
konsol = (1, 2, 3, 4, 5, 6, 7, 8, 9)
 type() fonksiyonu yardımıyla türünü öğrenelim.
 type(demet)
 konsol = tuple

not : demetlerde belli bir indekse ulaşma listelerle neredeyse aynıdır.

## Demetlerin Temel Metodları
------------------------------
index metoduyla içine verdiğimiz elemanın hangi indekste olduğunu bulabiliriz.
*Demeti oluşturalım.
demet = (1,2,3,"Mustafa","Murat","Coşkun")
* "Mustafa" elemanının indeksini buluyoruz.
demet.index("Mustafa").
konsol = 3 

!!!! count metoduyla içine verdiğimiz değerin demette kaç defa geçtiğini bulabiliriz.
örneğin;

demet = (1,23,34,34,2,1,4,5,1,1,34)
demet.count(1)
konsol = 4
demet.count(34)
konsol = 3

### Değiştirilmeme Özelliği
-----------------------------
Demetlerin değiştirilemez olduğunu artık biliyoruz


## Demetleri Ne Zaman Kullanalım ?
-----------------------------------
Aslında Python programcıları demetlerden ziyade listeleri daha çok kullanır. Ancak eğer programınızda değiştirilmesini istemediğiniz bilgiler varsa (Android uygulama sabitleri gibi) bunları demet içinde depolayabilirsiniz. Aynı zamanda, Read Only(Sadece Okuma) bir veritipi olduğu için listelere göre biraz daha hızlı çalışırlar.


























































