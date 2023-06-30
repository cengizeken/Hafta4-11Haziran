# 11 Haziran Çalışmaları

**11 Haziran** çalışmaları aşağıdaki linklerde verilen videolar üzerinden yapılacaktır.

###HTML5

- [Türkçe][Türkçe Video Linki]
- [Ingilizce][İngilizce Video Linki]


[Türkçe Video Linki]: https://www.youtube.com/watch?v=dBs_56iLkek&list=PLOCdSnI35cN-g7JuPVn5xWNrNVzZxmdJw
[İngilizce Video Linki]: https://www.youtube.com/watch?v=g3L2jUmnuNA&list=PLS1QulWo1RIbU9SCKLXBou3-p6LZye5L_

##Ders21 CSS3 Çoklu Element Seçici

Ortak Özelliklere sahip elementlere ayrı ayrı CSS uygulamak yerine aralarına virgül konularak tek seferde stil uygulanabilir.

bir elemente id verdiğimiz zaman ona tanımlayıcı bir kimlik vermiş oluruz. Hem CSS hemde JS tarafında sıklıkla kullanılır.

p::after-->elemanın içeriğinden sonra ekleme yap
p::before-->elemanın içeriğinden önce ekleme yap
p:first-letter-->elemanın ilk harfini seç
p::selection-->kullanıcı tarafından seçilen elemanı hedefler
p:first-letter-->hedeflenen elementin ilk satırını seç

##Ders22 PSeudo Classes
a:active->element özelliği aktif hale geçtiği anda stil uygulaması yapar
option:checked->Seçim kutularında kullanıldığında anlaşılması anlamlı olacaktır.
EX:
option:checked{
    color:red;
    background-color:gray;
    font-size:15px;
}
select{
    width:100px;
    font-size:12px;
}
<select>
        <option value="1">A</option>
        <option value="2">B</option>
        <option value="3">C</option>
</select>

disabled:pasif olan elemente stil uygulamaya yarayan sözde sınıftır(dakika:10:30)
empty->11:30, içeriği boş olan elemente stil uygulamaya yarayan sözde sınıf
enabled->pasif olmayan elemente stil uygulamaya yarayan sözde sınıftır(dakika:13.56)
first-child->sayfada aynı etiketin birden çok bulunduğu durumlarda sadece en baştaki etiketi hedeflemek için kullanılır. Aynı türdeki elementlerin ilkini hedefler ve stili sadece o elemente uygular(dakika:16.30)

##Ders23 PSeudo Classes
first-of-type:Aynı türden ilk elemanı stillendirmek için kullanılır(dakika:01.30)
focus:(dakika:03:30)
hover:(04.00)->elementlerin üzerine gelindiğinde stil uygulanır. text-transformnone,capitalize, uppercase, lowercase
in-range:Belirlediğimiz aralıkta sayılar varsa stili uygula(07.20)
invalid:hatalı eksik veya kabul edilmeyen değerler olduğunda uygulanır(09.47)
last-child->sayfada aynı etiketin birden çok bulunduğu durumlarda sadece en baştaki etiketi hedeflemek için kullanılır. Aynı türdeki elementlerin ilkini hedefler ve stili sadece o elemente uygular(dakika:13.46)

last-of-type:Aynı türden son elemanı stillendirmek için kullanılır(dakika:15.10)

link:(17.53) bağlantı veren link ifadelerini stillendirir
not:(21.29)->p:not(.p1)

##Ders24
nth-child(m)->0.00, mth element from start
nth-last-child(m)->2.50, mth element beginning from the end
only-of-type->3.30, 
optional->08.40:Html elementine girişin isteğe bağlı olduğu durumlarda biçimlendirme yapmamızı sağlar
root->kök olan element hedef alınır. Kök hedef her zaman <body> etiketidir.
:target:olay güdümlü çalışır. bir form elementine veya linke tıklandığında, # operatörü ile aynı sayfada yeniden link verip id ler yardımı ile ilgili elementi hedefler ve stilllendirir.(15.00)
örnek html/css içeriği şöyle olabilir


<input type "button" value ="1. satırı hedefle" onclick ="window.location.href = '#satir1'"/>
<a href = "#satir2"> ikinci satırı hedefle </a>
<p id="satir1"> ilk satır</p>
<p id="satir2"> ikinci satır</p>

:target{
    border: 1px solid black;
}