# Day 6 : 案例分享(2) B2B 網頁下單+後台月結+前台付款

## 案例說明及適用場景
- 也算是買賣業，但對象不是一般客戶，而是廠商
- 面對廠商，一般來說都會有寄倉、月結收款及收款時折扣問題，或下單時的折扣
- 可以選擇接電話下單，也可以讓廠商直接網頁下訂
- 當然收款時可以現金匯款收錢，也可以利用線上付款
- 類似像團購主網頁下單、廠商後台出貨、每月帳結收款

## 一.新增支付方式，每月付款
>用於電商購物車時，不用立即付款

![image](https://user-images.githubusercontent.com/1887931/134142616-71f24807-e219-42bb-a5de-fad6d2dac6ae.png)

## 二.帳款月結 (第一種選擇)
> 第一種 : odoo的正式流程，每筆訂單，出貨完成後，就形成應收，每筆應收都有其收款時間，時間到了後，再整批付款，付款金額若與應收不一致，可做調整分錄

- 依客戶分組，查看帳款的到期時間，再依狀態做篩選，可以先狀查詢結果匯出 客戶對帳單給客戶確認
![image](https://user-images.githubusercontent.com/1887931/134144210-12fa9862-928b-4530-9109-583e99b39c91.png)
- 勾選應付款的資料後，整批付款，選群體付款
  ![image](https://user-images.githubusercontent.com/1887931/134144601-b3aead46-8347-4160-8395-8feaaacd2567.png)

## 二.帳款月結 (第二種選擇)
> 第二種 : 以訂單為主，查看是否到期(需客製)或簡單的依訂單日期或出貨日期來做篩選或群組，一樣可下載 EXCEL，可客戶確認，無問題後，合併產生應收憑單 (缺點是沒有出貨時就產生應收)

![image](https://user-images.githubusercontent.com/1887931/134145292-2ce1460b-2030-411c-8aff-3e7cb3fcaef9.png)

- 選擇憑單線上付款
![image](https://user-images.githubusercontent.com/1887931/134145799-a24be369-ed15-46a0-af34-98203a143096.png)

- 廠商就可以於，我的帳戶中的應收憑單，做出線上支付
![image](https://user-images.githubusercontent.com/1887931/134146022-573ce415-15e9-4004-b427-ff99eddce652.png)
![image](https://user-images.githubusercontent.com/1887931/134146720-b2ebb8df-3044-489c-beb2-4ae40bce56ee.png)

## 簡易系統功能說明
- Odoo系統內大部份都有合併資料的功能，包含合併出貨，合併帳款、合併付款，可以思考後加以運用
- 所有可見的資料都可以分組篩選及匯出，所以Odoo內附的統計報表幾乎等於沒有，但他強大的篩選及分析表，也袛有在一些BI工具上才看的見
![image](https://user-images.githubusercontent.com/1887931/134147494-8f26c327-b343-4b02-8427-01dca88900f2.png)


## 小結
### 所有的資料，所有的欄位 都可篩選及匯入、匯出，資料是屬於企業所擁有的，而不是被系統所挷架
![image](https://user-images.githubusercontent.com/1887931/134147742-f806b2e5-f67e-4de8-a565-b12379fc2cc8.png)

