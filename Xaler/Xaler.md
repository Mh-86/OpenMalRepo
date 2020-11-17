Relatively new Xaler Sample. Never seen this before. Doc Written in Chinese.

#Xaler #VBA #Macro #Malicious #Sample #Infected

https://www.hybrid-analysis.com/sample/667abd23c284cb2cd37a65a4387335205aeb7488ac409709dcb4e72d94122ed1/5fb45620ed309a0ffc22941a

Threat Score: 99/100AV Detection: 85%Labeled as: W97M.Lexar

FILE TYPE - CDF

FILE SIZE - 69.00KB

SHA 256 - 667abd23c284cb2cd37a65a4387335205aeb7488ac409709dcb4e72d94122ed1

SHA 1 - 7b56f4f1c38dc7ec6ad27c7e09ed742af961b8f4

MD5 - 00adc1f9e19e31f58a9f64c5e6b397c6


TTP's

------------

 T1204 - User Execution
Suspicious Indicators:	
Contains embedded VBA macros with suspicious keywords
Informative Indicators	
Contains embedded VBA macros

 T1179 - Hooking
Informative Indicators:
Installs hooks/patches the running process
Loads rich edit control libraries
Hooks API calls

T1137 - Office Application Startup
Malicious Indicators: 
Contains embedded VBA macros with keywords that indicate auto-execute behavior

T1112 - Modify Registry
Informative Indicators: 
Removes Office resiliency keys (often used to avoid problems opening documents)

T1010 - Application Window Discovery
Informative Indicators: 
Scanning for window names

T1114 - Email Collection
Suspicious Indicators:
Found a potential E-Mail address in binary/memory
