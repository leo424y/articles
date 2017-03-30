最流行的程式語言JavaScript能做什麼？
===

首先很遺憾的一點是，“PHP雖然是最好的語言”，但是它不是最流行的語言。

![Sad](sad.jpg)

對不起的還有剛剛在4月TIOBE程式語言排行榜上榜的各個語言：

![Tiobe四月](tiobe.png)

你們都很棒，但是你們都擔當不了這個大任。

開始之前，我先說一下我常用的三個語言：Java、JavaScript、Python。

 - Java，讓我學到了很多架構層級的知識，這一點可以參考我之前寫的架構相關文件。雖然我一點兒也不喜歡這個語言，但是它真的很棒。
 - Python，它真的足夠簡單，以至於我喜歡拿它學習各種理論知識，如推薦系統、貝葉斯定理、自然語言處理等等。
 - JavaScript，看下文。

資料視覺化
---

在過去我閱讀的一些書籍裡面，主要是以Processing作為視覺化的語言——它起始於2001年，它最初是面向美術工作者和設計者建立的，後來變成了全面的設計和原型工具，可以用於建立複雜資料視覺化領域。

![Processing](processing.png)

Processing被帶入了到Web領域產生了Processing.js，還出現了D3.js。

![D3.js](d3js.jpg)

當然還有Plotly、Leaflet、Sigma JS等等的工具。

移動端應用： Cordova
---

接著就是PhoneGap（今天的Cordova），將WebView帶向了移動應用，也將JavaScript帶向了移動應用。

![Cordova](cordova.png)

使用Cordova，可以讓我們**一次開發多平臺釋出**。我們也順便提一下Ionic，作為混合應用的翹楚：

![Ionic](ionic.jpg)

移動端應用： React Native
---

既然我們已經提到了Cordova，那麼我們也應該說說**React Native**。也是一次開發多次執行：

![React Native](react-native.png)

雖然它的坑還有很多，但是還是值得期待的。

服務端：Node.js
---

正是V8的效能將JavaScript帶到了一個新的高度，於是Node.js誕生了——前端、後臺都可以用JavaScript，一個JavaScript的全棧時代。

![Nodejs](nodejs.png)

Mongodb作為資料庫，Express作為Server端MVC，他們可以提供一個RESTful服務，那麼再加上MVVM框架的Angular.js，你就知道我在說什麼!

![mean.png](mean.png)

桌面應用： NW.js 和 Electron
---

NW.js 是基於 Chromium 和 Node.js 執行的， 它們可以讓我們用HTML和JavaScript來製作桌面應用。除了NW.js還有最近比較火的Electron，Atom編輯器的

![Electron](electron.png)

與Cordova的多平臺構建多版本不同的是，Electron可以在一個平臺上構建多個平臺的應用。即我們可以在Mac OS上打包出Linux和Windows上的應用，而不需要在Windows再編譯一次。

帶向了桌面端，讓桌面和Web保持了一致。最成功的案例就是估值達30億美元的Slack：

![Slack](slack.jpg)

So，如果你使用桌面端的Slack就會很卡~~。

全平臺應用
---

還記得我寫的那篇《[一份程式碼構建移動、桌面、Web全平臺應用](https://www.phodal.com/blog/build-full-platform-application/)》，在Eletcron上執行Ionic，就意味著無限的可能性。

![一份程式碼構建移動、桌面、Web全平臺應用](growth-full-platforms.jpg)

能用Web開發的事情就用Web來完成就好了。

遊戲
---

自從WebGL被帶入瀏覽器的那一刻，就決定了這又是一個新的天地。

![HTML5 遊戲](html5-games.jpg)

讓我們忘記編譯、啟動更新、外掛等等的問題，並且我們還可以一次開發直接執行。

VR
---

如果你看到過之前的那篇《[JavaScript在VR世界的應用](https://www.phodal.com/blog/why-javascript-will-use-vr-world/)》，那麼你就會對這個內容有更多的印象。

主要思想還是通過WebView來渲染VR視角：

![Three.js Oculus](threejs-oculus.jpeg)

並且各瀏覽器產商各在推進WebVR 為虛擬現實裝置顯示提供支援。

AR
---

雖然大部分的AR應用可能離我們有點遠，但是離我們最近的就是Leap Motion——它可以利用手掌和手指動作來進行輸入，但無需手部接觸或者觸控。

![Leap Motion](ar.jpg)

同理於VR，讀取感測器的資料，再將其手勢交由瀏覽器端來處理。詳細可以參考我之前寫的：《[Leap Motion JavaScript開發 手勢控制基礎篇](https://www.phodal.com/blog/leap-motion-gestures-example/)》

硬體
---

早先我看到了Arduino在編譯的時候，以DSL的方式封裝了API。而NodeMCU則內建了Lua語言的支援，可以讓開始者使用Lua來開始。 而Tessel 原生就提供了JavaScript執行環境，我們寫需要寫好JavaScript就可以在上面執行。

![Tessel 2](tessel2.jpg)

Tessel 2屬於配置比較高的硬體，而低配的呢？

三星設計了JerryScript引擎，它能夠執行在小於64KB記憶體上，且全部程式碼能夠儲存在不足200KB的只讀儲存（ROM）上。

![IoT.js](iotjs.png)

想想就覺得未來是美好的。

物聯網
---

等等，上面三星推出的是IoT.js，這就意味著它已經可以在物聯網領域中應用了，為什麼還會有這裡的應用呢？我只是想稍微提一下這個：

![IoT Node.js](iot-nodejs.jpg)

上面說到的只是Node.js在Web中的應用，而物聯網和Web的很大不同之處在於，物聯網可以使用各種不同的協議，而這些協議都需要Node.js對其的支援。

因此，如果我們需要開始Web版、移動應用，那麼我們自然更需要其作為後臺。

作業系統介面
---

雖然更好的機器帶來了更好的效能，但是顯然人們對於原生應用的需求並沒有那麼強烈。Firefox OS已經在移動作業系統敗下陣來，但是這個操作被帶到了物聯網領域：

![Firefox OS](firefox-os.jpg)

這就意味著，我們可以使用JavaScript來開發作業系統的介面了。


你覺得JavaScript還能做什麼？
