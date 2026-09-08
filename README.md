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
git clone https://github.com/<your-repo>/incident-management-soc.git
cd incident-management-soc

# Launch the SOC stack
docker-compose up -d
