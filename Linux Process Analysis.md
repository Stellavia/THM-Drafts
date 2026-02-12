🔗 [Link to the Room](https://tryhackme.com/room/linuxprocessanalysis)

## 🏷️Perform thorough process and application analysis to identify an attacker's persistence methods.


&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Investigation Setup

&nbsp;









&nbsp;

---
><details><summary>❓After updating the PATH and LD_LIBRARY_PATH environment variables, run the command check-env. What is the flag that is returned in the output?</summary>THM{**************}</details>
---

&nbsp;

# Processes

&nbsp;










&nbsp;

---
><details><summary>❓WHich command lists all open files and the processes that opened them?</summary>lsof</details>
---
><details><summary>❓Use pstree to list out the process hierarchies. What is the name of the nc processes parent?</summary>abzkd83o4jakxld</details>
---

&nbsp;

# Cronjobs

&nbsp;













&nbsp;

---
><details><summary>❓Search around the system for suspicious system-level cronjob entries. What is the full URL of the C2 server?</summary>http://c2.intelligent-software.thm:8310/beacon</details>
---
><details><summary>❓List the user-level cronjobs in the system. What is the hidden flag in one of the scripts?</summary>THM{****************}</details>
---
><details><summary>❓Use pspy64 to monitor executions occurring through the system. What is the decoded flag value that is echoed every 15 secons?</summary>THM{****************}</details>
---

&nbsp;

# Services

&nbsp;







&nbsp;

---
><details><summary>❓List all running services on the system. What is the flag you discover in the backdoor service's description?</summary>THM{***************}</details>
---
><details><summary>❓View the journalctl logs associated with the backdoor service. What is the flag you discover?</summary>THM{****************}</details>
---

&nbsp;

# Autostart Scripts

&nbsp;







&nbsp;

---
><details><summary>❓What is the full URL that receives Janice's private SSH key on system startup?</summary>http://aabab.best-it-services.thm/id_rsa</details>
---
><details><summary>❓Identify and investigate the remaining .desktop files on the system. What is the command that executes with the Show Network Interfaces autostart script?</summary>ifconfig</details>
---

&nbsp;

# Application Artefacts

&nbsp;







&nbsp;

---
><details><summary>❓Analyse Janice's .viminfo log. What flag do you find within the Vim search history?</summary>THM{****************}</details>
---
><details><summary>❓Use DumpZilla to investigate Eduardo's Firefox bookmarks. What flag do you find in one of the entries?</summary>THM{**************************}</details>
---

**<!-- CONCLUSION -->**




