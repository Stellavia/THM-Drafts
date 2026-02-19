🔗 [Link to the Room](https://tryhackme.com/room/mbrandgptanalysis)

## 🏷️Learn how MBR and GPT forensics are carried out to identify attacks during the boot process.

1. [Introduction](#introduction)<br>
2. [Boot Process](#boot-process)<br>
  2.1 [Power-On the System](#power-on-the-system)<br>
  2.2 [Power-On-Self-Test (POST)](#power-on-self-test-post)<br>
  2.3 [Locate the Bootable Device](#locate-the-bootable-device)<br>
3. [What if MBR?](#what-if-mbr)<br>
  3.1 [Analyzing the MBR](#analyzing-the-mbr)<br>
  3.2 [Bootloader Code (Bytes 0-445)](#bootloader-code-bytes-0-445)<br>
  3.3 [Partitions Table (Bytes 446-509)](#)<br>
  3.4 [MBR Signature (Bytes 510-511)](#)<br>
4. [Threats Targeting MBR](#)<br>
5. [MBR Tampering Case](#)<br>
  5.1 [Scenario](#)<br>
  5.2 [Instructions](#)<br>
6. [What if GPT?](#)<br>
  6.1 [Protective MBR](#)<br>
  6.2 [Primary GPT Header](#)<br>
  6.3 [Partition Entry Array](#)<br>
  6.4 [Backup GPT Header](#)<br>
  6.5 [Backup Partition Entry Array](#)<br>
7. [Threats Targeting GPT](#)<br>
8. [UEFI Bootkit Case](#)<br>

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Introduction



---
><details><summary>❓What are the separate sections on a disk known as?</summary>partitions</details>
---
><details><summary>❓Which type of malware infects the boot process?</summary>bootkits</details>
---

# Boot Process


## Power-On the System
## Power-On-Self-Test (POST)
## Locate the Bootable Device


---
><details><summary>❓What is the name of the hardware diagnostic check performed during the boot process?</summary>Power-On-Self-Test</details>
---
><details><summary>❓Which firmware supports a GPT partitioning scheme?</summary>UEFI</details>
---
><details><summary>❓Which device has the operating system to boot the system?</summary>bootable device</details>
---


# What if MBR?


## Analyzing the MBR
## Bootloader Code (Bytes 0-445)
## Partitions Table (Bytes 446-509)
## MBR Signature (Bytes 510-511)


---
><details><summary>❓Which component of the MBR contains the details of all the partitions present on the disk?</summary>partition  table</details>
---
><details><summary>❓What is the standard sector size of a disk in bytes?</summary>512</details>
---
><details><summary>❓Which component of the MBR is responsible for finding the bootable partition?</summary>bootloader code</details>
---
><details><summary>❓What is the magic number inside the MBR?</summary>55 AA</details>
---
><details><summary>❓What is the maximum number of partitions MBR can support?</summary>4</details>
---
><details><summary>❓What is the size of the second partition in hte MBR file found in C:\Analysis\MBR\ ? (rounded to the nearest GB)</summary>16</details>
---


# Threats Targeting MBR

<!-- NO QUESTIONS -->



# MBR Tampering Case



## Scenario
## Instructions




---
><details><summary>❓How many partitions are on the disk?</summary>1</details
---
><details><summary>❓What is the first byte at the starting LBA of the partition? (represented by two hexadecimal digits)</summary>EB</details
---
><details><summary>❓What is the type of the partition? </summary>NTFS</details
---
><details><summary>❓What is the size of the partition? (rounded to the nearest GB)</summary>32</details
---
><details><summary>❓What is the flag hidden in the Administrator's Documents folder?</summary>THM{C***_T**_M**}</details
---

# What if GPT?


## Protective MBR
## Primary GPT Header
## Partition Entry Array
## Backup GPT Header
## Backup Partition Entry Array



---
><details><summary>❓How many partitions are supported by the GPT?</summary>128</details>
---

<!-- ADD ANSWER -->

><details><summary>❓What is the partition type GUID of the 2nd partition given in the attached GPT file?</summary></details>
---


# Threats Targeting GPT


<!-- NO QUESTIONS -->

# UEFI Bootkit Case

&nbsp;


---
><details><summary>❓Which partition has the bootloader in it?</summary>EFI System Partition</details>
---
><details><summary>❓What is the malicious string embedded in the bootloader?</summary>Hello, EFI Bootkit!</details>
---

&nbsp;
