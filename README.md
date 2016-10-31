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
