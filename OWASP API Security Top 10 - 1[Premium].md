🔗 [Link to the Room](https://tryhackme.com/room/owaspapisecuritytop105w)

## 🏷️Learn the basic concepts for secure API development (Part 1).

1. [Understanding APIs - A refresher](#understanding-apis-a-refresher)<br>
  1.1 [What is an API and Why is it important?](#what-is-an-api-and-why-is-it-important)<br>
  1.2 [Recent Data Breaches through APIs](#recent-data-breaches-through-apis)<br>
2. [Vulnerability I - Broken Object Level Authorisation (BOLA)](#vulnerability-i-broken-object-level-authorisation-bola)<br>
  2.1 [How does it Happen?](#how-does-it-happen)<br>
  2.2 [Likely Impact](#likely-impact)<br>
  2.3 [Practical Example](#practical-example)<br>
3. [Vulnerability II - Broken User Authentication (BUA)](#vulnerability-ii-broken-user-authentication-bua)<br>
  3.1 [How does it happen?](#how-does-it-happen)<br>
  3.2 [Likely Impact](#likely-impact)<br>
  3.3 [Practical Example](#practical-example)<br>
  3.4 [Mitigation Measures](#mitigatioon-measures)<br>
4. [Vulnerability III - Excessive Data Exposure](#vulnerability-iii-excessive-data-exposure)<br>
  4.1 [How does it happen?](#how-does-it-happen)<br>
  4.2 [Likely Impact](#likely-impact)<br>
  4.3 [Practical Example](#practical-example)<br>
  4.4 [Mitigation Measures](#mitigation-measures)<br>
5. [Vulnerability IV - Lack of Resources and Rate Limiting](#vulnerability-iv-lack-of-resources-and-rate-limiting)<br>
  5.1 [How does it happen?](#how-does-it-happen)<br>
  5.2 [Likely Impact](#likely-impact)<br>
  5.3 [Practical Example](#practical-example)<br>
  5.4 [Mitigation Measures](#mitigation-measures)<br>
6. [Vulnerability V - Broken Function Level Authorisation](#vulnerability-v-broken-function-level-authorisation)<br>
  6.1 [How does it happen?](#how-does-it-happen)<br>
  6.2 [Likely Impact](#likely-impact)<br>
  6.3 [Practical Example](#practical-example)<br>
  6.4 [Mitigation Measures](#mitigation-measures)<br>


&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Understanding APIs - A refresher


## What is an API and Why is it important?
## Recent Data Breaches through APIs

---
><details><summary>❓In the LinkedIn breach (Jun 2021), how many million records (sample) were posted by a hacker on the dark web?</summary>1</details>
---
><details><summary>❓Is the API documentation a trivial item and not used after API development (yea/nay)?</summary>nay</details>
---
><details><summary>❓I understand the APIs and am ready to learn OWASP Top 10 Principles.</summary>No answer needed</details>
---

# Vulnerability I - Broken Object Level Authorisation (BOLA)


## How does it Happen?
## Likely Impact
## Practical Example

---
><details><summary>❓Suppose the employee ID is an integer with incrementing value. Can you check through the vulnerable API endpoint the total number of employees in the company?</summary>3</details>
---
><details><summary>❓What is the flag associated with employee ID 2?</summary>THM{8*****}</details>
<!-- THM{838123} -->
---
><details><summary>❓What is the username of employee ID 3?</summary>Bob</details>
---

# Vulnerability II - Broken User Authentication (BUA)


## How does it happen?
## Likely Impact
## Practical Example
## Mitigation Measures


---
><details><summary>❓Can you find the token of hr@mht.com?</summary></details>
---
><details><summary>❓To which country does sales@mht.com belong?</summary>China</details>
---
><details><summary>❓Is it a good practice to send a username and password in a GET request (yea/nay)?</summary>nay</details>
---


# Vulnerability III - Excessive Data Exposure


## How does it happen?
## Likely Impact
## Practical Example
## Mitigation Measures

---
><details><summary>❓What is the device ID value for post-ID 2?</summary>iOS15.411</details>
---
><details><summary>❓What is the username value for post-ID 3?</summary>hacker#!</details>
---
><details><summary>❓Should we use network-level devices for controlling excessive data exposure instead of managing it through APIs (programmatically) - (yea/nay)?</summary>nay</details>
---

# Vulnerability IV - Lack of Resources and Rate Limiting


## How does it happen?
## Likely Impact
## Practical Example
## Mitigation Measures


---
><details><summary>❓Can rate limiting be carried out at the network level through firewall etc. (yea/nay)?</summary>yea</details>
---
><details><summary>❓What is the HTTP response code when you send a POST request to /apirule4/sendOTP_s using the email address hr@mht.com?</summary>200</details>
---
><details><summary>❓What is the "msg key" value after an HTTP POST request to /apirule4/sendOTP_s using the email address sale@mht.com?</summary>Invalid Email</details>
---

# Vulnerability V - Broken Function Level Authorisation




## How does it happen?
## Likely Impact
## Practical Example
## Mitigation Measures



&nbsp;


---
><details><summary>❓What is the mobile number for the username Alice?</summary>+1235322323</details>
---
><details><summary>❓Is it a good practice to send isAdmin value throught he hidden fields in form requests - yea/nay?</summary>nay</details>
---
><details><summary>❓What is the address flag of username admin?</summary>THM{3********}</details>
<!-- THM{3432$@#2!} -->
---


&nbsp;


<!-- CONCLUSION HERE -->

