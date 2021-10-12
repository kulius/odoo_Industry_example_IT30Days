# Day 25 : 案例分享(7.4) 庫存與製造 - 工單與工作中心

## 案例說明及適用場景
>- 當有工單的需求時
>- 每一個BOM表都有屬於自己的製程，而一個產品可以多個BOM表
>- 依製造訂單產生工單，用以追踨其工時

## 一.開啓工作中心
>- odoo14進行滿大幅度的改版，將原本的製造過程移除，將BOM直接與工作中心關聯 

![image](https://user-images.githubusercontent.com/1887931/136334853-b30eac7b-1118-4741-9d1b-595fb70db139.png)
## 二.設定BOM
>- 設定對應的製程及工作中心


![image](https://user-images.githubusercontent.com/1887931/136335515-9c9a7571-887e-4054-9d0e-e352e2174948.png)
## 三.製造訂單
>- 可依產品選擇不同的BOM表(製程)


![image](https://user-images.githubusercontent.com/1887931/136338070-1b3587fc-5dd1-47ea-ad3e-ee8adf2bde3a.png)
## 四.工單
>製造訂單開始後，產生對應的工單

![image](https://user-images.githubusercontent.com/1887931/136338602-8ce02262-267f-48af-9bd6-b30c7de774e4.png)
## 五.工單工作時數
>- 依工單填寫進行實數

![image](https://user-images.githubusercontent.com/1887931/136339084-1557c724-3a7f-4ff9-9242-ad9449174167.png)

## 小結
### 展開工單及進行時數記錄，可做為基礎的資料結構運用，配合IOT