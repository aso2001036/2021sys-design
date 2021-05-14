```uml
@startuml
顧客 -> webサイト: 注文
webサイト -> DB: 注文処理
DB -> DB: 購入処理
DB-> webサイト: 購入確定
webサイト -> 顧客: 購入確定
@enduml
```
