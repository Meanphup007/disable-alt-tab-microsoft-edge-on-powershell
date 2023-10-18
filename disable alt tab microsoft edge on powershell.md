## Navigate to the appropriate registry key
    Set-Location -Path "HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced"
## Set the value of MultiTaskingAltTabFilter to 3
    Set-ItemProperty -Path "HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced" -Name "MultiTaskingAltTabFilter" -Value 3
---
**NOTE**

    - 0 = Show open windows and all tabs in Microsoft Edge
    - 1 = Show Open windows and 5 most recent tabs in Microsoft Edge
    - 2 = Show Open windows and 3 most recent Edge tabs
    - 3 = Show Open windows only
---
## Kill Windows Explorer
    taskkill /f /im explorer.exe
## Start Windows Explorer
    start explorer
    
