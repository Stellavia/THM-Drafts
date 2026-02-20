🔗 [Link to the Room](https://tryhackme.com/room/advancedsqlinjection)

## 🏷️Learn advanced injection techniques to exploit a web app.

1. [Introduction](#introduction)<br>
2. [Quick Recap](#quick-recap)<br>
  2.2 [In-band SQL Injection](#inband-sql-injection)<br>
  2.3 [Inferential (Blind) SQL Injection](#inferential-blind-sql-injection)<br>
  2.4 [Out-of-band SQL Injection](#outofband-sql-injection)<br>
3. [Second-Order SQL Injection](#secondorder-sql-injection)<br>
  3.1 [Impact](#impact)<br>
4. [Filter Evasion Techniques](#filter-evasion-techniques)<br>
  4.1 [Character Encoding](#character-encoding)<br>
  4.2 [Preparing the Payload](#preparing-the-payload)<br>
5. [Filter Evasion Techinuques (continued)](#filter-evasion-techniques-continued)<br>
  5.1 [No-Quote SQL Injection](#noquote-sql-injection)<br>
  5.2 [No Spaces Allowed](#no-spaces-allowed)<br>
  5.3 [Practical Example](#practical-example)<br>
6. [Out-of-Band SQL Injection](#outofband-sql-injection)<br>
  6.1 [Why Use OOB](#why-use-oob)<br>
  6.2 [Techniques in Different Databases](#techniques-in-different-databases)<br>
  6.4 [Practical Example](#practical-example)<br>
7. [Other Techniques](#other-techniques)<br>
  7.1 [HTTP Header Injection](#http-header-injection)<br>
  7.2 [Exploiting Stored Procedures](#exploiting-stored-procedures)<br>
  7.3 [XML and JSON Injection](#xml-and-json-injection)<br>
8. [Automation](#automation)<br>
  8.1 [Major Issues During Identification](#major-issues-during-identification)<br>
  8.2 [Few Important Tools](#few-important-tools)<br>
9. [Best Practices](#best-practices)<br>
10. [BONUS](#bonus)<br>

&nbsp;

# 📚 Study Notes #

&nbsp;

# Introduction

&nbsp;









&nbsp;

---
><details><summary>❓What is the port on which MySQL service is running?</summary>3306</details>
---

&nbsp;

# Quick Recap

&nbsp;






&nbsp;

## In-band SQL Injection



&nbsp;

## Inferential (Blind) SQL Injection




---
><details><summary>❓What type of SQL injection uses the same communication channel for both the injection and data retrieval?</summary>In-band</details>
---
><details><summary>❓In out-of-band SQL injection, which protocol is usually used to send query results to the attacker’s server?</summary>HTTP</details>
---

&nbsp;


# Out-of-band SQL Injection


&nbsp;










&nbsp;

---
><details><summary>❓What type of SQL injection uses the same communication channel for both the injection and data retrieval?</summary>In-band</details>
---
><details><summary>❓In out-of-band SQL injection, which protocol is usually used to send query results to the attacker’s server?</summary>HTTP</details>
---

&nbsp;

# Second-Order SQL Injection

&nbsp;





&nbsp;

## Impact









&nbsp;

---
><details><summary>❓What is the flag value after updating the title of all books to “compromised”?</summary> THM{S*_H*****}</details>
---
><details><summary>❓What is the flag value once you drop the table hello from the database?</summary>THM{T***e_D*****d}</details>
---

&nbsp;

# Filter Evasion Techniques

&nbsp;








&nbsp;

## Character Encoding




&nbsp;

## Preparing the Payload









&nbsp;

---
><details><summary>❓What is the MySQL error code once an invalid query is entered with bad characters?</summary>1064</details>
---
><details><summary>❓What is the name of the book where book ID=6?</summary>Animal Series</details>
---

&nbsp;

# Filter Evasion Techinuques (continued)

&nbsp;




&nbsp;

## No-Quote SQL Injection





&nbsp;

## No Spaces Allowed




&nbsp;

## Practical Example






&nbsp;

---
><details><summary>❓What is the password for the username “attacker”?</summary>tesla</details>
---
><details><summary>❓Which of the following can be used if the SELECT keyword is banned? Write the correct option only. a) SElect, b) SeLect, c) Both a and b, d) We cannot bypass SELECT keyword filter</summary>c</details>
---

&nbsp;

# Out-of-Band SQL Injection

&nbsp;





&nbsp;

## Why Use OOB




&nbsp;

## Techniques in Different Databases




&nbsp;

## Echamples of Out-of-band Techniques




&nbsp;

## Practical Example







&nbsp;

---
><details><summary>❓What is the output of the @@version on the MySQL server?</summary>10.4.24-MariaDB</details>
---
><details><summary>❓What is the value of @@basedir variable?</summary>C:/xampp/mysql</details>
---

&nbsp;

# Other Techniques

&nbsp;






&nbsp;

## HTTP Header Injection



&nbsp;

## Exploiting Stored Procedures



&nbsp;

## XML and JSON Injection







&nbsp;

---
><details><summary>❓What is the value of the flag field in the books table where book_id =1?</summary>THM{H****}</details>
---
><details><summary>❓What field is detected on the server side when extracting the user agent?</summary>User-Agent</details>
---

&nbsp;

# Automation

&nbsp;






&nbsp;

## Major Issues During Identification





&nbsp;

## Few Important Tools








&nbsp;

---
><details><summary>❓Does the dynamic nature of SQL queries assist a pentester in identifying SQL injection (yea/nay)?</summary>nay</details>
---

&nbsp;

# Best Practices

&nbsp;







&nbsp;

## Secure Coders






&nbsp;

## Pentesters







&nbsp;

---
><details><summary>❓What command does MSSQL support to execute system commands?</summary>xp_cmdshell</details>
---

&nbsp;


# BONUS

&nbsp;

After completing this room you will earn a new badge: **SQL Slayer**

<!-- NO QUESTIONS -->

&nbsp;
