# OOAD-WEEK11
State Diagram

ภาพที่1 การชำระเงิน

 ```
@startuml
title payment
[*] -r-> notpayyet : Create Billing
notpayyet -r-> paid : Pay bill
paid--> [*] : Breaking billing

@enduml
 ```

![](http://www.plantuml.com/plantuml/img/HOqn2e0m34Ntd2Apq0jq4D4Bk8j3n231jagDGszlsiKn_x_tCpnAMTyOG4K3uqqbSb9OkXLTTZscIoqhhEXnoapAE4e8aWxugqRU9Bj1CnNSZ81wEylhbCVHtDEirbKR1awxFVu0)

ภาพที่2 การปิดเครื่อง

 ```
@startuml
title Shut Down
[*] -r-> Ready 
Ready : downloading for instructions.
Ready -r-> off : Switch is turned off.
off : do/shut Down the power.
off--> [*] 

@enduml
 ```
 
 ![](http://www.plantuml.com/plantuml/img/DOwn3i8m34JtVCNDI2ax0-h05z0HCLHDGYm56oMEeluzQGkJfNjtvnkBpbdhEnabJHvJh8gRD3QFqnCssolkVdOhp74kS1qccHtn2q4oY8lckYW9b-7dsdCIGhTFZNI9e0AjcRtRvC4SpCcv_Fz1eyT7ciyxjRrWMs3CwDdrVLy0)
 
 ภาพที่3 การถอดรหัสคำสั่ง
 
  ```
 @startuml
title Decode
[*] -r-> Ready 
Ready : downloading for instructions.
Ready --> Decoding 
Decoding : do/decoding instruction.
Decoding -d-> Decoding: Decoding not complete
Decoding--> Ready : Decoding complete. 

@enduml
 ```
 
 ![](http://www.plantuml.com/plantuml/img/JOyn3i8m34Ltdy8pKiBU0NNW1Ao88OeDYfJQA765k3qjq3IJRUczB_-nMYWsJnaiMMOySrHYk1vkw8exuOK3lH5-Oq3IbsGDbEI1TosOf5gPeoMLwl-KMxHlp0f1srRvIDlLYNvd77NkiAU86aQTdfcD6-tQUnsvKHu1HXPQcdq0)
 
 ภาพที่4 การอานคำสั่งจาก Memory
 
  ```
 @startuml
title Read instruction
[*] -r-> Ready 
Ready : do/waiting for instructions
Ready -r-> Reading : instruction Coming 
Reading : do/Reading instruction from memory
Reading -d-> Reading : Reading not com plete 
Reading -d-> Sending: Reading complete
Sending : do/sending instruction to CPU 
Sending -d-> Sending : Sending not Complete 
Sending --> Ready : Sending not complete

@enduml
  ```
  
  ![](http://www.plantuml.com/plantuml/img/LP0z2iCm38Ltdq9pmNJFK0AvG6dfL3gOs2c6s2goGiZjQoUEuqpwUP-UXDh0YdXoes3Beu67KHgi3qnJpnQzU5y-84dULcK1iOK6D5vdPTdwBmn8zKZ8J9bAJ5CJqA5BJN6eqMulQd0WTE2CGreABFN9TyyyClIH_es63Ppff_6fEE08hfp8odP1o4Lz0IDqznSKiFQBKtkMjdVPj8BBtyvaMI_Qs8tV_mC0)
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
