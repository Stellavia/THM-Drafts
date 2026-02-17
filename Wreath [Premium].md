🔗 [Link to the Room](https://tryhackme.com/room/wreath)

## 🏷️Learn how to pivot through a network by compromising a public facing web machine and tunnelling your traffic to access other machines in Wreath's network.


1. [INTRO - Accessing the Network](#intro---accessing-the-network)<br>
2. [INTRO - Backstory](#intro---backstory)<br>
3. [INTRO - Brief](#intro---brief)<br>
4. [WEBSERVER - Enumeration](#webserver---enumeration)<br>
5. [WEBSERVER - Exploitation](#webserver---exploitation)<br>
6. [PIVOTING - What is Pivoting?](#pivoting---what-is-pivoting)<br>
7. [PIVOTING - High-level Overview](#pivoting---high-level-overview)<br>
8. [PIVOTING - Enumeration](#pivoting---enumeration)<br>
9. [PIVOTING - Proxychains and Foxyproxy](#pivoting---proxychains-and-foxyproxy)<br>
10. [PIVOTING - SSH Tunnelling and Port Forwarding](#pivoting---ssh-tunnelling-and-port-forwarding)<br>
11. [PIVOTING - plink.exe](#pivoting---plinkexe)<br>
12. [PIVOTING - Socat](#pivoting---socat)<br>
13. [Pivoting - Chisel](#pivoting---chisel)<br>
14. [Pivoting - sshuttle](#pivoting---sshuttle)<br>
15. [Pivoting - Conclusion](#pivoting---conclusion)<br>
16. [GIT SERVER - Enumeration](#git-server---enumeration)<br>
17. [GIT SERVER - Pivoting](#git-server---pivoting)<br>
18. [GIT SERVER - Code Review](#git-server---code-review)<br>
19. [GIT SERVER - Exploitation](#git-server---exploitation)<br>
20. [GIT SERVER - Stabilisation and Post Exploitation](#git-server---stabilisation-and-post-exploitation)<br>
21. [COMMAND AND CONTROL - Introduction](#command-and-control---introduction)<br>
22. [COMMAND AND CONTROL - Empire - Installation](#command-and-control---empire---installation)<br>
23. [COMMAND AND CONTROL - Empire - Overview](#command-and-control---empire---overview)<br>
24. [COMMAND AND CONTROL - Empire - Listeners](#command-and-control---empire---listeners)<br>
25. [COMMAND AND CONTROL - Empire - Stagers](#command-and-control---empire---stagers)<br>
26. [COMMAND AND CONTROL - Empire - Agents](#command-and-control---empire---agents)<br>
27. [COMMAND AND CONTROL - Empire - Hop Listeners](#command-and-control---empire---hop-listeners)<br>
28. [COMMAND AND CONTROL - Git Server](#command-and-control---git-server)<br>
29. [COMMAND AND CONTROL - Empire - Modules](#command-and-control---empire---modules)<br>
30. [COMMAND AND CONTROL - Empire - Interative Shell](#command-and-control---empire---interactive-shell)<br>
31. [COMMAND AND CONTROL - Conclusion](#command-and-control---conclusion)<br>
32. [PERSONAL PC - Enumeration](#personal-pc---enumeration)<br>
33. [PERSONAL PC - Pivoting](#personal-pc---pivoting)<br>
34. [PERSONAL PC - The Wonders of Git](#personal-pc---the-wonders-of-git)<br>
35. [PERSONAL PC - Website Code Analysis](#personal-pc---website-code-analysis)<br>
36. [PERSONAL PC - Exploit PoC](#personal-pc---exploit-poc)<br>
37. [AV EVASION - Introduction](#av-evasion---introduction)<br>
38. [AV EVASION - AV Detection Methods](#av-evasion---av-detection-methods)<br>
39. [AV EVASION - PHP Payload Obfuscation](#av-evasion---php-payload-obfuscation)<br>
40. [AV EVASION - Compiling Netcat and Reverse Shell](#av-evasion---compiling-netcat-and-reverse-shell)<br>
41. [AV EVASION - Enumeration](#av-evasion---enumeration)<br>
42. [AV EVASION - Privilege Escalation](#av-evasion---privilege-escalation)<br>
43. [EXFILTRATION - Exfiltration Techniques](#exfiltration---exfiltration-techniques)<br>
44. [CONCLUSION - Debrief and Report](#conclusion---debrief-and-report)<br>
45. [CONCLUSION - Final Thoughts](#conclusion---final-thoughts)<br>




<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/1fa7a328-269b-4c53-bd58-ce0fcd20008f" />

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# INTRO - Accessing the Network

# INTRO - Backstory


# INTRO - Brief


# WEBSERVER - Enumeration


---
><details><summary>❓How many of the first 15000 ports are open on the target?</summary>4</details>
---
><details><summary>❓Perform scan on these open ports. What OS does Nmap think is running?</summary>CentOS</details>
---
><details><summary>❓Open the IP in your browser -- what site does the server try to redirect you to?</summary>https://thomaswreath.thm</details>
---
><details><summary>❓Read through the text on the page. What is Thomas' mobile phone number?</summary>+447821548812</details>
---
><details><summary>❓Look back at your service scan results: what server version does Nmap detect as running here?</summary>MiniServ 1.890 (Webmin httpd)</details>
---
><details><summary>❓What is the CVE number for this exploit?</summary>CVE-2019-15107</details>
---


# WEBSERVER - Exploitation


---
><details><summary>❓What user was the server running as?</summary>root</details>
---
<!-- ADD ANSWER -->
><details><summary>❓What is the root user's password hash?</summary></details>
---
><details><summary>❓What is the full path to this file?</summary>/root/.ssh/id_rsa</details>
---

# PIVOTING - What is Pivoting?
# PIVOTING - High-level Overview
# PIVOTING - Enumeration
# PIVOTING - Proxychains and Foxyproxy
# PIVOTING - SSH Tunnelling and Port Forwarding
# PIVOTING - plink.exe
# PIVOTING - Socat
# Pivoting - Chisel
# Pivoting - sshuttle
# Pivoting - Conclusion
# GIT SERVER - Enumeration
# GIT SERVER - Pivoting
# GIT SERVER - Code Review
# GIT SERVER - Exploitation
# GIT SERVER - Stabilisation and Post Exploitation
# COMMAND AND CONTROL - Introduction
# COMMAND AND CONTROL - Empire - Installation
# COMMAND AND CONTROL - Empire - Overview
# COMMAND AND CONTROL - Empire - Listeners
# COMMAND AND CONTROL - Empire - Stagers
# COMMAND AND CONTROL - Empire - Agents
# COMMAND AND CONTROL - Empire - Hop Listeners
# COMMAND AND CONTROL - Git Server
# COMMAND AND CONTROL - Empire - Modules
# COMMAND AND CONTROL - Empire - Interactive Shell
# COMMAND AND CONTROL - Conclusion
# PERSONAL PC - Enumeration
# PERSONAL PC - Pivoting
# PERSONAL PC - The Wonders of Git
# PERSONAL PC - Website Code Analysis
# PERSONAL PC - Exploit PoC
# AV EVASION - Introduction
# AV EVASION - AV Detection Methods
# AV EVASION - PHP Payload Obfuscation
# AV EVASION - Compiling Netcat and Reverse Shell
# AV EVASION - Enumeration
# AV EVASION - Privilege Escalation
# EXFILTRATION - Exfiltration Techniques and Post Exploitation
# CONCLUSION - Debrief and Report
# CONCLUSION - Final Thoughts

&nbsp;

<!-- NO QUESTIONS -->

---
><details><summary>❓</summary></details>
---

&nbsp;
