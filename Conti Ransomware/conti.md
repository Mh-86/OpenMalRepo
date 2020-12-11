Conti Ransomware
LINK: https://malpedia.caad.fkie.fraunhofer.de/details/win.conti

Conti is a new family of ransomware observed in the wild by the Carbon Black Threat Analysis Unit (TAU). Unlike most ransomware, Conti contains  unique features that separate it in terms of performance and focus on network-based targets.  

Conti uses a large number of independent threads to perform encryption, allowing up to 32 simultaneous encryption efforts, resulting in faster encryption compared to many other families. 

Conti also utilizes command line options to allow for control over how it scans for data, suggesting that the malware may commonly be spread and directly controlled by an adversary. This control introduces the novel ability of skipping the encryption of local files and only targeting networked SMB shares, including those from IP addresses specifically provided by the adversary. This is a very rare ability that’s previously been seen with the Sodinokibi ransomware family. 

Source: Source: https://www.carbonblack.com/blog/tau-threat-discovery-conti-ransomware/
