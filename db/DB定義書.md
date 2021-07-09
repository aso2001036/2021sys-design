# DB定義書
## ER図
[ER図はこちら]( https://github.com/aso2001036/2021sys-design/blob/main/ER.md "ER図はこちら" )

# DBテーブルカラム詳細一覧

***データベース***

d_purchase
|行名|型|not null|主キー|外部キー|
|----|--|--------|------|-----|
|order_id|bigint(20)|〇|〇||
|customer_code|varchar(50)|〇|||
|purchase_date|date|〇|||
|total_price|int(11)|〇|||

d_purchase_detail
|行名|型|not null|主キー|外部キー|
|----|--|--------|------|-----|
|detail_id|bigint(20)|〇|〇||
|order_id|bigint(20)|〇|〇||
|customer_code|varchar(50)|〇|||
|purchase_date|date|〇|||
|total_price|int(11)|〇|||

m_customers
|行名|型|not null|主キー|外部キー|
|----|--|--------|------|-----|
|costomer_code|varchar(50)|〇|〇||
|pass|varchar(50)|〇|〇||
|name|varchar(20)|〇|||
|address|varchar(20)|〇|||
|tel|varchar(100)|〇|||
|mail|varchar(20)|〇|||
|del_flag|int(1)||||
|reg_date|date|〇|||

m_category
|行名|型|not null|主キー|外部キー|
|----|--|--------|------|-----|
|category_id|int(11)|〇|〇||
|name|varchar(20)|〇|||
|reg_date|date|〇|||

m_items
|行名|型|not null|主キー|外部キー|
|----|--|--------|------|-----|
|item_id|int(11)|〇|〇||
|item_name|varchar(20)|〇|||
|price|int(11)|〇|||
|category_id|int(11)|〇|||
|image|varchar(200)|〇|||
|detail|int(11)|〇|||
|del_flag|varchar(500)|〇|||
|reg_date|int(11)|〇|||

