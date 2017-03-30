全棧工程師的百寶箱：圖形工具篇
===

在上一篇《[全棧工程師的百寶箱：黑魔法之文件篇](http://mp.weixin.qq.com/s?__biz=MjM5Mjg4NDMwMA==&mid=2652973386&idx=1&sn=c775725513879f52b1d40219b7d457a4#rd)》我們介紹了一些文件工具，今天讓我來分享一下，我常用的一些圖形工具，主要有兩類：

  - 流程圖
  - 資料視覺化

##流程圖：Graphviz

說到流程圖還是再次提及一下，我們之前說到的**Graphviz ** 。

> Graphviz （英文：Graph Visualization Software的縮寫）是一個由AT&T實驗室啟動的開源工具包，用於繪製DOT語言指令碼描述的圖形。它也提供了供其它軟體使用的庫。

它的主要特點是程式碼生成影象，並且足夠的簡單。

在我的那個“Web Developer 成長路線圖”(GitHub: [https://github.com/phodal/developer](https://github.com/phodal/developer))裡，就是用這個工具生成下面這個複雜的圖形。

![tree.png](tree.png)

而其程式碼特別簡單——和我們平時表達的手法是一樣的，即：

```
"包管理" -> "包釋出" -> "自動部署"
"CLI" -> "部署"
"指令碼語言(Bash,Perl,Ruby,Python etc)" -> "部署"
"指令碼語言(Bash,Perl,Ruby,Python etc)" -> "構建"
"*nix" -> "軟體編譯" -> "部署"
"構建" -> "軟體編譯"
```

 Graphviz有一個大的優點和弱點是：自動生成，導致畫線的時候很出現出問題。接著，我們就來看看手動畫線的例子。

##流程圖： Visio vs Dia vs OmnIGraffle

在Windows世界裡，在這一類的工具裡面最常見的算是Visio:

![MS-Visio-flowchart.png](MS-Visio-flowchart.png)

遺憾的是，它並不支援在Mac OS上使用。而且，它並不在我購買的Office 365套裝裡。

在Mac世界裡，最好的工具算是OmniGraffle，就是很貴——我們平時使用的是公司的Mac電腦，使用盜版軟體是有法律風險的。

![Omnigrafflescreen.jpg](Omnigrafflescreen.jpg)

在GNU/Linux世界裡，我們使用Dia。

> Dia 是開放原始碼的流程圖軟體，是GNU計劃的一部分，程式創立者是Alexander Larsson。Dia使用單一檔案介面模式，類似於GIMP與Inkscape。 Dia將多種需求以模組化來設計，如流程圖、網路圖、電路圖等。各模組之間的符號仍是可以通用的，並沒有限制。

![dia_screenshot.png](dia_screenshot.png)

順便安利一下，我最喜歡的作業系統OpenSuSE——簡潔、尾長、綠色。

![opensuse.jpg](opensuse.jpg)

OpenSuSE在KDE桌面下效果最讚了——因為KDE和OpenSuSE都是德國製造。總的來說，會比Debian系的Debian和Ubunt，及RetHat系的CentOS及Fedora穩定、漂亮。

令人遺憾的是這三個工具，我都用不了。Mac對X Windows的支援不是一般的差，於是我就需要別的替代工具。

##線上流程圖：Processon

這個工具還是相當好用，至少是在GxFxW內比較快——我之前使用過Creately、draw.io、Gliffy等等的一些工具，只是隨著版圖的擴充套件，很多地區都已經“xx”了。

![tlok.jpg](tlok.jpg)

不過遺憾的是：他們沒有給我廣告費。

> ProcessOn是一個線上協作繪圖平臺，為使用者提供最強大、易用的作圖工具！支援線上創作流程圖、BPMN、UML圖、UI介面原型設計、iOS介面原型設計等。

同樣的，在我的那個“Developer進階書單”（GitHub: [https://github.com/phodal/booktree](https://github.com/phodal/booktree))中，就是用這個工具畫出規規矩矩的線。

![BookTree.png](BookTree.png)

並且，它還是跨平臺的。

##各種圖： Word和Excel

由於翻譯和寫書的需要，我成了一個Office 365訂閱使用者。於是發現在Word等一系列的Office工具中，自帶了一個SmartArt的工具：

![smart-art.png](smart-art.png)

可以畫出很多很有意思的圖形，比如：

![程式設計之路.png](程式設計之路.png)

又或者是：

![growth-lob.png](growth-lob.png)

分分鐘就能畫一個的節奏。

##腦圖： XMind

我想這個一般人都是知道的。

> XMind思維導圖軟體被著名網際網路媒體Lifehacker評選為“最佳頭腦風暴和思維導圖工具”及”最受歡迎的思維導圖軟體”。

它有一個很大的優點是使用了全球最先進的Eclipse RCP 軟體架構，支援跨平臺使用。它有一個很大的缺點是使用了全球最先進的Eclipse RCP 軟體架構，導致了有點卡。

相比於流程圖什麼的，它只適合做腦圖。

![banner_index.png](banner_index.png)

如果你還在使用Eclipse，那麼你應該試試Intellij IDEA了。

##各種圖：D3.js

> D3.js（D3或Data-Driven Documents）是一個用動態圖形顯示資料的JavaScript庫，一個資料視覺化的工具。

與上面的工具相比，這個工具可能沒有那麼方便。但是，作為一個資料視覺化工具，它不僅僅可以做出各種炫酷的圖形：

![unemployment.png](unemployment.png)

還可以做出一個技能樹：

![sherlock.png](sherlock.png)

這個項目的GitHub見：[https://github.com/phodal/sherlock](https://github.com/phodal/sherlock)

##地圖：Leaflet

> Leaflet 是一個為建設移動裝置友好的互動地圖，而開發的現代的、開源的JavaScript 庫。

雖然它與上面的圖形沒有啥關係，但是它帶了一個圖字啊。與Google Map原生的API，或者OpenStreet相比，它最大的優點是對移動裝置支援好。

並且，它也是一個可以根據資料（GEOJSON，地理資料）生成圖形的工具。

![vmap.jpg](vmap.jpg)
