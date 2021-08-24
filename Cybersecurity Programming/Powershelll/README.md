# About

This assigment was about create a module with his manifest and a menu called `menuFC.ps1` which call functions from the module created. The functions in the module called `FC.psm1` allows you to check for 

- Firewall profile status 

- Network profile 
- Firewall blocking rules

Where you can change the status of each one even you can check your `Blocking Rules` and add new ones or delete it.



# Module Functions
```
CommandType     Name                                               Version    Source
-----------     ----                                               -------    ------
Function        Check-ProfilleStat                                 1.0        FC
Function        Change-ProfileStat                                 1.0        FC
Function        Check-NetProfile                                   1.0        FC
Function        Change-Netprofile                                  1.0        FC
Function        Check-BlockingRules                                1.0        FC
Function        Add-BlockingRules                                  1.0        FC
Function        Del-BlockingRules                                  1.0        FC
```
As i explain before each functions has a different purpose 



# Main Script
```
-----Welcome-----

Choose an option
                [1] Check Profile Status
                [2] Change Profile Status
                [3] Check Network Profile
                [4] Change Network Profile
                [5] Check Blocking Rules
                [6] Add Blocking Rules
                [7] Delete Blocking Rules
                [8] Exit
:
```



All the options are into a while loop which is going to stop just if you want it, if not the whole menu will be shown in screen, it also validates for the correct options so if you choose a wrong option the menu will be displayed again 

