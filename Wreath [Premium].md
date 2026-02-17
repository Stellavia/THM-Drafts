🔗 [Link to the Room](https://tryhackme.com/room/wreath)

## 🏷️Learn how to pivot through a network by compromising a public facing web machine and tunnelling your traffic to access other machines in Wreath's network.


1. [INTRO - Accessing the Network](#intro---accessing-the-network)<br>
2. [INTRO - Backstory](#intro---backstory)<br>
3. [INTRO - Brief](#intro---brief)<br>
4. [WEBSERVER - Enumeration](#webserver---enumeration)<br>
5. [WEBSERVER - Exploitation](#webserwer---exploitation)<br>
6. [PIVOTING - What is Pivoting?](#pivoting---what-is-pivoting-?)<br>
7. [PIVOTING - High-level Overview](#pivoting---high---level-overview)<br>
8. [PIVOTING - Enumeration](#pivoting---enumeration)<br>
9. [PIVOTING - Proxychains and Foxyproxy](#pivoting---proxychains-and-foxyproxy)<br>
10. [PIVOTING - SSH Tunnelling and Port Forwarding](#pivoting---ssh-tunnelling-and-port-forwarding)<br>
11. [PIVOTING - plink.exe](#pivoting---plinkexe)<br>
12. [PIVOTING - Socat](#pivoting---socat)<br>
13. [Pivoting - Chisel](#pivoting---chisel)<br>
14. [Pivoting - sshuttle](#pivoting---sshuttle)<br>
15. [Pivoting - Conclusion](#)<br>
16. [GIT SERVER - Enumeration](#)<br>
17. [GIT SERVER - Pivoting](#)<br>
18. [GIT SERVER - Code Review](#)<br>
19. [GIT SERVER - Exploitation](#)<br>
20. [GIT SERVER - Stabilisation and Post Exploitation](#)<br>
21. [COMMAND AND CONTROL - Introduction](#)<br>
22. [COMMAND AND CONTROL - Empire - Installation](#)<br>
23. [COMMAND AND CONTROL - Empire - Overview](#)<br>
24. [COMMAND AND CONTROL - Empire - Listeners](#)<br>
25. [COMMAND AND CONTROL - Empire - Stagers](#)<br>
26. [COMMAND AND CONTROL - Empire - Agents](#)<br>
27. [COMMAND AND CONTROL - Empire - Hop Listeners](#)<br>
28. [COMMAND AND CONTROL - Git Server](#)<br>
29. [COMMAND AND CONTROL - Empire - Modules](#)<br>
30. [COMMAND AND CONTROL - Empire - Interative Shell](#)<br>
31. [COMMAND AND CONTROL - Conclusion](#)<br>
32. [PERSONAL PC - Enumeration](#)<br>
33. [PERSONAL PC - Pivoting](#)<br>
34. [PERSONAL PC - The Wonders of Git](#)<br>
35. [PERSONAL PC - Website Code Analysis](#)<br>
36. [PERSONAL PC - Exploit PoC](#)<br>
37. [AV EVASION - Introduction](#)<br>
38. [AV EVASION - AV Detection Methods](#)<br>
39. [AV EVASION - PHP Payload Obfuscation](#)<br>
40. [AV EVASION - Compiling Netcat and Reverse Shell](#)<br>
41. [AV EVASION - Enumeration](#)<br>
42. [AV EVASION - Privilege Escalation](#)<br>
43. [EXFILTRATION - Exfiltration Techniques](#)<br>
44. [CONCLUSION - Debrief and Report](#)<br>
45. [CONCLUSION - Final Thoughts](#)<br>




<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/1fa7a328-269b-4c53-bd58-ce0fcd20008f" />

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# INTRO - Accessing the Network
# INTRO - Backstory
# INTRO - Brief
# WEBSERVER - Enumeration
# WEBSERVER - Exploitation
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
