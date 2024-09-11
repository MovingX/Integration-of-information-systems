```mermaid

@startuml
left to right direction
actor "Оплатить" as toPay
actor "Клиент" as client
rectangle Автомойка {
  usecase "Управление профилем" as UC1
  usecase "Управлять своим авто" as UC2
  usecase "Выбрать город" as UC3
  usecase "Выбрать мойку" as UC4
  usecase "Выбрать дату и время" as UC5
  usecase "Выбрать услугу" as UC6
  usecase "Выбрать способ оплаты" as UC6
  usecase "Оплачивать услуги" as UC7
  usecase "Отмена услуги" as UC8

}
client --> UC1
client --> UC2
client --> UC3
client --> UC4
client --> UC5
client --> UC6
client --> UC7
client --> UC8
UC7 --> toPay

@enduml

```
