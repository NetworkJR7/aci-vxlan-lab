# 🚀 ACI VXLAN Lab – Network Automation with Python

## 📌 Overview

This project simulates a **modern Data Center network** inspired by **Cisco ACI architecture**, implementing VXLAN overlay networking and Python-based automation.

It demonstrates how traditional networking evolves into **policy-driven and automated infrastructures**, aligning with real-world **DevNet / NetDevOps environments**.

---

## 🧠 Architecture

* **Underlay Network:** 10.0.x.x (Linux-based routing)
* **Overlay Network:** VXLAN (192.168.x.x)
* **Control Node:** Kali Linux (routing, NAT, automation)
* **Endpoints:**

  * Web Server → 10.0.1.10
  * DB Server → 10.0.2.10

---

## 🏗️ Topology

> Simulated ACI Fabric with Spine-Leaf architecture

* 1 Spine
* 2 Leafs
* Endpoints connected to Leafs
* Centralized control logic (ACI-like model)

---

## 🔧 Technologies Used

* Linux Networking (`iproute2`)
* VXLAN (Overlay networking)
* `iptables` (microsegmentation & firewall)
* Python (automation & orchestration)
* SSH (remote execution)

---

## 🔐 Security & Microsegmentation

Implemented **policy-based segmentation** inspired by Cisco ACI contracts:

### ✅ Allowed

* Web ↔ DB communication (restricted ports)

### ❌ Denied

* Inter-VNI unauthorized traffic
* Lateral movement between segments

---

## 🤖 Automation

Python scripts automate key infrastructure tasks:

* VXLAN deployment
* Firewall policy configuration
* Remote command execution via SSH

### Example

```bash
python scripts/deploy.py
```

---

## 📂 Project Structure

```
aci-vxlan-lab/
├── scripts/
│   ├── deploy.py
│   ├── web_setup.py
│   └── db_setup.py
├── configs/
├── diagrams/
└── README.md
```

---

## 🧪 Key Skills Demonstrated

* VXLAN & Overlay Networking
* Spine-Leaf Architecture Concepts
* Network Troubleshooting (routing, NAT, segmentation)
* Infrastructure Automation with Python
* Security & Microsegmentation

---

## 💼 Real-World Relevance

This project reflects real scenarios in:

* Cisco ACI environments
* Data Center Networking
* Cloud Networking (AWS / Azure VPC concepts)
* DevNet / NetDevOps roles

---

## 📈 Next Improvements (Roadmap)

* Add logging instead of print (Python logging module)
* Implement CLI arguments (`argparse`)
* Include API-based automation (REST / ACI simulation)
* Dockerize lab components
* Add monitoring (NetFlow / logs)

---

## 👨‍💻 Author

**Jaime Rosero Mesa**
Senior Network Engineer → Transitioning into Cybersecurity & Network Automation

---
