# Day 2 : Odoo = 免費且完整的ERP + 完善的開發平台 + 第三方的免費Addon + 多人參與的商城

## 自我學習過程
>5年前透過學校老師的介紹，重新再次認識及了解Odoo，印象中那時 Open ERP 己更名為 Odoo 8，全Web的操作界面，深深吸引著我，更重要的是，袛要一行程式嗎，就可以達成M2O(多對1)，O2M(1對多)的效果，再無太多學習資源的狀況下，就決定投入，甚至到上海找顧問學習開發

## 免費且完整的ERP
- [Odoo 官方網站](https://www.odoo.com/zh_TW)
![image](https://user-images.githubusercontent.com/1887931/133721389-2d0da183-e65c-496b-8029-f9ab27069dea.png)

## 完善的開發平台
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