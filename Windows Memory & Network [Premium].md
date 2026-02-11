🔗 [Link to the Room](https://tryhackme.com/room/windowsmemoryandnetwork)

## 🏷️ Identify C2 traffic & post-exploit activity in Windows memory. 

# 📚 Study Notes #

&nbsp;

## Introduction

<!-- No Questions -->

## Scenario Information

<!-- No Questions -->

## Environment & Setup

<!-- No Questions -->

## Analyzing Active Connections

---
><details><summary>❓What is the remote source port number used in the connection between 192.168.1.192 and 10.0.0.129:8081?</summary>55985</details>
---
><details><summary>❓Which internal IP address received a connection on port 22 from the compromised host?</summary>192.168.0.30</details>
---
><details><summary>❓What is the exact timestamp when the connection from the IP addresses in question 1 was established?</summary>2025-05-07 07:13:56.000000</details>
---
><details><summary>❓What is the local port used by the system to initiate the SSH connection to 192.168.0.30?</summary>55987</details>
---
><details><summary>❓What is the protocol used in the connection from 192.168.1.192:55985 to 10.0.0.129:8081</summary>TCPv4</details>
---
><details><summary>❓What is the order in which the potential malicious processes established outbound connections?</summary>windows-update.exe, updater.exe, powershell.exe</details>
---

## Investigating Remote Access and C2 Communications 

---
><details><summary>❓What Volatility plugin can be used to correlate memory regions showing suspicious execution permissions with processes, helping to detect Meterpreter-like behavior?</summary>windows.malfind</details>
---
><details><summary>❓What is the virtual memory address space of the suspicious injected region in updater.exe? Answer format: 0xABCDEF</summary>0x1a0000</details>
---
><details><summary>❓What is the first 2-bytes signature found in the shellcode that was extracted from updater.exe using windows.malfind? Answer format: In hex.</summary>4d5a</details>
---

## Post-Exploitation Communication

---
><details><summary>❓Which local port was used by powershell.exe to connect to the internal host 192.168.0.30?</summary>55987</details>
---
><details><summary>❓What was the remote IP address targeted by windows-update.exe during its HTTP POST attempt?</summary>10.0.0.129</details>
---
><details><summary>❓What port was windows-update.exe listening on, based on the netscan output?</summary>4443</details>
---

## Putting it All Together

---
><details><summary>❓What IP did updater.exe connect to for the reverse shell?</summary>10.0.0.129</details>
---
><details><summary>❓Which folder is used for persistence by the attack we analyzed within this memory dump?</summary>C:\\UserszoperatorzAppDatazRoaming\Microsoft\Windows\StartMenu\Programs\Startup\</details>
---
><details><summary>❓Which MITRE technique matches the reflective DDL injection used by updater.exe</summary>T1055.002</details>
---
><details><summary>❓What is the domain that was discovered within the windows-update.exe file?</summary>external-attacker.thm</details>
---
