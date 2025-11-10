# 🛡️ HIDS using Osquery

This project implements a **Host-based Intrusion Detection System (HIDS)** on Linux using **Osquery**.  
It was developed as part of the *Sécurité des Applications et des Systèmes d’Exploitation* module at **Université Mohammed V – Faculté des Sciences de Rabat**.

---

## 🚀 Overview
The system continuously monitors a Linux host to detect abnormal or malicious behavior.  
It automates data collection, analysis, and false positive filtering using **Python**, **SQLite**, and **cron**.

---

## ⚙️ Components
- **Osquery** – collects system data via scheduled SQL queries.  
- **export_osquery.py** – parses Osquery logs and stores results in a SQLite database.  
- **detect_false_positives.py** – filters irrelevant alerts to reduce noise.  
- **osquery.conf / packs/** – define monitoring rules and query schedules.  
- **Cron jobs** – automate data export and analysis.

---

## 📊 Results
- 🚫 **85% reduction** in alert noise  
- ⚡ **2.7 ms** average alert processing time  
- ✅ **92%** of known false positives detected

---

## 🔮 Future Work
- Integration with **SIEM** (Wazuh, ELK, Splunk)  
- Visualization dashboards (Grafana / Kibana)  
- Automated deployment via **Ansible** or **Terraform**



## 📄 License
This project is released under the [MIT License](LICENSE).

