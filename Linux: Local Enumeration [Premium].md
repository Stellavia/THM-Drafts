🔗 [Link to the Room](https://tryhackme.com/room/lle)

## 🏷️Learn to efficiently enumerate a linux machine and identify possible weaknesses

1. [Unit 1 - tty](#unit-1---tty)<br>
2. [Unit 1 - ssh](#unit-1---ssh)<br>
3. [Unit 2 - Basic enumeration](#unit-2---basic-enumeration)<br>
4. [Unit 3 - /etc](#unit-3---etc)<br>
5. [Unit 4 - Find command and interesting files](#unit-4---find-command-and-interesting-files)<br>
6. [Unit 4 - SUID](#unit-4---suid)<br>
7. [BONUS: Port Forwarding](#bonus-port-forwarding)<br>
8. [Unit 5 - Automating scripts](#unit-5---automating-scripts)<br>
9. [Resources and what is next?](#resources-and-what- is-next-?)<br>

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Unit 1 - tty

&nbsp;








&nbsp;

---
><details><summary>❓How would you execute /bin/bash with perl?</summary>perl -e 'exec "/bin/bash";'</details>
---

# Unit 1 - ssh





---
><details><summary>❓Where you can usually find the id_rsa file? (User = user)</summary>/home/user/.ssh/id_rsa</details>
---
><details><summary>❓Is there an id_rsa file on the box? (yay/nay)</summary>nay</details>
---

&nbsp;

# Unit 2 - Basic enumeration

&nbsp;








&nbsp;

---
><details><summary>❓How would you print machine hardware name only?</summary>uname -m</details>
---
><details><summary>❓Where can you find bash history?</summary>~/.bash_history</details>
---
><details><summary>❓What's the flag?</summary>thm{c****_***_******y}</details>
---

&nbsp;

# Unit 3 - /etc

&nbsp;









&nbsp;

---
><details><summary>❓Can you read /etc/passwd on the box? (yay/nay)</summary>yay</details>
---

&nbsp;

# Unit 4 - Find command and interesting files

&nbsp;












&nbsp;

---
><details><summary>❓What's the password you found?</summary>THMSkidyPass</details>
---
><details><summary>❓Did you find a flag?</summary>thm{c***_***e}</details>
---

&nbsp;

# Unit 4 - SUID

&nbsp;










&nbsp;

---
><details><summary>❓Which SUID binary has a way to escalate your privileges on the box?</summary>grep</details>
---
><details><summary>❓What's the payload you can use to read /etc/shadow with this SUID?</summary>grep '' /etc/shadow</details>
---

&nbsp;

# BONUS: Port Forwarding

&nbsp;











&nbsp;

---
><details><summary>❓Try using those commands on your system!</summary>No answer needed</details>
---

&nbsp;

# Unit 5 - Automating scripts

&nbsp;









&nbsp;

---
><details><summary>❓Got it!</summary>No answer needed</details>
---

&nbsp;

# Resources and what is next?

&nbsp;







&nbsp;

---
><details><summary>❓Read the above and consider completing mentioned rooms.</summary>No answer needed</details>
---
&nbsp;



