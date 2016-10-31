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
 
 ภาพที่5 การประมวลผล
 
   ```
 @startuml
title Execute 
[*] -r-> Ready 
Ready : do/waiting for instructions
Ready -r-> Executing 
Executing : do/cxecuting instruction
Executing -d-> Executing : Executing not complete 
Executing -->Ready : Memory instruction Executed 
Executing -r-> Buffering : I/O instruction Executed 
Buffering : do/keep output in memory 
Buffering -d-> Output : Buffering complete 
Output : do/Outputing the Result 
Output --> Ready : Output complete 
@enduml
   ```
   
   ![](http://www.plantuml.com/plantuml/img/TP4n3y8W48LtViND9gHxXwOnSN0mJLoDGrEkIYpGm17jlnUARUdWn95xtxl7KJjgBNarC98q89m-s7b2OBV37RZb5Lon5HEmT9GWJF5k9KdzWDvOaDgHzHr9ezrFCrF99whOLivqjrupDXDniSFBhDQ6e3Dg730cp11UBV4kg8oTSklbIM97n8n7t_Teqv1pqVo1SbM8_q8SmNWQFGK0L9gNgURyJHAKsOmj-DeCTgcEVNfYsBNp0wqAlgw_N1mtbngr2F_s1G00)
 
 Activity Diagram
 
 ภาพที่1 การตื่นนอน
 
    ```
 @startuml
title The awakening 
[*] --> Wake..up 
Wake..up -l-> Eat..Breakfast : hungry 
Wake..up -r-> Go..Back..To..Sleep : not hungry 
Eat..Breakfast -d-> [*] 
Go..Back..To..Sleep -d-> [*] 
@enduml
   ```
   
 ![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuIh9BCb9LGZ9I5L8B4_CJitBp4jNu8hMYbNGrRLJ20UAwEcL5YXmmLcwEK1nryGIFJsdejJ4xBJ4uX85AuMCqhpqeafaPKL0PUxvG5M9oTbwUY50Ld1EQce1K6rUVWbSFPf1kYb0NI3BkR1fHSWwfEQb01qF0000)
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
