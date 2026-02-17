🔗 [Link to the Room](https://tryhackme.com/room/linuxforensics)

## 🏷️Learn about the common forensic artifacts found in the file system of Linux Operating System

1. [OS and account information](#os-and-account-information)<br>
2. [System Configuration](#system-configuration)<br>
  2.1 [Hostname](#hostname)<br>
  2.2 [Timezone](#timezone)<br>
  2.3 [Network Configuration](#network-configuration)<br>
  2.4 [Active network connections](#active-network-connections)<br>
  2.5 [Running processes](#running-processes)<br>
  2.6 [DNS information](#dns-information)<br>
3. [Persistence mechanisms](#persistence-mechanisms)<br>
  3.1 [Cron jobs](#cron-jobs)<br>
  3.2 [Service startup](#service-startup)<br>
  3.3 [.Bashrc](#bashrc)<br>
4. [Evidence of Execution](#evidence-of-execution)<br>
  4.1 [Sudo execution history](#sudo-execution-history)<br>
  4.2 [Bash history](#bash-history)<br>
  4.3 [File accessed using vim](#file-accessed-using-vim)<br>
5. [Log files](#log-files)<br>
  5.1 [Syslog](#syslog)<br>
  5.2 [Auth logs](#auth-logs)<br>
  5.3 [Third-party logs](#third---party-logs)<br>


&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# OS and account information

&nbsp;













&nbsp;

---
><details><summary>❓Which two users are the members of the group audio? Format user1,user2</summary>ubuntu,pulse</details>
---
><details><summary>❓In the attached VM, there is a user account named tryhackme. What is the uid of this account?</summary>1001</details>
---
><details><summary>❓A session was started on this machine on Sat Apr 16 20:10. How long did this session last?</summary>01:32</details>
---

&nbsp;

# System Configuration

&nbsp;






&nbsp;

## Hostname

&nbsp;








&nbsp;

## Timezone

&nbsp;










&nbsp;

## Network Configuration

&nbsp;








&nbsp;

## Active network connections

&nbsp;







&nbsp;

## Running processes

&nbsp;







&nbsp;

## DNS information

&nbsp;







&nbsp;

---
><details><summary>❓What is the hostname of the attached VM?</summary>Linux4n6</details>
---
><details><summary>❓What is the timezone of the attached VM?</summary>Asia/Karachi</details>
---
><details><summary>❓What program is listeninig on the address 127.0.01:5901?</summary>Xtigervnc</details>
---
><details><summary>❓What is the full path of this program?</summary>/usr/bin/Xtigervnc</details>
---
><details><summary>❓Read about the flags used above with the netstat and ps commands in their respective man pages.</summary>No answer needed</details>
---

&nbsp;

# Persistence mechanisms

&nbsp;











&nbsp;

## Cron jobs

&nbsp;










&nbsp;

## Service startup

&nbsp;








&nbsp;

## .Bashrc

&nbsp;








&nbsp;

---
><details><summary>❓In the bashrc file, the size of the history file is defined. What is the size of the history file that is set for the user Ubuntu in the attached machine?</summary2000</details>
---

&nbsp;

# Evidence of Execution

&nbsp;











&nbsp;

## Sudo execution history

&nbsp;









&nbsp;

## Bash history

&nbsp;








&nbsp;

## File accessed using vim

&nbsp;












&nbsp;

---
><details><summary>❓The user tryhackme used apt-get to install a package. What was the command that was issued?</summary>sudo apt-get install apache2</details>
---
><details><summary>❓What was the current working directory when the command to install net-tools was issued?</summary>/home/ubuntu</details>
---

&nbsp;

# Log files

&nbsp;






&nbsp;

## Syslog

&nbsp;






&nbsp;

## Auth logs

&nbsp;





&nbsp;

## Third-party logs

&nbsp;








&nbsp;

---
><details><summary>❓Though the machine's current hostname is the one we identified in Task 4. The machine earlier had a different hostname. What was the previous hostname of the machine?</summary>tryhackme</details>
---

&nbsp;

<!-- CONCLUSION -->

&nbsp;
