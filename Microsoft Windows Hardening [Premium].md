
🔗 [Link to the Room](https://tryhackme.com/room/microsoftwindowshardening)

## 🏷️To learn key attack vectors used by hackers and how to protect yourself using different hardening techniques.

1. [Understanding General Concepts](#understanding-general-concepts)<br>
2. [Identity & Access Management](#identity-&-access-management)<br>
3. [Network Management](#network-management)<br>
4. [Application Management](#application-management)<br>
5. [Storage Management](#storage-management)<br>
6. [Updating Windows](#updating-windows)<br>
7. [Cheatsheet for Hardening Windows](#cheatsheet-for-hardening-windows)<br>

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Understanding General Concepts

&nbsp;








&nbsp;

---
><details><summary>❓What is the startup type of App Readiness service in the services panel?</summary>Manual</details>
---
><details><summary>❓Open Registry Editor and find the key "tryhackme". What is the default value of the key?</summary>{THM_***_****}</details>
---
><details><summary>❓Open the Diagnosis folder and go through the various log files. Can you find the flag?</summary>{THM_*******}</details>
---
><details><summary>❓Open the Event Viewer and play with various event viewer filters like Information, Error, Warning etc. Which error type has the maximum number of logs?</summary>No answer needed</details>
---

&nbsp;

# Identity & Access Management

&nbsp;










&nbsp;

---
><details><summary>❓Find the name of the Administrator Account of the attached VM</summary>Harden</details>
---
><details><summary>❓Go to the User Account Control Setting Panel (Control Panel > All Control Panel Items > User Accounts). What is the default level of Notification?</summary>Always Notify</details>
---
><details><summary>❓How many standard accounts are created in the VM?</summary>0</details>
---

&nbsp;

# Network Management

&nbsp;








&nbsp;

---
><details><summary>❓Open Windows Firewall and click on Monitoring in the left pane - which of the following profiles is active? Domain, Private, Public?</summary>Public</details>
---
><details><summary>❓Find the IP address resolved for the website tryhack.me in the Virtual Machine as per the local hosts file.</summary>192.168.1.140</details>
---
><details><summary>❓Open the command promnpt and enter arp -a. What is the Physical address for the IP address 255.255.255.255?</summary>ff-ff-ff-ff-ff-ff</details>
---

&nbsp;

# Application Management

&nbsp;








&nbsp;

---
><details><summary>❓Windows Defender Antivirus is configured to exclude a particular extension from scanning. What is the extension?</summary>.ps</details>
---
><details><summary>❓A Word document is received from an unknown email address. It is best practice to open it immediately on your personal computer (yay/nay).</summary>nay</details>
---
><details><summary>❓What is the flag you received after executing the Office Hardening Batch file?</summary>{THM_*******}</details>
---

&nbsp;

# Storage Management

&nbsp;






&nbsp;

---
><details><summary>❓A security engineer has misconfigured the attached VM and stored a BitLocker recovery key in the same computer. Can you read the last six digits of the recovery key?</summary>377564</details>
---
><details><summary>❓How many characters does the BitLocker recovery key have in the attached VM?</summary>48</details>
---
><details><summary>❓A backup file is placed on the Desktop of the attached VM. What is the extension of that file?</summary>.bkf</details>
---

&nbsp;

# Updating Windows

&nbsp;







&nbsp;

---
><details><summary>❓What is the CVE score for the vulnerability CVE ID CVE-2022-32230?</summary>7.8</details>
---

&nbsp;

# Cheatsheet for Hardening Windows

&nbsp;

<!-- NO QUESTIONS -->


&nbsp;
