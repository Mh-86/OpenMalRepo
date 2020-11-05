#Dharma #Ransomware #Crysis

https://app.any.run/tasks/471cd691-fb02-4d0c-8f25-3763ac13edcd/

https://www.joesandbox.com/analysis/292749/0/html

MIME: application/x-dosexec

File info: PE32 executable (GUI) Intel 80386, for MS Windows

MD5 0C4CBF1CB8E5065F8DF8C8ADC4F80E84

SHA1 FE9FA42F2CD4E261783B14B6CF9A28B51162590D

SHA256 B565C8E1E81796DB13409F37E4BD28877272B5E54AB5C0A3D9B6A024E7F5A039

SSDEEP 1536:MBWL+KXPSQN5VLWWYYHY9S4AZG43JW0NLLJBIO3YHP1SKIRGQ:QW+ASQN5AW/HLM2JW0NNJBL3AND


-------

MITRE 

-------



T1059 - Command-Line Interface - payload.exe starts CMD.EXE for commands execution

cmdline: "C:\Windows\system32\cmd.exe"

image: C:\Windows\system32\cmd.exe


T1106 - Execution through API - payload.exe Application launched itself

cmdChild: "C:\Users\admin\AppData\Local\Temp\payload.exe" -a

cmdParent: "C:\Users\admin\AppData\Local\Temp\payload.exe"

image: C:\Users\admin\AppData\Local\Temp\payload.exe

time: 3125 ms


T1050 - New Service - vssvc.exe Executed as Windows Service

cmdline: C:\Windows\system32\vssvc.exe

image: C:\Windows\system32\vssvc.exe


T1060 -  payload.exe Changes the autorun value in the registry

key: HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Run

name: payload.exe

operation: write

typeValue: REG_SZ

value: C:\Windows\System32\payload.exe

time: 3281 ms


T1060 -  payload.exe Writes to a start menu file

created: NONE

device: DISK_FILE_SYSTEM

name: C:\Users\admin\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup\payload.exe

object: FILE

operation: WRITE

status: 0x00000103

time: 3281 ms


T1486 - Data Encrypted for Impact - payload.exe Renames files like Ransomware

created: NONE

device: DISK_FILE_SYSTEM

name: C:\MSOCache\All Users\{90140000-0015-0407-0000-0000000FF1CE}-C\AccLR.cab

newname: C:\MSOCache\All Users\{90140000-0015-0407-0000-0000000FF1CE}-C\AccLR.cab.id-C4BA3647.[yourfiles1@tutanota.com].FLYU

object: FILE

operation: RENAME

status: 0x00000103

time: 3469 ms


T1490 - Inhibit System Recovery - cmd.exe Deletes shadow copies

cmdline: vssadmin delete shadows /all /quiet

image: C:\Windows\system32\vssadmin.exe

time: 4078 ms
