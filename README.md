<div align="center">

# 👾 Rick Robinson — Security Operations Engineer

**Senior Security Engineer | Network Defense | SIEM & Threat Detection**

[![FortiGate](https://img.shields.io/badge/FortiGate-HA%20%7C%20FIPS--CC-red?style=flat-square&logo=fortinet)](https://github.com/RickRobinsonNetworks)
[![PaloAlto](https://img.shields.io/badge/Palo%20Alto-PCNSE%20Certified-00AEEF?style=flat-square)](https://github.com/RickRobinsonNetworks)
[![Elastic SIEM](https://img.shields.io/badge/Elastic-SIEM%20%7C%20SOC%20Lab-005571?style=flat-square&logo=elastic)](https://github.com/RickRobinsonNetworks)
[![SD-WAN](https://img.shields.io/badge/FortiGate%20SD--WAN-ADVPN%20%7C%20FortiOS-red?style=flat-square&logo=fortinet)](https://github.com/RickRobinsonNetworks)

</div>

---

## 🛡️ About Me

Production Network & Security Engineer managing enterprise firewall clusters, SD-WAN infrastructure, and SOC tooling across multi-site environments. I build and document everything — from HA failover runbooks to full SOC detection pipelines — in a bare-metal EVE-NG home lab running the same stack I manage in production.

- 🔥 **Daily drivers:** FortiGate 60F HA (FIPS-CC, FortiOS 7.4.x), PaloAlto VM-300, FortiGate SD-WAN
- 🧪 **Lab platform:** EVE-NG bare-metal | Ryzen 9 3950X | 128 GB RAM
- 📡 **Detection stack:** Elastic SIEM (1,696 rules) + Wazuh 4.14.5 + Shuffle SOAR + DFIR-IRIS
- 🎓 **Certifications:** M.S. | NSE 4/5 (FortiGate Firewall) | PCNSA PCNSE (Palo Alto Firewall)

---

## 🗂️ Featured Lab Projects

### 🔐 [FortiGate-HA-FIPS-SOC-Lab](https://github.com/RickRobinsonNetworks/FortiGate-HA-FIPS-SOC-Lab)
> **FortiGate 60F Active/Passive HA with FIPS-CC Mode, mTLS Syslog & SOC Integration**

Full production-mirror lab: HA clustering, FIPS-CC activation (config scrubbing, pre-checks), encrypted syslog to Elastic/Wazuh via mTLS, FortiManager config-push behavior, and hard-recovery partition swap procedure.

`FortiGate` `HA-Clustering` `FIPS-CC` `FortiManager` `mTLS-Syslog` `FortiOS-7.4`

---

### 🌐 [SDWAN-ADVPN-BGP-OSPF-Lab](https://github.com/RickRobinsonNetworks/SDWAN-ADVPN-BGP-OSPF-Lab)
> **FortiGate SD-WAN Overlay + FortiGate ADVPN with BGP/OSPF Route Distribution**

Multi-site SD-WAN fabric (FortiOS 7.4.x, multi-site SD-WAN hub/spoke, SLA health checks, path steering policies) with FortiManager orchestration. ADVPN dynamic tunnels with OSPF and BGP redistribution across hub-spoke and full-mesh topologies.

`FortiGate-SDWAN` `ADVPN` `IPSec` `BGP` `OSPF` `FortiManager` `FortiGate`

---

### 🔴 [PaloAlto-PCNSA-Lab-Series](https://github.com/RickRobinsonNetworks/PaloAlto-PCNSA-Lab-Series)
> **14-Lab PAN-OS Series: Security Profiles, SSL Decryption, Panorama, HA & Routing**

Progressive lab series (X1–X14) aligned with PCNSE objectives. Covers Security Profile Groups (AV, Vulnerability, URL, WildFire), SSL/TLS Forward Proxy decryption with certificate management, Panorama device-group push, PAN-OS HA pair configuration (priority, preemption, HA1/HA2 links), routing (RIB/FIB, BGP, OSPF), and deployment modes (L3, vWire, Tap).

`PAN-OS` `Panorama` `SSL-Decryption` `Security-Profiles` `HA` `BGP` `OSPF` `Certificates` `PCNSE`

---

### 🔭 [Elastic-SOC-Detection-Lab](https://github.com/RickRobinsonNetworks/Elastic-SOC-Detection-Lab)
> **Full-Stack SOC: Elastic SIEM + Wazuh + Shuffle SOAR + DFIR-IRIS**

End-to-end SOC pipeline: multi-source syslog ingestion (FortiGate, PaloAlto, FortiGate SD-WAN syslog via DNAT), 1,696 detection rules tuned and enabled, custom QEMU churn detection (rules 100510/100511), automated alert triage via Shuffle (SOC-01/02/03 workflows), and case management in DFIR-IRIS. Includes Zabbix infrastructure monitoring with Wazuh agent coverage across all SOC VMs.

`Elastic-SIEM` `Wazuh` `Shuffle-SOAR` `DFIR-IRIS` `Syslog` `Detection-Engineering` `Zabbix`

---

### 🔒 [SSL-Decryption-PKI-Lab](https://github.com/RickRobinsonNetworks/SSL-Decryption-PKI-Lab)
> **Certificate Authority Design, SSL/TLS Inspection & mTLS Implementation**

OpenSSL ROOT-CA build, subordinate CA chaining, certificate deployment on FortiGate and PaloAlto for SSL forward-proxy decryption. mTLS syslog configuration (FIPS-CC encrypted channel to Elastic). Covers certificate lifecycle: CSR generation, signing, revocation, trust anchors, and browser/endpoint trust distribution.

`PKI` `SSL-Decryption` `mTLS` `OpenSSL` `FortiGate` `PaloAlto` `Certificates` `FIPS`

---

### 📊 [FortiAnalyzer-FortiManager-Runbooks](https://github.com/RickRobinsonNetworks/FortiAnalyzer-FortiManager-Runbooks)
> **Operational Runbooks: FortiAnalyzer Log Correlation & FortiManager Config Orchestration**

Production-grade runbooks covering FortiAnalyzer log normalization and event correlation, FortiManager config push behavior under FIPS-CC, ADOM management, policy package deployment, and HA sync troubleshooting (hasync WARN, sync_type 18, BYOD device identity root cause). Includes lnkmtd memory bug workaround and EMTL site incident post-mortem.

`FortiAnalyzer` `FortiManager` `FortiOS` `HA-Sync` `ADOM` `Runbooks` `Production`

---

### 📈 [Zabbix-Infrastructure-Monitoring-Lab](https://github.com/RickRobinsonNetworks/Zabbix-Infrastructure-Monitoring-Lab)
> **Zabbix Network & Host Monitoring | SNMP Polling | Wazuh Integration | EVE-NG SOC Stack**

Full infrastructure monitoring layer for the SOC lab: Zabbix server deployment, agent rollout across all SOC VMs, SNMP polling of FortiGate/PaloAlto/FortiSwitch, trigger thresholds and alert escalation, and integration with Wazuh for correlated SOC visibility. Also covers qemu-cpu-monitor deployment on the EVE-NG host with custom Wazuh detection rules 100510/100511.

`Zabbix` `SNMP` `Infrastructure-Monitoring` `Wazuh` `EVE-NG` `FortiGate` `PaloAlto` `SOC`

---

## 🧰 Tech Stack

| Domain | Tools & Platforms |
|---|---|
| **Next-Gen Firewalls** | FortiGate 60F (FIPS-CC), PaloAlto VM-300, Panorama |
| **SD-WAN** | FortiGate SD-WAN (FortiOS 7.4.x), ADVPN, FortiManager |
| **Centralized Mgmt** | FortiManager, FortiAnalyzer, Panorama |
| **Routing Protocols** | BGP, OSPF, ADVPN, IPSec IKEv1/v2 |
| **SIEM / Detection** | Elastic Stack, Wazuh 4.14.5, 1,696+ detection rules |
| **SOAR / Case Mgmt** | Shuffle, DFIR-IRIS |
| **PKI / Crypto** | OpenSSL, mTLS, SSL Decryption (FP/FI), FIPS-CC |
| **Monitoring** | Zabbix (SNMP + agent), qemu-cpu-monitor, Wazuh agents |
| **Lab Platform** | EVE-NG bare-metal, QEMU/KVM |

---

## 📁 Repo Structure Pattern

All lab repos follow this standard layout:

```
repo/
├── README.md          # Lab overview, topology, objectives
├── topology/          # EVE-NG .unl exports, draw.io diagrams
├── configs/           # Sanitized device configs (CLI export)
├── runbooks/          # Step-by-step Word/Markdown runbooks
├── verification/      # show/diagnose output captures
└── screenshots/       # Kibana dashboards, GUI captures
```

---

<div align="center">

**Rick Robinson Security Operations**
*Building production-quality labs. Documenting everything.*

</div>
