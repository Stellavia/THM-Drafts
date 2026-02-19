🔗 [Link to the Room](https://tryhackme.com/room/fat32analysis)

## 🏷️Examine the FAT32 filesystem from a forensic point of view.

1. [FAT32: Relevancy in Cyber Security](#fat32-relevancy-in-cyber-security)<br>
  1.1 [USB attacks](#usb-attacks)<br>
  1.2 [Attack Media Using FAT32](#attack-media-using-fat32)<br>
2. [FAT32 Structure: Reserved and FAT Areas](#fat32-structure-reserved-and-fat-areas)<br>
  2.1 [FAT32 Structure](#fat32-structure)<br>
  2.2 [Reserved Area](#reserved-area)<br>
  2.3 [Boot Sector](#boot-sector)<br>
  2.4 [FAT Area](#fat-area)<br>
3. [FAT32 Structure: Data Area](#fat32-structure-data-area)<br>
  3.1 [Data Area](#data-area)<br>
  3.2 [Long File Name](#long-file-name)<br>
  3.3 [Short File Name](#short-file-name)<br>
  3.4 [Key Takeaways](#key-takeaways)<br>
4. [FAT32: Analysis Techniques and Tools](#fat32-analysis-techniques-and-tools)<br>
  4.1 [Filesystem Analysis Techniques](#filesystem-analysis-techniques)<br>
  4.2 [Filesystem Integrity and Structural Analysis](#filesystem-integrity-and-structural-analysis)<br>
  4.3 [Data Recovery and Content Analysis](#data-recovery-and-content-analysis)<br>
5. [T1564.001 Hidden Files and Directories](#t1564-001-hidden-files-and-directories)<br>
  5.1 [Manual Analysis](#manual-analysis)<br>
    5.1.1 [Directories](#directories)<br>
  5.2 [Automated Analysis](#automated-analysis)<br>
    5.2.1 [Directories](#directories)<br>
    5.2.2 [Files](#files)<br>
6. [T1070.006 Indicator Removal: Timestomp](#t1070-006-indicator-removal-timestomp)<br>
  6.1 [Manual Analysis](#manual-analysis)<br>
  6.2 [Automated Analysis](#automated-analysis)<br>
7. [T1070.004 File Deletion and T1070.009 Clear Persistence](#t1070-004-file-deletion-and-t1070-009-clear-persistence)<br>
  7.1 [Manual Analysis](#manual-analysis)<br>
  7.2 [Automated Analysis](#automated-analysis)<br>
8. [Challenge](#challenge)<br>

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION + ENVIRONMENT AND SETUP HERE -->

&nbsp;

# FAT32: Relevancy in Cyber Security

&nbsp;




## USB attacks






## Attack Media Using FAT32







&nbsp;

---
><details><summary>❓What is the name of the attack that targeted the Iranian nuclear program?</summary>Stuxnet</details>
---
><details><summary>❓What category of tactic is MITRE ATT&CK TA0005?</summary>Defense Evasion</details>
---

&nbsp;

# FAT32 Structure: Reserved and FAT Areas

&nbsp;



## FAT32 Structure


## Reserved Area


## Boot Sector


## FAT Area








&nbsp;

---
<!-- ADD QA HERE -->

><details><summary>❓</summary></details>
---
<!-- ADD QA HERE -->

><details><summary>❓</summary></details>
---

&nbsp;

# FAT32 Structure: Data Area

&nbsp;



## Data Area

## Long File Name



## Short File Name

## Key Takeaways





&nbsp;

---
><details><summary>❓What is the filename of the file that starts at cluster 9?</summary>careers.txt</details>
---
><details><summary>❓What is the creation time of the file that starts at cluster 9? Please provide the hexadecimal value of the Creation time field.</summary>F484</details>
---

&nbsp;

# FAT32: Analysis Techniques and Tools

&nbsp;


## Filesystem Analysis Techniques



## Filesystem Integrity and Structural Analysis



## Data Recovery and Content Analysis






&nbsp;

---
><details><summary>❓Which analysis technique can we use to look for hidden files and directories?</summary>Directory Structure and File Name Analysis</details>
---

&nbsp;

# T1564.001 Hidden Files and Directories

&nbsp;



## Manual Analysis


### Directories


## Automated Analysis


### Directories


### Files




&nbsp;

---
><details><summary>❓What is the short file name of the hidden file in the M@IL0v3 directory?</summary>BEMYVA~1</details>
---
><details><summary>❓What is the flag found during automated analysis?</summary>THM{F****************3}</details>
---

&nbsp;

# T1070.006 Indicator Removal: Timestomp

&nbsp;



## Manual Analysis



## Automated Analysis




&nbsp;

---
><details><summary>❓What is the Accessed timestamp of the discovered suspicious file?</summary>2018-01-10 00:00:00</details>
---
><details><summary>❓What is the flag found during the automated analysis?</summary>THM{T*********D}</details>
---

&nbsp;

# T1070.004 File Deletion and T1070.009 Clear Persistence

&nbsp;




## Manual Analysis



## Automated Analysis




&nbsp;

---
><details><summary>❓Which hexadecimal sequence identifies a deleted file?</summary>E5</details>
---
><details><summary>❓What is the output of the delected PowerShell script after executing it? Note: in real-life investifations, we will only execute a suspicious file in a sandboxed environment.</summary>THM{r********_3******3}</details>
---

&nbsp;

# Challenge

&nbsp;












&nbsp;

---
><details><summary>❓At which offset does the FAT1 table begin? Fill in the complete offset number XXXXXX.</summary>0020FC00</details>
---
><details><summary>❓What is the name of the hidden directory on the imaeg? (Excluding the System Volume Information folder and the Recycle Bin).</summary>Exfiltrated_data</details>
---
><details><summary>❓What is the flag found in the hidden directory?</summary>THM{D********L}</details>
---
><details><summary>❓What is the size (bytes) of the archive file in the hidden directory?</summary>10862</details>
---
><details><summary>❓What is the name of the deleted file that is present on the image?</summary>Reverseshell.py</details>
---
><details><summary>❓What is the flag included in the deleted file?</summary>THM{B***********D}</details>
---
><details><summary>❓What is the name of the file that has suspicious timestamp(s) (name.extension)?</summary>Legal_Affairs_Notes.txt</details>
---
><details><summary>❓What is the flag included in the file with suspicious timestaps?</summary>THM{D***********G}</details>
---

&nbsp;

<!-- CONCLUSION HERE -->

&nbsp;
