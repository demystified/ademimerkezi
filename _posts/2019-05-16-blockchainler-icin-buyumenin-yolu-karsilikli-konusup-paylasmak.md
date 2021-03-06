---
layout: post
title:  "Blockchain'ler için büyümenin yolu karşılıklı konuşup paylaşmak"
date:   2019-05-07 12:42:56 +0300
categories: Genel
---

Geçtiğimiz [yazıda](/genel/2019/05/07/bir-Blockchain-digeri-ile-konusur-mu.html) interoperability (karşılıklı çalışabilirlik) konusuna bakmış, bu alandaki en bilinen iki oyuncu Polkadot ve Cosmos Network'ü bu yazıya bırakmıştık. 

### Paylaşmak güzeldir, rekabet de iyidir

Aslında hem Polkadot hem de Cosmos Network ana hatları ile aynı misyonu paylaşıyorlar: Ethereum ile başlayan Blockchain'lerin birbirleri ile etkileşimi olayını bir adım öteye götürmek. 

Farklılıkları detaylarda. Çok teknik konulara girmeden kim olduklarını, ortak yönlerini ve farklarını anlatalım ki interoperability denen kavram aklımızda daha netleşsin. 

### Polkadot

<img align="left" src="/assets/polkadot_v1.png">

[Polkadot](https://polkadot.network/), Ethereum'un kurucularından ve ana gelişticilerinden [Gavin Wood](http://gavwood.com/)'un çocuğu. Gavin sonradan görüş ayrılığına düştüğü Ethereum Foundation'ı bırakarak Polkadot üzerine yoğunlaşmaya karar veriyor.

Her ne kadar 2014 yılına kadar uzanan bir geçmişi olsa da, Polkadot'un asıl yazılım süreci 2017 yılının sonlarında [başlıyor](https://medium.com/polkadot-network/polkadot-2018-recap-677dab3e995b). Öncesinde ise Ekim 2017'de 144 Milyon ABD Doları token satışı ile fonlama [topluyorlar](https://cointelegraph.com/news/new-startup-from-ethereum-co-founder-gavin-wood-plans-60-million-ico-wsj). Tabii sadece Gavin değil sürecin içinde olan. Polkadotun arkasında [Parity](https://www.parity.io/) ve [Web3](https://web3.foundation/) isimli iki yapı var. "İyi güzel de kim bunlar?" derseniz:

<img align="left" src="/assets/web3_foundation_v3.jpg"> [Web3 Foundation](https://web3.foundation/) Gavin Wood tarafından İsviçre'de kurulmuş, adem-i merkezi (merkezi olmayan) bir dünya vizyonuna sahip bir vakıf. Bu amacı gerçekleştirecek projelere destek veriyorlar. Başlangıçta Ethereum gelişimi üzerine odaklansalar da, sonraları başka alanlara da girmiş durumdalar. 

&nbsp;


<img align="left" src="/assets/parity_v1.png"> [Parity](https://www.parity.io/) ise, 80'i aşkın geliştiriciye sahip, Blockchain altyapı teknolojisi geliştiren bir yazılımcı şirketi (teknik detay: Rust dili kullanıyorlar). Açık kaynak ürünler geliştiriyorlar. Temel hedefleri Web 3 Foundation'ın vizyonunu hayata geçirerek, kişiden kişiye (P2P) işlemler aracılığı ile yürüyen, merkezi ticari güçlere bağımlı olmayan bir toplum oluşturmak. 

Adem-i merkezi yeni girişimlere altyapı sağlıyorlar kısacası. Eğer Ethereum üzerine bir proje geliştirmek istiyorsanız Parity Ethereum, yok kendi bağımsız Blockchain'inizi geliştirmek istiyorsanız [Substrate](https://www.parity.io/substrate) yazılımını size sunuyorlar. 

İşte Polkadot da geliştirdikleri bu projelerin birbirleri ile iletişimini sağlayan bir protokol olarak hizmet veriyor. Web3 Foundation sahibi olduğu Polkadot'un yazılımını geliştirme işini Parity'e vermiş. (Her ikisinde de Gavin Wood'un olmasının bunda payı vardır elbet :)).  

### Cosmos Network

<img align="left" src="/assets/cosmos_network_v2.png"> Cosmos Network de yapı olarak Polkadot'a benziyor. Onlar da Polkadot gibi 2017 yılında başlıyor ve aynı yılın Nısan ayında token satarak fonlama yapıyorlar - ilginç olan yaklaşık 17 Milyon ABD Doları hedef ile çıkıp [bu rakamı 28 dakika içinde toplayarak](https://icoholder.com/en/cosmos) token satışını bitiriyorlar.   Arkasında da Polkadot gibi iki yapı var: [Tendermint](https://tendermint.com/about) ve [The Interchain Foundation](https://interchain.io/). 

&nbsp;

<img align="left" src="/assets/interchain_tendermint.png"> 

[The Interchain Foundation](https://interchain.io/) yukarıdaki Web3 Foundation gibi Cosmos Network'unu geliştirmek üzere İsviçre'de kurulmuş bir vakıf. [Tendermint](https://tendermint.com/about) ise aynı Parity gibi bir teknoloji geliştirme şirketi. Interchain Foundation, Polkadot'da Web3 Foundation'ın yaptığına benzer şekilde Cosmos Network geliştirme işini Tendermint'e vermiş. 

### Ortak noktaları neler?

Ortak noktaları çok. Her iki ağ da, bağımsız blockchainlerin birarada yaşayacağı bir ekosistem yaratmaya çalışıyor. Bu ekosistemi yaratırken, dünya sadece bu ekosistemlerden oluşacak diye düşünmüyorlar doğal olarak. Diğer büyük şu an mevcut ekosistemler ile de bir köprü kuruyorlar kendilerine. 

Özellikle Bitcoin'in kullanıcı tarafında ağırlığı olması nedeniyle Bitcoin Blockchain'ine bir bağlantıları var. Keza yazılımcıların ağırlığının Ethereum'da olması nedeniyle oraya da bağlantı geliştiriyorlar. 

İyi de bir ekosistem içinde olmanın ne faydası var diye aklınızdan geçiyor ise: Geçen [yazıda](/genel/2019/05/07/bir-Blockchain-digeri-ile-konusur-mu.html) açıklamıştık, şimdi bir örnek daha verelim:

Ethereum gibi bir network üzerinde çalışan uygulamaları kullanarak, örneğin [AirSwap](https://www.airswap.io/) ile kişiden kişiye dijital varlık değişimi yapabilirsiniz, yani bir Blockchain'e ait token'ı bir başka Blockchain'e ait token ile değiştirebilirsiniz. Ya da kimseye başvurmadan herhangi bir kredi skorlamasına tabi olmadan kendi kendinize elinizde olan Ethereum parası ETH'i teminat verip,  [DAI sabitparası borçlanabilirsiniz](/genel/2019/02/15/MakerDAO-kredi-kullaniminda-cigir-acar-mi.html). Ethereum sistemi içinde olmanız farklı Blockchain'ler arası bu işlemleri yapmanıza olanak sağlıyor. 

Bütün bunlar Ethereum üzerinde kurulu yapılar arasında yapılabilir. Ancak Ethereum halka açık bir altyapı olduğu için ağır ilerliyor, ayrıca pek çok kısıtı var geliştiriciler için. İşte Polkadot ve Cosmos Network, özel yapılar olarak hem daha hızlı hareket ediyorlar, hem de Blockchain geliştiricilerine daha fazla bağımsızlık vaat ediyorlar. 

Bu arada hem Polkadot hem de Cosmos Network'un sistemi korumak amacıyla Proof-of-Stake algoritmalarının değişik versiyonlarını kullandıklarını belirtelim (o nedir diye soracak olursanız teknik olarak [şu yazımızda](/genel/2018/11/01/Proof-of-Workun-rakipleri-kimler.html) anlatmaya çalışmıştık). 

**Özet olarak her iki network de şu üç noktada ekosistemi geliştirmeye çalışıyorlar. Karşılıklı çalışılabilirlik (interoperability), ölçeklenebilirlik (scalibility) ve güvenlik (security).**

### Farkları neler peki?
Farkları aslında ayrıntılarda. Bir benzetme yaparmak gerekirse: Polkadot bir parça tabildot veren yemekhaneler gibi. Cosmos ise daha çok alakart yemek sunuyor sanki. Çok fazla teknik detaya girmeden bahsedelim: 

Blockchain'lerin güvenliğini madenciler sağlıyor. Madenciler kısıtlı sayıda olduğu için bir Blockchain geliştiricisi olarak yeterli sayıda madenci bulmak zor olabiliyor. Polkadot ve Cosmos Network'un Blockchain'lere sunduğu en önemli faydalardan biri sahip oldukları madenci havuzu kullandırmaları. Ama detayda farklılıkları da var: 

Polkadot, elindeki madencileri sistem içindeki Blockchain'lere eşit olarak dağıtıyor. Cosmos'da ise, bir Blockchain sisteme gelip ne kadar madenci ihtiyacı olduğunu ve bu hizmet için ne kadar ödül vereceğini açıklıyor. Madenciler buna göre istedikleri Blockchain'in güvenliğini sağlıyorlar; daha özgür ama daha az disiplinli bir yapı. 

Polkadot, güvenlik başta olmak üzere tüm Blockchain'lere sabit bir hizmet veriyor. Yani sistemlerine bağlanıyor ve aynı hizmeti alıyorsunuz bir Blockchain olarak. 

Cosmos Network ise her bir Blockchain'i kendisine bağlamanın çok da gerçekci olmayacağı düşüncesi ile iki katmanlı bir sistem öngörüyor. Bir tarafta altyapı olarak Cosmos var. Bir tarafta da daha üst seviyede Blockchain'lerin başta güvenlik olmak üzere çeşitli ihtiyaçlarını karşılayacak ikinci bir seviye bulunuyor - ki buna Cosmos Hub diyorlar. Cosmos Hub, bir nevi onların neler yapacaklarını göstermek amacıyla kurdukları ağ. Ama ne kadar çok fonksiyonu barındırırsanız, üzerinizdeki (ya da içinizdeki) Blockchain'leri o kadar kısıtlamak zorunda olacağınızı düşünerek, bu ikinci katmanı bir nevi opsiyonel sunuyorlar. 

Örneğin duymuşsunuzdur; Binance, girişimlere kendi kullanıcılarına hızlı erişim olanağı veren [bir sistem kuruyor Binance Chain adında](https://cointelegraph.com/news/binance-chain-launches-firm-expects-to-execute-mainnet-swap-on-april-23). İşte bu sistem için altyapı olarak Cosmos'u kullanacaklar. Yani en yalın halinde iletişimi sağlayacak en alttaki ağı Cosmos olacak, Binance Chain bunun üzerine Cosmos Hub gibi bir hub olacak ama örneğin güvenlik için muhtemelen Cosmos'u değil kendi ağlarını kullanacaklar. 

### Gelecek nasıl olacak?

Gerek Polkadot gerekse Cosmos, Ethereum tarafından başlatılan interoperability kavramının bir sonraki evreye taşımaya adanmış girişimler. Her ne kadar her iki girişimin arkasında özel/kapalı yazılım grupları olsa da, bütün kodları Açık Kaynak. Yeni Blockchain girişimleri için bunları kullanmakta bir sakınca yok. Belirsiz olan, bunlardan hangisinin ivme kazanacağı ve kazanan olacağı. 

Bu girişimler henüz yolunda başındalar. Vizyonları çok geniş ancak şu ana kadar daha çok basit işlemleri gerçekleştirebilmeye odaklandılar. Gelecekte fonksiyonları artacak ama buna bağlı olarak karmaşıklaşacakları için daha fazla risk barındırır hale gelecekler. Belki de girişimler işlerini şansa bırakmayacak ve şu an piyasa lideri olan ancak yavaş gelişen Ethereum içinde kalmaya devam edecekler. Sonucu görmek için beş on yıl arası beklemek gerekiyor sanırım. 

--

*Not 1: Konumuz sistemleri tanıtmak olduğu için her iki network'un çıkardığı token'lara özellikle değinmedik.

&nbsp;

*Not 2: Yazdığımız 50+ yazının bir bütünlük içinde nelerden oluştuğuna bakmak isterseniz [Hakkımızda](/about/) sayfasına göz atabilirsiniz.*
