# Day 7 : 案例分享(2.2) B2B 客製寄倉處理

## 案例說明及適用場景
- 概念上是屬於暫收款的機制，但與特定商品綁定
- 寄倉通常都會搭配商品折扣，所以在退換貨的處理上也會較為特殊
- 一般的功能需求
  - 在報價單輸入商品，選寄倉時不出貨
  - 在報價單輸入商品，寄倉出貨時無帳款
  - 同種類商品換貨
  - 查看客戶寄倉數量
  - 查看客戶寄庫價格(換不同類型時商品時使用)
- 需要滿大量的客製，但還是專門寫一篇文章，主要是適用性滿高的，提供一些客製思維

## 一.於銷售明細，新增寄庫選項
- 選項內容包含
  - 寄庫
  - 寄庫出
  - 寄庫退
  - 寄庫退換
  
![image](https://user-images.githubusercontent.com/1887931/134340584-7310c41a-b9ae-4904-bf22-00642c297dec.png)

## 二.新增客戶寄倉總數量資料表(依銷售明細即時運算)，銷售明細即為寄倉歷程
> 減少資料刪除還需回覆的問題。直接與銷售明細關聯，資料保持一致

![image](https://user-images.githubusercontent.com/1887931/134341378-090c6b5f-810c-4735-8e45-ce87aa424bec.png)

## 三.簡易控制，寄庫不出貨，寄庫出沒帳款
> odoo 原生當報價單確認時，會自動產生出貨單，需控制，寄庫出也需控制不能產生帳款，這邊比較建議沖轉暫收款

![image](https://user-images.githubusercontent.com/1887931/134341879-71bc80cb-0d50-4e11-894a-953c7299ed7d.png)

## 四.寄庫換貨，以銷售明細直接定義
> 將寄庫商品與出貨商品分開，同時可以處理實際出貨的商品及想扣掉的寄倉商品

![image](https://user-images.githubusercontent.com/1887931/134342335-3afdd1b3-bae0-43c0-b106-2ad8cfe0770a.png)


## 簡易系統功能說明
- 主要想要表達如何搭配Odoo原生流程去客製系統，我相信袛要具備基礎的客製能力都可以達成

## 小結
### 銷售、客戶、庫存、會計(應收)，各自獨立，反而方便我們從中加以客製，Odoo原生的功能若有時間都可自己看原始碼加以理解
