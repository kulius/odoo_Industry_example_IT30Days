# Day 3 : 案例分享(1.2) B2C經典流程 電子商務、POS + 進銷存 + 會計(應收付) +製造(產品組合、產品轉換)

## 二.電子商務->金流->後台對帳->銷單出貨
- 進入商城，加入購物車，並結帳
- 採客製過的綠界金物流
![day4_addcar](https://user-images.githubusercontent.com/1887931/133928046-3d5d1831-2899-4c30-a9a9-f6269c2ce214.gif)
- 以訂單的觀點來查看，該筆己支付，並且己產生收款的日記帳分錄，但還未出貨
![image](https://user-images.githubusercontent.com/1887931/133928406-92e6f5c6-716e-421e-b8fa-92920be89844.png)
![image](https://user-images.githubusercontent.com/1887931/133928428-9cb7f4ed-7a2e-46f9-8d5f-81e99da378f5.png)
- 進行出貨
  ![image](https://user-images.githubusercontent.com/1887931/133928526-29469272-fbc5-428b-b960-27acf2b82640.png)
- 創建應收，當傳票過帳後，會發現該筆己被支付
![image](https://user-images.githubusercontent.com/1887931/133928592-16e1aff7-d3b9-42fb-ad01-078e3f37a00e.png)

## 簡易系統功能說明
- Odoo 的資料是自動流轉的，當設定好後，除銷售訂單需要輸入，其他都是點選
- 電子商務、銷售、庫存、會計，各模組各自獨立，但Odoo本身提供很好的連接性，可以透過關聯的值，直點點選便可進入
- 就算沒有透過綠界的客製，也可以使用內建的Paypal，來進行測試支付，但前題是你要有domain
- odoo13版有一個自己創建應收的選項，但在14版改消了，改為強制型的銷帳模式

## 小結
### Odoo最大的優點也是最大的缺點，他每一版都在改變，隨時會加入他新的技術及新的系統流程觀點，你真的可以相信他一直在進步

