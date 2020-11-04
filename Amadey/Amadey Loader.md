# Amadey Loader malware family samples

Amadey Loader (a.k.a. Project a2019) is a malware downloader written in C++; it is sold on
underground forums.


• Unlike most Windows malware that is compiled with Visual Studio, Amadey is compiled with the
MingW32 compiler.

• Amadey uses unencrypted HTTP POST requests to communicate with its command-and-control
(C2) server.

• The malware provides basic download-and-execute functionality with the ability to geotarget
and selectively deploy second-stage payloads.

• Amadey has been updated numerous times since its inception, with the current version being
1.09.
