#lokibot #loki #malware #infected #sample

---------------------------------------------------------------------------
password: infected
---------------------------------------------------------------------------

sandbox: https://app.any.run/tasks/ce9bb0bc-0133-4e41-9178-c99ed65c4aba/

 SHA256 34A2F0477B0C7F0F99EF0922AD87384E4857B0D51A0B209C66DB1AC9B409CC56 
 SHA1 B27520C6E870A88230A7E8411875977647C36F04 
 MD5 A0E701175AA6BD7C6FD4F8632D7E8E40

-----------------------------------------

Dropped executable file  
 SHA256 C:\Users\admin\AppData\Roaming\F63AAA\A71D80.exe

34A2F0477B0C7F0F99EF0922AD87384E4857B0D51A0B209C66DB1AC9B409CC56 

DNS requests  
 DOMAIN masterworkhanger(.)com 

Connections  
 IP 47.88.102(.)244 

HTTP/HTTPS requests  
 URL hxxp://masterworkhanger(.)com/chisom/fre.php



---------------------------------------------------------------------------
MITRE:

T1106 - Execution through API
 Application launched itself
cmdChild: "C:\Users\admin\AppData\Local\Temp\9rmo9VWSFs6r4v1.bin.exe"
cmdParent: "C:\Users\admin\AppData\Local\Temp\9rmo9VWSFs6r4v1.bin.exe"
image: C:\Users\admin\AppData\Local\Temp\9rmo9VWSFs6r4v1.bin.exe


T1204 - User Execution
 Manual execution by user
cmdline: "C:\Windows\explorer.exe"
image: C:\Windows\explorer.exe


T1081 - Credentials in Files
 Actions looks like stealing of personal data
access: FILE_READ_ATTRIBUTES
created: SUPERSEDED
device: DISK_FILE_SYSTEM
name: C:\Users\admin\AppData\Local\Comodo\Dragon\User Data\Default\Web Data
object: UNKNOWN TYPE
operation: CREATE
