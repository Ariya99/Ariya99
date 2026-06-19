<!-- ===================== HERO SECTION ===================== -->

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Inter&size=30&duration=2500&pause=800&center=true&vCenter=true&width=800&lines=Platform+Engineer+%7C+DevOps+Architect;Kubernetes+%7C+Cloud+%7C+Infrastructure+%26+AI"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Engineer-0ea5e9?style=for-the-badge&logo=kubernetes&logoColor=white"/>
  <img src="https://img.shields.io/badge/DevOps-Automation-6366f1?style=for-the-badge&logo=linux&logoColor=white"/>
  <img src="https://img.shields.io/badge/Cloud-Native-10b981?style=for-the-badge"/>
</p>

<br/>

<!-- ===================== ABOUT ===================== -->

## 👨‍💻 About Me

<div align="center">

I design and engineer **production-grade infrastructure platforms**.

My focus is building:

🚀 Distributed systems & cloud-native infrastructure  
☸️ Kubernetes platform engineering  
⚙️ DevOps automation & GitOps workflows  
🔐 Secure, scalable and reliable environments  

**Open to relocate to EU**

</div>

<br/>

<!-- ===================== PROFESSIONAL SUMMARY ===================== -->

## 🧾 Professional Summary

DevOps Engineer and Solution Architect with **6+ years of experience** designing, implementing, and operating scalable infrastructure platforms and cloud-native environments. Experienced in Kubernetes platform engineering, CI/CD automation, GitOps workflows, observability, Linux infrastructure, and enterprise production systems. Proven track record improving scalability, automation, and operational efficiency; currently expanding expertise in AI infrastructure, LLM-based systems, and AI-assisted DevOps automation.

<br/>

<!-- ===================== ENGINEERING FOCUS ===================== -->

## 🏗️ Engineering Focus

<div align="center">

| ☸️ Kubernetes | ⚙️ Automation | 🔐 Security |
|---|---|---|
| Cluster architecture | Infrastructure as Code | CI/CD pipelines |
| Container orchestration | GitOps workflows | Security hardening |
| Service mesh | DevOps automation | Access control |

</div>

<br/>

<!-- ===================== SYSTEM ARCHITECTURE ===================== -->

## 🧠 System Architecture

```mermaid
flowchart LR
  Dev["Developers<br/>(git push, PRs)"] --> Repo["Git Repository"]
  Repo --> CI["CI/CD Pipeline<br/>(GitHub Actions / Bamboo)"]
  CI --> Registry["Image Registry<br/>(JFrog / Docker Hub)"]
  CI --> Tests["Automated Tests<br/>(Security / E2E)"]
  Tests --> Registry
  CI --> Notify["CI -> Slack / Ticketing"]

  Repo --> GitOps["GitOps Operator<br/>(ArgoCD / Flux)"]
  Registry --> GitOps
  GitOps --> K8sProd["K8s Cluster — Prod"]
  GitOps --> K8sStg["K8s Cluster — Staging"]

  LB["Global LB / CDN"] --> WAF["WAF / API Gateway"]
  WAF --> Ingress["Ingress Controller / External LB"]
  Ingress --> Mesh["Service Mesh<br/>(Istio / Linkerd)"]
  Mesh --> Apps["Microservices / Pods"]

  Apps --> Postgres["PostgreSQL HA"]
  Apps --> Redis["Redis Cluster"]
  Apps --> Kafka["Kafka Cluster"]
  Apps --> ES["Elasticsearch"]
  Storage["PV / CSI / Object Storage"] -.-> Postgres
  Storage -.-> ES

  Apps --> Metrics["Prometheus / Metrics"]
  Apps --> Traces["Jaeger / OpenTelemetry"]
  Apps --> Logs["Fluentd → ELK"]
  Metrics --> Grafana["Grafana Dashboards"]
  Logs --> Kibana["Kibana"]
  Grafana --> Alert["Alerting / PagerDuty"]
  Alert --> Oncall["Incident Mgmt"]

  IAM["Identity & Access<br/>(OIDC, RBAC)"] -.-> K8sProd
  Secrets["Vault / External KMS"] -.-> Apps
  Policy["Policy Engine<br/>(OPA / Gatekeeper)"] -.-> GitOps
  Backup["Backup & DR Services"] -.-> Storage

  style GitOps fill:#eef6ff,stroke:#0ea5e9,stroke-width:1px
  style LB fill:#f0f9ff,stroke:#2563eb,stroke-width:1px
  style Metrics fill:#fff7ed,stroke:#f59e0b,stroke-width:1px
  style IAM fill:#f8fafc,stroke:#ef4444,stroke-width:1px
```

A simplified, modern architecture view: developers push changes to Git, CI builds and pushes images to a registry, GitOps reconciles the desired state into the Kubernetes platform which houses API gateway/ingress, service mesh, and microservices. Stateful systems (Postgres HA, Redis, Kafka, Elasticsearch) are attached as well as a centralized observability stack that feeds alerting and incident management.

<br/>

<!-- ===================== FEATURED PROJECTS ===================== -->

## 🚀 Featured Projects

### ⭐ DevOps Automation Toolkit
Infrastructure automation collection:
- Linux server bootstrap
- SSH hardening & security automation
- Kubernetes utilities
- Operational scripts
- Deployment helpers

### ☸️ Kubernetes Platform Engineering
Hands-on infrastructure:
- Kubernetes cluster deployment
- Ingress architecture
- Monitoring stack
- Container lifecycle management
- Production operations

### 🌐 API Gateway & Cloud Networking
Built and managed:
- API gateway architecture
- Service routing & traffic management
- Secure exposure patterns
- High availability design

### 🗄️ Database Reliability
Experience with:
- PostgreSQL high availability
- Replication & backup strategies
- Database operations
- Data integrity

### 📡 Distributed Infrastructure
Implemented:
- Kafka messaging platforms
- Elasticsearch clusters
- Observability pipelines
- Scalable backend services

### 💼 Multi-Project Production Platform
nahalgsht.com | visaland.org | panafor.com | aia.tools
- Designed and implemented production infrastructure for multiple web platforms
- Built centralized monitoring using Prometheus, Grafana, and Uptime Kuma
- Created GitHub Actions CI/CD workflows and GitOps-based deployment processes
- Automated deployments, monitoring, health checks, and operational workflows
- Implemented secure VPN-over-DNS networking solution

<br/>

<!-- ===================== PROFESSIONAL EXPERIENCE ===================== -->

## 💼 Professional Experience

### DevOps Engineer — Sabaidea Corporation (May 2025 - Feb 2026)
- Built and maintained Kubernetes-based production platforms using Kubernetes, Rancher, and Docker
- Designed platform architecture for scalable microservices including API Gateway, ingress, networking, and service discovery
- Implemented CI/CD automation using Bamboo, Bitbucket, and JFrog Artifactory
- Built monitoring and observability solutions using Prometheus, Grafana, and ELK Stack
- Integrated enterprise on-premise projects: Snappfood, Tejarat Bank, Taline, MTN Irancell, MCI
- **Delivered infrastructure supporting millions of daily API requests**
- **Reduced downtime by ~40% and improved incident detection time by ~60%** through monitoring and automation

### Lead DevOps Engineer — Tecnotree Corporation (Sep 2023 - Apr 2025)
- Led DevOps delivery and optimization for telecom platforms: CLM, CBS, HCBS, EIA
- Managed delivery lifecycle for 60+ enterprise telecom projects
- Improved deployment workflows using Kubernetes, Ansible, Git, and TeamCity
- Collaborated with development, architecture, business, and operations teams
- Supported go-live operations, incident response, and reliability improvements
- Worked with PostgreSQL, MySQL, Oracle Database, and Cassandra environments
- Mentored engineers and improved DevOps practices across teams

### Linux Administrator — Tecnotree / Parspack (Nov 2021 - Aug 2023)
- Managed Linux infrastructure: Ubuntu, RHEL, CentOS, AlmaLinux, Rocky Linux
- Installed and maintained Nginx, Apache, MySQL, PHP, DNS, SSH, and FTP services
- Resolved networking and infrastructure issues: DNS, DHCP, VPN, TCP/IP, SSH tunneling
- Supported cloud hosting, CDN, and enterprise infrastructure environments

<br/>

<!-- ===================== TECH STACK ===================== -->

## ⚙️ Technology Stack

### Platform Engineering & DevOps
<p align="center">
  <img src="https://skillicons.dev/icons?i=kubernetes,docker,linux,terraform,ansible,python,go,bash,postgres,redis,kafka,nextjs,typescript,html,css,tailwind"/>
</p>

Kubernetes • Rancher • Docker • Terraform • Ansible • GitHub Actions • GitLab CI • Bamboo • Bitbucket • Jenkins • JFrog Artifactory

### Cloud & Infrastructure
<p align="center">
  <img src="https://skillicons.dev/icons?i=aws,gcp,git,github,jenkins"/>
</p>

AWS • GCP • Git • GitHub • Networking • VPN • Security

### Observability & Monitoring
<p align="center">
  <img src="https://skillicons.dev/icons?i=prometheus,grafana"/>
</p>

Prometheus • Grafana • ELK Stack • Zabbix • Uptime Kuma

### Data Platforms
- PostgreSQL (HA & Replication)
- MySQL
- Redis
- Kafka
- Elasticsearch
- Cassandra
- CockroachDB
- Oracle Database

### AI & MLOps
- RAG Applications
- LLM Integration & AI Agents
- Vector Search
- AI-Assisted DevOps Automation
- MLOps Fundamentals

<br/>

<!-- ===================== ENGINEERING PRINCIPLES ===================== -->

## 🔥 Engineering Principles

<div align="center">

| Principle | Focus |
|-----------|-------|
| ⚡ Automation over repetition | Reduce manual work |
| 📋 Infrastructure as Code | Version control everything |
| 🔐 Security by default | Security from day one |
| 📊 Observability everywhere | Visibility and monitoring |
| 💪 Design for failure | Resilience first |
| 📈 Reliable systems at scale | Production ready |

</div>

<br/>

<!-- ===================== EDUCATION ===================== -->

## 🎓 Education

- **Master of Computer & Information Sciences** — Azad University
- **Bachelor of Physics** — Kharazmi University

<br/>

<!-- ===================== CERTIFICATIONS ===================== -->

## 🏅 Certifications

- LPIC-1, LPIC-2
- DevOps Foundations
- Kubernetes Monitoring with Prometheus
- Grafana Application Performance Monitoring
- CEH (Certified Ethical Hacker)
- PWK (Penetration Testing with Kali Linux)

<br/>

<!-- ===================== LANGUAGES ===================== -->

## 🗣️ Languages

- **English** — Advanced
- **Persian** — Native
- **Italian** — Intermediate

<br/>

<!-- ===================== GITHUB ACTIVITY ===================== -->

## 📊 GitHub Activity

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Ariya99&theme=react-dark&hide_border=true"/>
</p>

<br/>

<!-- ===================== CONNECT ===================== -->

## 🌐 Connect With Me

<p align="center">
  <a href="https://www.linkedin.com/in/ariya-pourmirza-06aa0916a/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin"/>
  </a>
  <a href="mailto:ariyapourmirza@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0ea5e9,100:6366f1&height=120&section=footer"/>
</p>
