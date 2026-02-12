🔗 [Link to the Room](https://tryhackme.com/room/csp)

## 🏷️

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

# Introduction

&nbsp;






---
><details><summary>❓What does CSP stand for?</summary>Content Security Policy</details>
---
><details><summary>❓Content Security Policy</summary>XSS</details>
---
><details><summary>❓In which part of the HTTP response does the server usually send the policy to the client?</summary>header</details>
---

&nbsp;

# Directives

&nbsp;






&nbsp;

---
><details><summary>❓Which directive can we use to restrict the loading of scripts on our website?</summary>script-src</details>
---
><details><summary>❓Which directive can we use to restrict the loading of videos on our website?</summary>media-src</details>
---
><details><summary>❓If we want to log CSP violations, which directive do we need to set to have the browser report violations to us?</summary>report-uri</details>
---

&nbsp;

# Sources

&nbsp;









&nbsp;

---
><details><summary>❓If we want to allow script execution via functions such as eval() from already trusted scripts, what source should we allow in our script-src directive?</summary>'unsafe-eval'</details>
---
><details><summary>❓What directive-source combination should we add to our policy if we want to specifically block all JavaScript content from running on our website?</summary>script-src 'none'</details>
---

&nbsp;

# Creating a Content Security Policy

&nbsp;








&nbsp;

---
><details><summary>❓What hashing algorithm can you use to verify the scripts being loaded? (Without the numbers)</summary>SHA</details>
---
><details><summary>❓Can you include the URLs of the permitted scripts directly in your security policy? (Yes / No)</summary>Yes</details>
---

&nbsp;

# Bypassing a Content Security Policy

&nbsp;









&nbsp;

---
><details><summary>❓If Ajax/XHR requests are blocked, can we still exfiltrate sensitive information? (Yes / No)</summary>Yes</details>
---

&nbsp;

# CSP Sandbox

&nbsp;

Deploy CSP Sandbox machine.

&nbsp;

# CSP Sandbox :: Attack challenges

&nbsp;





&nbsp;

# CSP Sandbox :: Defent challenges

&nbsp;

<!-- NO QUESTIONS -->


&nbsp;
