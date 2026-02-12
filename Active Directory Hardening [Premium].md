🔗 [Link to the Room](https://tryhackme.com/room/activedirectoryhardening)

## 🏷️To learn basic concepts regarding Active Directory attacks and mitigation measures.

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Understanding General Active Directory Concepts


## Domain Controller

<img width="920" height="145" alt="image" src="https://github.com/user-attachments/assets/6404b849-04f0-4399-8e38-161cb7d8dd48" />

## Trees and Forests
<img width="560" height="247" alt="image" src="https://github.com/user-attachments/assets/d8266cfc-eab0-4f52-9508-db2d15c8edb9" />


## Trust in Active Directory 


<img width="504" height="342" alt="image" src="https://github.com/user-attachments/assets/dd8f7f57-9fdc-4997-a914-cbcd11e99682" />




<img width="877" height="396" alt="image" src="https://github.com/user-attachments/assets/ef4edf2a-76e5-4792-9393-9df4b6483b39" />




---
><details><summary>❓What is the root domain in the attached AD machine?</summary>tryhackme.loc</details>
---


# Securing Authentication Methods





## LAN Manager Hash 

The best recommendation is to prevent Windows from storing the password's LM hash. You can access it through the following:

Group Policy Management Editor > Computer Configuration > Policies > Windows Settings > Security Settings > Local Policies > Security Options > double click Network security - Do not store LM hash value on next password change policy > select "Define policy setting" 

<img width="1081" height="575" alt="image" src="https://github.com/user-attachments/assets/b1694ba2-5098-4a98-8292-d966f31c8de7" />


&nbsp;

## SMB Signing 


All supported Windows versions have an SMB packet signing option.
Group Policy Management Editor > Computer Configuration > Policies > Windows Settings > Security Settings > Local Policies > Security Options > double click Microsoft network server: Digitally sign communication (always) > select Enable Digitally Sign Communications

<img width="1085" height="578" alt="image" src="https://github.com/user-attachments/assets/82e744b0-ce2d-432b-a44c-662d11ff7183" />


&nbsp;

## LDAP Signing
- We can enable LDAP signing through the following:
Group Policy Management Editor > Computer Configuration > Policies > Windows Settings > Security Settings > Local Policies > Security Options > Domain controller: LDAP server signing requirements > select Require signing from the dropdown
<img width="1083" height="579" alt="image" src="https://github.com/user-attachments/assets/f3c93f6f-d0a2-489d-8ecc-c24d0efa2808" />


&nbsp;

## Password Rotation 



&nbsp;

### Password Policies

For viewing and configuring the password policy, you can use the following:
Group Policy Management Editor > Computer Configuration > Policies > Windows Settings > Security Settings > Account Policies > Password Policy
<img width="794" height="576" alt="image" src="https://github.com/user-attachments/assets/7858b1e3-a9f3-4c0e-99fc-a23227cdeaaa" />

&nbsp;

### Understanding Password Policy Settings

Enforce password history: Prevent at least 10 to 15 old passwords from being set as new ones. 
Minimum password length: The minimum password length should be set between 10 to 14.
Complexity requirements: Must not contain the name of the user account and ensure the password has uppercase letters, lowercase letters, digits, or special characters.

&nbsp;

---
><details><summary>❓Change the Group Policy Setting in the VM, so it does not store the LAN Manager hash on the next password change.</summary>No answer needed</details>
---
><details><summary>❓What is the default minimum password length (number of characters) in the attached VM?</summary>7</details>
---

&nbsp;

# Implementing Least Privilege Model

<img width="271" height="289" alt="image" src="https://github.com/user-attachments/assets/a682601a-5c92-4fd5-b8f0-376a907981e0" />


## Tiered Access Model 
<img width="334" height="216" alt="image" src="https://github.com/user-attachments/assets/aeb85150-1904-4605-9ba1-aa1201bfbd5e" />


---
><details><summary>❓Computers and Printers must be added to Tier 0 - yea/nay?</summary>nay</details>
---
><details><summary>❓Suppose a vendor arrives at your facility for a 2-week duration task. Being a System Administrator, you should create a high privilege account for him - yea/nay?</summary>nay</details>
---

&nbsp;


# Microsoft Security Compliance Toolkit


## Installing Security Baselines 

Here is how you can download and install the security baselines for Windows Server in a simple way:
Open Microsoft Security Compliance Website > click Download > click Windows Servers Security Baseline.zip > Download
<img width="1210" height="508" alt="image" src="https://github.com/user-attachments/assets/0faa34be-4865-43ad-9440-7a4ad7dd59ab" />

Open extracted folder > Scripts > & select desired baseline & execute with PowerShell
<img width="753" height="488" alt="image" src="https://github.com/user-attachments/assets/ad2efea5-660e-492c-b7c5-a0f5dbb15113" />

&nbsp;

## Policy Analyser 

<img width="1230" height="504" alt="image" src="https://github.com/user-attachments/assets/3a9fe12b-bc99-4a2e-a4f7-a5bd57f903e4" />

<img width="588" height="433" alt="image" src="https://github.com/user-attachments/assets/2105f2bc-95b4-48a7-9d7a-104123c15923" />



&nbsp;

---
><details><summary>❓Find and open BaselineLocalInstall script in PowerShell editor - Can you find the flag?</summary>THM{*****}</details>
---
><details><summary>❓Find and open MergePolicyRule script (Policy Analyser) in PowerShell editor - Can you find the flag?</summary></details>
---

&nbsp;


# Protecting Against Known Attacks


---
><details><summary>❓Does Kerberoasting utilise an offline-attack scheme for cracking encrypted passwords - yea/nay?</summary>yea</details>
---
><details><summary>❓As per the generated report, how many users have the same password as aaron.booth?</summary>186</details>
---

# Windows Active Directory Hardening Cheat Sheet

&nbsp;


<img width="1123" height="794" alt="image" src="https://github.com/user-attachments/assets/59103e54-ab84-45d8-9bcc-c41ecbf90d61" />




<!-- NO QUESTIONS -->

