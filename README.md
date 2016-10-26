# OOAD-WEEK10
Sequence Diagram

## ส่งงาน OOAD-WEEK10 Sequence Diagram

ภาพที่ 1 สั่งอาหาร
```
@startuml
skinparam sequenceArrowThickness 2
skinparam roundcorner 20
skinparam maxmessagesize 60
skinparam sequenceParticipant underline

actor customers
participant "First Class" as A
participant "Second Class" as B
participant "Last Class" as C

customers -> A: do menu
activate A

A -> B: order
activate B

B -> C: make food
activate C
C --> customers: food
destroy C

@enduml
```
![](http://www.plantuml.com/plantuml/img/RP31JiCm38RlVWfhzqdJ3XnwcDP6uiG12Lx0IWn4RUBEJXZmzAH2sbg9y_Vx_soVhP2McYQmCUQPb18QNofdpxsgN5y_eXypc-5n5L6fENZHp8h7mmea-aejJEziyOVnuV1FxtCpHXzdoWLR3UiKCmEGBwBegnL9h0RpAhPxZ6e5tKHcEoJ3VejVs4iEApvi-HDjfXt0pOFx4_OT1i74kIvRn4ygt0pGBspeKBGjUIS3mB0GrxLpHyOtaN2d3Xpk6xq9khz0O2igtuiRuCmvjAV_0W00)


ภาพที่ 2 ATM
```
@startuml
skinparam sequenceArrowThickness 2
skinparam roundcorner 20
skinparam maxmessagesize 60
skinparam sequenceParticipant underline
actor me
participant "step 1" as A
participant "step 2" as B
participant "step 3" as C
me -> A: Skewer card
activate A
A -> B: pass word
activate B
B -> C: press money
activate C
C --> B: processor
destroy C
B --> A: receive money
deactivate B
A --> me: keep gard
deactivate A
@enduml
```

![](http://www.plantuml.com/plantuml/img/RP51QiCm44NtSueX-q3gGXTUbDY-GA6zW90_gN0aEICvRdhwZaoWMdZztip_6frJDf8NVwKqkJ0RCPuJRWk2HISIrwzlPwU0bBYf58bB66sK0E7cL05lVhpAveBaVi5lfvsz7vheh9jDoAnh85SNG6HiZi8UD5Vya39cVZcmITpja6OZ_GvvtSX0H1vyVEUkvSy9gnQsHiQIvkucGxTILtZVycpqcMkiQK_K5peebN857mCU_toWWO_FQObMZIWq8cM9ZnBURrIp1HRkZkUyAdL4jraUBK_GwfTIi3AquXbXr5_w0m00)


ภาพที่ 3 สอบถามยอดเงินมือถือ

```
@startuml
participant me
me -> step1: press number
activate step1 #FFBBBB
step1 -> step1:  call
activate step1 #DarkSalmon
step1 -> step2: << Ask balance >>
activate step2
step2 --> step1: Listen balance
deactivate step2
deactivate step1
step1 -> me: place the phone
deactivate step1
@enduml
```

![](http://www.plantuml.com/plantuml/img/PP3F2eCm3CRlUOh0pXxqA29k34-xxGbY3LXiOsdZddy56MMQI_vzFpwI8Ib5tRs3aBCrDf0eUWRmZ5MFIJdKBOR8AQ7iVk88PDH-IFbOucqS7pa0ZhP0QCYvY_f9SNsJyvkSYAR5hiDxMd4YHs8O-_wVRWwYmQgOl6mkv8V0p2VYDAYBf-TybwFiemjZM3RXgne6bZc_vmi0)



ภาพที่ 4 จองโรงแรม
```
@startuml

me -> employee: hello
employee --> me: welcome to hotel
|||
me -> employee: Reservations hotel
employee --> me: okay  when
|||
me -> employee: next week
employee --> me: ok how many rooms
|||
me -> employee: two rooms
employee --> me: ok

@enduml

```

![](http://www.plantuml.com/plantuml/img/RO_H3S8m34J_FOKNw09yeCx01X6S55GxHeaXHChm1AdzQZxFT_TENek7x6yL8WKlLuQ-n1fmuGWHeqFpCamTvmgvsyYwSJI7KE_zrBsX87-2FosLFNO2sHOQSur8KqJ2rySOjbbpC2jhI8spcPOfmAljxWH0j28z_d__0000)


```

ภาพที่ 5 ตู้กดน้ำ

@startuml

hide footbox
title dispenser waters

me -> dispenser: put coin
me -> dispenser: press waters
dispenser --> me: receive waters 
@enduml

```

![](http://www.plantuml.com/plantuml/img/ROwn3O0m30HxJ-45M205OXKWZx144cGxmFYa0D7G_j-zVZ0VrMlQY5Q9uAKKdyf5Bhw1ezYER50-HuSQKG9t_PS7tglpN2J_D0gpL_oMkaOb15RCa0CFm3GWn_RZ1W00)






























README.md 
md เป็นภาษา Markdown นิยมใช้ใน wiki ของ github 

ตัวอย่างโค้ด
```
# Heading ระดับ 1 
## Heading ระดับ 2
### Heading ระดับ 3
 
```

ผลที่ได้
# Heading ระดับ 1 
## Heading ระดับ 2
### Heading ระดับ 3


## Code ภาษาซี

ตัวอย่างโค้ด
<pre>
  ``` c
  #include <stdio.h>
  Main()
  {
     Printf("Hello");
  }
  ```
</pre> 
ผลที่ได้
  ``` c
  #include <stdio.h>
  Main()
  {
     Printf("Hello");
  }
  ```
 
