# Day 10 : 案例分享(3.3) 會計模組-調節、立沖帳、應收付與收支款 

## 案例說明及適用場景
- 當我們有某一個科目，需要管理他是否還有餘額未被處理，這個科目就是所謂的 調節科目，或是我們稱為的立沖帳科目
- 早期最常被運用的場景為，A客戶的2123-01 A客戶應收款項，於1/1 欠款 5000，2/1 欠款6000，3/1 還款7000，請問該客戶還有哪一天的應收款項多少錢
- 袛要是如同上述的場景，像預收付款項、應收付款項....等等等，都可以這樣運用
## 一.先於科目表，是否為調節科目
>需特定類型的科目才有 調節的選項

![圖片](https://user-images.githubusercontent.com/1887931/134765232-2cfd2539-e01e-4940-809f-d61dfd08d34a.png)

## 二.新增一筆傳票日記錄分錄，即可看到未調節資料
> 可以用對應的業務夥伴加以區分，並善用Odoo即有的蒐尋及群組功能

![圖片](https://user-images.githubusercontent.com/1887931/134765507-634b169d-ad19-47b7-a233-08c19a67c4be.png)
## 三.Odoo 調節界面，立沖帳處理
>- 可以使用點選的方式讓需調節的資料往上移動
>- 若有差額，系統顯示手動操作，看是否需關聯其他科目

![圖片](https://raw.githubusercontent.com/kulius/odoo_Industry_example_IT30Days/main/gif/day10-01.gif)

## 四.應收付與銀行之前的立沖帳
>可透過前一章節提到的發票輸入與銀行對帳單自動處理

![圖片](https://user-images.githubusercontent.com/1887931/134766140-11de2266-3541-47a5-a426-785665bcc255.png)

## 小結
### 立沖帳為會計管理的核心之一，透過系統自帶的調節功能，可更快速的掌握未沖資訊