﻿---
title: 'PBX 與 IP PBX 組態: Exchange 2013 Help'
TOCTitle: PBX 與 IP PBX 組態
ms:assetid: fb086680-6e3e-477a-a5d8-e24ca30196ee
ms:mtpsurl: https://technet.microsoft.com/zh-tw/library/Bb430797(v=EXCHG.150)
ms:contentKeyID: 54652610
ms.date: 05/21/2018
mtps_version: v=EXCHG.150
ms.translationtype: MT
---

# PBX 與 IP PBX 組態

 

_<strong>適用版本：</strong> Exchange Server 2010 Service Pack 2 (SP2), Exchange Server 2013, Exchange Server 2016_

_<strong>上次修改主題的時間：</strong> 2016-12-09_

逐漸，購買組織，安裝和維護硬體元件，例如專用交換機進行交換 (Pbx) 或 IP Pbx，才能支援自己電話語音的系統。許多組織已購買他們自己的電話語音設備及降低費用其人員相關聯維護其電話系統並因為他們想要更多控制權的電話語音功能所提供。

為組織擁有及維護其電話語音網路，他們必須購買所需的電話語音硬體元件。他們也必須考量電話語音設備及支援其電話語音系統其人員所需的訓練日常的維護。本主題討論不同類型的電話語音商務或組織的系統和其所需要的電話語音硬體元件。主題也提供電話語音設定的不同類型的範例。


> [!IMPORTANT]  
> 我們建議在規劃部署 Microsoft Exchange 2013的所有客戶整合通訊都取得 UM 專家的協助。這有助於確保順利升級舊版的語音郵件系統。啟用新的 UM 部署或升級現有的語音信箱系統的要求解 Pbx、 IP Pbx 以及整合通訊的重要知識。如需要連絡的人的詳細資訊，查看<a href="https://go.microsoft.com/fwlink/p/?linkid=261951">Microsoft PinPoint</a>網站。




<strong>目錄</strong>

Overview of Telephony Systems

Legacy and Traditional PBX Configurations

IP PBX Configurations

Calling or Called Party Identification

## 電話語音系統概觀

中電路切換型網路，例如公用交換電話網路 (PSTN)、 多個通話傳送相同傳輸中型不同。常見問題、 PSTN 中所用的中型是銅的。不過，也可能使用光纖助讀纜線。

電路切換型網路是在其中有存在的專用的連線的網路。專用的連線為基礎的電路或中設定兩個節點讓他們可以彼此通訊之間的通道。兩個節點之間建立撥號之後，可以使用連線只能由下列兩個節點。當通話會使用下列其中一個節點的結束時，會取消連線。

不同類型或類別的企業與組織中找到的電話系統包括電路型網路、 IP 型網路或兩者。每種類型的電話系統具有不同的優點和缺點您需要規劃和實作的電話語音系統時所應考量。

  - <strong>Centrex:</strong> Centrex 為電話公司租用給企業與組織的電話服務的類型。繁體中文 Centrex 電話系統摒除對於公司或組織購買的電話語音硬體站上以支援組織的電話系統。一般而言，Centrex 系統會使用小型的分公司的列程式及依月份為基礎的電話公司從租賃 Centrex 服務。Centrex 電話系統有時候會使用較大型組織，但最常政府、 公用和私人組織中找到。Centrex 經常使用類比電話線路公司或組織的連線。但是它也可用 T1 電路解多工器站上支援類比與數位散或 ISDN 行。
    
    Centrex 型電話語音系統中電話的公司中央 office 會做為電話交換。它具有設計用於支援指定組織的需求。中央電話 office 來自公司到適當的內部或外部電話號碼的呼叫進行路由。Centrex 使用電話公司的中央 office exchange 內部的來電轉接回到副檔名。例如，Centrex，與電話 exchange 或電話的公司中央 office 知道哪些副檔名是內部。讓具有位於組織的電話語音網路內的員工可以在相同的電話語音網路中的另一位員工的撥號對應表或撥號對應表使用四位數分機號碼。當通話時所撥打的內部電話分機號碼時，已轉接至電話公司的中央 office 並路由傳送回至啟動通話的分機號碼。

繁體中文 Centrex 電話系統的變化稱為*IP Centrex*。在 IP Centrex 電話系統傳送通話透過 Voice over IP (VoIP) 閘道的電話公司中央 office 其位於或其位於站上的服務提供者。在此類電話系統中，VoIP 閘道會將通話透過網際網路或透過 VoIP 為基礎的網路可以傳送的 IP 型資料封包轉譯。不過，如果通話透過網際網路傳送、 是接收通話並再將轉譯傳統電路切換型電話的電話通常是另一個 VoIP 閘道。

目前已備妥的電話系統必須安裝、 繁體中文 Centrex 的組織部署及維護一或多個 VoIP 閘道的整合通訊才能正常運作。整合的通訊可能會要求您安裝、 部署及維護 IP Centrex 所使用的 VoIP 閘道器。數個變數會決定您是否需要 VoIP 閘道。這些變數加入 （類比、 數位或 IP） 您組織中使用的電話和 IP Centrex 系統所支援的通訊協定的類型。

  - <strong>主要電話：</strong> 索引鍵電話系統中電話的公司中央 office 已連接到使用標準類比或數位電話線組織。多個電話所連接的單一電話分機號碼讓該線條或分機號碼相關聯的所有電話時呼叫放入組織使用此電話號碼，會同時都響起。

與金鑰電話系統、 個別使用者會跨散共用行。因此，來電者將不會會嘗試撥打到組織時遇到經常忙線訊號。主要電話系統通常會使用小型的辦公室位置內部的通話數是高但外部通話數量很低。

主要電話系統變得更複雜一段時間及可使用整合通訊如果新增 VoIP 閘道。不過，即使使用支援的 VoIP 閘道一些較不複雜的系統可能無法運作。

  - <strong>PBX:</strong> 舊版的 PBX 會切換通話的電話語音裝置的電話語音或電路切換型網路。舊版的 PBX 是 PBX 都不會有的網路介面卡且無法傳遞 IP 封包。因為他們無法傳遞 IP 封包，某些企業版及組織已取代舊版的 Pbx 與 IP Pbx。如需支援的整合通訊的 Pbx 的清單，請參閱[Exchange 2013 的電話語音 advisor](https://docs.microsoft.com/zh-tw/exchange/voice-mail-unified-messaging/telephone-system-integration-with-um/telephony-advisor-for-exchange-2013)。
    
    大部分及較大-中型公司使用 Pbx。PBX 可讓使用者或共用加速被視為外部的 PBX 電話通話的外部的行數 PBX 的訂閱者。PBX 是比給予每位使用者在公司外部的專用的電話線的更加較不昂貴的解決方案。電話、 傳真機、 數據機及許多其他通訊裝置，以及可以連接至 PBX。
    
    PBX 設備通常是安裝在組織的內部部署，並連接散位於站上與電話公司間的通話。限制外部行數，又稱為主幹行、 一般會針對撥出及接聽通話的外部商務，來自 PSTN 等外部來源。
    
    若要讓舊版的 PBX 以便用於整合通訊，您必須部署支援的 VoIP 閘道。如需支援的 VoIP 閘道的清單，請參閱[Exchange 2013 的電話語音 advisor](https://docs.microsoft.com/zh-tw/exchange/voice-mail-unified-messaging/telephone-system-integration-with-um/telephony-advisor-for-exchange-2013)。

  - <strong>IP PBX:</strong> IP PBX 是有支援 IP 通訊協定的網路介面卡 PBX。它是電話的一段切換通常位於組織或商務而不是電話的電話的公司辦公室正在位於設備。有兩種 IP Pbx： 繁體中文 IP Pbx 和混合式 IP Pbx。繁體中文 IP Pbx 及混合式 IP Pbx 支援 IP 通訊協定將語音交談中封包傳送至 VoIP 型電話。不過，混合式 IP Pbx 也會連線傳統類比和數位散。
    
    IP Pbx 較為經常管理比舊版的 pbx 設定因為系統管理員可以更輕鬆地設定 IP PBX 服務使用網際網路瀏覽器或另一種 IP 型的工具。此外，沒有其他電線、 纜線或修補程式面板有安裝。與 IP PBX，您可以移動 IP 型電話純粹拔除電話並再次將它插入新的位置。這可讓您避免將電話移從舊版的 PBX 廠商所需的高成本的服務通話。此外，擁有 IP PBX 的組織不需要維護與管理不同的電路切換型及封包切換網路所需的其他基礎結構成本可能會形成。如 IP Pbx 整合通訊所支援的清單，查看[Exchange 2013 的電話語音 advisor](https://docs.microsoft.com/zh-tw/exchange/voice-mail-unified-messaging/telephone-system-integration-with-um/telephony-advisor-for-exchange-2013)。
    
    回到頁首

## 舊式與傳統 PBX 組態

在具有舊式或傳統 PBX 的電話語音網路上，PBX 會執行下列動作：

  - 建立兩個使用者之電話機間的連線或電路。

  - 只要使用者需要連線，即維持連線。

  - 提供會計用途的資訊 (例如，通話計量)。

除了上列清單中包含的三個功能之外，PBX 還可提供其他通話功能，例如：

  - 自動語音應答

  - 通話計費

  - 代接電話

  - 來電轉接

  - 插撥功能

  - 電話會議

  - 直接進線撥號 (DID)

  - 勿擾功能 (DND)

雖然有數個 Pbx 製造商，因此皆符合兩個基本類別： 類比與數位。這些類型的 Pbx 經常稱為*legacy*或*traditional* Pbx。

通常 PBX 系統連線至電話公司的中央 office 使用特殊電話線路名為 T1 與 E1 線條。T1 和 E1 線路有多個通道。這些電話線也稱為是*trunk lines.*它們可讓中央的辦公室或傳送較佳的效率使用簡化的電線版面配置的同一列上的多個通話 PBX。PBX 也可以使用類比或 ISDN 行。

您可以正確地設定 PBX、 控制多少通道或您想要設定接收來自外部來電者和多少通道的通話的行至來自來電者在貴組織內的通話投入的行。設定通道或行的數目有助於防止忙線訊號，並可讓您設定的通道或通話中心之類的應用程式專設的行數。正確地設定 PBX 是因為它減少所需的租用行數管理的通道或組織中的行符合成本效益的方法。

PBX 可路由的特定撥打的電話號碼的特定的電話，讓使用者可以有其專屬的個別的電話號碼或分機號碼。這就是所謂的直接向內撥號號碼。當使用者撥打的電話號碼時，電話公司會傳送到 PBX DID 號碼使用之撥號號碼識別服務 (DNIS)。由於電話公司使用 DNIS 傳送數字，所以沒有路由傳送通話的運算子介入需要。PBX 有正確路由至發話者所撥打的號碼的電話的相關資訊。如需支援的整合通訊的 Pbx 的清單，請參閱[Exchange 2013 的電話語音 advisor](https://docs.microsoft.com/zh-tw/exchange/voice-mail-unified-messaging/telephone-system-integration-with-um/telephony-advisor-for-exchange-2013)。

回到頁首

## 類比與數位 PBX

類比 Pbx 傳送語音和通話訊號資訊，例如撥打的電話號碼、 觸控音為類比音效。因此，音效會永遠不數位。若要正確直接呼叫、 PBX 與電話公司的中央 office 必須聆聽的訊號的資訊。


> [!NOTE]  
> 按鍵式更嚴格來說稱為雙音多頻率。當來電者按下電話鍵盤上的按鍵時，電話會產生兩種不同音： 高頻率音和低頻率音。人員會將電話播放，會發出只有單一音或頻率。傳送兩種音與不同頻率，同時減少訊號音會被解譯為人工語音或人工語音會被解譯為訊號音的可能性。




數位 Pbx 編碼或成數位格式 digitize 類比音效。數位 Pbx 通常編碼使用 G.711 或 G.729 標準產業音訊轉碼器的聲音。編碼數位的語音之後，將其傳送通道上使用電路切換。設定端對端的電路切換集開啟連線。通道離開開啟通話長度與來電者的獨佔式使用。不過，在 PBX 所使用的訊號方法製造商而定。PBX 製造商可能擁有自己的專利訊號通話安裝程式的方法。


> [!NOTE]  
> 數位 PBX 可支援數位與類比長途電話線。




在大型組織中 Pbx 讓可以在不同的實體位置的員工連絡另一個使用者的分機號碼。這可以透過使用單一 PBX 完成或可能會涉及多個網路相連的 Pbx。在不同的辦公室位置 Pbx 可從單一的透明電路切換型網路連線使用 T1 或 E1 線路。當這些行連接 Pbx 在一起時，這些常稱為*tie lines*。Pbx 彼此之間使用 PBX-PBX 通訊協定，例如 QSIG 平局行。QSIG 讓一組 Pbx act 好像他們是單一的 PBX。

這種 PBX 的環境也可以包含進階的功能，例如通話傳輸和電話會議。除了容許進階功能，有兩個相連的 pbx 設定也可以將儲存組織 money 因為會降低員工的不同位置間的長途電話費。這是因為兩個員工之間的通話停留在 Pbx 之間平局列並要求使用者撥號對應表只針對其他使用者，而不是通長途電話來電的分機號碼。

在包含一個或多個類比或數位 Pbx 電話語音環境中，VoIP 閘道，則需要在 PBX 與Exchange 2013用戶端存取和信箱伺服器之間轉換成資料網路上找到的 IP 型通訊協定的電話語音網路上找到的電路型通訊協定。如需 VoIP 閘道器的詳細資訊，請參閱下列主題：

  - [UM IP 閘道](https://docs.microsoft.com/zh-tw/exchange/voice-mail-unified-messaging/connect-voice-mail-system/um-ip-gateways)

  - [Connect a VoIP 閘道與 PBX 通訊](connect-a-voip-gateway-to-communicate-with-a-pbx-exchange-2013-help.md)

如需整合通訊支援的 VoIP 閘道清單，請參閱 [Exchange 2013 的電話語音 advisor](https://docs.microsoft.com/zh-tw/exchange/voice-mail-unified-messaging/telephone-system-integration-with-um/telephony-advisor-for-exchange-2013)。

回到頁首

## IP PBX 組態

將 IP PBX 是支援 IP 通訊協定使用乙太網路或封包切換 LAN 連線散 PBX。它會語音交談傳送 IP 或資料封包。將 IP PBX 可能會有多個介面。這些包括資料的網路介面與其他允許的電話語音或電路切換型網路連線的介面。

即時的網際網路通訊協定的開發具有進行可能已順利傳送語音和傳真訊息透過資料網路。這類即時的網際網路通訊協定包含與整合通訊的 VoIP 通訊協定： 工作階段初始通訊協定 (SIP) 透過傳輸控制通訊協定 (TCP) 為語音訊息。這些通訊協定已進行可能已順利傳送語音和傳真訊息透過資料網路。即時 VoIP 通訊協定所將語音郵件傳送封包切換或資料的網路上以便傳遞順序與 timing 資料封包可以維護和控制。如果未使用下列通訊協定來維護和控制傳遞和資料封包的時機、 人員語音會細分及聲音不一致或圖像可能會出現亂碼。如需支援的整合通訊 IP Pbx 的清單，請參閱[Exchange 2013 的電話語音 advisor](https://docs.microsoft.com/zh-tw/exchange/voice-mail-unified-messaging/telephone-system-integration-with-um/telephony-advisor-for-exchange-2013)。


> [!NOTE]  
> 整合通訊只支援 SIP over TCP。




## 傳統 IP PBX 組態

標準或傳統 IP PBX 包含至少單一網路介面所使用 VoIP 通訊協定的資料網路連線。它也可能會包含其他的網路介面或其他啟用其連線至現有電話語音網路等 PSTN 的電話語音介面。其他位於資料在網路上使用 IP 資料封包的 VoIP 主機通訊允許資料網路的連線。這些 VoIP 主控包括其他 IP Pbx、 VoIP 型電話、 VoIP 閘道和用戶端存取及執行 UM 服務的信箱伺服器。將傳統 IP PBX 不支援類比或數位散。它支援僅限 VoIP 電話。

因為 IP PBX 可能已連接至資料網路並將 PSTN 的電路通訊協定轉換為封包交換型 VoIP 通訊協定，所以可能不需要 IP 閘道即可與資料網路上的 Client Access Server 和 Mailbox Server 通訊。

## IP PBX 混合式組態

混合式 IP Pbx 可以提供類比、 數位和 VoIP 為基礎的功能。如果將 IP PBX 上已安裝正確的介面並已正確安裝的軟體支援多個介面的類型、 IP PBX 會被視為混合式 IP PBX。IP PBX 混合式讓類比、 數位和 IP 型散混合使用。

新的 IP PBX 大多可支援及提供三種語音通訊，要不然，傳統 IP PBX 安裝必要的介面與軟體或韌體更新，也可升級至混合式 IP PBX。

混合的類比、 數位和 IP 型散讓使用者在組織中使用許多新功能和也會提供更好的彈性電話語音環境中。使用 IP PBX 混合式也可讓更多逐步移轉完全 VoIP 型電話語音環境及語音郵件系統為您組織的。

多個因素決定 VoIP 閘道可在用戶端存取和信箱伺服器連線時所需。這些因素是 IP PBX 或 IP PBX 混合式和整合通訊所使用的 VoIP 通訊協定的相容性。如果不需要 VoIP 閘道，它會降低的電話語音基礎結構的複雜性，您必須具備的整合通訊的支援將簡化。

回到頁首

## 發話方或受話方識別

呼叫或被呼叫方識別是電話公司服務可以接聽來電者的電話號碼及告知有時會呼叫者和通話的其他資訊的名稱。此資訊是使用通話訊號傳送透過序列纜線。從公司電話的 PBX 或 IP PBX 接到電話，通話會包含呼叫識別資訊如下所示：

  - 呼叫方的號碼

  - 受話方的號碼

  - 狀態碼 (例如無人接聽)、線路的狀態或狀況、忙線與來電一律轉接。

  - 通話使用的線路或通訊埠號碼

  - 在 \[電話語音、 訊號資訊用來交換來設定、 控制、 網路上的端點之間的資訊，並結束呼叫。由整合通訊支援數種 VoIP 閘道和 IP Pbx 所使用的訊號方法使用的訊號方法而定的正在使用的裝置類型與電話公司所使用的訊號方法的類型。最重要因素是已連接到電話公司和 VoIP 閘道或 IP PBX 的裝置必須支援至少其中一個訊號方法可讓呼叫或被呼叫一起傳送和接收到來電者的廠商資訊。如需訊號支援 VoIP 閘道的組態資訊的詳細資訊，請參閱[Exchange 2013 的電話語音 advisor](https://docs.microsoft.com/zh-tw/exchange/voice-mail-unified-messaging/telephone-system-integration-with-um/telephony-advisor-for-exchange-2013)。

雖然有其他信號方法可以使用，但兩個最普遍的信號方法為：

  - <strong>簡體中文訊息服務台介面 (SMDI)：</strong> SMDI 是用來提供訊號通話控制和電話系統和語音信箱系統之間介面中的呼叫識別資訊通訊協定。它用來提供語音信箱系統需要處理來電的資訊。每次來電傳送透過 SMDI 序列介面或 RS 232 介面、 線條或連接埠、 通話、 類型及呼叫或被呼叫方號碼識別傳送的資訊。SMDI 纜線連接從裝置例如 PBX 與 VoIP 閘道上的序列連線。不過，SMDI 也會使用與 IP Pbx。SMDI 通訊協定允許只 10 位數的每個通話的最大值並呼叫數。這是通訊協定的限制，且無法變更。

  - <strong>頻內︰</strong>頻內訊號允許訊號，呼叫控制和電話公司從呼叫識別資訊的交換。此資訊會傳送相同通道上並在同一個頻內 (以 3.4 kHz 300 Hz) 為語音與通話期間進行其他音效。例如，當使用者撥打電話使用 DTMF 或按鍵式撥號和談到稱為方、 按鍵和語音交談使用相同的通道和頻內。因為控制信號公開給使用者，而且是較熱門的訊號方法比 SMDI 頻內訊號為較不安全。頻內訊號套用只以通道相關聯訊號 (CAS)。

回到頁首

