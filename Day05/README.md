# Day 5 : 案例分享(1.3) B2C經典流程 電子商務、POS + 進銷存 + 會計(應收付) +製造(產品組合、產品轉換)

## 三.製造(產品組合)->POS->日結結帳、扣庫存
- 於製造設定物料清單 (A = B + C)，
>概念上就是賣A，但是扣B 和C 的庫存，記得選套件

![image](https://user-images.githubusercontent.com/1887931/134003298-a37581c4-6487-4af3-95d8-8ff21537e4da.png)
  
- POS 銷售
  >不太推使用Odoo的POS，主要是不太好客製，功能也離台灣習慣用的POS有點落差，主要還有電子發票的客製有點麻煩，有能力串接的話，把每日的帳和庫存轉進Odoo即可

![image](https://user-images.githubusercontent.com/1887931/134003950-f7e06ce9-225b-4c1e-9f40-fbad7003ebcd.png)
- 日結結帳
>進行關帳後，才會產生對的的扣庫存及傳票日記帳

![image](https://user-images.githubusercontent.com/1887931/134004560-2a328909-4885-4d04-8826-af749a11ad24.png)
- 查看庫存調撥的資訊
>依我們所設定的物料清單(BOM)扣庫存

![image](https://user-images.githubusercontent.com/1887931/134004758-e24f6531-ef9f-4ded-aa19-271d0950ebc4.png)

## 簡易系統功能說明
- Odoo POS 的資料相對來說是獨立的，透過結帳才有傳票日記帳及扣庫存的行為，但有參數可以設定即時扣帳
- 製造模組 我常用在產品組合及委外加工的部份，這部份後續案例會提到，小企業或簡單的買賣業都可以使用


## 小結
### Odoo的特色之一在於清楚歸屬功能應歸屬的模組，該庫存就庫存，銷售就銷售，會計就會計，所以較不會出現重覆的邏輯

