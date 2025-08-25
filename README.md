# 👋 Hola, soy Antonio Bueno Antón  

Ingeniero especializado en **Cloud Computing**, **desarrollo backend** y **seguridad en la nube**, con experiencia en despliegue seguro de infraestructuras usando **Docker** y **Kubernetes**. Actualmente curso un **Máster en Cloud Computing y Seguridad de Redes** en la *University of Bolton* (Reino Unido).  
Soy proactivo, flexible y me apasiona trabajar en equipo, manteniendo siempre altos estándares de calidad y profesionalidad.  

📫 **Contacto rápido:**  
- 📧 **Email:** antonio.buenoanton@gmail.com  
- 📞 **Teléfono:** +34 637 397 160  
- 💼 **LinkedIn:** [linkedin.com/in/abuenoan](https://www.linkedin.com/in/abuenoan)  

---

## 💻 Experiencia Profesional  

### 🟢 Lead Backend Engineer & DevOps Coordinator | **Omega – SEL Employer** (Jun 2025 – Actualidad, Alicante, España)  
- Desarrollo de APIs en **Python** (FastAPI, Uvicorn) para inferencia de modelos con **vLLM** y **llama.cpp**.  
- Orquestación de servicios con Docker Compose y creación de UIs con **React** y **Streamlit**.  
- Liderazgo técnico: definición de workflows, asignación de tareas, revisión de código y coordinación de equipo.  
- Gestión completa de pipelines DevOps: **GitLab CI/CD**, despliegues en **Azure, AWS y GCP**, aprovisionamiento de infraestructura y automatización.  
- Integración de herramientas colaborativas (Slack, Jira) y aseguramiento de calidad en las entregas.  

### 🔵 Analista de Software | **Minsait** (Ene 2023 – Nov 2024, Sevilla, España)  
- Backend en **Java SpringBoot** sobre Docker y despliegue en **OpenShift/Kubernetes**.  
- Gestión de señales con **MQTT**, **NodeRed** y **StreamSets**.  
- Administración de BBDD SQL y NoSQL.  
- Desarrollo full stack (HTML, CSS, JS, Thymeleaf) y testing (JUnit, Mockito, JMeter).  
- Soporte a cliente mediante guardias *in-call*.  

### 🔵 Solution Assistant | **NTT DATA** (Nov 2021 – Ene 2023, Sevilla, España)  
- Desarrollo backend en **Java, SpringBoot, JSP, Jasper**.  
- Migración de monolitos a microservicios.  
- Consultas a BBDD SQL y NoSQL.  
- Debugging e incidencias en entornos virtualizados.  
- Documentación y trato directo con cliente.  

---

## 🚀 Proyectos Destacados

### 🛡️ ACR Vulnerability Density
**Descripción breve**  
Pipeline empírico y reproducible para analizar la densidad de vulnerabilidades y su evolución temporal en imágenes base almacenadas en Azure Container Registry (ACR), usando Trivy. Escanea imágenes seleccionadas en cuatro momentos (T0–T3), consolida los resultados y genera gráficos listos para tu TFM o análisis académico.

**Problema abordado**  
Las imágenes base (como `alpine`, `debian-slim`, `ubuntu`, etc.) cambian con el tiempo, y sus vulnerabilidades pueden crecer o desplazarse incluso sin modificaciones directas. Este proyecto cuantifica ese **drift de vulnerabilidades**, ayudando a evaluar riesgos recurrentes en pipelines de CI/CD.

**Tecnologías usadas**  
- Infraestructura como código: **Terraform** (infraestructura ACR + RG en Azure)  
- Automatización de procesos: Shell scripts (`bash`) para login, pull/tag/push, escaneo con Trivy  
- Análisis y visualización: **Python** (pandas + matplotlib)  
- Diseño reproducible: `Makefile`, versiones fijadas (`pyenv`, Trivy DB), logs de herramientas para trazabilidad

**Impacto / Resultados**  
- Permite medir la densidad de vulnerabilidad normalizada por MB: `(CRITICAL + HIGH) / size_mb`  
- Generación de CSV comparativos y gráficos semanales (T0 a T3) con evolución de CVEs y crecimiento acumulado  
- Alta reproducibilidad: versiones del escáner, identidades de paquetes y timestamps registrados automáticamente

**Enlace al proyecto completo:** [github.com/abuenoa/acr-vuln-density](https://github.com/abuenoa/acr-vuln-density)  


### 🗂️ Architecture Diagram – Diagram-as-Code
**Descripción breve**  
Repositorio público de ejemplo en el que muestro cómo crear **diagramas de arquitectura como código** utilizando la librería [Diagrams de Mingrammer](https://diagrams.mingrammer.com/).  
El proyecto genera un **diagrama multi-cloud genérico** (usuarios → CDN → WAF → Load Balancer → Web/API → Cache/Workers/DB, junto con CI/CD y observabilidad), demostrando buenas prácticas de documentación de arquitecturas sin exponer información sensible.

**Problema abordado**  
La documentación de arquitecturas suele quedar obsoleta rápidamente cuando se hace en diagramas manuales (Visio, Draw.io, etc.). Con un enfoque *diagram-as-code* se obtiene:
- **Versionado en Git** (histórico de cambios y revisiones en PRs).  
- **Reproducibilidad** (ejecución automática del script para regenerar diagramas).  
- **Anonimización** de entornos reales mediante ejemplos genéricos.

**Tecnologías usadas**  
- **Python** + [Diagrams (mingrammer)](https://github.com/mingrammer/diagrams)  
- **Graphviz** como motor de renderizado  
- Ejecución reproducible mediante entorno virtual y `requirements.txt`

**Mi rol y aportación**  
- Creación de un **ejemplo multi-cloud genérico**, reutilizando distintos iconos (Azure, GCP, Redis, Kafka, GitLab, Jenkins, Prometheus, Grafana, etc.).  
- Redacción de documentación y README orientados a mostrar el proyecto como **herramienta didáctica y de portfolio**.  
- Configuración de buenas prácticas: `.gitignore`, licencia MIT, dependencias claras.  

**Impacto / Resultados**  
- Repo público que cualquiera puede clonar y usar como **plantilla de diagramas de arquitectura**.  
- Proyecto que muestra mi capacidad de combinar **infraestructura cloud**, **buenas prácticas de DevOps** y **documentación clara**.  
- Ejemplo reutilizable para equipos que necesiten diagramar sin exponer infra real.  

**Enlace al proyecto completo:** [github.com/abuenoa/architecture-diagram-example](https://github.com/abuenoa/architecture-diagram-example)  

> Créditos: este proyecto se apoya en la librería **Diagrams** creada por [@mingrammer](https://github.com/mingrammer), a quien agradezco por hacer posible esta forma de diagramar infraestructuras con Python.  


### ​⛅ Windy – WeatherAppBolton (colaboración de equipo)

**Descripción breve**  
Portal frontend + backend serverless para consultar datos meteorológicos.  
- **Frontend:** HTML/CSS/JS, interfaz sencilla y responsive.  
- **Backend:** Funciones AWS Lambda en Python que consumen APIs (outras como OpenWeather o similares) y exponen datos al frontend.

**Problema abordado**  
Crear una aplicación web ágil e intuitiva para consultar el tiempo, utilizando arquitectura serverless para reducir costes de infraestructura, escalabilidad y mantener un despliegue ligero y eficiente.

**Tecnologías usadas**  
- **Frontend:** HTML, CSS, JavaScript puro (sin frameworks pesados), diseño responsive.  
- **Backend:** Python + AWS Lambda, posiblemente con layers o integración con API Gateway.  
- **Infraestructura:** Serverless (sin servidor fijo), APIs externas, despliegue a través de GitHub Actions o manual.

**Mi rol como colaborador**  
- Implementación de funciones Lambda para consultar y procesar datos meteorológicos.
- Gestión de Roles y Usuarios mediante el servicio IAM.
- Gestión de APIs mediante API Gateway en AWS.
- Gestión de Alarmas y notificaciones mediante SNS y CloudWatch.
- Integración entre frontend y backend, garantizando baja latencia.  
- Asistencia en despliegue y testing de extremo a extremo (end-to-end), incluyendo pruebas y ajustes UX.

**Enlace al proyecto completo:**  
- Frontend: [WeatherAppBolton/windy-frontend](https://github.com/WeatherAppBolton/windy-frontend)  
- Backend: [WeatherAppBolton/windy-backend](https://github.com/WeatherAppBolton/windy-backend)


## 🎓 Formación  

- **MSc Cloud Computing and Network Security** *(2024–2025)*  
  *University of Bolton (Manchester, UK)* – DevOps, Pentesting, InfoSec y seguridad de redes.  

- **Grado en Ingeniería Informática y Tecnologías Virtuales** *(2018–2023)*  
  *Universidad Loyola Andalucía (España)* – Especialización en desarrollo web/móvil, videojuegos y machine learning.  
  *(Tercer mejor estudiante de la promoción)*  

---

## 🛠️ Habilidades Técnicas  

**Lenguajes de programación:**  
Java (SpringBoot) · Python (FastAPI) · HTML/CSS/JavaScript/PHP · Bash  

**Infraestructura Cloud:**  
Kubernetes · Docker · AWS EKS · OpenShift · Azure · GCP · Terraform · Helm  

**Bases de datos:**  
SQL · MongoDB · PostgreSQL · Redis  

**CI/CD & DevOps:**  
GitLab · Jenkins · GitHub Actions · SonarQube · Jira · SourceTree  

**Streaming y datos en tiempo real:**  
Kafka · MQTT · Zookeeper · StreamSets · NodeRed  

**Monitorización y testing:**  
Grafana · JMeter · JUnit · Mockito · Graylog · TestLink  

---

## 🌍 Idiomas  
- 🇪🇸 Español: Nativo  
- 🇬🇧 Inglés: C1 Cambridge English Certificate (Julio 2024)  

---

## 🏆 Premios y Reconocimientos  
- **Iberian 2025 – IT Challenge:** Top 11 de 500+ equipos.  

---

📄 **CV completo en PDF:** [Descargar aquí](mailto:antonio.buenoanton@gmail.com)  

✨ Gracias por visitar mi perfil. Estoy abierto a colaboraciones, proyectos interesantes y oportunidades que me reten profesionalmente.  
