---
layout: post
title:  "Şifreleme mi? Çok karışık değil mi?"
date:   2018-04-04 14:25:15 +0300
categories: Genel
---

Şifreleme deyince aklımıza çok karışık acayip konular geliyor olabilir. Normal. Aslında çok da karışık değil ama anlayabilmek için biraz çaba sarfetmek lazım. Peki neden önemli bu şifreleme? 

"Tamam şifreleme var, Bitcoin de bunu yapıyor zaten" deyip geçebilirsiniz. Bu da bir görüş açısı. Ama şifrelemenin nasıl olduğunu, blockchain protokollerinin altyapısının nasıl çalıştığını anlamak bize bu protokolleri günlük hayatımızda nasıl kullanırızın ipuçlarını verebilir. 

Efendim, daha önce de belirtmiştik. Modern şifreleme teknolojisi aslında 1970'lerden beri var. 1990'larda ise internetin yaygınlaşması ise bilginin ve iletişimin yaygınlaşmasını sağladı. Tabii bilgiyi yayarsınız bir sorun yok - paylaştıkça çoğalır. Ama aynı sistem üzerinden para gibi kaygan bir varlığı geçirmek isterseniz, çok ciddi güvenlik sağlamanız lazım. Orada da, merkezi kurumlar örneğin bankalar yardımcı oldu, güvenlik sistemleri getirdiler, paramızı transfer etme ve saklama konusunda bize yardımcı oldular. 

İşte Satoshi Nakamoto dediğimiz kişi(ler) bu şifrelemeyi yeni teknoloji ile birleştirerek bu aradaki kurumları yok etmeye sağladılar. Dolayısıyla şifreleme sayesinde koca bir aracıyı tabiri caiz ise ıskartaya çıkardılar.. 

### Şifrelemeli mi, şifrelememeli mi?

Bir kapalı bir kutu (belki de bir kağıt öğütücü) düşünün. Bir taraftan anlamlı bir sözcük veriyorsunuz, diğer taraftan rakam ve sayılardan oluşan anlamsız bir bütün veriyor. 

... Kağıt öğütücü --- 

Bir örnek yapalım dilerseniz: 

| Girdi  | Sonuç  |
|---|---|
| Merhaba  | 7fdc9f4717c5fe66df286c700fab969b4d6209d03aa84624c5f8f58c17c9c058  |

Siz de [deneyebilirsiniz](http://www.xorbin.com/tools/sha256-hash-calculator) - aynı sonucu bulacaksınız (bu sonuca teknik olarak **hash** deniyor). 

İşte işin özü bu. Değişik şifreleme mekanizmalarından en popüler olan SHA 256 şifreleme böyle çalışıyor. Girin herhangi bir SHA-256 şifreleme sitesine "Merhaba" yazın, yukarıdaki sonucun aynısını verecek size. 64 karakterli bir dizi. 

-- 

Peki buraya uzunca bir paragraf koymak istesek ne olur? Mesela, 

| Girdi  | Sonuç  |
|---|---|
| Ey Türk Gençliği! Birinci vazifen, Türk istiklâlini, Türk Cumhuriyetini, ilelebet, muhafaza ve müdafaa etmektir. Mevcudiyetinin ve istikbalinin yegâne temeli budur. Bu temel, senin, en kıymetli hazinendir. İstikbalde dahi, seni bu hazineden mahrum etmek isteyecek, dahilî ve haricî bedhahların olacaktır. Bir gün, İstiklâl ve Cumhuriyeti müdafaa mecburiyetine düşersen, vazifeye atılmak için, içinde bulunacağın vaziyetin imkân ve şerâitini düşünmeyeceksin! Bu imkân ve şerâit, çok nâmüsait bir mahiyette tezahür edebilir. İstiklâl ve Cumhuriyetine kastedecek düşmanlar, bütün dünyada emsali görülmemiş bir galibiyetin mümessili olabilirler. Cebren ve hile ile aziz vatanın, bütün kaleleri zaptedilmiş, bütün tersanelerine girilmiş, bütün orduları dağıtılmış ve memleketin her köşesi bilfiil işgal edilmiş olabilir. Bütün bu şerâitten daha elîm ve daha vahim olmak üzere, memleketin dahilinde, iktidara sahip olanlar gaflet ve dalâlet ve hattâ hıyanet içinde bulunabilirler. Hattâ bu iktidar sahipleri şahsî menfaatlerini, müstevlilerin siyasi emelleriyle tevhit edebilirler. Millet, fakr ü zaruret içinde harap ve bîtap düşmüş olabilir.  Ey Türk istikbalinin evlâdı! İşte, bu ahval ve şerâit içinde dahi, vazifen; Türk İstiklâl ve Cumhuriyetini kurtarmaktır! Muhtaç olduğun kudret, damarlarındaki asil kanda mevcuttur! | c369b0a6ca659b4d370ff8b0a54ad582d49d7cb1d42125059658ed8d94996276  |

Viola! Gene bambaşka bir dizi ama yine 64 karakterli. Buraya isterseniz girdi olarak koca bir ansiklopedi koyun, sonuç yine 64 karakterli bir dizi olacak. 

--

Şimdi bu ilk örneğimize geri dönelim: Merhaba kelimesinin sonuna bir "!" işareti ekleyelim, bakalım ne olacak?

| Girdi  | Sonuç  |
|---|---|
| Merhaba!  | b1726b923349fd632fa7ce8b62a06c5a3f785be1db4f6a831eef58d70c7a45cc  |

Gördünüz mü? Herşey değişti. İlk kelimeden tamamen farklı bir sonuç çıktı ortaya. Ama dikkat edin 64 karakterli yine. 

Bu önemli, o yüzden biraz daha açalım. Aynı girdiler hep aynı sonucu veriyor. Ama girdi de bir harf değiştirin, çıkan sonuç bambaşka oluyor.  Bu ne işe yarıyor? Şuna: Eğer elinizde bir bilgi var ve bu bilgi sonucu ortaya çıkan bir sonuç da varsa, bu girdi hakikaten bu sonucu mu veriyor test edebiliyorsunuz. Yani girdinin orjinalliğini ya da tutarlılığını (yani sonradan değiştirilip değiştirilmediğini) çok rahat görebilirsiniz. 

Bu arada şunu da belirtmekte fayda var. Bu şifreleme mekanizmalarının özelliği şu:; sonucu biliyor olmanız girdiyi de bildiğiniz anlamına gelmiyor. Yani, girdiyi biliyorsanız sonucu bulabiliyorsunuz ama sonuçtan geriye bilgiye gidemiyorsunuz. 

--

Bilginin tutarlı olduğunu bilmek ne işimize yarıyor? Bakın burası da çok önemli. Ama bunun için bir örnek daha verelim: Yukarıda gördüğünüz gibi "Merhaba" kelimesine "!" işareti ekliyorsunuz ve ortaya çıkan sonucun "Merhaba!" kelimesinin sonucu olduğunu test edebiliyorsunuz değil mi? Yani iki bilgiyi aldınız, bir araya getirdiniz, sonra sisteme soktunuz ve bir sonuç çıktı. Bu iki kelimeyi bilen kişi sonucu da görebiliyor. 

Ben eğer kimsenin görmesini istemediğim bir bilgiyi size göndermek istersem nasıl yapacağım? Burada birkaç koşulun doğru olduğuna emin olmamız gerekiyor
- Ben bilgiyi yazarken bu bilgiyi sadece sizin okuyabileceğine  emin olmam gerekiyor
- Siz, bu bilginin benden geldiğine emin olmak istiyorsunuz
- Aynı zamanda hem ben hem siz bu bilginin benden size gelirken yolda değiştirilmemiş olduğuna emin olmamız gerekiyor


### "Özel Anahtar" ve "Genel Anahtar"
Yukarıdaki koşulların sağlanabilmesi için şifrelene teknolojinin önemli bir parçasını daha açmamız gerekecek: "Özel Anahtar" ve "Genel Anahtar". Sizin, benim ve herkesin yaratabileceği her bireyin kendine ait bir "Özel Anahtar" bir de "Genel Anahtar" var. 

Özel Anahtar ve Genel Anahtarı bana ait birbirlerinin aynı olan iki anahtar gibi düşünebiliriz. Aradaki tek fark, Özel Anahtarın  sadece benim bildiğim (hiç kimse ile paylaşmadığım) bir anahtar. Genel Anahtar ise yine bana ait, ama herkes ile paylaştığım tüm dünyanın görebileceği bir anahtar olması. İlişkileri ise şu: Bemim Özel Anahtarım ile kapadığım kapıyı (şifrelediğim mesajı) Genel Anahtarı bilen herkes açabiliyor (şifreyi açıp mesajı görebiliyor).   

Dilerseniz bir örnek ile anlatalım: Tüm dünya ile bir bilgi paylaşmak istediğim bir mesaj var. Örneğin "Yarın New York'a gideceğim!". İki önemli ihtiyacım var: 1. Bu bilginin benden geldiğinin bilinmesi (otantik olması) 2. Mesajın içeriğinin herkese doğru ulaşması (bir başkası tarafından değiştirilememesi). 

Eğer ben  "Yarın New York'a gideceğim" yazısını kendi Özel Anahtarım ile karıştırıp dünyaya yayınlarsam (yani şifrelersem), çıkan sonuca bakan biri, benim Genel Anahtarımı alıp bu ortaya çıkan şifreli sonucu ile birleştirirse (yani şifreyi çözerse) sonuçta benim tarafımdan gelen, benim imzaladığım mesajı görür.  

Bunu bir örnek üzerinden anlatmaya çalışalım: 

Diyelim yukarıdaki gibi bir bilgiyi e-posta olarak gönderiyorsunuz. İlk olarak ne yapıyorum? Kendi e-postama giriyor ve sizin email'inizi yazıyorum, sonra mesaji yazıyorum ve gönder tuşuna basıyorum. Aynı olayı yukarıdaki gibi şifreleme işlemine tabi tutalım. Yaptığım işler şu şekilde: 

1. Mesajı yazıyorum. Şimdi bu mesajı bana ait sadece benim bildiğim "Özel Anahtar" ile birleştiriyorum. Ortaya bir sonuç çıkıyor. 
2. Bu sonuç Benzer şekilde burada da, "Genel Anahtar" benim email adresim, "Özel Anahtar" da bu mesajı yazanın ben olduğunu gösteren bana ait "Dijital İmza".  


### Peki Bitcoin şifrelemesi nasıl çalışıyor?

Hatırlar mısınız, önceki bir yazımızda şunu demiştik: "Blockchain sisteminde yükü çeken makinelerin bu yaptıkları işlemleri kayıt etme, daha sonra da teyid etme işlemi sonucu aldıkları ödüle (ya da lotarya) Bitcoin deniyor. Neden lotarya deniyor? Zira, bu on dakikada bir yapılan teyit işlemi aslında çok zor bir bulmaca. Bir nevi Sudoku oyunu gibi düşünün"

Şimdi dilerseniz bu bulmaca konusunu biraz daha açalım. Ortada tabii ki bir bulmaca yok ama bir şifreleme işlemi var. Aynı yukarıda olduğu gibi "input" ve "output" kısmı olan bir SHA şifrelemesi. 

Input'un iki parçası var 
- Belli bir süre içinde gerçekleşen tüm işlemlerin bir dökümü 
- Bir de bir sayı

Output ise yukarıdaki gibi 64 karakterli bir şifre. 

Sistem söyle çalışıyor. 
1. Her 10 dakikada bir Bitcoin ile yapılan bütün işlemler toplanıyor biraraya ve makinelere gönderiliyor
2. Sonra sistem bütün makinelere şunu söylüyor: *"Ey makineler, işlemlerin toplam dökümünü aldınız, şimdi bu işlem dökümünü alın yanına öyle bir sayı ekleyin ki, şifrelemeye koyduğunuzda çıkan output dört tane sıfır ile başlasın"*
3. Makineler bu çıktıyı alıyor ve sırayla rakamları denemeye başlıyorlar. Önce 1 ekliyor, çıkan sonuca bakıyor, yok olmadı "370ff8b0.." ile başlayan bir output verdi. Sonra 2 ekliyor, yine bakıyor bu sefer "58ed8d94.." diye başlayan bir sayı verdi.. Böyle böyle sırayla tüm sayılar deneniyor. Ta ki bir sayı (diyelim "25264") bize "0000..." ile başlayan bir sonuç verene kadar!
4. "0000.." ile başlayan sonucu ilk bulan makine "Buldum!" diyerek bu sonuca ulaştıran sayıyı "25264" diğer makinelere haber veriyor. 
5. Sonucu gören makineler, işlem dökümünü 25264 sayısı ile birlikte şifreye sokuyorlar, bakıyorlar hakikaten çıkan sonuç "0000.." ile başlıyor, "tamam" diyorlar, "sonuç doğru" ve bir sonraki 10 dakika için yapılan işlemlere geçiyorlar. 
6. 25264 rakamını bulan makine işte bu ödülü (şu anda 12.5 Bitcoin yani 100,000 ABD Doları civari bir rakam) kazanıyor!

### Bu kadar mı?

Evet, aslında işin özü bu kadar basit. Zaten diyoruz ya, Bitcoin üzerindeki bütün işlemler görülebiliyor diye. Yapılan bütün işlemler hangi partiden geliyor hangi partiye gidiyor, ne kadar işlem yapılıyor hepsi görülüyor. Ancak görülmeyen ne? Hangi partiden gelip hangi partiden gittiği de sistem üzerinde şifreli olarak görülüyor. Mesela örnek bir işlem bakalım: 

