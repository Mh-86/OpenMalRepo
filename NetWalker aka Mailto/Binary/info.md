WTVConverter.exe

#netwalker #ransomware

MIME: application/x-dosexec

SAMPLE ANALYZED : https://app.any.run/tasks/ab6c19e9-4a28-4835-8a76-d6e4e63200ea/#

File info: PE32 executable (GUI) Intel 80386, for MS Windows

MD5 258ED03A6E4D9012F8102C635A5E3DCD

SHA1 A3BC2A30318F9BD2B51CB57E2022996E7F15C69E

SHA256 8639825230D5504FD8126ED55B2D7AEB72944FFE17E762801AAB8D4F8F880160

SSDEEP 3072:KV4ZAWXDSXCOWN+V75SSIECX7FWR5JNFB23Y2O1NM5DC:B1X7VWVSPDOJND01


----------------------

MITRE

---------------------




T1053 - Scheduled Task- Loads the Task Scheduler COM API

image: C:\Windows\System32\taskschd.dll

protect: EXECUTABLE

status: LOAD

time: 203 ms


T1176 - Browser Extensions -  Modifies files in Chrome extension folder

created: NONE

device: DISK_FILE_SYSTEM

name: C:\Users\admin\AppData\Local\Google\Chrome\User Data\Default\Extensions\pkedcjkdefgpdelpbcmbmeomcjbeemfm\7919.1028.0.0_0\angular.js

object: FILE

operation: WRITE

status: 0x00000103

time: 10703 ms


T1081 - Credentials in Files - Stealing of credential data

filename: C:\Users\admin\AppData\Local\Google\Chrome\User Data\Default\Login Data.0b1567

md5: 36b012769459c7de4401be2e0972de97

size: 33030

string: https://m.facebook.com/honey@pot.com

time: 12219 ms


T1003 - Credential Dumping - Reads the cookies of Google Chrome

created: NONE

device: DISK_FILE_SYSTEM

name: C:\Users\admin\AppData\Local\Google\Chrome\User Data\Default\Cookies

object: FILE

operation: READ

status: 0x00000103

time: 8234 ms


T1114 - Email Collection - Stealing of credential data

filename: C:\Users\admin\AppData\Local\Google\Chrome\User Data\Default\Login Data.0b1567

md5: 36b012769459c7de4401be2e0972de97

size: 33030

string: https://m.facebook.com/honey@pot.com

time: 12219 ms


T1486 - Data Encrypted for Impact - Renames files like Ransomware

created: NONE

device: DISK_FILE_SYSTEM

name: C:\Users\admin\Desktop\airwall.png

newname: C:\Users\admin\Desktop\airwall.png.0b1567

object: FILE

operation: RENAME

status: 0x00000103

time: 1937 ms


T1490 - Inhibit System Recovery - Deletes shadow copies

cmdline: C:\Windows\system32\vssadmin.exe delete shadows /all /quiet

image: C:\Windows\system32\vssadmin.exe

time: 187 ms


