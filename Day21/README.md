# Day 21 : 案例分享(6.4) 人事、差勤與薪資 - 薪資計算

## 案例說明及適用場景
>- odoo原生並無薪資計算，但有免費的第三方可供修改參考 或是直接使用 台灣的付費版本
>- 架構上個人覺得還不錯，所以獨立一篇文章給大家參考
>- 可依照不同的職務定義薪資結構，不同的項目可以定義計算的方式，接下來每月固定產出

## 一.參考及可購買模組
>- [Odoo 14 HR Payroll](https://apps.odoo.com/apps/modules/14.0/om_hr_payroll/)
>- [元植-人力資源模組班](https://www.yuanchih-consult.com/blog/odoo-1/post/odoo-144)

![image](https://user-images.githubusercontent.com/1887931/135981750-3b57aa87-ed35-4fcc-8bf2-b4eb89c5253e.png)
## 二.定義職務薪資結構
>- 可定義薪資結構及計算內容
>- 企業的薪資都有其複雜的地方，我們需要不同的項次來做為客製的計算

![image](https://user-images.githubusercontent.com/1887931/135982082-763cd548-718b-43e7-aa61-2dc70f36dc33.png)
## 三.依不同項次，設定計算方式
>- 簡單的計算，可以直接設定欄位加減
>- 複雜的計算，可以透過呼叫Function

![image](https://user-images.githubusercontent.com/1887931/135982350-6a2b61d2-1c59-4d9c-b458-e61929bd1526.png)
## 四.勞健保
>台灣的勞健保，可先設定在員工及合同資訊

![image](https://user-images.githubusercontent.com/1887931/135982576-6ba1deda-c716-4d8a-865a-282b6acd05a6.png)
![image](https://user-images.githubusercontent.com/1887931/135982762-b8341550-791c-4376-9d6d-a53bdb155bcf.png)
## 五.每月產生薪資
>- 排程或批次產生當月薪資
>- 定義當月其他輸入項
>- 轉入會計傳票及付款

![image](https://user-images.githubusercontent.com/1887931/135983045-b7947ca4-a7d4-41ed-b7d4-2bef83bb78f1.png)

![image](https://user-images.githubusercontent.com/1887931/135983289-0e034e1a-29c6-4b91-8ee6-dc3679ca1f30.png)

## 小結
### 提供一些思路，供大家若有機會使用odoo時的薪資解決方案