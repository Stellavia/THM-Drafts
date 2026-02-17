🔗 [Link to the Room](https://tryhackme.com/room/analysingvolatilememory)

## 🏷️Learn how the Windows OS manages volatile data in different files on disk. Explore how to extract and analyse volatile data from those artefacts.

1. [Lab Connection](#lab-connection)<br>
2. [Managing Volatile Data - An Overview](#managing-volatile-data---an-overview)<br>
3. [PageFile: Overview](#pagefile-overview)<br>
4. [Hybernation File](#hybernation-file)<br>
5. [Crash Dump: Overview](#crash-dump-overview)<br>
6. [Analysis Crash Dump](#analysis-crash-dump)<br>


&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Lab Connection

&nbsp;










&nbsp;


---
><details><summary>❓Connect to the Lab. How many tools are present in the EZ tools folder on the Desktop?</summary>12</details>
---

&nbsp;


# Managing Volatile Data - An Overview

&nbsp;










&nbsp;


---
><details><summary>❓What is the default page size (in KB) in most Operating systems?</summary>4</details>
---
><details><summary>❓What is the name of the hibernation file?</summary>hiberfil.sys</details>
---
><details><summary>❓Which file is considered as the extension of the RAM?</summary>pagefile.sys</details>
---

&nbsp;

# PageFile: Overview

&nbsp;










&nbsp;


---
><details><summary>❓Which Registry Hive contains the information about the pagefile?</summary>SYSTEM</details>
---
><details><summary>❓Examine the domain-histogram. Which domain associated with distributing Malware has occured 192 times? Defang the domain.</summary>3z[.]nu</details>
---
><details><summary>❓Check the domain on VirusTotal; What is the verdict about this suspicious-looking domain?</summary>malware</details>
---

&nbsp;

# Hybernation File

&nbsp;











&nbsp;

---
><details><summary>❓At the time of hibernation, which network scanning tool was running?</summary>wireshark</details>
---
><details><summary>❓What is the process ID associated with the network scanning tool?</summary>5604</details>
---
><details><summary>❓Examine the command lines executed on this host; which data wiping tool was executed on the host?</summary>diskwipe.exe</details>
---
><details><summary>❓What is the full path, from which the data wiping tool was executed?</summary>C:\Users\Administrator\Downloads\Tools\DiskWipe.exe</details>
---

&nbsp;

# Crash Dump: Overview

&nbsp;











&nbsp;

---
><details><summary>❓What is the value of CrashDumpEnabled field in the Registry?</summary>1</details>
---
<!-- ADD ANSWER -->
><details><summary>❓Examine the Reliability Monitor chart. What is the report ID of the last crash dump?</summary></details>
---
><details><summary>❓How many times the system has reported critical events in the past?</summary>7</details>
---
><details><summary>❓What is the default path set for placing the crash dump in the settings?</summary>%SystemRoot%\MEMORY.DMP</details>
---

&nbsp;

# Analysis Crash Dump

&nbsp;










&nbsp;

---
><details><summary>❓Which application was responsible for the first crash?</summary>myfault</details>
---
><details><summary>❓What is the process ID associated with a suspicious-looking process called evil.exe?</summary>1970</details>
---
><details><summary>❓Which command can be used to find the exact time of the crash?</summary>!time</details>
---
><details><summary>❓One of the variables in PEB contains a secret flag; what is the value of the flag?</summary>THM{__I**_***_**_*****_**_***__}</details>
---

&nbsp;




