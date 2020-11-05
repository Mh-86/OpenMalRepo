
INTRODUCTION:
CrySIS, aka Dharma, is a family of ransomware that has been evolving since 2016. We have noticed that this ransomware has become increasingly active lately, increasing by a margin of 148 percent from February until April 2019. The uptick in detections may be due to CrySIS’ effective use of multiple attack vectors.

CrySIS/Dharma targets Windows systems, and this family primarily targets businesses. It uses several methods of distribution:

CrySIS is distributed as malicious attachments in spam emails. Specific to this family is the use of malicious attachments that use double file extensions, which under default Windows settings may appear to be non-executable, when in reality they are.
CrySIS can also arrive disguised as installation files for legitimate software, including AV vendors. CrySIS operators will offer up these harmless looking installers for various legitimate applications as downloadable executables, which they have been distributing through various online locations and shared networks.
Most of the time, CrySIS/Dharma is delivered manually in targeted attacks by exploiting leaked or weak RDP credentials. This means a human attacker is accessing the victim machines prior to the infection by brute-forcing the Windows RDP protocol on port 3389.

In a recent attack, CrySIS was delivered as a download link in a spam email. The link pointed to a password-protected, self-extracting bundle installer. The password was given to the potential victims in the email and, besides the CrySIS/Dharma executable, the installer contained an outdated removal tool issued by a well-known security vendor.
This social engineering strategy worked to bring down user defenses. Seeing a familiar security solution in the installation package tricked users into believing the downloadable was safe, and the attack was successful.

The infection chain:
Once CrySIS has infected a system, it creates registry entries to maintain persistence and encrypts practically every file type, while skipping system and malware files. It performs the encryption routine using a strong encryption algorithm (AES-256 combined with RSA-1024 asymmetric encryption), which is applied to fixed, removable, and network drives.
Before the encryption routine, CrySIS deletes all the Windows Restore Points by running the vssadmin delete shadows /all /quiet command.
The Trojan that drops the ransomware collects the computer’s name and a number of encrypted files by certain formats, sending them to a remote C2 server controlled by the threat actor. On some Windows versions, it also attempts to run itself with administrator privileges, thus extending the list of files that can be encrypted.
After a successful RDP-based attack, it has been observed that before executing the ransomware payload, CrySIS uninstalls security software installed on the system.
