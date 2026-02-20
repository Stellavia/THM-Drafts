🔗 [Link to the Room](https://tryhackme.com/room/btwindowsinternals)

## 🏷️Explore the core processes within a Windows operating system and understand what normal behaviour is. This foundational knowledge will help you identify malicious processes running on an endpoint!

1. [Task Manager](#task-manager)<br>
2. [System](#system)<br>
3. [System > smss.exe](#system-smssexe)<br>
4. [csrss.exe](#csrssexe)<br>
5. [wininit.exe](#wininit.exe)<br>
6. [wininit.exe > services.exe](#wininitexe-servicesexe)<br>
7. [Wininit.exe > services.exe > svchost.exe](#wininitexe-servicesexe-svchostexe)<br>
8. [lsass.exe](#lsassexe)<br>
9. [winlogon.exe](#winlogonexe)<br>
10. [explorer.exe](#explorerexe)<br>


&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Task Manager

&nbsp;






<!-- NO QUESTIONS -->

&nbsp;

# System

&nbsp;







&nbsp;

---
><details><summary>❓What PID should System always be?</summary>4</details>
---

&nbsp;

# System > smss.exe

&nbsp;









&nbsp;

---
><details><summary>❓Aside from csrss.exe, what process does smss.exe spawn in Session 1?</summary>winlogon.exe</details>
---

&nbsp;

# csrss.exe

&nbsp;









&nbsp;

---
><details><summary>❓What was the process which had PID 384 and PID 488?</summary>smss.exe</details>
---

&nbsp;

# wininit.exe

&nbsp;









&nbsp;

---
><details><summary>❓Which process might you not see running if Credential Guard is not enabled?</summary>lsaiso.exe</details>
---

&nbsp;

# wininit.exe > services.exe

&nbsp;








&nbsp;

---
><details><summary>❓How many instances of services.exe should be running on a Windows system?</summary>1</details>
---

&nbsp;

# Wininit.exe > services.exe > svchost.exe

&nbsp;







&nbsp;

---
><details><summary>❓What single letter parameter should always be visible in the Command line or Binary path?</summary>k</details>
---

&nbsp;

# lsass.exe

&nbsp;







&nbsp;

---
><details><summary>❓What is the parent process for LSASS?</summary>wininit.exe</details>
---

&nbsp;

# winlogon.exe

&nbsp;







&nbsp;

---
><details><summary>❓What is the non-existent parent process for winlogon.exe</summary>smss.exe</details>
---

&nbsp;

# explorer.exe

&nbsp;







&nbsp;

---
><details><summary>❓What is the non-existent process for explorer.exe?</summary>userinit.exe</details>
---


&nbsp;

<!-- CONCLUSION -->



&nbsp;
