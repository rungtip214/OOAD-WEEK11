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
