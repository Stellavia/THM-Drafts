
🔗 [Link to the Room](https://tryhackme.com/room/introtok8s)

## 🏷️An introduction to Kubernetes covering the basics of cluster creation and hardening.

1. [Kubernetes 101](#kubernetes-101)<br>
2. [Kubernetes Architecture](#kubernetes-architecture)<br>
3. [Kubernetes Landscape](#kubernetes-landscape)<br>
4. [Kubernetes Configuration](#kubernetes-configuration)<br>
5. [Kubectl](#kubectl)<br>
6. [Kubernetes & DevSecOps](#kubernetes-&-devsecops)<br>
7. [Hands-on with Kubernetes](#hands-on-with-kubernetes)<br>

&nbsp;

# 📚 Study Notes #

<!-- INTRODUCTION HERE -->

&nbsp;

# Kubernetes 101

&nbsp;












&nbsp;

---
><details><summary>❓Which benefit of Kubernetes means that it can run on any type of infrastructure?</summary>highly portable</details>
---
><details><summary>❓Fil in the blank "Kubernetes is a __________ system".</summary>container orchestration</details>
---

&nbsp;

# Kubernetes Architecture

&nbsp;















&nbsp;

---
><details><summary>❓What is the smallest deployable unit of computing you can create in Kubernetes?</summary>pod</details>
---
><details><summary>❓Which control plane component is a key/value store which contains data pertaining to the cluster and its current state?</summary>etcd</details>
---
><details><summary>❓Which worker node component is responsible for network communicatio within the cluster?</summary>kube-proxy</details>
---

&nbsp;

# Kubernetes Landscape

&nbsp;












&nbsp;

---
><details><summary>❓Which Kubernetes component exposes pods and serves as an access point?</summary>service</details>
---
><details><summary>❓Which Kubernetes component can guarantee the availability of X number of pods?</summary>replicaset</details>
---
><details><summary>❓What Kubernetes component is used to define a desired state?</summary>deployments</details>
---

&nbsp;

# Kubernetes Configuration

&nbsp;
















&nbsp;

---
><details><summary>❓In a config file, you have just declared that you want 4 nginx pods. In which one of the 'required fields' has this been declared?</summary>spec</details>
---
><details><summary>❓The configuration file is for a deployment. In which one of the 'required fields' is this declared?</summary>kind</details>
---
><details><summary>❓The pods in this deployment will be exposed by a service. In the service configuration file, the target port was set to 80. What should you put as the 'containerPort'?</summary>80</details>
---

&nbsp;

# Kubectl

&nbsp;












&nbsp;

---
><details><summary>❓... troubleshoot a pod by gathering some details about it?</summary>describe</details>
---
><details><summary>❓... access the container's shell?</summary>exec</details>
---
><details><summary>❓... check the status of running pods?</summary>get</details>
---
><details><summary>❓... turn a defined configuration (YAML file) into a running process?</summary>apply</details>
---

&nbsp;

# Kubernetes & DevSecOPS

&nbsp;
















&nbsp;

---
><details><summary>❓Which best container security practice is used to regulate access to a Kubernetes cluser and its resources?</summary>RBAC</details>
---
><details><summary>❓What is used to define security policies at 3 levels?</summary>Pod Security Standards</details>
---
><details><summary>❓What enforces these policies?</summary>Pod Security Admission</details>
---
><details><summary>❓What Kubernetes object can be used to store sensitive information and should, therefore, be managed securely?</summary>Secret</details>
---

&nbsp;

# Hands-on with Kubernetes

&nbsp;











&nbsp;

---
><details><summary>❓</summary>THM{***_************}</details>
---
><details><summary>❓What apiVersion is used for the RoleBinding?</summary>rbac.authorization.k8s.io/v1</details>
---

&nbsp;

