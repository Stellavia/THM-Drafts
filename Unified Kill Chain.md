🔗 [Link to the Room](https://tryhackme.com/room/unifiedkillchain)

## 🏷️The Unified Kill Chain is a framework which establishes the phases of an attack, and a means of identifying and mitigating risk to IT assets.

1. [What is a Kill Chain](#what-is-a-kill-chain)<br>
2. [What is Threat Modelling](#what-is-threat-modelling)<br>
3. [Introducing the Unified Kill Chain](#introducing-the-unified-kill-chain)<br>
4. [Goal: In (Initial Foothold)](#goal-in-initial-foothold)<br>
  4.1 [Reconnaissance (MITRE Tactic TA0043)](#reconnaissance-mitre-tactic-ta0043)<br>
  4.2 [Weaponization (MITRE Tactic TA0001)](#weaponization-mitre-tactic-ta0001)<br>
  4.3 [Social Engineering (MITRE Tactic TA0001)](#social-engineering-mitre-tactic-ta0001)<br>
  4.4 [Exploitation (MITRE Tactic TA0002)](#exploitation-mitre-tactic-ta0002)<br>
  4.5 [Persistence (MITRE Tactic TA0003)](#persistence-mitre-tactic-ta0003)<br>
  4.6 [Defence Evasion (MITRE Tactic TA0005)](#defence-evasion-mitre-tactic-ta0005)<br>
  4.7 [Command and Control (MITRE Tactic TA0011)](#command-and-control-mitre-tactic-ta0011)<br>
   4.8 [Pivoting (MITRE Tactic TA0008)](#pivoting-mitre-tactic-ta0008)<br>
5. [Goal: Through (Network Propagation)](#goal-through-network-propagation)<br>
  5.1 [Pivoting (MITRE Tactic TA0008)](#pivoting-mitre-tactic-ta0008)<br>
  5.2 [Discovery (MITRE Tactic TA0007)](#discovery-mitre-tactic-ta0007)<br>
  5.3 [Privilege Escalation (MITRE Tactic TA0004)](#privilege-escalation-mitre-tactic-ta0004)<br>
  5.4 [Execution Access (MITRE Tactic TA0006)](#execution-access-mitre-tactic-ta0006)<br>
  5.5 [Lateral Movement (MITRE Tactic TA0008)](#lateral-movement-mitre-tactic-ta0008)<br>
6. [Goal: Out (Action on Objectives)](#goal-out-action-on-objectives)<br>
  6.1 [Exfiltration (MITRE Tactic TA0010)](#exfiltration-mitre-tactic-ta0010)<br>
  6.2 [Impact (MITRE Tactic TA0040)](#impact-mitre-tactic-ta0040)<br>
  6.3 [Objectives](#objectives)<br>
7. [Practical](#practical)<br>

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# What is a Kill Chain

&nbsp;








&nbsp;

---
><details><summary>❓Where does the term "Kill Chain" originate from?</summary>Military</details>
---

&nbsp;

# What is Threat Modelling

&nbsp;









&nbsp;

---
><details><summary>❓What is the technical term for a piece of software or hardware in IT (Information Technology)</summary>Asset</details>
---

&nbsp;

# Introducing the Unified Kill Chain

&nbsp;










&nbsp;

---
><details><summary>❓In what year was the Unified Kill Chain framework released?</summary>2017</details>
---
><details><summary>❓According to the Unified Kill Chail, how many phases are there to an attack?</summary>18</details>
---
><details><summary>❓What is the name of the attack phase where attacker employs techniques to evade detection?</summary>Defense Evasion</details>
---
><details><summary>❓What is the name of the attack phase where an attacker employs techniques to remove data from a network?</summary>Exfiltration</details>
---
><details><summary>❓What is the name of the attack phase where an attacker achieves their objectives?</summary>Objectives</details>
---

&nbsp;

# Goal: In (Initial Foothold)

&nbsp;




&nbsp;

## Reconnaissance (MITRE Tactic TA0043)





&nbsp;

## Weaponization (MITRE Tactic TA0001)






&nbsp;

## Social Engineering (MITRE Tactic TA0001)






&nbsp;

## Exploitation (MITRE Tactic TA0002)









&nbsp;

## Persistence (MITRE Tactic TA0003)





&nbsp;

## Defence Evasion (MITRE Tactic TA0005)





&nbsp;

## Command and Control (MITRE Tactic TA0011)





&nbsp;

## Pivoting (MITRE Tactic TA0008)







&nbsp;

---
><details><summary>❓What is an example of a tactic to gain a foothold using emails?</summary>Phishing</details>
---
><details><summary>❓Impersonating an employee to request a password reset is a form of what?</summary>Social Engineering</details>
---
><details><summary>❓An adversary setting up the Command & Control server is what phase of the Unified Kill Chain?</summary>Weaponization</details>
---
><details><summary>❓Exploiting a vulnerability present on a system is what phase of the Unified Kill Chain?</summary>Exploitation</details>
---
><details><summary>❓Moving from one system to another is an example of?</summary>Pivoting</details>
---
><details><summary>❓Leaving behind a malicious service that allows the adversary to log back into the target is what?</summary>Persistence</details>
---

&nbsp;

# Goal: Through (Network Propagation)

&nbsp;






&nbsp;

## Pivoting (MITRE Tactic TA0008)




&nbsp;

## Discovery (MITRE Tactic TA0007)







&nbsp;

## Privilege Escalation (MITRE Tactic TA0004)





&nbsp;

## Execution Access (MITRE Tactic TA0006)





&nbsp;

## Lateral Movement (MITRE Tactic TA0008)








&nbsp;

---
><details><summary>❓As a SOC analyst, you pick up an alert pointing to failed logins from an administrator account. What phase of the Unified Kill Chain would an attacker be seeking to achieve?</summary>Privilege Escalation</details>
---
><details><summary>❓Mimikatz, a known post-exploitation tool, was detected on the IT Manager's workstation. The Security logs show that the tool was attempting to dump OS and user secrets. Which Unified Kill Chain phase does this activity correspond to?</summary>Credential Access</details>
---

&nbsp;

# Goal: Out (Action on Objectives)

&nbsp;






&nbsp;

## Exfiltration (MITRE Tactic TA0010)






&nbsp;

## Impact (MITRE Tactic TA0040)





&nbsp;

## Objectives







&nbsp;

---
><details><summary>❓While monitoring the network as a SOC analyst, you observe a big traffic spike. Most of the network traffic is sent to an unknown, suspicious IP address. What Unified Kill Chain phase could describe this activity?</summary>Exfiltration</details>
---
><details><summary>❓Personally identifiable information (PII) has been released to the public by an adversary. Your organisation is facing reputational losses and scrutiny for the breach. What part of the CIA triad would be affected by this action?</summary>Confidentiality</details>
---

&nbsp;

# Practical

&nbsp;








&nbsp;

---
><details><summary>❓Match the scenario prompt to the correct phase of the Unified Kill Chain to reveal the flag at the end. What is the flag?</summary>THM{U**_S******O}</details>
<!-- THM{UKC_SCENARIO} -->
---

&nbsp;

<!-- CONCLUSION HERE -->

The UKC is a modern extension of other frameworks, such as Lockhead Martin's "Cyber Kill Chain" framework

There are other rooms on TryHackMe where you can learn about frameworks in cybersecurity such as Principles of Security, Pentesting Fundamentals or Cyber Kill Chain.
You should check them out ;)

&nbsp;

&nbsp;
