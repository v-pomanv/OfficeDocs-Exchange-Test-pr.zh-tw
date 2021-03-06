﻿---
title: 'Exchange 2013 的新功能: Exchange 2013 Help'
TOCTitle: Exchange 2013 的新功能
ms:assetid: 97501135-2149-4590-8373-98e638ac8eb1
ms:mtpsurl: https://technet.microsoft.com/zh-tw/library/JJ150540(v=EXCHG.150)
ms:contentKeyID: 50473827
ms.date: 01/12/2018
mtps_version: v=EXCHG.150
ms.translationtype: HT
---

# Exchange 2013 的新功能

 

_**適用版本：** Exchange Server 2013_

_**上次修改主題的時間：** 2016-12-09_

查看 Exchange 2013 中的所有最新功能。

Microsoft Exchange Server 2013 為 Exchange Server 產品線帶來豐富的新科技、功能與服務。其目標是為了因應個人和組織不斷增加的協同作業需求與不斷改變的通訊習慣。在此同時，Exchange Server 2013 還可降低您的整體擁有成本，不管是進行 Exchange 2013 內部部署或在雲端佈建信箱皆然。Exchange 2013 所設計的新特色和功能如下：

  - **支援多世代的工作力**  對使用者來說，與社交媒體整以及找人更輕鬆非常重要。*智慧搜尋* 學習使用者通訊和協同合作行為，以加強並確定 Exchange 搜尋結果的優先順序。此外，有了 Exchange 2013，使用者可以將多個來源的連絡人合併，以提供單一的個人檢視畫面，方法是將多個位置的連絡人連結在一起即可。

  - **提供引人入勝的體驗**  Microsoft Outlook 2013 和 Microsoft Outlook Web App 提供一個全新的外觀，Outlook Web App 具有精簡的使用者介面並採用觸控功能，可提升使用行動裝置與 Exchange 的經驗。

  - **整合 SharePoint 和 Lync**  Exchange 2013 透過站台信箱和就地 eDiscovery 讓Microsoft SharePoint 2013 和 Microsoft Lync 2013 強力整合。這些產品提供一組功能，可供使用網站信箱進行企業 eDiscovery 和共同作業等之用。

  - **幫助符合不斷改變的法務遵循需求** 法務遵循和 eDiscovery 對許多組織來說一直都深具挑戰性，Exchange 2013 不僅可協助您搜尋和尋找 Exchange 中的資料，還可跨組織尋找資料。隨著搜尋和索引功能的改善，您可跨 Exchange 2013、Lync 2013、SharePoint 2013 和 Windows 檔案伺服器進行搜尋。此外，資料遺失防護 (DLP) 的功能可協助您保護組織資料安全，避免使用者誤將敏感資訊傳送給未經授權人士。透過深度內容分析，DLP 可協助您識別、監視和保護機密資料。

  - **提供彈性的解決方案**  Exchange 2013 建立在 Exchange Server 2010 架構上，已重新設計簡化了範圍、硬體使用率和故障隔離程序。

如需 Exchange Server 2013 自量產發行 (RTM) 版本後所進行之變更的相關資訊，請參閱 [更新 Exchange 2013](updates-for-exchange-2013-exchange-2013-help.md)。

如需有關 Exchange 2013 的最新資訊，請參閱以下部分：

Exchange 系統管理中心

Exchange 2013 架構

安裝程式

郵件原則及符合性

反惡意程式碼保護

郵件流程

收件者

共用和協同合作

與 SharePoint 和 Lync 整合

用戶端和行動裝置

整合通訊

批次信箱移動

[高可用性和站台恢復](high-availability-and-site-resilience-exchange-2013-help.md)

Exchange 工作負載管理


> [!NOTE]  
> 如需 Exchange Server 2013 中已移除、中止或更換之舊版 Exchange 的相關功能資訊，請參閱<a href="what-s-discontinued-in-exchange-2013-exchange-2013-help.md">Exchange 2013 已中止的功能</a>。另外，您可能對 <a href="release-notes-for-exchange-2013-exchange-2013-help.md">Exchange 2013 版本資訊</a> 有興趣。




## Exchange 系統管理中心

Exchange 2013 提供單一整合的管理主控台，讓使用者更方便使用且最佳化內部部署、線上或混合部署的管理。Exchange 2013 中的 *Exchange 系統管理中心* (EAC) 會取代 Exchange 2010 Exchange 管理主控台 (EMC) 和 Exchange 控制台 (ECP)(不過，“ECP” 仍然是 EAC 所用之虛擬目錄的名稱)。EAC 的一些功能包括：

  - **清單檢視**  EAC 中的清單檢視功能已移除 ECP 中存在的按鍵限制。ECP 過去限制顯示最多 500 個物件，如果您要檢視未列於詳細資料窗格中的物件，就必須使用搜尋和篩選功能來尋找這些特定物件。在 Exchange 2013 中，從 EAC 清單檢視內可檢視的限制則約為 20,000 個物件。在 EAC 傳回結果後，EAC 用戶端會執行搜尋和排序，如此可大幅提高效能 (相較於 Exchange 2010 中的 ECP)。此外還新增分頁功能，讓您可以針對結果分頁。您還可以設定頁面大小並將其匯出到 .csv 檔。

  - **新增/移除收件者清單檢視中的欄位**  您可選擇要檢視的欄位為何，而且有了本機 Cookie，您便可使用存取 EAC 的每台機器來儲存自訂清單檢視。

  - **保護 ECP 虛擬目錄安全**  您可在 ECP IIS 虛擬目錄中分割網際網路和內部網路的存取，以允許或不許使用管理功能。有了這個功能，您可以允許或拒絕嘗試從組織環境外部網際網路存取 EAC 的使用者存取，同時允許存取使用者的 Outlook Web App 選項。

  - **公用資料夾管理**  在 Exchange 2010 和 Exchange 2007 中，公用資料夾是透過公用資料夾系統管理主控台進行管理。公用資料夾現在則位於 EAC 中，不需要另外的工具來管理這些資料夾。

  - **通知**  在 Exchange 2013 中，EAC 現在有通知檢視器，讓您檢視長時間執行程序的狀態，而且您可以選擇在程序完成時透過電子郵件訊息收到通知。

  - **角色存取控制 (RBAC) 使用者編輯器**  在 Exchange 2010 中，您可以在 Exchange 工具箱中使用 RBAC 使用者編輯器，來新增使用者以管理角色群組。在 Exchange 2013 中，RBAC 使用者編輯器現在已可在 EAC 找到，而且您不需要另外一套工具來管理 RBAC。

  - **整合通訊工具**  在 Exchange 2010 中，您可以使用呼叫統計資料和使用者通話記錄工具，協助提供啟用 UM 之使用者特定來電的 UM 統計資料和資訊。在 Exchange 2013 中，呼叫統計資料和使用者通話記錄工具現在已可在 EAC 中找到，而且您不需要另外一套工具來管理這些內容。

  - **群組增強功能**  Exchange 系統管理中心 (EAC) 現在可在 \[群組\] \[選取成員\] 視窗中顯示多達 10,000 名收件者。當您開啟 \[選取成員\] 視窗時，預設會傳回多達 500 名收件者，但您可以按一下收件者清單下方的 \[取得所有結果\]，以列出多達 10,000 名的收件者。我們現在支援使用捲軸瀏覽 500 名以上的收件者，而且也新增增強的搜尋功能，可讓您篩選收件者清單中顯示的收件者。您可以依據下列項目進行篩選：
    
      - 縣/市
    
      - 公司
    
      - 國家/地區
    
      - 部門
    
      - 辦公室
    
      - 職稱

如需詳細資訊，請參閱 [Exchange 2013 中的 Exchange 系統管理中心](exchange-admin-center-in-exchange-2013-exchange-2013-help.md)。

## Exchange 2013 架構

舊版的 Exchange 之前已最佳化過，其架構仍有部分技術限制。例如，在部署 Exchange 2007 期間，其中一個主要限制是 CPU 的效能。為了減緩限制，Exchange 2007 被分割成不同的伺服器角色，以透過伺服器分割允許範圍。但是，Exchange 2007 和 Exchange 2010 中的伺服器角色已緊密結合在一起。角色的緊密結合有幾個缺點，包括版本依存關係、地理親和性 (需要所有角色同屬某一特定站台)、工作階段親和性 (需要昂貴的層級 7 硬體載入平衡) 以及命名空間複雜性。

今日，CPU 的維護成本已大幅降低，昂貴的成本不再是一項限制因素。隨著該限制的解除，Exchange 2013 簡化範圍、硬體使用率和故障隔離的主要設計目標得以實現。有了 Exchange 2013，我們可以將伺服器角色的數量減為三個：Client Access、Mailbox 和 Edge Transport server role。

信箱伺服器包含所有可於 Exchange 2010 中找到的伺服器元件：用戶端存取協定、 傳輸服務、 信箱資料庫和整合通訊。信箱伺服器處理所有該伺服器使用中信箱的所有活動。用戶端存取伺服器提供驗證、 有限重新導向和代理服務。用戶端存取伺服器本身不做任何資料轉譯。用戶端存取伺服器為精簡且無狀態的伺服器。戶端存取伺服器上永遠不會佇列或儲存任何東西。用戶端存取伺服器提供所有常見的用戶端存取協定：HTTP、POP 與 IMAP 以及 SMTP。

有了此一架構，用戶端伺服器和信箱伺服器將變成所謂的「鬆散藕合」。特定信箱的所有處理程序和活動都會在駐留該信箱使用者資料庫副本所在位置之信箱伺服器上發生。所有資庫呈現和資料轉換都將在使用中資料庫副本的本機執行，消除用戶端伺服器和信箱伺服器之間版本不相容的疑慮。

透過 Exchange 2013 Service Pack 1，我們已經重新引進 Edge Transport server role。Edge Transport role 通常會部署在周邊網路、內部 Active Directory 樹系之外，以及設計來將 Exchange 部署的攻擊面減至最小。藉由處理所有連結網際網路的郵件流程，它也會新增其他的郵件保護及安全層，以防止病毒和垃圾郵件，並可套用傳輸角色來控制郵件流程。如需 Edge Transport Server role 的相關資訊，請參閱 [Edge Transport Server](edge-transport-servers-exchange-2013-help.md)。

Exchange 2013 架構具有下列好處：

  - **版本升級彈性**  沒有更多固定的升級要求。用戶端存取伺服器可以單獨且按任何信箱伺服器相關順序升級。

  - **工作階段差異**  使用 Exchange 2010，用戶端存取伺服器需要部分通訊協定具有工作階段親和性。在 Exchange 2013 中，用戶端存取和信箱元件會存放在同一個信箱伺服器上。因為用戶端存取伺服器只是為使用者將所有連線代理到特定信箱伺服器，用戶端伺服器並不需要工作階段親和性。這讓用戶端存取伺服器的傳入連線可以採用最少連線或 round-robin 這類負載平衡技術技巧來進行平衡。

  - **部署簡單**  有了 Exchange 2010 的彈性站台設計，您最多只需要八個不同命名空間：兩個供網際網路命名空間之用、兩個供 Outlook Web App 後原動作之用、一個供 Autodiscover 使用、兩個供 RPC 用戶端存取之用，另外一個供 SMTP 使用。如果您是從 Exchange 2003 或 Exchange 2007 升級，還是需要傳統命名空間。有了 Exchange 2013，命名空間的數量可減到兩個。如果您與 Exchange 2007 共用命名空間，您仍需要建立一個傳統命名空間，但如果您與 Exchange 2010 或您所安裝新 Exchange 2013 組織共用命名空間，您只需要兩個命名空間：一個用於用戶端通訊協定，另一個用於自動探索。您可能還需要一個 SMTP 命名空間。

架構性變更會導致用戶端連接性也有部分變更。首先，RPC 不再是支援的直接存取通訊協定。換句話說，所有 Outlook 連線都必須使用 RPC over HTTPS (也稱為 Outlook Anywhere) 連線。乍看之下，這似乎會使連線受限，但實際上這種方法提供了一些額外好處。最顯而易見的好處是，用戶端存取伺服器上不需要有 RPC 用戶端存取服務。這使得平常彈性站台解決方案所需的命名空間可以減至兩個。此外，也沒有提供 RPC 用戶端存取服務親和性的必要。

而且，Outlook 用戶端不必再像所有舊版 Exchange 一樣，得連線到 FQDN。Outlook 會使用自動探索來建立新連線點，該連線點由信箱 GUID、@ 符號和使用者 SMTP 主位址的網域部分組成。這個動作只會刪除不受歡迎的訊息「管理員已變更您的信箱，請重新開機。」僅 Outlook 2007 和更高版本支援 Exchange 2013。

自 Exchange 2010 起，信箱元件的高可用性模組並未有重大變更，高可用性的單位仍然是資料庫可用性群組 (DAG)。DAG 仍使用 Windows 伺服器容錯移轉叢集。連續複製仍然支援檔案模式和區塊模式複製。但是，這裡也有一些改進。由於移轉記錄代碼的改進與被動資料庫上檢查點的強化，所以縮短了容錯移轉時間。Exchange 儲存區服務在 Managed 程式碼中已重寫 (請參閱本主題稍後的「管理的儲存區」一節)。現在，每一個資料庫會在其所有處理程序下執行，以將儲存區問題隔離到另一個單一資料庫中。

## 管理的儲存區

在 Exchange 2013 中，*管理的儲存區*是重寫的最新資訊儲存區處理程序 Microsoft.Exchange.Store.Service.exe 和 Microsoft.Exchange.Store.Worker.exe 的名稱。新的 \[管理的儲存區\] 是以 C\# 編寫，與 Microsoft Exchange 複寫服務 (MSExchangeRepl.exe) 緊密整合，透過改善彈性提供更高的可用性。除此之外，透過診斷方法的改善，「管理的儲存區」也變成可允許細微管理更多資源耗用與加速根本原因分析的架構。

「管理的儲存區」可與 Microsoft Exchange 複寫服務一同用來管理信箱資料庫，該複寫服務持續使用可延伸儲存引擎 (ESE) 作為資料庫引擎。Exchange 2013 對資料庫結構描述含有重大變更，對舊版 Exchange 提供許多最佳化功能。除了這些變更外，Microsoft Exchange 複寫服務也負責處理所有與信箱伺服器相關的服務可用性。此架構的變更使資料庫的容錯移轉更快，並改善實體磁碟故障的處理方式。

「管理的儲存區」也和 Search Foundation 搜尋引擎 (SharePoint 2013 所使用的同一個搜尋引擎) 整合在一起，以提供比舊版 Exchange 提供之 Microsoft Search 更強的索引和搜尋功能。

如需詳細資訊，請參閱 [高可用性和站台恢復](high-availability-and-site-resilience-exchange-2013-help.md)。

## 憑證管理

管理數位憑證是 Exchange 組織最重要的安全工作之一。確認憑證適當設定是為企業提供郵件安全傳遞基礎結構的關鍵。在 Exchange 2010 中，Exchange 管理主控台是管理憑證的主要方法。在 Exchange 2013 中，憑證管理功能是透過 Exchange 系統管理中心的新 Exchange 2013 系統管理員使用者介面提供。

Exchange 2013 的任務是著重在減少系統管理員必須管理的憑證數量，減少系統管理員需與憑證互動的機會，以及允許透過集中位置來管理憑證。憑證管理的改變所產生的好處如下：

  - 可在用戶端伺服器或信箱伺服器上執行憑證管理。依預設，信箱伺服器已安裝了自我簽署的憑證。用戶端存取伺服器會自動信任 Exchange 2013 信箱伺服器上自我簽署的憑證，所以用戶端不會收到 Exchange 2013 用戶端伺服器所提供，來自 Windows 憑證授權單位 (CA) 或信任的協力廠商之非自我簽署憑證的自我簽署憑證不被信任的警告。

  - 在舊版 Exchange 中，很難看見數位憑證的到期日為何。在 Exchange 2013 中，當任何 Exchange 2013 伺服器上所儲存的憑證到期時，通知中心將會顯示警告。系統管理員也可以選擇透過電子郵件接收這些通知。

如需詳細資訊，請參閱 [數位憑證和 SSL](digital-certificates-and-ssl-exchange-2013-help.md)。

## 安裝程式

安裝程式已完全重寫，所以安裝 Exchange 2013 和確認是否已取得最新產品彙總套件和安全修正檔的程序史無前例的輕鬆。這裡是我們所做的一些改進：

  - **永遠提供最新的安裝程式**  當您執行「安裝程式」精靈時，您會收到下載和使用最新版產品彙總套件、安全修復檔和語言套件的選項。此選項不只會更新執行 Exchange 所用的檔案；安裝程式本身也會更新。此設計可讓我們於發佈後繼續改善安裝程式，並在要求更新或變更後加入和更新整備檢查。
    
    如果您使用無人看管的安裝模式，我們不能自動下載更新。不過，您仍可以利用最新版安裝程式事先下載最新的更新，同時使用 `/UpdatesDir: <path>` 參數讓安裝程式在開始安裝程序前自行更新。

  - **改善就緒檢查**  就緒檢查可確認您的電腦和組織是否準備好安裝 Exchange 2013。在您收到必必要的安裝資訊後，安裝開始前就會執行就緒檢查。新的就緒檢查引擎現在會在繼續安裝與回報您需要執行哪些動作前執行所有檢查，而且檢查速度比之前更快。利用舊版 Exchange，您可告訴安裝程式安裝哪些所需的 Windows 功能，而不必另外手動安裝。

  - **簡化和現代化的精靈**  我們已將所有安裝 Exchange 不一定需要的步驟從安裝程式精靈移除。剩下的就是一個可一次簡易安裝的精靈，引導您完成安裝程序。

如需詳細資訊，請參閱 [規劃及部署](planning-and-deployment-for-exchange-2013-installation-instructions.md)。

## 郵件原則及符合性

Exchange 2013 有兩個全新的郵件原則和符合性功能：資料外洩防護和 Microsoft 權限管理連接器。

*資料外洩防護* (DLP) 功能可協助您保護機密資料，並告知使用者內部的符合性原則。DLP 還可協助您維持組織安全，以防止使用者可能誤將機密資訊傳送給未授權人員。DLP 有助於您識別、監視和保護機密資料。Exchange 2013 可根據個人識別資訊 (PII) 和支付卡產業資料安全標準協會 (PCI) 等法規標準提供內建的 DLP 原則，同時可延伸支援企業其他重要原則。此外，Outlook 2013 中的新 PolicyTip 會在傳送機密資料前，通知使用者相關違規原則。

Microsoft 權限管理連接器 (RMS 連接器) 是選用應用程式，可透過連線到雲端式的 Microsoft 權限管理服務，協助您增強 Exchange 2013 伺服器的資料防護。安裝 RMS 連接器之後，它可在資訊的整個週期提供持續的資料保護，並且因為這些是可自訂的服務，所以您可以定義所需的保護層級。例如，您可以限制特定使用者才能進行電子郵件存取，或針對特定郵件設定僅限檢視權限。

若要深入了解這些功能，請參閱：

[資料遺失防護](https://docs.microsoft.com/zh-tw/exchange/security-and-compliance/data-loss-prevention/data-loss-prevention)

[版權管理連接器](https://go.microsoft.com/fwlink/p/?linkid=330432)

## 就地封存、 保留和 eDiscovery

Exchange 2013 包含以下就地封存、 保留和 eDiscovery 的改善，有助於組織符合法務遵循需求：

  - **就地保留** 就地保留是一種新的整合保留模式，讓您在以下案例符合法律封存需求：
    
      - 保留查詢結果 (查詢型保留)，允許跨信箱的範圍不變性。
    
      - 放置時間型保留以符合保留要求 (例如，保留信箱中所有項目七年、需要在 Exchange 2010 中使用單一項目搜索/刪除項目保留的情況)。
    
      - 在無限保留上放置一個信箱 (類似 Exchange 2010 中的訴訟暫止)。
    
      - 放置一個使用者在多個保留上，以符合不同案例的要求。

  - **就地 eDiscovery**  就地 eDiscovery 允許授權的使用者在 Exchange 2013 組織中跨所有信箱和就地封存來搜尋信箱資料，並複製郵件至探索信箱供預覽。在 Exchange 2013 中，就地 eDiscovery 已升級為允許探索管理程式以執行更多的有效搜尋和保留。這些增強功能包括：
    
      - **同盟搜尋** 允許您跨整個資料存放庫搜尋和保留資料。有了 Exchange 2013，您可跨 Exchange、SharePoint 2013 和 Lync 2013 執行就地 eDiscovery 搜尋。您也可以使用 SharePoint 2013 中的 eDiscovery 中心執行就地 eDiscovery 搜尋和保留。
    
      - **查詢型就地保留** 允許您儲存查詢結果，該查詢允許跨信箱的範圍不變性。
    
      - **匯出搜尋結果** 探索管理程式可從 SharePoint 2013 eDiscovery 主控台將信箱內容匯出為 .pst 檔。信箱匯出要求指令程式不再需要將信箱匯出為 .pst 檔。
    
      - **關鍵字統計資料**  搜尋統計資料可按搜尋字詞提供分析統計資料。這可讓探索管理程式對如何進一步縮小搜尋查詢快速作出最佳決定，以提供最佳結果。eDiscovery 搜尋結果是按相關性排序。
    
      - **KQL 語法**  探索管理程式可以在搜尋查詢中使用關鍵字查詢語言 (KQL) 語法。KQL 與 Exchange 2010 中探索搜尋所用的進階查詢語法 (AQS) 類似。
    
      - **就地 eDiscovery 和保留精靈**  探索管理程式可以使用新的就地 eDiscovery 和保留精靈來執行 eDiscovery 和保留操作。
        
        > [!NOTE]  
        > 如果 SharePoint 2013 無法使用，Exchange 系統管理中心可提供 eDiscovery 功能的子集。


  - **在 Outlook Web App 中跨主要和封存信箱搜尋**  使用者可以在 Outlook Web App 中跨主要和封存信箱進行搜尋。另外兩個搜尋則不再必要。

  - **封存 Lync 內容**  Exchange 2013 支援在使用者信箱中封存 Lync 2013 內容。您也可以使用就地保留將 Lync 內容保留，或使用就地 eDiscovery 來搜尋 Exchange 中封存的 Lync 內容。

  - **保留原則**  保留原則可幫助您的組織降低電子郵件和其他通訊風險，同時符合電子郵件保留的要求。保留 則包括下列增強功能：
    
      - **支援 \[行事曆\] 和 \[工作\] 保留標記**  您也可以針對 \[行事曆\] 和 \[工作\] 預設資料夾建立保留原則標記，以將過期項目移到這些資料夾中。這些資料夾中的項目也會根據信箱所套用的封存原則設定移動到使用者的封存中。
    
      - **改善特定期間保留項目的能力**  您可使用保留原則和時間型就地保留功能，強化某一段時間保留項目的能力。

如需詳細資訊，請參閱 [郵件原則及符合性](messaging-policy-and-compliance-exchange-2013-help.md)。

## 傳輸規則

在 Exchange Server 2013 中的傳輸規則，在 Exchange Server 2010 中一樣可繼續使用。然而，在 Exchange 2013 中的傳輸規則有一些變更。最重要的變更是支援資料遺失防護 (DLP) 的功能。另外，也提供了一些新述詞和動作、提升監視功能並增加一些架構變更。

如需詳細資訊，請參閱[傳輸規則的新功能](what-s-new-for-transport-rules-exchange-2013-help.md)。

## 資訊版權管理

資訊版權管理 (IRM) 與密碼編譯模式 2 相容，Active Directory Rights Management Services (AD RMS) 密碼編譯模式透過使用 RSA 的 2048 位元金鑰和 SHA-1 的 256 位元金鑰，提供更強的加密支援。此外，模式 2 可讓您使用 SHA-2 雜湊演算法。如需 AD RMS 中有關密碼編譯模式的更多詳細資訊，請參閱 [AD RMS 密碼編譯模式](https://go.microsoft.com/fwlink/p/?linkid=263219)。

## 稽核

Exchange 2013 包含下列關於稽核的改進功能：

  - **稽核報告**  EAC 包含稽核報告功能，所以您可以從信箱稽核記錄與系統管理員稽核記錄來執行稽核報告或匯出項目。信箱稽核記錄會記錄信箱擁有者以外人員存取信箱的行為。這種記錄可以協助您判斷存取信箱的人員以及他們進行的動作。系統管理員稽核記錄會記錄系統管理員所執行的任何動作 (以 Exchange 管理命令介面指令程式為基礎)。這種記錄可以協助您疑難排解組態問題，或識別安全性或法務遵循相關問題的原因。如需詳細資訊，請參閱 [Exchange 稽核報告](https://docs.microsoft.com/zh-tw/exchange/security-and-compliance/exchange-auditing-reports/exchange-auditing-reports)。

  - **檢視系統管理員稽核記錄**  您不需要匯出系統管理員稽核記錄，並等待長達 24 小時才收到以電子郵件寄送的系統管理員稽核記錄，您可以在 EAC 中檢視系統管理員稽核記錄項目。若要這麼做，請移至 \[規範管理\] \> \[稽核\]，並按一下 \[檢視系統管理員稽核記錄\]。可在多個頁面上顯示最多 1000 個項目。若要縮小搜尋範圍，您可以指定日期範圍。如需詳細資訊，請參閱[檢視系統管理員稽核記錄](https://docs.microsoft.com/zh-tw/exchange/security-and-compliance/exchange-auditing-reports/view-administrator-audit-log)。

## 反惡意程式碼保護

Exchange 2013 內建惡意程式碼篩選功能，可幫助您保護網路，免在電子郵件傳輸時遭惡意程式碼軟體攻擊。Exchange 伺服器會掃描所有所有 Exchange 傳送或接收的郵件是否有惡意程式碼 (病毒和間諜軟體)。如果偵測到惡意程式碼，該郵件將被刪除。當郵件因被感染而刪除或無法傳遞時，寄件者或系統管理員可能也會傳送通知給您。您也可以將受感染的附件更換為預設或自訂郵件，以通知收件者偵測電腦是否有惡意程式碼。

如需有關反惡意程式碼保護的詳細資訊，請參閱[反惡意程式防護](anti-malware-protection-exchange-2013-help.md)。

## 郵件流程

組織中的郵件流程為何？為何在 Exchange 2013 中這些功能有重大改變？以下針對所做變更提供簡要概述：

  - **傳輸管線**  在 Exchange 2013 中的傳輸管線現在已由幾種不同服務取代：用戶端存取伺服器上的前端傳輸服務、信箱伺服器上的傳輸服務以及信箱伺服器上的信箱傳輸服務。如需詳細資訊，請參閱 [郵件流程](mail-flow-exchange-2013-help.md)。

  - **路由**  在 Exchange 2013 中路由的郵件會被識為 DAG 界限及 Active Directory 站台界限。此外，郵件路由已經改善，以更直接的方式為內部收件者佇列郵件。如需詳細資訊，請參閱 [郵件路由](mail-routing-exchange-2013-help.md)。

  - **連接器**  傳送連接器和接收連接器的預設郵件大小上限，如 *MaxMessageSize* 參數所指定的已由 10MB 增加為 25MB。如需有關如何設定連接器參數的更多詳細資訊，請參閱 [Set-SendConnector](https://technet.microsoft.com/zh-tw/library/aa998294\(v=exchg.150\)) 和 [Set-ReceiveConnector](https://technet.microsoft.com/zh-tw/library/bb125140\(v=exchg.150\))。
    
    您可透過本機 Active Directory 站台的前端傳輸伺服器，在信箱伺服器的傳輸服務中設定傳送連接器，方法是使用 **Set-SendConnector**指令程式的 *FrontEndProxyEnabled* 參數，從而鞏固如何從傳輸服務路由郵件的方法。

  - **Edge Transport**   您可以選擇性地將 Edge Transport Server 安裝在您的周邊網路，以減少攻擊面，並提供郵件保護和安全性。如需詳細資訊，請參閱 [Edge Transport Server](edge-transport-servers-exchange-2013-help.md)。

## 收件者

本節介紹 Exchange 2013 中管理收件者的增強功能：

  - **群組命名原則**  系統管理員現在可以使用 EAC 來建立*群組命名原則*，該原則可讓您標準化和管理組織中使用者所建立的通訊群組名稱。您可以要求使用者在建立通訊群組時，將特定首碼和尾碼新增至通訊群組的名稱，而且您可以封鎖特定字詞，防止使用這些字詞。此功能有助於減少群組名稱中不當字詞的使用。
    
    如需詳細資訊，請參閱 [建立通訊群組命名原則](https://docs.microsoft.com/zh-tw/exchange/recipients-in-exchange-online/manage-distribution-groups/create-group-naming-policy)。

  - **郵件追蹤**  系統管理員也可以使用 EAC 來追蹤組織中使用者所接收或傳送之電子郵件的傳遞資訊。您只要選取信箱，然後搜尋不同使用者所傳送或接收的郵件即可。您可以搜尋主旨行中的特定文字，藉以縮小搜尋的範圍。產生的傳遞回報會透過傳遞程序追蹤郵件，並且指定郵件已成功傳遞、擱置傳遞或尚未傳遞。
    
    如需詳細資訊，請參閱 [使用傳遞回報追蹤郵件](track-messages-with-delivery-reports-exchange-2013-help.md)。

## 共用和協同合作

本節介紹 Exchange 2013 中的共用和協同合作增強功能。

  - **公用資料夾**  公用資料夾現在可善用信箱儲存區現有的高可用性和儲存技術。公用資料夾架構使用特殊設計的信箱來儲存階層與公用資料夾內容。新設計也意味著再也沒有公用資料夾資料庫。公用資料夾複寫目前使用連續複寫模型。階層和內容信箱的高可用性是由資料庫可用性群組 (DAG) 提供。藉由此設定，我們可以從多重主要發行集模式移到單一主要發行集模式。
    
    組織中的 Outlook Web App 使用者現在有能力新增公用資料夾至 \[我的最愛\]，或將它們從 \[我的最愛\] 移除。在過去，此作業只能在 Outlook 中進行。
    
    如需詳細資訊，請參閱 [公用資料夾](public-folders-exchange-2013-help.md)。

  - **站台信箱**  電子郵件和文件傳統會保留在兩個獨立的資料存放庫中。通常，大部分團隊會使用這兩種媒介進行協同合作。挑戰是電子郵件和文件會使用不同的用戶端來存取，導致使用者生產力和使用者經驗降低。
    
    *站台信箱*在 Exchange 2013 中是一個全新的概念，我們嘗試以這個概念來解決這些問題。站台信箱透過使用相同的用戶端介面，允許存取 SharePoint 站台和 Outlook 2013 中的電子郵件文件，來改善協同合作與使用者生產力。站台信箱功能是由 SharePoint 站台成員資格 (擁有者和成員) 組成，透過 Exchange 信箱的電子郵件與 SharePoint 站台的文件共用儲存，並使用同一個管理介面來解決佈建和週期需求。
    
    如需詳細資訊，請參閱 [網站信箱](site-mailboxes-exchange-2013-help.md)。

  - **共用信箱**  在舊版的 Exchange 中，建立共用信箱是一個相當複雜的程序，您必須使用 Exchange 管理命令介面來設定代理人權限。在 Exchagne 2013 中，您現在可以透過 Exchange 系統管理中心執行一個步驟來建立共用信箱。在 EAC 中，移至 \[收件者\] \> **共用信箱** 以建立一個共用信箱。共用信箱現在是一個收件者類型，所以您可以透過使用者介面或命令介面輕易搜尋共用信箱。
    
    如需詳細資訊，請參閱 [共用信箱](shared-mailboxes-exchange-2013-help.md)。

## 與 SharePoint 和 Lync 整合

Exchange 2013 為 SharePoint 2013 與 Lync 2013 提供更強力的整合。此高效整合的好處包括：

  - Exchange 2013 與 SharePoint 2013 整合可允許使用者透過使用站台信箱更有效地進行協同合作。

  - Lync Server 2013 可以封存 Exchange 2013 中的內容並使用 Exchange 2013 作為連絡人存放區。

  - 探索管理程式可以跨 SharePoint 2013、Exchange 2013 和 Lync 2013 資料執行就地 eDiscovery 和保留搜尋。

  - Oauth 驗證允許夥伴應用程式在需要時當作服務或模擬使用者進行驗證。

如需詳細資訊，請參閱 [與 SharePoint 和 Lync 整合](integration-with-sharepoint-and-lync-exchange-2013-help.md)。

## 用戶端和行動裝置

Outlook Web App 使用者介面是專為平板電腦、智慧型手機，以及桌上和膝上型電腦設計的全新介面。新功能包括提供允許使用者和系統管理員使用的 Outlook 應用程式，延伸了 Outlook Web App 的功能；連絡人連結，讓使用者可以從他們的 LinkedIn 帳戶新增連絡人的功能；以及行事曆外觀和功能的更新。

如需詳細資訊，請參閱 [Exchange 2013 中 Outlook Web App 的新功能](what-s-new-for-outlook-web-app-in-exchange-2013-exchange-2013-help.md)。

## 整合通訊

基本上，在 Exchange 2013 中的整合通訊含有 Exchange 2010 中所含的語音信箱功能，不過，這些現存功能已增加某些新的或強化的功能在內。更重要的是，Exchange 2013 整合通訊中的架構變更，導致 Exchange 2010 中整合通訊伺服器角色的元件、服務和功能在 Exchange 2013 用戶端存取和信箱伺服器角色之間被分開。

如需詳細資訊，請參閱[什麼是整合通訊新 Exchange 2013](what-s-new-for-unified-messaging-in-exchange-2013-exchange-2013-help.md)。

## 批次信箱移動

Exchange 2013 引進了批次移動的概念。新的移動架構建立在 MRS (信箱複寫服務) 之上，可提供進階的管理功能。新的批次移動架構提供以下增強功能：

  - 可大批次移動多個信箱的功能。

  - 移動與報告期間所進行的電子郵件通知。

  - 自動重試並確定移動作業的優先次序。

  - 可一起移動主要和個人封存信箱，或分開移動。

  - 手動移動要求最終處理選項，允許您完成移動前先預覽移動結果。

  - 定期增量已同步處理將移轉所作變更。

如需詳細資訊，請參閱 [管理內部移動](manage-on-premises-moves-exchange-2013-help.md)。

## 高可用性和站台恢復

Exchange 2013 使用 DAG 和信箱資料庫副本，以及單一項目搜索、保留原則和遲延資料庫副本等其他功能，來提供可用性、站台恢復及 Exchange 原生資料保護。Exchange 資訊儲存庫與可延伸儲存引擎 (ESE) 等高可用性平台已全數加強功能以提供更佳可用性、更輕鬆的管理方法並且降低成本。這些增強功能包括：

  - **受管理的可用性**  有了受管理的可用性，內部監視和以復原為導向的功能可緊密整合，協助防止故障、主動復原服務，並自動初始化伺服器的容錯移轉或警告系統管理員採取行動。將重點放在監控並管理使用者體驗，而非僅著重於伺服器與元件存留時間，才可協助服務持續可用。

  - **受管理的儲存區**  受管理的儲存區是 Exchange 2013 中最近重寫之資訊儲存區處理程序的名稱。全新的 Managed Store 使用 C\# 編寫，且與 Microsoft Exchange 複寫服務 (MSExchangeRepl.exe) 緊密整合，以透過更強大的備援提供更高可用性。

  - **每一磁碟有多個資料庫的支援**  Exchange 2013 的增強功能可讓您在同一個磁碟上支援多個資料庫 (主動和被動副本混合)，因此可盡可能善用大型磁碟的容量和 IOPS。

  - **自動重新植入**  讓您在磁碟故障後，快速復原資料庫備援。如果磁碟故障，儲存在該磁碟上的資料庫副本會從主動資料庫副本被複製到備用磁碟的同一個伺服器上。若多個資料庫複本儲存於故障的磁碟上，可於備用磁碟上全部自動重新植入。這樣可啟用更快速的重新植入，因使用中的資料庫可能位於多個伺服器上，且資料為平行複製。

  - **自動從儲存故障復原**  此功能持續展現 Exchange 2010 中的創新技術，允許系統復原影響備援的故障。除了 Exchange 2010 檢查錯誤行為外，Exchange 2013 也包含了 I/O 時間、MSExchangeRepl.exe 耗用過多記憶體，以及系統因無法排程威脅而狀態不良之嚴重情況的額外復原行為。

  - **遲延副本增強**  遲延副本現在可以使用自動記錄播放來自行處理部份延期。遲延複本將自動降低記錄檔在各種情況下的重要性，例如單頁還原以及磁碟空間過低等情形。若系統偵測到頁面修補需要遲延複本，記錄將自動重新顯示遲延複本以執行頁面修補。遲延複本也將於達到磁碟空間過低臨界值、或者偵測到該遲延複本為特定時間內唯一可用的複本時，啟用自動重新顯示功能。此外，遲延複本可利用安全網讓復原或啟用更加容易。*網路安全性* 是 Exchange 2013 中的改善功能，以 Exchange 2010 的傳輸暫放為基礎。

  - **單一副本警示增強**  Exchange 2010 中所引進的單一副本警示已不再是另一個排程指令碼。現在，它已和系統中受管理可用性元件整合在一起，屬於 Exchange 內的原生功能之一。

  - **DAG 網路自動設定**  DAG 網路可以自動透過系統設定 (以組態設定為基礎)。除手動設定選項外，DAG 也可區分 MAPI 與複寫網路，並自動設定 DAG 網路。

如需這些功能的詳細資訊，請參閱＜[高可用性和站台恢復](high-availability-and-site-resilience-exchange-2013-help.md)＞和＜[變更至與舊版不同的高可用性與站台回復性](changes-to-high-availability-and-site-resilience-over-previous-versions-exchange-2013-help.md)＞。

## Exchange 工作負載管理

Exchange 工作量為 Exchange 伺服器功能、協定或明確定義為 Exchange 系統資源管理的服務。每一個 Exchange 工作負載會耗用到 CPU 、信箱資料庫操作等系統資源，或 Active Directory 要求執行使用者要求或執行背景工作。Exchange 工作負載範例包括 Outlook Web App、Exchange ActiveSync、信箱移轉和信箱助理員等。

在 Exchange 2013 中管理 Exchange 工作負載的方法有兩種：

  - **監視系統資源的健康狀況**  根據系統資源的健康狀況來管理工作負載是 Exchange 2013 中的新功能。

  - **控制個人使用者如何耗用資源**  控制個人使用者如何耗用資源在 Exchange 2010 (此版稱為使用者節流) 中是可行的，且此功能已為 Exchange 2013 擴充。

如需這些功能的相關資訊，請參閱 [Exchange 工作負載管理](exchange-workload-management-exchange-2013-help.md)。

