# Day 14 : 案例分享(4.3) 簽核與費用模組 - 簽核關卡及條件設定

## 案例說明及適用場景
>- 簽核與流程及人員組織架構為正相關
>- 一般簡易的判斷包含金額，商品類型，申請人或由申請部門，可能都有內部不同的思考
>- 例 A部門，要經過A財務，B部門要經過B財務

## 一.順序
>一筆設定決定一個關卡，每個關卡獨立判斷，可依順序決定

![圖片](https://user-images.githubusercontent.com/1887931/135187286-c9c553af-6b2c-4068-af05-4416f0b60e94.png)

## 二.通知及E-MAIL
>可於簽核開卡決定後，發送E-MAIL可預期會審批的人員

![圖片](https://user-images.githubusercontent.com/1887931/135187454-9592aa4d-5a87-480b-892c-6c9e312d6642.png)

## 三.填寫意見
>可決定是否在審核時一定要填寫意見

![圖片](https://user-images.githubusercontent.com/1887931/135187752-0b348202-a8e7-4b63-a789-71047a898a31.png)
![圖片](https://user-images.githubusercontent.com/1887931/135122253-31272faa-f97b-4403-85ac-0dac7d373b6d.png)

## 四.審批人設定
>- 可指定給個人
>- 可指定給群組
>- 可撰寫程式取得人員 例 部門主管
>- 依Odoo的模組特色來思考，此簽核模組並無強制一定要安裝人事模組，所以他提供了其他可能性

![圖片](https://user-images.githubusercontent.com/1887931/135188513-471baf6f-45ab-476a-be44-691132e95cf1.png)

## 五.何時趨動簽核
>透過定義類型，依該模組的特定欄位進行判斷

![圖片](https://user-images.githubusercontent.com/1887931/135188615-b03805eb-36e1-4842-a37f-b8d1129d28b0.png)

## 小結
### 設定上必需要有一定的Odoo資料結構的基礎，雖然沒有好用的UI來拖拉關卡來形成簽核，但相對的提供了更多可能性