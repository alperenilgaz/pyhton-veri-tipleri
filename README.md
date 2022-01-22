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
a[0] **eğer 1 yazarsak ğ harfini 2 yazarsak u harfini 3 yazarasak z harfini bastırır.**
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
     1.örnek :4.indeksten başla 10.indekse kadar(dahil değil) 
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
       a[::-1]
       konsol : 'ralnuyo ilekilhet'  yazısını gösterir.
       
 ## String Özellikleri
 ----------------------
Bir string'in uzunluğunu nasıl buluruz ? Bunun için Python'da len() fonksiyonu bulunmaktadır.
Peki, Pythonda stringler toplanabiliyor mu ? Python'da bunu yapmak pythonda mümkündür.    

1.örnek: Stringleri toplayalım yani birbirine ekleyelim.
a="necip "
b="fazil "
c="kisakürek "
a+b+c
konsol : necip fazil kisakürek yazisini gösterir
        
        
2.örnek :         
a="oğuz atay"
a+="tutunamayanlar"
a
konsol : oğuz atay tutunamayanlar yazisini gösterir.

=> Bir string ile bir sayıyı da çarpabiliriz.
örnek : 
a="alp=
a*3
konsol :'alpalpalp' yazısını verir.
        
        
        
        
        
        
        
        
       
