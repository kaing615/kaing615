<img
  width="100%"
  src="./profile-banner.svg"
  alt="Tam Nguyen Dinh | Kai Nguyen"
/>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img
      src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=21&duration=2800&pause=900&color=38BDF8&center=true&vCenter=true&width=760&lines=Software+Engineer;Node.js+%26+TypeScript+Backend;Cloud+%26+DevOps;Building+Reliable+Production+Systems"
      alt="Typing introduction"
    />
  </a>
</p>

<p align="center">
  <img
    src="https://komarev.com/ghpvc/?username=kaing615&label=PROFILE+VIEWS&color=0ea5e9&style=for-the-badge"
    alt="Profile views"
  />
  <img
    src="https://img.shields.io/badge/LOCATION-VIETNAM-0284c7?style=for-the-badge&logo=googlemaps&logoColor=white"
    alt="Location: Vietnam"
  />
  <img
    src="https://img.shields.io/badge/OPEN_TO-COLLABORATION-22c55e?style=for-the-badge"
    alt="Open to collaboration"
  />
</p>

<p align="center">
  <a href="mailto:kainguyen615@gmail.com">
    <img
      src="https://img.shields.io/badge/Email-0f172a?style=for-the-badge&logo=gmail&logoColor=white"
      alt="Email"
    />
  </a>
  <a href="https://linkedin.com/in/tamnguyendinh615">
    <img
      src="https://img.shields.io/badge/LinkedIn-0f172a?style=for-the-badge&logo=linkedin&logoColor=38bdf8"
      alt="LinkedIn"
    />
  </a>
  <a href="https://github.com/kaing615">
    <img
      src="https://img.shields.io/badge/GitHub-0f172a?style=for-the-badge&logo=github&logoColor=white"
      alt="GitHub"
    />
  </a>
  <a href="https://drive.google.com/file/d/1IdYpM2aDYfHiAtUJvQSGK_Z6H3fQV9U3/view?usp=sharing">
    <img
      src="https://img.shields.io/badge/View_Resume-0ea5e9?style=for-the-badge&logo=googledrive&logoColor=white"
      alt="View resume"
    />
  </a>
</p>

---

## `$ whoami`

I'm **Tam Nguyen Dinh**, also known as **Kai Nguyen**, a Software Engineer focused on backend development, internal platforms and reliable software delivery.

I enjoy building applications and backend services with **Node.js** and **TypeScript**, then taking them all the way to production through containers, CI/CD, cloud infrastructure and observability.

<table>
  <tr>
    <td><strong>Current role</strong></td>
    <td>Software Engineer Intern</td>
  </tr>
  <tr>
    <td><strong>Core focus</strong></td>
    <td>Backend engineering, internal platforms and software delivery</td>
  </tr>
  <tr>
    <td><strong>Currently learning</strong></td>
    <td>Node.js, TypeScript, backend architecture and cloud-native systems</td>
  </tr>
  <tr>
    <td><strong>Technical interests</strong></td>
    <td>Backend systems, platform engineering and cloud-native architecture</td>
  </tr>
  <tr>
    <td><strong>Open to</strong></td>
    <td>Software engineering, backend and platform engineering projects</td>
  </tr>
  <tr>
    <td><strong>Career goal</strong></td>
    <td>Build reliable, scalable and maintainable software systems</td>
  </tr>
</table>

---

## `$ current_focus`

```text
CODE ──► API ──► TEST ──► CONTAINERIZE ──► DEPLOY ──► OBSERVE
Node/TS   REST      CI/CD         Docker        K8s/AWS      Grafana
```

> Build useful software, automate delivery and keep production systems reliable.

### How I approach engineering

- Design maintainable backend services and APIs with clear responsibilities.
- Use TypeScript and structured application architecture to keep code predictable and easier to evolve.
- Build reproducible environments with containers and automated delivery workflows.
- Keep deployments small, traceable and easy to roll back.
- Treat monitoring and observability as part of the software lifecycle.
- Document systems and workflows so they remain maintainable by the whole team.

---

## `$ system --overview`

A software delivery architecture connecting backend services, data stores, CI/CD, containers, cloud infrastructure and observability.

```mermaid
flowchart LR
    DEV["Developer"]
    GIT["GitHub Repository"]
    API["Node.js / TypeScript API"]

    subgraph CICD["CI/CD Pipeline"]
        CI["GitHub Actions / Jenkins"]
        TEST["Build & Test"]
        SCAN["Security Scan"]
        REG["Container Registry"]
    end

    subgraph DELIVERY["GitOps Delivery"]
        ARGO["Argo CD"]
        CONFIG["Kubernetes Manifests"]
    end

    subgraph CLOUD["Cloud Infrastructure"]
        LB["Ingress / Load Balancer"]

        subgraph K8S["Kubernetes Cluster"]
            APP1["Application Pod"]
            APP2["Application Pod"]
            WORKER["Background Worker"]
        end

        DB[("PostgreSQL / MySQL")]
        CACHE[("Redis")]
        STORAGE[("Persistent Storage")]
    end

    subgraph OBS["Observability"]
        METRICS["Prometheus"]
        DASHBOARD["Grafana"]
        LOGS["Centralized Logs"]
        ALERTS["Alerting"]
    end

    DEV -->|"develop"| API
    API -->|"git push"| GIT
    GIT --> CI
    CI --> TEST
    TEST --> SCAN
    SCAN -->|"Build image"| REG

    CONFIG --> ARGO
    REG --> ARGO
    ARGO -->|"Continuous delivery"| K8S

    LB --> APP1
    LB --> APP2

    APP1 --> DB
    APP2 --> DB
    APP1 --> CACHE
    APP2 --> CACHE
    WORKER --> CACHE

    APP1 --> STORAGE
    APP2 --> STORAGE

    K8S --> METRICS
    K8S --> LOGS
    METRICS --> DASHBOARD
    METRICS --> ALERTS
```

### Deployment flow

```text
DEVELOPER
    │
    ▼
GIT PUSH
    │
    ▼
BUILD ──► TEST ──► SECURITY SCAN
    │
    ▼
CONTAINER REGISTRY
    │
    ▼
ARGO CD ──► KUBERNETES
               │
               ├──► APPLICATION
               ├──► DATABASE
               ├──► CACHE
               └──► MONITORING
```

### Engineering principles

- **Maintainable backend services:** Keep application logic structured, testable and easy to evolve.
- **Reliable data access:** Use relational databases and caching appropriately for application workloads.
- **Automated delivery:** Build, test and package applications through CI pipelines.
- **Containerized workloads:** Package services as reproducible Docker images.
- **Declarative deployment:** Manage Kubernetes resources through version-controlled manifests.
- **GitOps workflow:** Use Argo CD to synchronize declared and running states.
- **Observable systems:** Collect metrics, logs, dashboards and operational alerts.
- **Secure pipeline:** Add dependency, source-code and container-image scanning before deployment.

---

## `$ toolkit --list`

### Backend & Software Engineering

<p align="left">
  <img
    src="https://skillicons.dev/icons?i=ts,nodejs,express,js,postman,git&perline=6"
    alt="Backend and software engineering technologies"
  />
</p>

### Databases & Caching

<p align="left">
  <img
    src="https://skillicons.dev/icons?i=mongodb,mysql,postgres,redis&perline=4"
    alt="Databases and caching technologies"
  />
</p>

### Cloud, Infrastructure & DevOps

<p align="left">
  <img
    src="https://skillicons.dev/icons?i=aws,docker,kubernetes,jenkins,githubactions,grafana,linux,bash&perline=8"
    alt="Cloud infrastructure and DevOps technologies"
  />
</p>

<p align="left">
  <img
    src="https://img.shields.io/badge/Argo_CD-EF7B4D?style=flat-square&logo=argo&logoColor=white"
    alt="Argo CD"
  />
  <img
    src="https://img.shields.io/badge/CI%2FCD-0EA5E9?style=flat-square&logo=githubactions&logoColor=white"
    alt="CI/CD"
  />
  <img
    src="https://img.shields.io/badge/Automation-22C55E?style=flat-square&logo=gnubash&logoColor=white"
    alt="Automation"
  />
  <img
    src="https://img.shields.io/badge/Observability-F97316?style=flat-square&logo=grafana&logoColor=white"
    alt="Observability"
  />
</p>

### Additional Development Tools

<p align="left">
  <img
    src="https://skillicons.dev/icons?i=react,nextjs,html,css,python,fastapi,pytorch,tensorflow,sklearn&perline=9"
    alt="Additional development technologies"
  />
</p>

---

## `$ capabilities --summary`

| Area | Technologies and practices |
| --- | --- |
| **Backend** | Node.js, TypeScript, Express and REST API development |
| **Databases** | PostgreSQL, MySQL, MongoDB and Redis |
| **Containers** | Docker, container images, volumes, networking and Docker Compose |
| **CI/CD** | GitHub Actions, Jenkins, automated build, test and deployment workflows |
| **Cloud** | AWS fundamentals, cloud infrastructure and deployment architecture |
| **Orchestration** | Kubernetes fundamentals, workloads, services and configuration |
| **GitOps** | Argo CD and declarative application delivery |
| **Observability** | Grafana, monitoring concepts, metrics and service visibility |
| **Automation** | Bash, Python scripting and repeatable operational workflows |
| **Systems** | Linux administration, networking and troubleshooting |

---

## `$ github --stats`

<p align="center">
  <img
    width="70%"
    src="https://streak-stats.demolab.com?user=kaing615&theme=github-dark-blue&hide_border=true&border_radius=12"
    alt="GitHub contribution streak"
  />
</p>

---

## `$ connect --with-me`

<p align="center">
  Interested in software engineering, backend systems or cloud-native platforms?
  <br />
  Feel free to contact me about projects, internship opportunities or technical collaboration.
</p>

<p align="center">
  <a href="mailto:kainguyen615@gmail.com">
    <img
      src="https://img.shields.io/badge/kainguyen615%40gmail.com-0ea5e9?style=for-the-badge&logo=gmail&logoColor=white"
      alt="Email address"
    />
  </a>
  <a href="https://linkedin.com/in/tamnguyendinh615">
    <img
      src="https://img.shields.io/badge/Connect_on_LinkedIn-0f172a?style=for-the-badge&logo=linkedin&logoColor=38bdf8"
      alt="Connect on LinkedIn"
    />
  </a>
</p>

<details>
  <summary><strong>Personal social profiles</strong></summary>

  <br />

  <p align="left">
    <a href="https://facebook.com/dtam215">
      <img
        src="https://img.shields.io/badge/Facebook-0f172a?style=flat-square&logo=facebook&logoColor=38bdf8"
        alt="Facebook"
      />
    </a>
    <a href="https://instagram.com/dtam_.21">
      <img
        src="https://img.shields.io/badge/Instagram-0f172a?style=flat-square&logo=instagram&logoColor=fb7185"
        alt="Instagram"
      />
    </a>
  </p>
</details>

<br />

<p align="center">
  <sub>Building software. Automating delivery. Running it reliably.</sub>
</p>

<img
  width="100%"
  src="https://capsule-render.vercel.app/api?type=waving&color=0%3A0ea5e9%2C50%3A0f172a%2C100%3A020617&height=120&section=footer"
  alt="Footer"
/>
