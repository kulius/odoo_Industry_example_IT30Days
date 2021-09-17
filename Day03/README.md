# Day 3 : 案例分享(一) B2C經典流程 電子商務、POS + 進銷存 + 會計(應收付) +製造(產品組合)

## 案例分享
會想來使用Odoo的公司，通常是在市面上現有ERP系統找不到解決方案的公司，歸納一下
- 新創事業，無法花太多錢 (這是大多數人的前提)
- 想走電子商務，在蝦皮、MOMO、PCHOME有基礎，但想自架官網
- 想要有一個進銷存，管管庫存，管管帳，而不是每日統計 蝦皮、MOMO、PCHOME 的EXCEL
- 有現有店面，也有電商，想來個會員積點，想線上線下一條龍服務
- 有採購，有簡單的委外加工，沒有大型庫房，想管控進出貨
- 公司有會計系統、有POS系統，還要在電商操作系統，到處是系統，但袛有一個人
>當您有個小買賣，有店面，有電商，有庫存，有CRM，有會計，有製造，是基本需求，為何市面上沒有整合的解決方案，或是那個解決方案，根本就不是小買賣能負擔的

## 電子商務->線上付款串金流->確認收款->庫存出貨串物流
- [Odoo 官方網站](https://www.odoo.com/zh_TW)
![image](https://user-images.githubusercontent.com/1887931/133721389-2d0da183-e65c-496b-8029-f9ab27069dea.png)

## 現場販售POS->電子發票->日結過帳->扣庫存
- M2O(多對1)
```
//資料庫ORM語法
    user_id = fields.Many2one(
        'res.users', string='Salesperson', index=True, tracking=2, default=lambda self: self.env.user,
        domain=lambda self: [('groups_id', 'in', self.env.ref('sales_team.group_sale_salesman').id)])

//View呈現XML語法
    <field name="user_id"/>

```
![image](https://github.com/kulius/odoo_Industry_example_IT30Days/blob/main/gif/day2_m2o.gif?raw=true)
- O2M(1對多)
```
//資料庫ORM語法
    order_line = fields.One2many('sale.order.line', 'order_id', string='Order Lines', states={'cancel': [('readonly', True)], 'done': [('readonly', True)]}, copy=True, auto_join=True)

//View呈現XML語法
    <field name="order_line"/>

```
![image](https://github.com/kulius/odoo_Industry_example_IT30Days/blob/main/gif/day2_o2m.gif?raw=true)

## 第三方的免費Addon
- OCA odoo 開源組織 [The Odoo Community Association Website (OCA)](https://odoo-community.org/)
- OCA 提供的開源 addon [Oca - Odoo Community Association · GitHub](https://github.com/OCA)
- Odoo Apps Store [免費 addon](https://apps.odoo.com/apps?price=Free)

## 多人參與的商城
商城所販售的addon，都是原始碼，下載後，都可直接修改，odoo 8 時，大部份都是免費的addon，到現在，大多數都是付費addon，我反而覺得很好，因為有持續性的收入，才能讓社群、商城往更好的發展
- 官方商城 [Odoo Apps Store](https://apps.odoo.com/apps)
![image](https://user-images.githubusercontent.com/1887931/133722092-1d65d7c8-4f5b-4e8d-a5e4-d6aac3877ddc.png)

## 學習資源
- [odoo 官方文件](https://www.odoo.com/documentation/14.0/)
- [元植管理顧問 odoo中文化的主要作者](https://www.yuanchih-consult.com/)