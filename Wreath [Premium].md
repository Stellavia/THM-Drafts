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
  12.1 [Reverse Shell Relay](#reverse-shell-relay)<br>
  12.2 [Port Forwarding - Easy](#port-forwarding---easy)<br>
  12.3 [Port Forwarding - Quiet](#port-forwarding---quiet)<br>
14. [Pivoting - Chisel](#pivoting---chisel)<br>
  14.1 [Reverse SOCKS Proxy](#reverse-socks-proxy)<br>
  14.2 [Forward SOCKS Proxy](#forward-socks-proxy)<br>
  14.3 [Remote Port Forward](#remote-port-forward)<br>
15. [Pivoting - sshuttle](#pivoting---sshuttle)<br>
16. [Pivoting - Conclusion](#pivoting---conclusion)<br>
17. [GIT SERVER - Enumeration](#git-server---enumeration)<br>
18. [GIT SERVER - Pivoting](#git-server---pivoting)<br>
19. [GIT SERVER - Code Review](#git-server---code-review)<br>
20. [GIT SERVER - Exploitation](#git-server---exploitation)<br>
  20.1 [With cURL](#with-curl)<br>
  20.2 [With BurpSuite](#with-burpsuite)<br>
21. [GIT SERVER - Stabilisation and Post Exploitation](#git-server---stabilisation-and-post-exploitation)<br>
22. [COMMAND AND CONTROL - Introduction](#command-and-control---introduction)<br>
23. [COMMAND AND CONTROL - Empire - Installation](#command-and-control---empire---installation)<br>
24. [COMMAND AND CONTROL - Empire - Overview](#command-and-control---empire---overview)<br>
25. [COMMAND AND CONTROL - Empire - Listeners](#command-and-control---empire---listeners)<br>
26. [COMMAND AND CONTROL - Empire - Stagers](#command-and-control---empire---stagers)<br>
27. [COMMAND AND CONTROL - Empire - Agents](#command-and-control---empire---agents)<br>
28. [COMMAND AND CONTROL - Empire - Hop Listeners](#command-and-control---empire---hop-listeners)<br>
29. [COMMAND AND CONTROL - Git Server](#command-and-control---git-server)<br>
30. [COMMAND AND CONTROL - Empire - Modules](#command-and-control---empire---modules)<br>
31. [COMMAND AND CONTROL - Empire - Interative Shell](#command-and-control---empire---interactive-shell)<br>
32. [COMMAND AND CONTROL - Conclusion](#command-and-control---conclusion)<br>
33. [PERSONAL PC - Enumeration](#personal-pc---enumeration)<br>
  33.1 [How do Empire Modules work?](#how-do-empire-modules-work)<br>
  33.2 [Upload/Download](#upload-download)<br>
  33.3 [Local Scripts](#local-scripts)<br>
34. [PERSONAL PC - Pivoting](#personal-pc---pivoting)<br>
35. [PERSONAL PC - The Wonders of Git](#personal-pc---the-wonders-of-git)<br>
36. [PERSONAL PC - Website Code Analysis](#personal-pc---website-code-analysis)<br>
37. [PERSONAL PC - Exploit PoC](#personal-pc---exploit-poc)<br>
38. [AV EVASION - Introduction](#av-evasion---introduction)<br>
39. [AV EVASION - AV Detection Methods](#av-evasion---av-detection-methods)<br>
40. [AV EVASION - PHP Payload Obfuscation](#av-evasion---php-payload-obfuscation)<br>
41. [AV EVASION - Compiling Netcat and Reverse Shell](#av-evasion---compiling-netcat-and-reverse-shell)<br>
42. [AV EVASION - Enumeration](#av-evasion---enumeration)<br>
43. [AV EVASION - Privilege Escalation](#av-evasion---privilege-escalation)<br>
44. [EXFILTRATION - Exfiltration Techniques](#exfiltration---exfiltration-techniques)<br>
45. [CONCLUSION - Debrief and Report](#conclusion---debrief-and-report)<br>
46. [CONCLUSION - Final Thoughts](#conclusion---final-thoughts)<br>




<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/1fa7a328-269b-4c53-bd58-ce0fcd20008f" />

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# INTRO - Accessing the Network

&nbsp;








<!-- NO QUESTIONS -->

&nbsp;

# INTRO - Backstory

&nbsp;









<!-- NO QUESTIONS -->

&nbsp;

# INTRO - Brief

&nbsp;








<!-- NO QUESTIONS -->

&nbsp;

# WEBSERVER - Enumeration

&nbsp;










&nbsp;

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

&nbsp;

# WEBSERVER - Exploitation

&nbsp;










<!-- NO QUESTIONS -->

&nbsp;

---
><details><summary>❓What user was the server running as?</summary>root</details>
---
<!-- ADD ANSWER -->
><details><summary>❓What is the root user's password hash?</summary></details>
---
><details><summary>❓What is the full path to this file?</summary>/root/.ssh/id_rsa</details>
---

&nbsp;

# PIVOTING - What is Pivoting?

&nbsp;










<!-- NO QUESTIONS -->

&nbsp;

# PIVOTING - High-level Overview

&nbsp;








&nbsp;

---
><details><summary>❓Which type of pivoting creates a channel through which information can be sent hidden inside another protocol?</summary>Tunnelling</details>
---
><details><summary>❓Research: Not covered in this Network, but good to know about. Which Metasploit Framework Meterpreter command can be used to create a port forward?</summary>portfwd</details>
---

&nbsp;

# PIVOTING - Enumeration

&nbsp;










&nbsp;

---
><details><summary>❓What is the absolute path to the file containing DNS entries on Linux?</summary>/etc/resolv.conf</details>
---
><details><summary>❓What is the absolute path to the hosts file on Windows?</summary>C:\Windows\System32\drivers\etc\hosts</details>
---
><details><summary>❓How could you see which IP addresses are active and allow ICMP echo requests on the 172.16.0.x/24 network using Bash?</summary>for i in {1..255}; do (ping -c 1 172.16.0.${i} | grep "bytes from" &; done)</details>
---

&nbsp;

# PIVOTING - Proxychains and Foxyproxy

&nbsp;








---
><details><summary>❓What line would you put in your proxychains config file to redirect through a socks4 proxy on 127.0.0.1:4242?</summary>socks4 127.0.0.1 4242</details>
---
><details><summary>❓What command would you use to telnet through a proxy to 172.16.0.100:23?</summary>proxychains telnet 172.16.0.100 23</details>
---
><details><summary>❓You have discovered a webapp running on a target inside an isolated network. Which tool is more apt for proxying to a webapp: Proxychains (PC) or FoxyProxy (FP)?</summary>FP</details>
---

&nbsp;

# PIVOTING - SSH Tunnelling and Port Forwarding

&nbsp;





---
><details><summary>❓If you're connecting to an SSH server from your attacking machine to create a port forward, would this be a local (L) port forward or a remote (R) port forward?</summary>L</details>
---
><details><summary>❓Which switch combination can be used to background an SSH port forward or tunnel?</summary>-fN</details>
---
><details><summary>❓It's a good idea to enter our own password on the remote machine to set up a reverse proxy, Aye or Nay?</summary>Nay</details>
---
><details><summary>❓What command would you use to create a pair of throwaway SSH keys for a reverse connection?</summary>ssh-keygen</details>
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details>
---
><details><summary>❓What command would you use to set up a forward proxy on port 8000 to user@target.thm, backgrounding the shell?</summary>ssh -D 8000 user@target.thm -fN</details>
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details>
---

&nbsp;

# PIVOTING - plink.exe

&nbsp;




---
><details><summary>❓What tool can be used to convert OpenSSH keys into PuTTY style keys?</summary>puttygen</details>
---

&nbsp;

# PIVOTING - Socat

&nbsp;



## Reverse Shell Relay


## Port Forwarding - Easy


## Port Forwarding - Quiet


---
><details><summary>❓Which socat option allows you to reuse the same listening port for more than one connection?</summary>reuseaddr</details>
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details
---

&nbsp;

# Pivoting - Chisel

&nbsp;

## Reverse SOCKS Proxy
## Forward SOCKS Proxy
## Remote Port Forward


---
><details><summary>❓What command would you use to start a chisel server for a reverse connection on your attacking machine? Use port 4242 for the listener and do not background the process.</summary>./chisel server -p 4242 --reverse</details>
---
><details><summary>❓What command would you use to connect back to this server with a SOCKS proxy from a compromised host, assuming your own IP is 172.16.0.200 and backgrounding the process?</summary>./chisel client 172.16.0.200:4242 R:socks &</details>
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details>
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details>
---


&nbsp;

# Pivoting - sshuttle

&nbsp;






---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details>
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details>
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details>
---

&nbsp;

# Pivoting - Conclusion

&nbsp;













&nbsp;

# GIT SERVER - Enumeration

&nbsp;






---
><details><summary>❓Excluding the out of scope hosts, and t he current host (.200), how many hosts were discovered active on the network?</summary>2</details>
---
><details><summary>❓In ascending order, what are the last octets of these host IPv4 addresses? (e.g. if the address was 172.16.0.80, submit the 80)</summary>100,150</details>
---
><details><summary>❓Scan the hosts -- which one does not return a status of "filtered" for every port (submit the last octed only)?</summary>150</details>
---
><details><summary>❓Let's assume that the other host is inaccessible from our current position in the network. Which TCP ports (in ascending order, comma separated) below port 15000, are open on the remaining target?</summary>80,3389,5985</details>
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details>
---

&nbsp;

# GIT SERVER - Pivoting

&nbsp;




---
><details><summary>❓What is the name of the program running the service?</summary>Gitstack</details>
---
><details><summary>❓Do these default credentials work (Aye/Nay)?</summary>Nay</details>
---
<!-- ADD THIS QUESTION AND ANSWER -->
><details><summary>❓</summary></details>
---

&nbsp;

# GIT SERVER - Code Review

&nbsp;





---
><details><summary>❓Look at the information at the top of the script. On what date was this exploit written?</summary>18.01.2018</details>
---
<!-- ADD TEXT -->
><details><summary>❓Bearing this in mind, is the script written in Python2 or Python3?</summary>Python2</details>
---
><details><summary>❓Just to confirm that you have been paying attention to the script: What is the name of the cookie set in the POST request made on line 74 (line 73 if you didn't add the shebang) of the exploit?</summary>csrftoken</details>
---

&nbsp;

# GIT SERVER - Exploitation

&nbsp;

## With cURL
## With BurpSuite


---
><details><summary>❓First up, let's use some basic enumeration to get to grips with the webshell: What is the hostname for this target?</summary>git-serv</details>
---
><details><summary>❓What operating system is this target?</summary>Windows</details>
---
><details><summary>❓What user is the server running as?</summary>NT AUTHORITY\SYSTEM</details>
---
<!-- ADD LONG TEXT -->
><details><summary>❓How many make it to the waiting listener?</summary>0</details>
---
<!-- ADD LONG  TEXT -->
---







&nbsp;

# GIT SERVER - Stabilisation and Post Exploitation

&nbsp;




---
<!-- ADD HASH -->
><details><summary>❓What is the Administrator password hash?</summary></details>
---
<!-- ADD HASH -->
><details><summary>❓What is the NTLM password hash for the user "Thomas"?</summary></details>
---
><details><summary>❓What is Thomas' password?</summary>i<3ruby</details>
---

&nbsp;

# COMMAND AND CONTROL - Introduction

&nbsp;





<!-- NO QUESTIONS -->

&nbsp;

# COMMAND AND CONTROL - Empire - Installation

&nbsp;






<!-- NO QUESTIONS -->

&nbsp;

# COMMAND AND CONTROL - Empire - Overview

&nbsp;







---
><details><summary>❓Can we get an agent back from the git server directly (Aye/Nay)?</summary>Nay</details>
---

&nbsp;

# COMMAND AND CONTROL - Empire - Listeners

&nbsp;





<!-- NO QUESTIONS -->

&nbsp;

# COMMAND AND CONTROL - Empire - Stagers

&nbsp;





<!-- NO QUESTIONS -->

&nbsp;

# COMMAND AND CONTROL - Empire - Agents

&nbsp;




---
><details><summary>❓Using the help command for guidance: in Empire CLI, how would we run the whoami command inside an agent?</summary>shell whoami</details>
---

&nbsp;

# COMMAND AND CONTROL - Empire - Hop Listeners

&nbsp;






<!-- NO QUESTIONS -->

&nbsp;

# COMMAND AND CONTROL - Git Server

&nbsp;






<!-- NO QUESTIONS -->

&nbsp;

# COMMAND AND CONTROL - Empire - Modules

&nbsp;







<!-- NO QUESTIONS -->

&nbsp;

# COMMAND AND CONTROL - Empire - Interactive Shell

&nbsp;









<!-- NO QUESTIONS -->

&nbsp;

# COMMAND AND CONTROL - Conclusion

&nbsp;






<!-- NO QUESTIONS -->

&nbsp;

# PERSONAL PC - Enumeration

&nbsp;



## How do Empire Modules work?
## Upload/Download
## Local Scripts




---
><details><summary>❓Scan the top 50 ports of the last IP address you found in Task 17. Which ports are open (lowest to highest, separated by commas)?</summary>80,3389</details>
---

&nbsp;

# PERSONAL PC - Pivoting

&nbsp;






---
<!-- ADD LONG TEXT -->
><details><summary>❓</summary>PHP 7.4.11</details>
---

&nbsp;

# PERSONAL PC - The Wonders of Git

&nbsp;




---
><details><summary>❓Use your WinRM access to look around the Git Server. What is the absolute path to the Website.git directory?</summary>C:\Gitstack\Repositories\Website.git</details>
---

<!-- ADD LONG TEXT -->




&nbsp;

# PERSONAL PC - Website Code Analysis

&nbsp;




---
><details><summary>❓Read through the file. What does Thomas have to phone Mrs Walker about?</summary>Neighbourhood Watch Meetings</details>
---

<!-- ADD LONG  TEXT -->

---
><details><summary>❓Aside from the filter, what protection method is likely to be in place to prevent people from accessing this page?</summary>Basic Auth</details>
---

<!-- ADD LONG TEXT -->

---
><details><summary>❓Which extensions are accepted (comma separated, no spaces or quotes)?</summary>jpg,jpeg,png,gif</details>
---

&nbsp;

# PERSONAL PC - Exploit PoC

&nbsp;





<!-- NO QUESTIONS -->


&nbsp;

# AV EVASION - Introduction

&nbsp;











---
><details><summary>❓Which category of evasion covers uploading a file to the storage on the target before executing it?</summary>On-Disk Evasion</details>
---
><details><summary>❓What does AMSI stand for?</summary>Anti-Malware Scan Interface</details>
---
><details><summary>❓Which category of evasion does AMSI affect?</summary>In-Memory Evasion</details>
---

&nbsp;

# AV EVASION - AV Detection Methods

&nbsp;





---
><details><summary>❓What other name can be used for Dynamic/Heuristic detection methods?</summary>Behavioural</details>
---
><details><summary>❓If AV software splits a program into small chunks and hashes them, checking the results against a database, is this a static or dynamic analysis method?</summary>Static</details>
---
><details><summary>❓When dynamically analysing a suspicious file using a line-by-line analysis of the program, what would antivirus software check against to see if the behaviour is malicious?</summary>Pre-defined rules</details>
---
><details><summary>❓What could be added to a file to ensure that only a user can open it (preventing AV from executing the payload)?</summary>Password</details>
---

&nbsp;

# AV EVASION - PHP Payload Obfuscation

&nbsp;









---
><details><summary>❓What is the Host Name of the target?</summary>WREATH-PC</details>
---
><details><summary>❓What is our current username (include the domain in this)?</summary>wreath-pc\thomas</details>
---

&nbsp;

# AV EVASION - Compiling Netcat and Reverse Shell

&nbsp;









---
><details><summary>❓What output do you get when running the command: certutil.exe ?</summary>CertUtil: -dump command completed successfully.</details>
---

&nbsp;

# AV EVASION - Enumeration

&nbsp;







---
<!-- ADD TEXT -->
><details><summary>❓</summary>SelmpersonatePrivilege</details>
---
><details><summary>❓What is the Name (second column from the left) of this service?</summary>SystemExplorerHelpService</details>
---
><details><summary>❓Is the service running as the local system account (Aye/Nay)?</summary>Aye</details>
---

&nbsp;

# AV EVASION - Privilege Escalation

&nbsp;






<!-- NO QUESTIONS -->

&nbsp;

# EXFILTRATION - Exfiltration Techniques and Post Exploitation

&nbsp;





---
><details><summary>❓Is FTP a good protocol to use when exfiltrating data in a modern network (Aye/Nay)?</summary>Nay</details>
---
><details><summary>❓For what reason is HTTPS preferred over HTTP during exfiltration?</summary>Encryption</details>
---
<!-- LONG TEXT -->
---
><details><summary>❓What is the Administrator NT hash for this target?</summary>a05c3c807ceeb48c47252568da284cd2</details>
---

&nbsp;

# CONCLUSION - Debrief and Report

&nbsp;










<!-- NO QUESTIONS -->

&nbsp;

# CONCLUSION - Final Thoughts

&nbsp;

<!-- NO QUESTIONS -->

---

