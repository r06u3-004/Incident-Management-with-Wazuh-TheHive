# Incident-Management-with-Wazuh-TheHive


## 📌 Overview

This project sets up a **Security Operations Center (SOC)** environment for **incident management** using:

- **Wazuh** → Security monitoring & log analysis  
- **TheHive** → Incident response & case management  
- **Cortex** → Observable analysis & automation  
- **MISP** → Threat intelligence sharing  
- **Shuffle** → Workflow orchestration  

The architecture is containerized with **Docker Compose**, enabling quick deployment of a full SOC lab.

---

## ⚙️ Architecture

The SOC stack includes:

- **TheHive** (Incident management platform)  
- **Cassandra + Elasticsearch** (Databases & indexing)  
- **Cortex** (Automation & analysis)  
- **MISP** (Threat intelligence platform)  
- **Shuffle** (Workflow orchestration)  
- **MinIO** (Storage backend)  
- **OpenSearch** (Search engine for Shuffle)  

All services communicate via the Docker network **`SOC_NET`**.

---

## 🔑 Key Features

- Centralized **incident management** with TheHive  
- Automated **observable analysis** via Cortex  
- Integrated **threat intelligence** with MISP  
- **Workflow orchestration** through Shuffle  
- Scalable architecture with **Docker Compose**  

---

## 🚀 Deployment

### Prerequisites
- Docker & Docker Compose installed  
- Minimum 8 GB RAM recommended  
- Open ports for SOC services  

### Quick Start
```bash
# Clone the repository

# Launch the SOC stack
docker-compose up -d


# ⚠️ Configuration Notes

Some configuration files (e.g. `application.conf`, `cassandra.yaml`, `elasticsearch.yml`) must be customized before deployment.  
Sensitive commands and credentials are masked for security reasons.

---

## 🌐 Access Points

| Service       | Port |
|---------------|------|
| TheHive       | 9000 |
| Cortex        | 9001 |
| MinIO         | 9002 |
| Elasticsearch | 9200 |
| OpenSearch    | 9201 |
| MISP HTTP     | 8080 |
| MISP HTTPS    | 8443 |
| Cassandra     | 9042 |

---

## 🛡️ Use Case

This lab demonstrates how to build a **SOC environment** for:

- Incident detection & response  
- Threat intelligence integration  
- Automated analysis of observables  
- Workflow orchestration for security operations  

It is ideal for **training, testing, and research** in cybersecurity.

---

## 📚 Documentation

- [TheHive Project](https://thehive-project.org/)  
- [Wazuh Documentation](https://documentation.wazuh.com/)  
- [Cortex](https://github.com/TheHive-Project/Cortex)  
- [MISP](https://www.misp-project.org/)  
- [Shuffle](https://shuffler.io/)  
