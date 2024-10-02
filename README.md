Esatimates(Примерные показатели) <br>
Регион: Сахалинская область <br>
Численность населения: 500.000 человек. <br>
DAU: 15% от 500.000 = 75.000 человек. <br>
RPS: 75.000/24/3600 ~ 1 чел./сек. <br>


![schema](UseCase.png)

```plantuml

@startuml
left to right direction
actor "Оплатить" as toPay
actor "Клиент" as client
rectangle Автомойка {
  usecase "UC1: Управление профилем" as UC1
  usecase "UC2: Управлять своим авто" as UC2
  usecase "UC3: Выбрать город" as UC3
  usecase "UC4: Выбрать мойку" as UC4
  usecase "UC5: Выбрать дату и время" as UC5
  usecase "UC6: Выбрать услугу" as UC6
  usecase "UC7: Выбрать способ оплаты" as UC7
  usecase "UC8: Оплачивать услуги" as UC8
  usecase "UC9: Отмена услуги" as UC9

}
client --> UC1
client --> UC2
client --> UC3
client --> UC4
client --> UC5
client --> UC6
client --> UC7
client --> UC8
client --> UC9
UC7 --> toPay


@enduml

```

UC1

я как дмитрий сузуки автозвук хочу услуги мойки с бассами чтобы мой слух прозрел. <br>
я как клиент-геймер хочу компьютерный клуб чтобы с кайфом играть в ксочку пока моится тачка. <br>
 
