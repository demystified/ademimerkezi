Geçtiğimiz [yazıda](/genel/2019/05/07/bir-Blockchain-digeri-ile-konusur-mu.html) Interoperability (karşılıklı çalışabilirlik) konusuna bakmış, bu alandaki en önemli iki oyuncu olan Polkadot ve Cosmos Network'ü bu yazıya bırakmıştık. 

### Paylaşmak güzeldir, rekabet de iyidir

Aslında Polkadot ve Cosmos Network'un yaptıkları ana hatları ile aynı - Ethereum ile başlayan Blockchain'lerin birbirleri ile etkileşimde olma olayını bir adım öteye götürmek. Sadece detaylarda farklılık gösteriyorlar. 

Çok teknik detaya girmeden kim olduklarını, ortak yönlerini ve farklarını anlatalım ki aslında interoperability denen kavram aklımızda daha netleşsin. 

### Polkadot


| ![polkadot.png](/assets/polkadot.png) | 
|:--:| 
| *Kaynak: [polkadot](https://polkadot.network/)* |

[Polkadot](https://polkadot.network/), Ethereum'un kurucularından ve ana gelişticilerinden [Gavin Wood](http://gavwood.com/)'un çocuğu. Gavin sonradan görüş ayrılığına düştüğü Ethereum Foundation'ı bırakarak Polkadot üzerine yoğunlaşmaya karar veriyor. 

Her ne kadar 2014 yılına kadar uzanan bir geçmişi olsa da, Polkadot'un asıl yazılım süreci 2017 yılının sonlarında [başlıyor](https://medium.com/polkadot-network/polkadot-2018-recap-677dab3e995b). Tabii sadece Gavin değil sürecin içinde olan. Tüm altyapının arkasında [Parity](https://www.parity.io/) ve [Web3](https://web3.foundation/) denen iki yapı var. "İyi güzel de kim bunlar?" derseniz:


| ![web3_foundation.jpg](/assets/web3_foundation.jpg) | 
|:--:| 
| *Kaynak: [web3 Foundation](https://web3.foundation/)* |

[Web3 Foundation](https://web3.foundation/) Gavin Wood tarafından İsviçre'de kurulmuş, adem-i merkezi (merkezi olmayan) bir dünya vizyonu ile hareket eden bir vakıf. Bu amacı gerçekleştirecek projelere destek veriyorlar. Başlangıçta yoğunlukla Ethereum gelişimi üzerine odaklansalar da, sonraları başka alanlara da girmiş durumdalar. 



| ![parity.png](/assets/parity.png) | 
|:--:| 
| *Kaynak: [parity](https://www.parity.io/)* |

[Parity](https://www.parity.io/) ise, 80'i aşkın geliştiriciye sahip, Blockchain altyapı teknolojisi geliştiren bir yazılımcı şirketi (teknik detay: Rust dili kullanıyorlar). Açık kaynak ürünler geliştiriyorlar. Temel hedefleri Web 3 Foundation'ın vizyonunu hayata geçirerek, kişiden kişiye (P2P) işlemler aracılığı ile yürüyen, merkezi ticari güçlere bağımlı olmayan bir toplum oluşturmak. 

Adem-i merkezi yeni girişimlere altyapı sağlıyorlar kısacası. Eğer Ethereum üzerine bir proje geliştirmek istiyorsanız Parity Ethereum, yok kendi bağımsız Blockchain'inizi geliştirmek istiyorsanız [Substrate](https://www.parity.io/substrate) yazılımını size sunuyorlar. 

İşte Polkadot da geliştirdikleri bu projelerin birbirleri ile iletişimini sağlayan bir protokol olarak hizmet veriyor. Web3 Foundation sahibi olduğu Polkadot'un yazılımını geliştirme işini Parity'e vermiş. (Her ikisinde de Gavin Wood'un olmasının bunda payı vardır elbet :)).  

### Cosmos Network

| ![cosmos_network.png](/assets/cosmos_network.png) | 
|:--:| 
| *Kaynak: [cosmos network](https://cosmos.network/)* |
Cosmos Network de yapı olarak Polkadot'a benziyor. Arkasında Polkadot gibi iki yapı var. [Tendermint](https://tendermint.com/about) ve [The Interchain Foundation](https://interchain.io/) 

| ![tendermint.png](/assets/tendermint.png) | 
|:--:| 
| *Kaynak: [tendermint](https://tendermint.com/)* |

Tendermint, yukarıda bahsettiğimiz Parity gibi bir teknoloji geliştirme şirketi. The Interchain Foundation da, yine yukarıdaki Web3 Foundation gibi Cosmos Network'unu geliştirmek üzere İsviçre'de kurulmuş bir vakıf. Onlar da Polkadot'da Web3 Foundation'ın yaptığı gibi, Cosmos Network geliştirme işini Tendermint'e vermişler. 

| ![interchain_foundation.png](/assets/interchain_foundation.png) | 
|:--:| 
| *Kaynak: [interchain_foundation](https://interchain.io/)* |

### Ortak noktaları neler?

Ortak noktaları çok. Her iki ağ da, bağımsız blockchainlerin birarada yaşayacağı bir ekosistem yaratmaya çalışıyorlar. Bu ekosistemi yaratırken, dünya sadece bu ekosistemlerden oluşacak diye düşünmüyorlar doğal olarak. Diğer büyük şu an mevcut ekosistemler ile de bir köprü kuruyorlar kendilerine. Özellikle Bitcoin'in kullanıcı tarafında ağırlığı olması Bitcoin Blockchain'ine bir bağlantıları var. Yazılımcıların ağırlığının Ethereum'da olması nedeniyle oraya da bağlantıları var. 

İyi de bir ekosistem içinde olursa ne olur, ne faydası var diye aklınızdan geçiyor ise: Geçen yazıda bir örnek vermiştik. Bir tane daha verelim. Örneğin Ethereum gibi bir network üzerinde çalışan uygulamaları kullanarak, örneğin [AirSwap](https://www.airswap.io/) kişiden kişiye dijital varlık değişimi yapabilirsiniz, yani bir Blockchain'e ait token'ı bir başka Blockchain'e ait token ile değiştirebilirsiniz. Ya da kimseye başvurmadan herhangi bir kredi skorlamasına tabi olmadan kendi kendinize elinizde olan Ethereum parası ETH'i teminat verip,  DAI sabitparası borçlanabilirsiniz. 

Bütün bunlar Ethereum üzerinde kurulu yapılar arasında yapılabilir. Ancak Ethereum halka açık bir altyapı olduğu için ağır ilerliyor, ayrıca pek çok kısıtı var geliştiriciler için. İşte Polkadot ve Cosmos Network, özel yapılar olarak hem daha hızlı hareket ediyorlar, hem de Blockchain yaratıcıları daha bağımsız yapma vaadleri var. 

Bu arada hem Polkadot hem de Cosmos Network'un sistemi korumak amacıyla Proof-of-Stake algoritmalarını kullandıklarını belirtelim (o nedir diye soracak olursanız teknik olarak [şu yazımızda](/genel/2018/11/01/Proof-of-Workun-rakipleri-kimler.html)anlatmaya çalışmıştık). Bu arada her iki ağ'ın ataklara karşı makinelerin 1/3'ünün fazlasının daha koruyacak 

*Özet olarak her iki network de şu üç noktada ekosistemi geliştirmeye çalışıyorlar. Karşılıklı çalışılabilirlik (interoperability), ölçeklenebilirlik (scalibility) ve güvenlik (security).*

### Farkları neler peki?
Farkları aslında ayrıntılarda. Bir benzetme yaparmak gerekirse: Polkadot bir parça tabildot veren yemekhaneler gibi. Cosmos ise daha çok alakart yemek sunuyor sanki. Çok fazla teknik detaya girmeden bahsedelim: 

Blockchain'lerin güvenliğini madenciler sağlıyor. Madenciler kısıtlı sayıda olduğu bir Blockchain geliştiricisi olarak yeterli sayıda madenci bulmak zor olabiliyor. Polkadot ve Cosmos Network'un Blockchain'lere verdiği en önemli faydalardan biri sahip oldukları madenci havuzu kullandırmaları. Ama detayda farklılıkları da var: 

Polkadot, elindeki madencileri sistem içindeki Blockchain'lere eşit olarak dağıtıyor. Cosmos'da ise, öncelikle bir Blockchain gelip ne kadar madenci ihtiyacı olduğunu ve bu hizmet için ne kadar ödül vereceğini açıklıyor. Madenciler istedikleri Blockchain'in güvenliğini sağlıyorlar, daha özgür ama daha az disiplini olan bir yapı. 

İşte bu güvenlik başta olmak üzere değişik hizmetlerin nasıl verildiği konusunda Polkadot ile Cosmos arasında felsefe farkı var. 

Polkadot, tüm Blockchain'lere sabit bir hizmet veriyor. Yani sistemlerine bağlanıyor ve aynı hizmeti alıyorsunuz bir Blockchain olarak. 

Cosmos Network ise her bir Blockchain'i kendisine bağlamanın çok da gerçekci olmayacağı düşüncesi ile iki katmanlı bir sistem öngörüyor. Bir tarafta altyapı olarak Cosmos var. Bir tarafta da daha üst seviyede Blockchain'lerin başta güvenlik olmak üzere çeşitli ihtiyaçlarını karşılayacak ikinci bir seviye - ki buna Cosmos Hub diyorlar. Cosmos Hub, bir nevi onların neler yapacaklarını göstermek amacıyla kurdukları ağ. Ama ne kadar çok fonksiyonu barındırırsanız, üzerinizdeki (ya da içinizdeki) Blockchain'leri o kadar kısıtlamak zorunda olacağınızı düşünerek, bunu opsiyonel sunuyorlar. 

Örneğin, duymuşsunuzdur Binance geliştiricilere kendi ekosisteminde kendi kullanıcılarına yönelik [bir sistem kuruyor Binance Chain adında](https://cointelegraph.com/news/binance-chain-launches-firm-expects-to-execute-mainnet-swap-on-april-23). İşte bu sistem için altyapı olarak Cosmos'u kullanacaklar, yani en yalın halinde iletişimi sağlayacak en alttaki ağı. 

### Gelecek nasıl olacak?

Gerek Polkadot gerekse Cosmos, Ethereum tarafından başlatılan interoperability kavramının bir sonraki evreye taşımaya adanmış girişimler. Her ne kadar her iki girişimin arkasında özel/kapalı yazılım grupları olsa da, bütün kodları Açık Kaynak. Yeni Blockchain girişimleri için bunları kullanmakta bir sakınca yok. Belirsiz olan, bunlardan hangisinin ivme kazanacağı ve kazanan olacağı. 

Bu girişimler henüz yolunda başındalar. Vizyonları çok geniş ancak şu ana kadar çok daha basit işleri yapmaya odaklandılar. Gelecekte fonksiyonları artacak ama buna bağlı olarak ne kadar karmaşıklaşırlar ise o kadar risk barındırır hale gelecekler. Belki de girişimler işlerini şansa bırakmayacak ve şu an piyasa lideri olan ancak yavaş gelişen Ethereum içinde kalmaya devam edecekler. Sonucu görmek için beş on yıl arası beklemek gerekiyor sanırım. 

Not: Konumuz sistemleri tanıtmak olduğu için her iki network'un çıkardığı token'lara özellikle değinmedik. 
