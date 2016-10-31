# OOAD-WEEK11
State Diagram

ภาพที่1 การสร้างและพิมพ์เอกสาร
 ```
@startuml
title turn on COMPUTER

[*] --> OFF
OFF : switch shut down
OFF -r-> ON
ON : turn on computer

ON -d-> Boot : computer work
Boot : loading System

Boot -l-> Ready : boot computer into works
Ready : computer available
Ready --> [*]
@enduml
 ```
