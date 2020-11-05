netwalker.ps1
#Netwalker #Ransomware

File info: ASCII text, with very long lines, with no line terminators

MD5 
B1F0093B89561C6123070165BD2261E2

SHA1 
AAC57162DC1311F07A869F7163BD30E0D62DCC0E

SHA256 
F4656A9AF30E98ED2103194F798FA00FD1686618E3E62FBA6B15C9959135B7BE

SSDEEP 
24576:3LWHR7HOXN6YTYO1OC8UCMIH/MUWL+ZN4LTC3O+WXCWNLALRCFIAM1BQ9P0IQWWS:L

https://app.any.run/tasks/a73c2f59-5c58-4e93-b467-ef627707293a/

T1086 - PowerShell - PowerShell script executed

cmdline: "C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe" "-file" "C:\Users\admin\AppData\Local\Temp\netwalker.ps1"

image: C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe


T1064 - Scripting -  PowerShell script executed

cmdline: "C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe" "-file" "C:\Users\admin\AppData\Local\Temp\netwalker.ps1"

image: C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe


T1176 - Browser Extensions - Modifies files in Chrome extension folder
created: NONE

device: DISK_FILE_SYSTEM

name: C:\Users\admin\AppData\Local\Google\Chrome\User Data\Default\Extensions\pkedcjkdefgpdelpbcmbmeomcjbeemfm\7919.1028.0.0_0\background_script.js

object: FILE

operation: FASTWRITE

status: 0x00000000

time: 41891 ms


T1055 - Process Injection - explorer.exe Application was injected by another process

fromName: C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe

fromPID: 2560


T1055 - Process Injection - powershell.exe Runs injected code in another process

toName: C:\Windows\explorer.exe

toPID: 292

time: 26375 ms

T1500 -  Compile After Delivery - powershell.exe Starts Visual C# compiler

cmdline: "C:\Windows\Microsoft.NET\Framework\v2.0.50727\csc.exe" /noconfig /fullpaths @"C:\Users\admin\AppData\Local\Temp\xcsm_k7b.cmdline"

image: C:\Windows\Microsoft.NET\Framework\v2.0.50727\csc.exe

time: 21657 ms


T1003 - Credential Dumping - Reads the cookies of Google Chrome

created: NONE

device: DISK_FILE_SYSTEM

name: C:\Users\admin\AppData\Local\Google\Chrome\User Data\Default\Cookies

object: FILE

operation: READ

status: 0x00000103

time: 32047 ms


T1486 - Data Encrypted for Impact 



BEHAVIOR:



Renames files like Ransomware

Application was injected by another process

Netwalker ransom note found

Runs injected code in another process

Starts Visual C# compiler

Modifies files in Chrome extension folder

NETWALKER was detected

Creates files like Ransomware instruction

Reads the cookies of Google Chrome

Creates files in the program directory

Creates files in the user directory

Dropped object may contain TOR URL's
