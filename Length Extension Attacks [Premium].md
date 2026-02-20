🔗 [Link to the Room](https://tryhackme.com/room/lengthextensionattacks)

## 🏷️Learn how hash functions enable attackers to extend and manipulate data using length extension attacks.

1. [Hash Functions](#hash-functions)<br>
  1.1 [Key Properties That Make Hash Functions Secure](#key-properties-that-make-hash-function-secure)<br>
  1.2 [Where Are Hash Functions Used?](#where-are-hash-functions-used)<br>
  1.3 [Vulnerabilities in Hash Functions](#vulnerabilities-in-hash-functions)<br>
2. [Hashing Internals](#hashing-internals)<br>
  2.1 [How Hash Functions Process Data](#how-hash-functions-process-data)<br>
  2.2 [Why Padding Matters](#why-padding-matters)<br>
  2.3 [How Hash Functions Use States](#how-hash-functions-use-states)<br>
  2.4 [Breakdown of Popular Hash Functions](#breakdown-of-popular-hash-functions)<br>
  2.5 [MD5](#md5)<br>
  2.6 [SHA-1](#sha-1)<br>
  2.7 [SHA-256](#sha-256)<br>
  2.8 [How Padding and State Manipulation Work](#how-padding-and-state-manupulation-work)<br>
  2.9 [SHA-256 Hashing Process](#sha-256-hashing-process)<br>
3. [Understanding Length Extension Attacks](#understanding-length-extension-attacks)<br>
  3.1 [How does it work?](#how-does-it-work)<br>
  3.2 [Visualizing the Attack](#visualizing-the-attack)<br>
  3.3 [Why does this work?](#why-does-this-work)<br>
  3.4 [Vulnerable Hash Functions](#vulnerable-hash-functions)<br>
4. [Practical - Attacking Signatures](#practical-attacking-signatures)<br>
  4.1 [The Scenario](#the-scenario)<br>
  4.2 [The Vulnerable Code](#the-vulnerable-code)<br>
  4.3 [Objective](#objective)<br>
  4.4 [Using Hash Extender for the attack](#using-hash-extender-for-the-attack)<br>
5. [Practical - Modifying a Signed Cookie](#practical-modifying-a-signed-cookie)<br>
  5.1 [Exploitation](#exploitation)<br>
  5.2 [Modifying the Cookie](#modifying-the-cookie)<br>
6. [Mitigation Techniques](#mitigation-techniques)<br>
  6.1 [Preventing Length Extension Attacks](#preventing-length-extension-attacks)<br>



&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Hash Functions

&nbsp;





&nbsp;

## Key Properties That Make Hash Functions Secure




&nbsp;

## Where Are Hash Functions Used?




&nbsp;

## Vulnerabilities in Hash Functions





&nbsp;

---
><details><summary>❓What property prevents an attacker from reversing a hash to get the original input?</summary>Pre-image Resistance</details>
---
><details><summary>❓What property ensures that no two different messages produce the same hash?</summary>Collision Resistance</details>
---

&nbsp;

# Hashing Internals

&nbsp;



&nbsp;

## How Hash Functions Process Data



&nbsp;

## Why Padding Matters



&nbsp;

## How Hash Functions Use States




&nbsp;

## Breakdown of Popular Hash Functions





&nbsp;

## MD5





&nbsp;

## SHA-1





&nbsp;

## SHA-256




&nbsp;

## How Padding and State Manipulation Work




&nbsp;

## SHA-256 Hashing Process






&nbsp;

---
><details><summary>❓What block size does SHA-256 use?</summary>512</details>
---
><details><summary>❓What function ensures data is aligned to fit block size requirements?</summary>Padding</details>
---
><details><summary>❓How many words does SHA-256's internal state have?</summary>8</details>
---

&nbsp;

# Understanding Length Extension Attacks

&nbsp;






&nbsp;

## How does it work?





&nbsp;

## Visualizing the Attack




&nbsp;

## Why does this work?




&nbsp;

## Vulnerable Hash Functions





&nbsp;

---
><details><summary>❓What hashing method prevents length extension attacks by using a secret key?</summary>HMAC</details>
---

&nbsp;

# Practical - Attacking Signatures

&nbsp;




&nbsp;

## The Scenario





&nbsp;

## The Vulnerable Code



&nbsp;

## Objective




&nbsp;

## Using Hash Extender for the attack





&nbsp;

---
><details><summary>❓</summary>What is the flag in the image?</details>
---

&nbsp;

# Practical - Modifying a Signed Cookie

&nbsp;






&nbsp;

## Exploitation





&nbsp;

## Modifying the Cookie





&nbsp;

---
><details><summary>❓What is the flag?</summary></details>
---

&nbsp;

# Mitigation Techniques

&nbsp;


## Preventing Length Extension Attacks



<!-- NO QUESTIONS -->


&nbsp;
