🔗 [Link to the Room](https://tryhackme.com/room/ntfsanalysis)

## 🏷️Explore the NTFS file system, its layout, and important components.

1. [NTFS Overview](#ntfs-overview)<br>
  1.1 [NTFS Comparison with Other File Systems](#ntfs-comparison-with-other-file-systems)<br>
2. [NTFS Components](#ntfs-components)<br>
  2.1 [Partition Boot Sector (PBS)](#partition-boot-sector-pbs)<br>
  2.2 [Master File Table (MFT)](#master-file-table-mft)<br>
  2.3 [$MFTMirr](#$mftmirr)<br>
  2.4 [System Files](#)<br>
  2.5 [File Data Area](#)<br>
  2.6 [Alternate Data Stream](#)<br>
  2.7 [Indentifying the Artifacts](#)<br>
  2.8 [Collecting the Artifacts](#)<br>
3. [MFT Record Analysis](#)<br>
  3.1 [Master File Table](#)<br>
  3.2 [Examining the MFT Record](#)<br>
  3.3 [Important Columns in the MFT Record](#)<br>
  3.4 [MACB Time](#)<br>
  3.5 [Why is the MACB Timestamp Important?](#)<br>
4. [NTFS Journaling](#)<br>
  4.1 [Types of NTFS Journals](#)<br>
  4.2 [Examining the Updated Reason](#)<br>
5. [Index Allocation Attribute ($130) Overview](#)<br>
  5.1 [Index Allocation Attribute ($130)](#)<br>
  5.2 [Slack Space](#)<br>
  5.3 [Forensics Value](#)<br>
  5.4 [Analyzing $130](#)<br>
  5.5 [File Attributes in the $130](#)<br>


&nbsp;

# 📚 Study Notes #

<!-- ADD INTRODUCTION and LAB CONNECTION -->

&nbsp;

# NTFS Overview

&nbsp;








&nbsp;

## NTFS Comparison with Other File Systems

&nbsp;









&nbsp;

---
><details><summary>❓Which feature does NTFS use to keep track of the changes within the file systems?</summary>journaling</details>
---

&nbsp;

# NTFS Components

&nbsp;








&nbsp;

## Partition Boot Sector (PBS)

&nbsp;








&nbsp;

### Forensics Value

&nbsp;







&nbsp;

## Master File Table (MFT)

&nbsp;






&nbsp;

### Forensics Value

&nbsp;





&nbsp;

## $MFTMirr

&nbsp;





&nbsp;

### Forensics Value

&nbsp;




&nbsp;

## System Files

&nbsp;





&nbsp;

### Forensic Value

&nbsp;






&nbsp;

## File Data Area

&nbsp;







&nbsp;

### Forensic Value

&nbsp;







&nbsp;

## Alternate Data Stream

&nbsp;







&nbsp;

## Indentifying the Artifacts

&nbsp;









&nbsp;

## Collecting the Artifacts

&nbsp;







&nbsp;

---
><details><summary>❓Double-click on the $UsnJrnl file in the $Extend folder; what is the first evidence file you find?</summary>$J</details>
---

&nbsp;

# MFT Record Analysis

&nbsp;






&nbsp;

## Master File Table

&nbsp;







&nbsp;

### Content of an MFT Record

&nbsp;









&nbsp;

## Examining the MFT Record

&nbsp;









&nbsp;

## Important Columns in the MFT Record

&nbsp;










&nbsp;

## MACB Time

&nbsp;










&nbsp;

## Why is the MACB Timestamp Important?

&nbsp;











&nbsp;

---
><details><summary>❓Which column indicates that the file is no longer present on the disk?</summary>In Use</details>
---
><details><summary>❓Examine the MFT record; what is the network sniffer installed on this system in the \Program Files\ directory?</summary>wireshark</details>
---
><details><summary>❓An anti-forensics tool responsible for wiping out an attacker's traces was installed in the \Downloads\Tools folder. What is the name of the tool?</summary>DiskWipe.exe</details>
---
><details><summary>❓According to the MFT record, is the anti-forensics tool currently present on the disk? (yay or nay)</summary>nay</details>
---
><details><summary>❓Examining the MFT record, it seems there is a record of a flag.txt file. What is the parent path of the file?</summary>.\tmp\secret_directory</details>
---
><details><summary>❓What is the content of the flag.txt file?</summary>W**D***_Y**_F****_*3</details>
---
><details><summary>❓What is the file name associated with the MFT entry number "584574"?</summary></details>
---

&nbsp;

# NTFS Journaling

&nbsp;








&nbsp;

## Types of NTFS Journals

&nbsp;










&nbsp;

### $LogFile

&nbsp;









&nbsp;

### Universal Sequence Number (USN) Journal ($USNJrnl)

&nbsp;












&nbsp;

### Structure of USNJrnl

&nbsp;











&nbsp;

### Extract the $J File

&nbsp;







&nbsp;

## Examining the Updated Reason

&nbsp;













&nbsp;

---
><details><summary>❓What is the text file name associated with entry number 95071 before renaming it?</summary>New Text Document.txt</details>
---
><details><summary>❓According to the record, what is the first operation performed on the file in the question above?</summary>FileCreate</details>
---
><details><summary>❓According to the record in $J, what is the count of the rename operation found against secred_code.txt?</summary>2</details>
---
><details><summary>❓According to the record, when was the secred_code.txt file deleted?</summary>2025-01-15 08:10:04</details>
---

&nbsp;

# Index Allocation Attribute ($130) Overview

&nbsp;










&nbsp;

## Index Allocation Attribute ($130)

&nbsp;








&nbsp;

## Slack Space

&nbsp;










&nbsp;

## Forensics Value

&nbsp;









&nbsp;

## Analyzing $130

&nbsp;










&nbsp;

## File Attributes in the $130

&nbsp;





&nbsp;

---
><details><summary>❓How many deleted files or folders are present in the $130 attribute file that was extracted in this task?</summary>52</details>
---
><details><summary>❓What is the parent MFT entry of the nmap directory?</summary>512386</details>
---

&nbsp;

<!-- NO QUESTIONS -->

&nbsp;
