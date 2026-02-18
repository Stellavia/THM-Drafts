🔗 [Link to the Room](https://tryhackme.com/room/extanalysis)

## 🏷️Discover the forensic basics of the EXT file system.

1. [EXT File System Structure](#ext-file-system-structure)<br>
2. [Forensic Artifacts in EXT](#forensic-artifacts-in-ext)<br>
  2.1 [Analyzing Inode Metadata](#analyzing-inode-metadata)<br>
  2.2 [Recovering Files](#recovering-files)<br>
3. [Analyzing File System Timestamps](#analyzing-file-system-timestamps)<br>
4. [Tools for EXT Forensics](#tools-for-ext-forensics)<br>
5. [Practical](#practical)<br>

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# EXT File System Structure

&nbsp;








&nbsp;

---
><details><summary>❓What is the member of the ext4_super_block struct that holds the offset value to the first data block?</summary>s_first_data_block</details>
---
><details><summary>❓What is the offset where we can find the member s_blocks_count_lo in the ext4_super_block struct? (decimal format)</summary>4</details>
---

&nbsp;

# Forensic Artifacts in EXT

&nbsp;







&nbsp;

## Analyzing Inode Metadata

&nbsp;






&nbsp;

## Recovering Files

&nbsp;










&nbsp;

---
><details><summary>❓What is the inode number for the file /etc/passwd in the VM?</summary>10083</details>
---

&nbsp;

# Analyzing File System Timestamps

&nbsp;









&nbsp;

---
><details><summary>❓What is the btime for the file /atc/passwd?</summary>2024-11-28 21:52:28.724316576</details>
---

&nbsp;

# Tools for EXT Forensics

&nbsp;











&nbsp;

---
><details><summary>❓Select Data Sources > ext4_case.img_1 Host > ext4_case.img and select the file normal_file.txt. Analyze the data in the File Metadata tab on the bottom pane. What is the inode number of the file?</summary>12</details>
---
><details><summary>❓What is the creation time of the file timestomped.txt? (Format: YYYY-MM-DD hh:mm:ss)</summary>2025-01-06 03:34:09</details>
---

&nbsp;

# Practical

&nbsp;










&nbsp;

---
><details><summary>❓Identify the timestomped file in the mounted file system in /mnt/ext_exercises. What is the original creation date of the file? (Format: YYYY-MM-DD hh:mm:ss)</summary>2025-01-09 02:27:53</details>
---
><details><summary>❓What is the flag in the deleted file that starts with the characters "FFFFFFFFFF" in the mounted file system in /mnt/ext_exercises ?</summary>THM{s****-d******-f***-y**g****-n***}</details>
---



&nbsp;

<!-- CONCLUSION -->

&nbsp;
