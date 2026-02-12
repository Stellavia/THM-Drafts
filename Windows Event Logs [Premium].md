🔗 [Link to the Room](https://tryhackme.com/room/windowseventlogs)

## 🏷️Introduction to Windows Event Logs and the tools to query them.


&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# What are Event Logs?






<!-- NO QUESTIONS -->




&nbsp;

# Event Viewer






&nbsp;

---
><details><summary>❓For the questions below, use Event Viewer to analyze Microsoft-WIndows-PowerShell/Operational log.</summary>No answer needed</details>
---
><details><summary>❓What is the Event ID for the earliest recorded event? (Exclude the warning event)</summary>4103</details>
---
><details><summary>❓Filter on Event ID 4104. What was the 2nd command executed in the PowerShell session?</summary>whoami</details>
---
><details><summary>❓What is the Task Category for Event ID 4104?</summary>Execute a Remote Command</details>
---
><details><summary>❓Analyze the Windows PowerShell log. What is the  Task Category for Event ID 800?</summary>Pipeline Execution Details</details>
---

&nbsp;

# wevtutil.exe








&nbsp;


---
><details><summary>❓How many log names are in the machine?</summary>1071</details>
---
><details><summary>❓What event files would be read when using the query-events command?</summary>event log, log file, structured query</details>
---
><details><summary>❓What option would you use to provide a path to a log file?</summary>/lf:true</details>
---
><details><summary>❓What is the VALUE for /q?</summary>Xpath query</details>
---
><details><summary>❓The questions below are based on this command: wevtutil qe Application /c:3 /rd:true /f:text</summary>No answer needed</details>
---
><details><summary>❓What is the log name?</summary>Application</details>
---
><details><summary>❓What is the /rd option for?</summary>Event read direction</details>
---
><details><summary>❓What is the /c option for?</summary>Maximum number of events to read</details>
---

&nbsp;

# Get-WinEvent







&nbsp;

---
><details><summary>❓Answer the following questions using the online help documentation for Get-WinEvent</summary>No answer needed</details>
---
><details><summary>❓Execute the command from Example 1 (as is). What are the names of the logs related to OpenSSH?</summary>OpenSSH/Admin,OpenSSH/Operational</details>
---
><details><summary>❓Execute the command from Example 8. Instead of the string *Policy* search for *PowerShell*. What is the name of the 3rd log provider?</summary>Microsoft-Windows-PowerShell-DesiredStateConfiguration-FileDownloadManager</details>
---
><details><summary>❓Execute the command from Example 9. Use Microsoft-Windows-PowerShell as the log provider. How many event ids are displayed for this event provider?</summary>192</details>
---
><details><summary>❓How do you specify the number of events to display?</summary>-MaxEvents</details>
---
><details><summary>❓When using the FilterHashtable parameter and filtering by level, what is the value for Informational?</summary>4</details>
---

&nbsp;

# XPath Queries







&nbsp;

---
**<!-- ADD ANSWER -->**
><details><summary>❓Using the knowledge gained on Get-WinEvent and XPath, what is the query to find WLMS events with a System Time of 2020-12-15T01:09:08.940277500Z?</summary></details>
---
**<!-- ADD ANSWER -->**
><details><summary>❓Using Get-WinEvent and XPath, what is the query to find a user named Sam with an Logon Event ID of 4720?</summary></details>
---
><details><summary>❓Based on the previous query, how many results are returned?</summary>2</details>
---
><details><summary>❓Based on the output from the question #2, what is Message?</summary>A user account was created</details>
---
><details><summary>❓Still working with Sam as the user, what time was Event ID 4724 recorded? (MM/DD/YYYY H:MM:SS [AM/PM])</summary>12/17/2020 1:57:14 PM</details>
---
><details><summary>❓What is the Provider Name?</summary>Microsoft-Windows-Security-Auditing</details>
---

&nbsp;

# Event IDs







&nbsp;

<!-- NO QUESTIONS -->

# Putting theory into practice









&nbsp;

---
><details><summary>❓What event ID is to detect a PowerShell downgrade attack?</summary>400</details>
---
><details><summary>❓What is the Date and Time this attack took place? (MM/DD/YYYY H:MM:SS [AM/PM])</summary>12/18/2020 7:50:33 AM</details>
---
><details><summary>❓A Log clear event was recorded. What is the 'Event Record ID'?</summary>27736</details>
---
><details><summary>❓What is the name of the computer?</summary>PC01.example.corp</details>
---
><details><summary>❓What is the name of the first variable within the PowerShell command?</summary>$Va5w3n8</details>
---
><details><summary>❓What is the Date and Time this attack took place? (MM/DD/YYYY H:MM:SS [AM/PM])</summary>8/25/2020 10:09:28 PM</details>
---
><details><summary>❓What is the Execution Process ID?</summary>6620</details>
---
><details><summary>❓What is the Group Security ID of the group she enumerated?</summary>S-1-5-32-544</details>
---
><details><summary>❓What is the event ID?</summary>4799</details>
---

&nbsp;

<!-- NIECO DO CONCLUSiON NAPIS TIEZ -->


