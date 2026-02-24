
🔗 [Link to the Room](https://tryhackme.com/room/introtosecurityarchitecture)

## 🏷️Learn about and implement security best practices for network environments.

1. [Network Segmentation](#network-segmentation)<br>
  1.1 [The Need for Secure Segmentation](#the-need-for-secure-segmentation)<br>
  1.2 [Tagging Unknown Traffic](#tagging-unknown-traffic)<br>
  1.3 [Routing Between VLANs](#routing-between-vlans)<br>
  1.4 [Analyzing a VLAN Configuration](#analyzing-a-vlan-configuration)<br>
2. [Common Secure Network Architecture](#common-secure-network-architecture)<br>
3. [Network Security Policies and Controls](#network-security-policies-and-controls)<br>
  3.1 [Traffic Filtering](#traffic-filteriing)<br>
  3.2 [Analyzing Packets and ACLs](#analyzing-packets-and-acls)<br>
4. [Zone-Pair Policies and Filtering](#zone-pair-policies-and-filtering)<br>
  4.1 [Firewalls](#firewalls)<br>
  4.2 [Zone-Pairs](#zone-pairs)<br>
  4.3 [Creating a Zone-Pair from Scratch](#creating-a-zone-pair-from-scratch)<br>
5. [Validating Network Traffic](#validating-network-traffic)<br>
  5.1 [SSL/TLS Inspection](#ssl-tls-inspection)<br>
6. [Addressing Common Attacks](#addressing-common-attacks)<br>
  6.1 [DHCP Snooping](#dhcp-snooping)<br>
  6.2 [Dynamic ARP Inspection](#dynamic-arp-inspection)<br>

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Network Segmentation

&nbsp;






&nbsp;

## The Need for Secure Segmentation





&nbsp;

## Tagging Unknown Traffic





&nbsp;

## Routing Between VLANs



&nbsp;

## Analyzing a VLAN Configuration






&nbsp;

---
><details><summary>❓How many trunks are present in this configuration?</summary>4</details>
---
><details><summary>❓What is the VLAN tag ID for interface eth12?</summary>30</details>
---

&nbsp;

# Common Secure Network Architecture

&nbsp;







&nbsp;

---
><details><summary>❓From the above table, what zone would a user connecting to a public web server be in?</summary>External</details>
---
><details><summary>❓From the above table, what zone would a public web server be in?</summary>DMZ</details>
---
><details><summary>❓From the above table, what zone would a core domain controller be placed in?</summary>Restricted</details>
---

&nbsp;

# Network Security Policies and Controls

&nbsp;






&nbsp;

## Traffic Filtering







&nbsp;

## Analyzing Packets and ACLs






&nbsp;

---
><details><summary>❓According to the corresponding ACL policy, will the first packet result in a drop or accept?</summary>accept</details>
---
><details><summary>❓According to the corresponding ACL policy, will the second packet result in a drop or accept?</summary>drop</details>
---

&nbsp;

# Zone-Pair Policies and Filtering

&nbsp;






&nbsp;

## Firewalls




&nbsp;

## Zone-Pairs





&nbsp;

## Creating a Zone-Pair from Scratch






&nbsp;

---
><details><summary>❓What is the flag found after filling in all blanks on the static site?</summary>THM{M*****_5*****}</details>
---

&nbsp;

# Validating Network Traffic

&nbsp;







&nbsp;

## SSL/TLS Inspection






&nbsp;

---
><details><summary>❓Does SSL inspection require a man-in-the-middle proxy? (Y/N)</summary>Y</details>
---
><details><summary>❓What platform processes data sent from an SSL proxy?</summary>Unified Threat Management</details>
---

&nbsp;

# Addressing Common Attacks

&nbsp;







&nbsp;

## DHCP Snooping






&nbsp;

## Dynamic ARP Inspection






&nbsp;

---
><details><summary>❓Where does DHCP snooping store leased IP addresses from untrusted hosts?</summary>DHCP Binding Database</details>
---
><details><summary>❓Will a switch drop or accept a DHCPRELEASE packet?</summary>Drop</details>
---
><details><summary>❓Does dynamic ARP inspection use the DHCP binding database? (Y/N)</summary>Y</details>
---
><details><summary>❓Dynamic ARP inspection will match an IP address and what other packet detail?</summary>MAC Address</details>
---

&nbsp;
