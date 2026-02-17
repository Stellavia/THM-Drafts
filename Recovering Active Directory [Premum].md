🔗 [Link to the Room](https://tryhackme.com/room/recoveringactivedirectory)

## 🏷️Learn basic techniques to recover an AD in case of compromise.

1. [Introduction](#introduction)<br>
2. [Immediate Actions - First Response](#immediate-actions---first-response)<br>
3. [How did it happen? Identifying Attack Pattern](#how-did-it-happen-identifying-attack-pattern)<br>
4. [Who did this? Locating an Infection Vector](#who-did-this-locating-an-infection-vector)<br>
5. [How to get it back? Domain Takeback](#how-to-get-it-back-domain-takeback)<br>
6. [Why did it happen? Common Misconfigurations](#why-did-it-happen-common-misconfigurations)<br>
7. [Post Recovery Actions](#post-recovery-actions)<br>

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Introduction

&nbsp;











&nbsp;

---
><details><summary>❓I can connect to the machine.</summary>No answer needed</details>
---
><details><summary>❓What is the flag value after connecting to the machine?</summary>THM{I_***_******T}</details>
---

&nbsp;

# Immediate Actions - First Response

&nbsp;












&nbsp;

---
><details><summary>❓What type of backups can be obtained from the Windows Server Backup utility (write the correct option only)? A: One-time, B: Incremental, C: Both A and B</summary>C</details>
---
><details><summary>How would you launch the Windows Server Backup utility through the Run dialog box?</summary>wbadmin.msc</details>
---
><details><summary>❓Is it good practice to isolate the infected network infrastructure for detailed network monitoring? (yea/nay).</summary>yea</details>
---

&nbsp;

# How did it happen? Identifying Attack Pattern

&nbsp;












&nbsp;

---
><details><summary>❓How many machines in the domain can you find when using PowerView?</summary>11</details>
---
><details><summary>❓What is the name of the utility in Windows that displays and keeps track of all the events?</summary>Event Viewer</details>
---

&nbsp;

# Who did this? Locating an Infection Vector

&nbsp;













&nbsp;

---
><details><summary>❓What is the email address for the user evil.guy?</summary>hack@crypto</details>
---
><details><summary>❓What is the total number of users logged on after Dec 1, 2022?</summary>1</details>
---
><details><summary>❓What event ID will be logged if a user is removed from a universal security group?</summary>4757</details>
---

&nbsp;

# How to get it back? Domain Takeback

&nbsp;












&nbsp;

---
><details><summary>❓Reset the password for the user evil.guy.</summary>No answer needed</details>
---
><details><summary>❓What is the command to perform the password reset operation for a computer in the domail?</summary>Reset-ComputerMachinePassword</details>
---
><details><summary>❓What is the security vulnerability that involves abusing Kerberos service tikets called?</summary>Silver ticket abuse</details>
---

&nbsp;

# Why did it happen? Common Misconfigurations

&nbsp;










&nbsp;

---
><details><summary>❓The type of attack that allows attackers to impersonate a domain controller and receive/forward requests on behalf of the domain controller is called?</summary>DCSync</details>
---
><details><summary>❓Is synchronising time on all network devices important to correlate logs on different devices? (yea/nay).</summary>yea</details>
---

&nbsp;

# Post Recovery Actions

&nbsp;











&nbsp;

---
><details><summary>❓Click the View Site button at the top of the task to launch the static site in split view. What is the flag after completing the exercise?</summary>THM{I_***_*********_*D}</details>
---

&nbsp;

<!-- CONCLUSION -->


&nbsp;
