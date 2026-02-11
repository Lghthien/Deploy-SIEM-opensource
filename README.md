# Open-Source SIEM System Development

Enterprise Internship Project – Security Monitoring & Log Engineering  

## Overview

This project focuses on designing and deploying a production-ready **Open-Source SIEM (Security Information and Event Management)** system using modern log engineering and security monitoring practices.

The system centralizes log collection, parsing, normalization, storage, and visualization across multiple infrastructure layers including servers, network devices, virtualization platforms, and applications.

---

## Architecture

[Endpoints]
↓
[Wazuh Agent]
↓
[Wazuh Manager]
↓
[Vector (Aggregator & Parser)]
↓
[OpenSearch Cluster]
↓
[OpenSearch Dashboards]


### Core Components

- **OpenSearch** – Log storage, indexing, and search engine
- **OpenSearch Dashboards** – Visualization and monitoring
- **Vector (Rust-based)** – Log collection, parsing, transformation (VRL)
- **Wazuh** – Endpoint log collection agent
- **Docker** – Containerized deployment
- **Nginx** – Load Balancer & Stream Proxy
- **ECS (Elastic Common Schema)** – Log normalization standard

---

## Key Features

### Centralized Log Collection
- Linux (Syslog, Auth logs)
- Windows (Event Viewer)
- Firewall (Fortigate)
- Web Server (Nginx/Apache)
- Database (MySQL)
- Docker Containers
- VMware ESXi
- Network Devices

### Log Processing Pipeline
- Parsing (Regex & VRL)
- Filtering noisy logs
- Tagging and indexing
- Data normalization using ECS
- Enrichment and transformation
- Bulk ingestion to OpenSearch

### High Availability & Scalability
- OpenSearch 3-node cluster
- Nginx Load Balancer
- Failover mechanism for agents
- VLAN / DMZ cross-network log forwarding via Stream Proxy

### Automation
- Auto-deployment scripts for Linux & Windows agents
- Migration from Fluentd to Vector
- Performance tuning & memory optimization
- Regex optimization to prevent memory leaks

---

## Production Achievements

- Designed and deployed full SIEM architecture in lab and production environments
- Migrated entire log pipeline from Fluentd to Vector (Rust-based performance optimization)
- Implemented ECS-based log normalization across heterogeneous sources
- Resolved complex ESXi parsing challenges using advanced multi-layer regex
- Fixed memory leak caused by inefficient backtracking expressions
- Implemented High Availability and Load Balancing architecture
- Delivered monitoring dashboards and operational documentation

---

## Technical Stack

- Python (automation scripting)
- Vector (VRL)
- OpenSearch
- Wazuh
- Docker & Docker Compose
- Nginx (Stream Proxy & Load Balancing)
- Linux System Administration
- Network Troubleshooting

---

## Skills Demonstrated

- SIEM Architecture Design
- Log Engineering & Data Normalization
- Performance Tuning & Troubleshooting
- High Availability System Design
- Production Incident Handling
- Infrastructure Monitoring
- Security Operations Support (SOC)

---

## Project Status

Production-ready deployment completed.  
System successfully handed over with full operational documentation.

---

## Author

Le Gia Hoang Thien  
Network & Security Engineering Student  
University of Information Technology – VNU-HCM  

---

## License

This project is for educational and research purposes.
