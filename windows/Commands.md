`TASKKILL /F /PID 19036

`tasklist /fi "pid eq 19036`

`netstat -ano | findstr "8080"`

`doskey /history`  
`chkdsk`  
`cls`

doskey /history  
chkdsk  
cls  
shutdown /s /t 5  
rmdir /s /q  
ping -c 3 gitlab.ca.cib


dir /s | more
dir | clip