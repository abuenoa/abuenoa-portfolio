# 👋 Hi, I'm Antonio Bueno Antón

**Technical Director (CTO)** & **Cloud Security Architect** specializing in the intersection of high-availability infrastructure and defensive security.

I bridge the gap between **Cloud Engineering** and **Post-Quantum Cryptography**, designing systems that survive hostile environments. Currently leading the technical strategy at **Omega AI**, building the secure tunnel between binary computing and the quantum future.

I am an engineer who believes that security is not a feature; it is the architecture itself.

## 📫 Quick Contact

* 📧 **Email:** [antonio.buenoanton@gmail.com](mailto:antonio.buenoanton@gmail.com)

* 📞 **Phone:** +34 637 397 160

* 💼 **LinkedIn:** [linkedin.com/in/abuenoan](https://www.linkedin.com/in/abuenoan)

* 🎓 **Education:** MSc Cloud Computing & Network Security (*University of Bolton, UK*)

## 💻 Professional Experience

### 🟢 Technical Director (CTO) | **Omega AI**

*(May 2025 – Present | Alicante, Spain / Remote)*

Leading the engineering roadmap for a **Quantum-Resilient AI Platform**. I advanced from *Team Leader* to *Technical Director* in under 4 months by restructuring the engineering culture and optimizing delivery pipelines.

* **Strategic Leadership & PQC Security:** Directing the technical vision for a secure "binary-to-quantum" AI platform. I supervise the architectural integration of **Post-Quantum Cryptography (PQC)** standards (NIST FIPS 203/204), applying algorithms like **Dilithium** to ensure data sovereignty against "Harvest Now, Decrypt Later" threats.

* **DevOps & Infrastructure Optimization:** Re-architected the CI/CD strategy using **GitLab**. Reduced pipeline runtime by **83%** and slashed data transfer costs by **95%** through modularization and artifact optimization.

* **AI Backend Architecture:** Architecting the core API infrastructure using **Python (FastAPI)** for real-time LLM inference (integrating **vLLM** and **llama.cpp** with SSE streaming).

* **Cloud Hardening:** Managing secure multi-cloud deployments (**Azure, AWS**) using **Docker** and **Kubernetes**. Implementation of strict **Zero Trust** policies (mTLS) and observability suites with **Grafana** and **Prometheus**.

### 🔵 Senior Cloud Consultant & Analyst | **Minsait (Indra)**

*(Jan 2023 – Nov 2024 | Seville, Spain)*

Core engineer for **Onesait Efficiency** and **Onesait Platform**, handling critical IoT data ingestion and platform engineering for Smart Energy sectors.

* **Global IoT Architecture:** Engineered data pipelines for a multi-tenant platform managing hundreds of heterogeneous devices across **LATAM and EMEA**. Ensured high-throughput ingestion using **Apache Kafka** and **MQTT**.

* **Platform Engineering:** Developed custom automation modules (nodes) for **Node-RED** using Java/Spring Boot, enabling other developers to orchestrate complex workflows without touching low-level code.

* **Microservices Orchestration:** Deployed and maintained scalable backend services on **OpenShift (Kubernetes)**, ensuring isolation and performance in a multi-client environment.

* **Tech Stack:** Java Spring Boot, StreamSets, Node-RED, Docker, OpenShift.

### 🔵 Solution Assistant | **NTT DATA**

*(Nov 2021 – Jan 2023 | Seville, Spain)*

Software Engineer for **SIGLO** (Sistema Integral de Gestión Logística), the mission-critical supply chain platform for the **Andalusian Health Service (SAS)**.

* **Legacy to Microservices Migration:** Played a key role in the architectural transition of a massive public health platform, moving from a monolithic legacy environment to a modern **Microservices architecture** while ensuring service continuity for hospitals.

* **Critical Infrastructure:** Developed and deployed financial and logistics features in a high-pressure live environment.

* **DevOps Adoption:** Helped standardize deployment pipelines using **Jenkins**, **SonarQube**, and **Git**, introducing modern CI/CD practices to the development lifecycle.

## 🛠 Core Technical Skills

| Domain | Technologies | 
 | ----- | ----- | 
| **Cloud & DevOps** | AWS, Azure, Docker, Kubernetes, OpenShift, GitLab CI/CD, Terraform | 
| **Security** | Post-Quantum Cryptography (Dilithium/Kyber), Zero Trust, mTLS, OAuth2 | 
| **Backend** | Python (FastAPI), Java (Spring Boot), Node.js | 
| **Data & IoT** | Kafka, MQTT, StreamSets, Node-RED, SQL/NoSQL, IPFS | 
| **Observability** | Prometheus, Grafana, SonarQube | 

*Last updated: December 2025*

---

## 🚀 Featured Projects

### 🛡️ ACR Vulnerability Density
**Brief Description**
An empirical and reproducible pipeline to analyze vulnerability density and its temporal evolution in base images stored in Azure Container Registry (ACR), using Trivy. It scans selected images at four points in time (T0–T3), consolidates results, and generates charts ready for academic analysis or Master's thesis use.

**Problem Addressed**
Base images (such as `alpine`, `debian-slim`, `ubuntu`, etc.) change over time, and their vulnerabilities can grow or shift even without direct modifications. This project quantifies that **vulnerability drift**, helping to evaluate recurrent risks in CI/CD pipelines.

**Technologies Used**
- Infrastructure as Code: **Terraform** (ACR + RG infrastructure in Azure)
- Process Automation: Shell scripts (`bash`) for login, pull/tag/push, and Trivy scanning
- Analysis & Visualization: **Python** (pandas + matplotlib)
- Reproducible Design: `Makefile`, pinned versions (`pyenv`, Trivy DB), and tool logs for traceability

**Impact / Results**
- Enables measurement of vulnerability density normalized by MB: `(CRITICAL + HIGH) / size_mb`
- Generation of comparative CSVs and weekly charts (T0 to T3) showing CVE evolution and cumulative growth
- High reproducibility: scanner versions, package identities, and timestamps are automatically logged

**Link to full project:** [github.com/abuenoa/acr-vuln-density](https://github.com/abuenoa/acr-vuln-density)


### 🗂️ Architecture Diagram – Diagram-as-Code
**Brief Description**
A public repository example where I demonstrate how to create **architecture diagrams as code** using the [Diagrams library by Mingrammer](https://diagrams.mingrammer.com/).
The project generates a **generic multi-cloud diagram** (users → CDN → WAF → Load Balancer → Web/API → Cache/Workers/DB, along with CI/CD and observability), demonstrating best practices for documenting architectures without exposing sensitive information.

**Problem Addressed**
Architecture documentation often becomes obsolete quickly when done via manual diagrams (Visio, Draw.io, etc.). A *diagram-as-code* approach provides:
- **Git Versioning** (history of changes and revisions in PRs).
- **Reproducibility** (automatic script execution to regenerate diagrams).
- **Anonymization** of real environments using generic examples.

**Technologies Used**
- **Python** + [Diagrams (mingrammer)](https://github.com/mingrammer/diagrams)
- **Graphviz** as the rendering engine
- Reproducible execution via virtual environment and `requirements.txt`

**My Role & Contribution**
- Creation of a **generic multi-cloud example**, reusing different icons (Azure, GCP, Redis, Kafka, GitLab, Jenkins, Prometheus, Grafana, etc.).
- Writing documentation and a README oriented towards showcasing the project as a **didactic and portfolio tool**.
- Configuration of best practices: `.gitignore`, MIT license, clear dependencies.

**Impact / Results**
- Public repo that anyone can clone and use as an **architecture diagram template**.
- Demonstrates my ability to combine **cloud infrastructure**, **DevOps best practices**, and **clear documentation**.
- Reusable example for teams needing to diagram without exposing real infra.

**Link to full project:** [github.com/abuenoa/architecture-diagram-example](https://github.com/abuenoa/architecture-diagram-example)

> Credits: This project relies on the **Diagrams** library created by [@mingrammer](https://github.com/mingrammer), whom I thank for enabling this way of diagramming infrastructure with Python.


### ​⛅ Windy – WeatherAppBolton (Team Collaboration)

**Brief Description**
Frontend + serverless backend portal for consulting weather data.
- **Frontend:** HTML/CSS/JS, simple and responsive interface.
- **Backend:** AWS Lambda functions in Python that consume APIs (such as OpenWeather or similar) and expose data to the frontend.

**Problem Addressed**
Creating an agile and intuitive web application to check the weather, using serverless architecture to reduce infrastructure costs, improve scalability, and maintain a lightweight and efficient deployment.

**Technologies Used**
- **Frontend:** HTML, CSS, pure JavaScript (no heavy frameworks), responsive design.
- **Backend:** Python + AWS Lambda, potentially with layers or API Gateway integration.
- **Infrastructure:** Serverless (no fixed server), external APIs, deployment via GitHub Actions or manual.

**My Role as Collaborator**
- Implementation of Lambda functions to query and process weather data.
- Management of Roles and Users via IAM service.
- API management via AWS API Gateway.
- Management of Alarms and notifications via SNS and CloudWatch.
- Integration between frontend and backend, ensuring low latency.
- Assistance in end-to-end deployment and testing, including UX testing and adjustments.

**Link to full project:**
- Frontend: [WeatherAppBolton/windy-frontend](https://github.com/WeatherAppBolton/windy-frontend)
- Backend: [WeatherAppBolton/windy-backend](https://github.com/WeatherAppBolton/windy-backend)

---

## 🎓 Education

- **MSc Cloud Computing and Network Security** *(2024–2025)*
  *University of Bolton (Manchester, UK)* – DevOps, Pentesting, InfoSec, and Network Security.

- **BSc in Computer Engineering and Virtual Technologies** *(2018–2023)*
  *Universidad Loyola Andalucía (Spain)* – Specialization in web/mobile development, video games, and machine learning.
  *(Third best student in the graduating class)*

---
## 🛠️ Technical Skills

**🤖 AI Engineering & LLM Inference:**
Python 3.11+ · PyTorch · **vLLM** · Triton Inference · ONNX Runtime · LangChain · MCP · Bathing Control

**🔐 Post-Quantum Cryptography (PQC) & Security:**
**LibOQS** · OpenSSL 3.5 (OQS Provider) · **Kyber/Dilithium Implementation** · Nessus · Metasploit · Snort (IDS/IPS) · Nmap · Digital Forensics (Autopsy, Volatility)

**☁️ Cloud Native & Multi-Cloud Orchestration:**
Kubernetes (K8s) · Docker · **OpenShift** · Helm · **Dstack** · **SkyPilot** · AWS · Azure · GCP · Terraform

**🚀 High-Performance Backend:**
**Spring Boot 3 (Reactive Stack/WebFlux)** · Java (Modern Syntax) · FastAPI (Python) · Feign/ReactiveFeign · WebSocket · MinIO (S3)

**⚡ Streaming & Data Engineering:**
**Kafka** (w/ Zookeeper) · MQTT · StreamSets · NodeRed · Apache NiFi · RabbitMQ

**💾 Data Persistence:**
PostgreSQL (TimeScale) · MongoDB · Redis (Cache) · MariaDB/MySQL

**⚙️ DevOps, CI/CD & Observability:**
GitLab CI/CD · Jenkins · Grafana · Prometheus · Graylog · JMeter (Stress Testing) · JUnit/Mockito

---

## 🌍 Languages
- 🇪🇸 Spanish: Native
- 🇬🇧 English: C1 Cambridge English Certificate (July 2024)

---

## 🏆 Awards & Recognitions
- **Iberian 2025 – IT Challenge:** Top 11 out of 500+ teams.

---

✨ Thanks for visiting my profile. I am open to collaborations, interesting projects, and opportunities that challenge me professionally.
