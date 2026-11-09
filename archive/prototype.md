1. User Flow

Login (by employee ID)
  ↓
Home
  ├── motors greasing 
  ├── job tracking
  ├── PM job
  ├── troubleshooting guid
  ├── Notifications
  ├── setting
  └── Profile



  motor greasing
  ├── new job request [1]
  ├── my jobs [2]
  ├── list of requsted jobs (pinding) [3]
  ├── list of online jobs [4]
  ├── recently closed jobs (24h) [5]
  ├── all closed jobs [6]
  ├── up coming jobs reminder list (dependes on motor runing hours, befor 4 days) [7]
  ├──
  └──

new job request (avalible for engeneers) [1]
  ├── scope list (Unit 1, Unit 2, Oil shale, ash, pob ) "hidden list"
  ├── motors list "hidden list, each scope have own motors list"
  ├── PTW number "input box"
  ├── DE Bearing "check box"
  |     ├──amount of grease
  ├── NDE Bbearing "check box"
  |     ├──amount of grease 
  ├── note "input box"
  └── submit
        ↓
        confermation message
        ↓
        add the job to the list of requsted jobs (pinding) and (my job for engineer)

  

my jobs [2]
  ├── list of my online jobs
  ├── list of my requsted (pinding) jobs (only for engineer)
  ├── closed jobs
  ├──

online job 
  ├── motor name and KKS (only reading)
  ├── job owner or requsted by (only reading)
  ├── PTW number (only reading)
  ├── DE bearing: requsted amount of grease | input box for applied amount (only job worker can eddit)
  ├── NDE bearing: requsted amount of grease | input box for applied amount (only job worker can eddit)
  ├── bearings temprture (online measuring) (only reading)
  ├── note (only reading)
  ├── add note (only job worker can eddit)
  ├── add pictures (only job worker can eddit)
  ├── update (only job worker can update)
  └── finish job (only job worker can finish)
        ↓
       move the job to closed jobs
 





list of requsted jobs (pinding) [3]
    feild components: request ID |  motor name  |   review  | pick up (avalible for technician)

review 
  ├── motor name and KKS (only reading)
  ├── job owner or requsted by
  ├── PTW number (only reading)
  ├── DE bearing: amount of grease (only reading)
  ├── NDE bearing: amount of grease (only reading)
  ├── bearing temprture (online measuring) (only reading)
  ├── note (only reading)
  ├── eddit (avilabile for job owner)
  ├── cancel and delete (avilabile for job owner)
  └── pick up (avalible for technician)


eddit (avilabile for job owner)
  ├── scope list (Unit 1, Unit 2, Oil shale, ash, pob ) "hidden list"
  ├── motors list "hidden list, each scope have own motors list"
  ├── PTW number "input box"
  ├── DE Bearing "check box"
  |     ├──amount of greas
  ├── NDE Bbearing "check box"
  |     ├──amount of greas 
  ├── note "input box"
  └── submit 
        ↓
    confermation eddit  message
        ↓
    apply eddit
    

  
cancel and delete
    ↓
confermation message
    ↓
add the job to deleted jobs




pick up
    ↓
confermation message
    ↓
add the job to online jobs and (my jobs for technician)
    



list of online jobs [4]
  feild components: job ID |  motor name  | job worker | progress | review 


review 
  ├── motor name and KKS (only reading)
  ├── job owner, requsted by (only reading)
  ├── job worke, picked up by (only reading)
  ├── PTW number (only reading)
  ├── DE bearing: applied amount of grease /requsted amount of grease (only reading)
  ├── NDE bearing: applied amount of grease /requsted amount of grease (only reading)
  ├── bearing temprture (online measuring) (only reading)
  ├── note (only reading)
  └── 


recently closed jobs (24h) [5]
  ├── list of recently closed jobs

feild components: job ID |  scope | motor name | closed date and time | review

review
  ├── motor name and KKS (only reading)
  ├── job owner or requsted by
  ├── job worke, picked up by  
  ├── PTW number (only reading)
  ├── DE bearing: applied amount of grease /requsted amount of greasee (only reading)
  ├── NDE bearing: applied amount of grease /requsted amount of grease (only reading)
  ├── max bearing temprture during the job (only reading)
  ├── owner note  (only reading)
  ├── worker note  (only reading)
  ├── picturs (only reading)
  ├── request date and time (only reading)
  └── finish date and time (only reading)




all closed jobs [6]

  ├── list of all closed jobs

feild components: job ID |  scope | motor name | closed date and time | review

review
  ├── motor name and KKS (only reading)
  ├── job owner or requsted by (only reading)
  ├── job worke, picked up by  
  ├── PTW number (only reading)
  ├── DE bearing: applied amount of grease /requsted amount of greasee (only reading)
  ├── NDE bearing: applied amount of grease /requsted amount of grease (only reading)
  ├── max bearing temprture during the job (only reading)
  ├── owner note  (only reading)
  ├── worker note  (only reading)
  ├── picturs (only reading)
  ├── request date and time (only reading)
  └── finish date and time (only reading)


up coming jobs reminder list (dependes on motor runing hours, befor 4 days) [7]
  ├── list of motors that need to grease soon (within 4 days)

feild components: scope | motor name |  remaining runing hours for greasing |review

review
  ├── scope
  ├── motor name and KKS
  ├── closed jobs list "hidden list"
  ├── motor tempreture
  ├── online runing hours
  ├── next greasing runing hours
  ├── remaining runing hours for greasing
  ├── make job request
  