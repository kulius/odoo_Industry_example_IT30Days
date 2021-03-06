# Day 11 : 案例分享(3.4) 會計模組-分析會計與資產折舊

## 案例說明及適用場景
>- 會計科目與客戶，一般常用的蒐尋，若還需其他統計效果，可以使用分析帳戶或分析標籤
>   - 分析帳戶-可用於部門、專案的分析統計
>   - 分析標籤-用於傳票明細蒐尋及統計 
## 一.設定
>需開啓分析帳戶、分析標籤

![圖片](https://user-images.githubusercontent.com/1887931/134792433-3821447a-4f53-4fb9-b459-d1d8ef4969bb.png)

## 二.日記帳明細時選入
> 善用Odoo即有的蒐尋及分組

![圖片](https://user-images.githubusercontent.com/1887931/134797359-10c82795-c7e5-41c7-98f3-d008d4cb9fcc.png)
## 三.先行定義資產類型
>設定對應科目，折舊月數、折舊方法

![圖片](https://user-images.githubusercontent.com/1887931/134797432-6fed7a9c-0d16-4f27-9255-978ddea060f4.png)

## 四.每月資產折舊自動產生傳票
> - 於輸入日記帳分錄時，新增資產
> - 資產依資產類型自動產生每月折舊
> - 透過排程每月自動產生

![圖片](https://user-images.githubusercontent.com/1887931/134797526-ec6f19a9-c5bc-40d8-a447-0173023b5051.png)

## 總結
### 會計與庫存為Odoo二大主要的核心架構，所有ERP的形為最終都會形成傳票，所以多花一些時間說明，一方面是提高大家對Odoo的認知，一方面後續的文章針對會計的部份就不再多所說明

