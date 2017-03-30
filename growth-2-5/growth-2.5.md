程式設計學習應用 Growth 2.5 釋出: 讓我們點亮全棧工程師的技能樹
===

> 2015年底，我建立 Growth 了應用，它向初學者們提供了一個學習路線。兩年來，已經有超過 3 萬個使用者使用過。本週裡，我們釋出了 2.5.0 版本，現在你可以點亮技能樹了~~。

在我建立 Growth 的時候，我沒有意識到它會如此地受歡迎~~（PS：我就是喜歡自誇）。


Overview
---

在 Growth 1.0 裡，我們向 APP 中新增了 Google Analytics，它可以分析出使用者的使用情況。如下圖所示：

![Growth 每週流量](growth-weekly.png)

在上一週裡，平均每天有三百多個使用者，這一週 2096 個使用者使用了 Growth。同時，瀏覽量表明 Growth 2.x 比 1.x 更受大家喜歡，但是還是遠遠不夠。

從開始使用 GA 的時間裡，累計有 36114 個使用者使用了 Growth，並且主要都是中國人——說了都於沒說。

![Growth 歷史資料](growth-overview.png)

其中，有大約 17,486 個 iOS 使用者：

![Growth iOS](growth-itunes.png)

而 Google Play 也統計到了 10,978 個使用者：

![Google play Growth Use](google-play.png)

這個資料表明，程式設計師中的大部分人都是使用  Google Play 的。儘管 Play 的 Android 使用者比 iOS 少了 70%，但是我們收到了156 個評分，遠遠高於 APP Store 的兩倍：

![iOS 評分與評論](ios-review.png)

到底是 Play 使用者的素質高，還是 iOS 的使用者比較懶？


Growth 2.5.0
---

在 Growth 2.5.0 裡，我們做了一些事情：

1. 出於安全及 App Strore 限制，我們使用 HTTPS 來替換全部的 API——這個運維工作量很大（由 Phodal 完成）
2. Ionic 2 在上個月推出了正式版，所以我們修改了大量的 beta.5 程式碼來適配這個版本（由 Phodal 完成）
3. 新增了技能樹功能。未來使用者，將可以從技能樹獲取到更多的知識（由 Phodal 完成）。

去年 8 月份的時候，我們使用了 Angular 2 Beta 和 Ionic 2 Beta 編寫了 Growth 2。無奈的是，Angular beta.5 的坑太多了，在 Growth 2.5 的時候，近乎重寫了整個應用。這就是為什麼，Growth 在很長一段時間都沒有更新的原因。

關於 Growth 技能樹
---

最初我推出 **Growth 技能樹**的收費版本目的是，**為了眾籌點錢來支付 Apple Developer**的 688 元開發者賬號。

我們花費了大量的時間，來維護這個開源應用。我們已經在 GitHub 上擁有 2043 次提交，這意味著每週期我們要提交 20 次程式碼。我們將花費了大量的時間，將這個應用從 Angular 1.x 遷移到了 Angular 2.x，從 Ionic 1.x 遷移到了 Angular 2.x。當然，這些都是應該的。

![Growth GitHub](growth-github.png)

除此，我還需要支付 Growth 論壇 [http://forum.growth.ren/](http://forum.growth.ren/) 的伺服器費用。

因此，我們推出了 Motree 項目，大致如下圖所示：

![Motree](growth-motree.png)

每個 Android 使用者都可以獲取到 Motree 的免費版，而 iOS 使用者則是經**更多優化**的收費版——為了 Apple Developer。

由於 Motree 本身是免費的，所以這個功能也遷移到了 Growth 2.5.0 中。

**我們也將在未來幾個月裡，提供更專業的 Motree 付費版，同時也會上架 Play 收費~~。**

嗯，就這樣，讓我們和上萬個使用者一起更新 Growth 2.5 吧~~。
