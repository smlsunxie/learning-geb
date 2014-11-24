實作分工
========

定義好規格，確認沒問題後，就可以根據規格開始進行實作。

在單兵作業的開發情形下，一般情況來說，我們需要先把前端 UI 準備好，有了 input 資料後，才可以開始進行後端的實作，但再多人開發的情形下，最理想的狀況下應該是要同時進行，才能最有效利用產能，最基本的分工如下：

-	前端：負責 UI 的呈現，一般來說規格的 input 是由前端提供。
-	後端：負責接收 input 後，實作商業邏輯，經過處理後，產出 output 讓前端接收以便後續 UI 呈現。
-	整合：一旦前後端開發完畢即可實際運行進行整合，此時前端人員可以將測試資料轉為正式向後端的接口進行 request，確保整個功能運作正常。

因為有可運行的規格作為後盾，讓前後端人員幾乎可以同步進行，讀者可能會有疑問，都還沒開始怎麼同步進行，是從前端開始還是後端？

在「測試資料與資料庫」有提到，在運行規格前可以先行建立測試資料，前後端開發也是同樣的道理，在尚未開始前後端整合前，可以根據規格模擬預期的資料，若是前端可以模擬要送往後端的資料，並且模擬後端產出的資料進行畫面呈現；後端的話因為已經有定義好的規格，只要直接運行規格並且實作，直到輸入資料處理後與規格相同，最後再進行整合，完成整個功能串接。