# 👋 Hi, I'm Antonio Bueno Antón

Engineer specializing in **Cloud Computing**, **backend development**, and **cloud security**, with experience in secure infrastructure deployment using **Docker** and **Kubernetes**. I am currently pursuing a **Master's in Cloud Computing and Network Security** at the *University of Bolton* (UK).

I am proactive, flexible, and passionate about teamwork, always maintaining high standards of quality and professionalism.

📫 **Quick Contact:**
- 📧 **Email:** antonio.buenoanton@gmail.com
- 📞 **Phone:** +34 637 397 160
- 💼 **LinkedIn:** [linkedin.com/in/abuenoan](https://www.linkedin.com/in/abuenoan)

---

## 💻 Professional Experience

### 🟢 Technical Director & Lead Engineer | **Omega AI** (May 2025 – Present, Alicante, Spain / Remote)
* **Strategic Leadership & PQC Security:** Directing the technical vision for a secure "binary-to-quantum" AI platform. I supervise the implementation of **Post-Quantum Cryptography (PQC)** standards, specifically applying algorithms like **Dilithium** to ensure cloud security and cryptographic resilience against quantum attacks.
* **Rapid Career Progression:** Advanced from *Team Leader* to *Technical Director* in under 4 months, taking ownership of the entire engineering roadmap, workflow definition, and team coordination (Jira, GitLab).
* **AI Backend Development:** Architecting the core API infrastructure using **Python (FastAPI, Uvicorn)** for real-time LLM inference (integrating **vLLM** and **llama.cpp** with SSE streaming) and voice features.
* **DevOps & Cloud Architecture:** Managing end-to-end pipelines via **GitLab CI/CD** and orchestrating secure multi-cloud deployments (**Azure, AWS, GCP**) using **Docker**. I ensure rigorous security standards and monitor system performance with **Grafana** and **Prometheus**.

### 🔵 Software Analyst | **Minsait** (Jan 2023 – Nov 2024, Seville, Spain)
- Backend development in **Java SpringBoot** on Docker and deployment on **OpenShift/Kubernetes**.
- Signal management with **MQTT**, **NodeRed**, and **StreamSets**.
- Administration of SQL and NoSQL databases.
- Full stack development (HTML, CSS, JS, Thymeleaf) and testing (JUnit, Mockito, JMeter).
- Client support via *on-call* shifts.

### 🔵 Solution Assistant | **NTT DATA** (Nov 2021 – Jan 2023, Seville, Spain)
- Backend development in **Java, SpringBoot, JSP, Jasper**.
- Migration from monoliths to microservices.
- SQL and NoSQL database queries.
- Debugging and incident resolution in virtualized environments.
- Documentation and direct client interaction.

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
