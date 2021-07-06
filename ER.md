```puml
@startuml
entity "顧客マスタ" as customer <m_customers>
<<M,MASTER_MARK_COLOR>> {
+ customer_cord [PK]
--
pass
name
address
tel
mail
del_flag
reg_date
}
@enduml
```
