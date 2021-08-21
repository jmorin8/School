# About

This assigment was about create a module with his manifest and a menu called `menuFC.ps1` which call functions from the module created. The functions in the module called `FC.psm1` allows you to check for 

- Firewall profile status 

- Network profile 
- Firewall blocking rules

Where you can change the status of each one even you can check your `Blocking Rules` and add new ones or delete it.

All the options are into a while loop 

```
Write-Host "-----Welcome-----"

[bool] $m = $true

while($m){
    $menu = Read-Host -Prompt "`nChoose an option`n`t`t[1] Check Profile Status`n`t`t[2] Change Profile Status`n`t`t[3] Check Network Profile`n`t`t[4] Change Network Profile`n`t`t[5] Check Blocking Rules`n`t`t[6] Add Blocking Rules`n`t`t[7] Delete Blocking Rules`n`t`t[8] Exit`n"

    switch($menu){
        1{Check-ProfilleStat}
        2{Change-ProfileStat}
        3{Check-NetProfile}
        4{Change-Netprofile}
        5{Check-BlockingRules}
        6{Add-BlockingRules}
        7{Del-BlockingRules}
        8{
            $m = $false
            Write-Host "`nExiting..."
        }
        default{
            Write-Host "Input an valid option!!`n"
        }
    }
}
```

Which is going to stop just if you want it, if not the whole menu will be shown in screen, it also validates for the correct options so if you choose a wrong option the menu will be displayed again 
