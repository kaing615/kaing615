<img
width="100%"
src="https://capsule-render.vercel.app/api?type=waving&color=0%3A020617%2C50%3A0f172a%2C100%3A0ea5e9&height=240&section=header&text=Tam%20Nguyen%20Dinh%20%7C%20Kai%20Nguyen&fontSize=40&fontColor=e2e8f0&fontAlignY=38&desc=Aspiring%20DevOps%20Engineer%20%7C%20Cloud%20%26%20Automation&descAlignY=59&descSize=18&animation=fadeIn"
alt="Tam Nguyen Dinh | Kai Nguyen"
/>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img
      src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=21&duration=2800&pause=900&color=38BDF8&center=true&vCenter=true&width=760&lines=Aspiring+DevOps+Engineer;Cloud+%26+Automation+Enthusiast;Docker+%7C+Kubernetes+%7C+CI%2FCD;Building+Reliable+Cloud-Native+Systems"
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

I'm **Tam Nguyen Dinh**, also known as **Kai Nguyen**, a DevOps Engineer focused on building reliable, automated and observable software delivery workflows.

I enjoy transforming application code into repeatable infrastructure through containers, CI/CD pipelines, cloud services and automation.

<table>
  <tr>
    <td><strong>Current role</strong></td>
    <td>DevOps Engineer Intern</td>
  </tr>
  <tr>
    <td><strong>Core focus</strong></td>
    <td>Cloud infrastructure, containers and CI/CD</td>
  </tr>
  <tr>
    <td><strong>Currently learning</strong></td>
    <td>Kubernetes, Argo CD, GitHub Actions and advanced CI/CD</td>
  </tr>
  <tr>
    <td><strong>Technical interests</strong></td>
    <td>Automation, observability and cloud-native architecture</td>
  </tr>
  <tr>
    <td><strong>Open to</strong></td>
    <td>DevOps, backend and cloud-native projects</td>
  </tr>
  <tr>
    <td><strong>Career goal</strong></td>
    <td>Build secure, scalable and developer-friendly platforms</td>
  </tr>
</table>

---

## `$ current_focus`

```text
SOURCE ──► BUILD ──► TEST ──► CONTAINERIZE ──► DEPLOY ──► OBSERVE
  Git        CI/CD             Docker          K8s          Grafana
                                              Argo CD
```

> Automate repetitive work, keep deployments predictable and make systems observable.

### How I approach engineering

* Automate repeatable processes to reduce manual errors.
* Build reproducible environments using containers and infrastructure configuration.
* Keep deployments small, traceable and easy to roll back.
* Add monitoring and observability instead of treating them as afterthoughts.
* Document workflows so systems remain maintainable by the whole team.

---

---

## `$ infrastructure --overview`

<p align="left">
  A cloud-native delivery architecture that connects source control, CI/CD, containers, Kubernetes, GitOps and observability.
</p>

```mermaid
flowchart LR
    DEV["Developer"]
    GIT["GitHub Repository"]

    subgraph CICD["CI/CD Pipeline"]
        CI["GitHub Actions<br/>Jenkins"]
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

    DEV -->|"git push"| GIT
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

### Infrastructure principles

* **Automated delivery:** Build, test and package applications through CI pipelines.
* **Containerized workloads:** Package services as reproducible Docker images.
* **Declarative deployment:** Manage Kubernetes resources through version-controlled manifests.
* **GitOps workflow:** Use Argo CD to synchronize declared and running states.
* **Scalable services:** Run multiple application replicas behind an ingress layer.
* **Observable systems:** Collect metrics, logs, dashboards and operational alerts.
* **Persistent data:** Separate stateless application workloads from databases and storage.
* **Secure pipeline:** Add dependency, source-code and container-image scanning before deployment.

## `$ toolkit --list`

### Cloud, Infrastructure & DevOps

<p align="left">
  <img
    src="https://skillicons.dev/icons?i=aws,docker,kubernetes,jenkins,githubactions,grafana,linux,bash,git&perline=9"
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

### Backend & Programming Languages

<p align="left">
  <img
    src="https://skillicons.dev/icons?i=nodejs,express,fastapi,python,js,ts&perline=6"
    alt="Backend technologies and programming languages"
  />
</p>

### Databases & Caching

<p align="left">
  <img
    src="https://skillicons.dev/icons?i=mongodb,mysql,postgres,redis&perline=4"
    alt="Databases and caching technologies"
  />
</p>

### Web, AI & Development Tools

<p align="left">
  <img
    src="https://skillicons.dev/icons?i=react,nextjs,html,css,pytorch,tensorflow,sklearn,postman&perline=8"
    alt="Web, artificial intelligence and development tools"
  />
</p>

---

## `$ capabilities --summary`

| Area              | Technologies and practices                                              |
| ----------------- | ----------------------------------------------------------------------- |
| **Containers**    | Docker, container images, volumes, networking and Docker Compose        |
| **Orchestration** | Kubernetes fundamentals, workloads, services and configuration          |
| **CI/CD**         | GitHub Actions, Jenkins, automated build, test and deployment workflows |
| **GitOps**        | Argo CD and declarative application delivery                            |
| **Cloud**         | AWS fundamentals, cloud infrastructure and deployment architecture      |
| **Observability** | Grafana, monitoring concepts, metrics and service visibility            |
| **Automation**    | Bash, Python scripting and repeatable operational workflows             |
| **Backend**       | Node.js, Express, FastAPI and REST API development                      |
| **Systems**       | Linux administration, networking and troubleshooting                    |

---

## `$ github --stats`

<p align="center">
  <img
    height="170"
    src="https://github-readme-stats.vercel.app/api?username=kaing615&show_icons=true&theme=github_dark&hide_border=true&border_radius=12&rank_icon=github&include_all_commits=true"
    alt="GitHub statistics"
  />
  <img
    height="170"
    src="https://github-readme-stats.vercel.app/api/top-langs/?username=kaing615&layout=compact&theme=github_dark&hide_border=true&border_radius=12&langs_count=8"
    alt="Most used programming languages"
  />
</p>

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
  Interested in DevOps, backend or cloud-native engineering?
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
  <sub>Learning continuously. Automating thoughtfully. Building reliably.</sub>
</p>

<img
width="100%"
src="https://capsule-render.vercel.app/api?type=waving&color=0%3A0ea5e9%2C50%3A0f172a%2C100%3A020617&height=120&section=footer"
alt="Footer"
/>
