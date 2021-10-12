# Day 22 : 案例分享(7.1) 庫存與製造 - 庫存移動(調撥)流程

## 案例說明及適用場景
>- 庫存是odoo中很特別的功能或流程
>- 單純以功能的思考核心有二個，複式庫存及推拉規則
>- 我們都希望庫存的移動是需要管理的，但事務的管理與真實移動管理，是很繁雜的事情
>- 事務的管理上，我們會希望有一張單據的產生，例出貨單、入庫單、品檢單、報廢單、維修單、領料單.....
>- 物品真實移動的管理，會希望有出及入的確認，出去的東西要有人簽名、進來的東西也要有人確認
>- 但小公司的倉庫可能是採購在管理，大公司的倉庫管理更是一門大學問
>- ERP的庫存如何與現場真實庫存理順，思考的關鍵

## 一.複式庫存
>- 若我們希望留下庫存移動的過程，並快速的統計數字，過往的系統經驗有一個案例是最標準的，那就是會計系統
>- 會計原則告訴我們，有借必有貸，借貸必相等
>- odoo庫存原則為，有出必有進，出進必相等
>- [官方說明文檔及影音](https://www.odoo.com/documentation/14.0/zh_CN/applications/inventory_and_mrp/inventory.html)

![image](https://user-images.githubusercontent.com/1887931/136120307-a5f47f5e-55d7-4788-a448-d0063290d7f9.png)
![image](https://user-images.githubusercontent.com/1887931/136119857-f555626c-a8aa-4f39-995d-1e51b01a318b.png)

## 二.真實庫位與虛擬庫位
>- 為達到複式庫存的需求，例客戶倉、供應商倉、盤盈倉...

![image](https://user-images.githubusercontent.com/1887931/136119961-1f1ccc9f-9498-4d8c-842c-b5190ea7707d.png)
## 三.作業類型
>- 可隨意新增 操作名稱，例:出貨單、公關調撥，維修報廢..
>- 當您了解到，有出必有進，出進必相等，所有單據的名稱己不是重點
>- 區分四種類型，收貨、交貨、內部調撥、製造，有功能行為的管控

![image](https://user-images.githubusercontent.com/1887931/136120043-32e4857a-c0b5-4caa-b6c7-f111db5203ed.png)

## 四.儀表板
>可針對作業類型進行操作

![image](https://user-images.githubusercontent.com/1887931/136120080-fd21fdbc-8b8a-47a6-a82c-39523336223d.png)

## 五.調撥單
>- 每個庫存操作都可視為 調撥
>- 單據狀態為 草稿、等待、準備好、完成

![image](https://user-images.githubusercontent.com/1887931/136120136-1ed29766-6737-4d82-ae06-6f82364975b6.png)

## 五.查看移動歷程或結果
>- 如同會計帳一樣，可以看總分類帳、明細帳、至哪天為止的科目餘額

![image](https://user-images.githubusercontent.com/1887931/136120225-10e21a85-3baa-42cc-9019-fe706f2f6589.png)

## 小結
### 若以會計觀念來思考odoo複式庫存，會很快進入狀況