<div align="center">

[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=28&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=800&lines=Sharif+Ullah;Full-Stack+.NET+Engineer+—+Since+2020;Clean+Architecture+%E2%80%A2+ERP+%E2%80%A2+Event-Driven+Systems;Docker+%E2%80%A2+RabbitMQ+%E2%80%A2+Keycloak+%E2%80%A2+Angular)](https://github.com/devsharif)

**Full-Stack .NET Engineer · Clean Architecture · Event-Driven Microservices**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/sharifullah)
[![NuGet](https://img.shields.io/badge/NuGet-004880?style=for-the-badge&logo=nuget&logoColor=white)](https://www.nuget.org/profiles/devsharif)
[![HackerRank](https://img.shields.io/badge/HackerRank-2EC866?style=for-the-badge&logo=hackerrank&logoColor=white)](https://www.hackerrank.com/sharifullah)
[![Gmail](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dev.sharifullah@gmail.com)
[![Location](https://img.shields.io/badge/Dhaka-Bangladesh-0AA36B?style=for-the-badge&logo=googlemaps&logoColor=white)](https://github.com/devsharif)

![Profile Views](https://komarev.com/ghpvc/?username=devsharif&label=profile+views&color=58a6ff&style=flat)

</div>

---

## Engineering Profile

<table>
<tr>
<td width="62%" valign="top">

**Sharif Ullah** — Full-Stack Software Engineer from Dhaka, Bangladesh, building production .NET systems since **2020**.

Specialized in **ASP.NET Core + Clean Architecture**: modular monoliths that evolve cleanly into **event-driven microservices** — hardened with Docker, RabbitMQ, Redis, and Keycloak SSO.

**Production track record:** ERP platforms · Diagnostic / hospital management · Payment-gateway integrations · Full-featured boilerplates · Extensions & tooling · Published NuGet packages.

- ◆ Architecture-first: SOLID, DDD, CQRS + MediatR, versioned REST APIs
- ◆ Data: SQL Server, PostgreSQL, MySQL, MongoDB, Redis — EF Core + Dapper
- ◆ Frontend: Angular, TypeScript, admin / ERP / reporting UIs
- ◆ Delivery: Docker Compose one-command stacks, GitHub Actions CI/CD, Serilog observability

</td>
<td width="38%" align="center" valign="middle">
<img src="https://raw.githubusercontent.com/devsharif/devsharif/main/gifs/coder.gif" width="100%" alt="engineering" />
<br/><sub>Music · Cycling · Gaming · Travelling</sub>
</td>
</tr>
</table>

---

## Core Stack

<div align="center">

[![Core](https://skillicons.dev/icons?i=cs,dotnet,ts,js,angular,nodejs,html,css,bootstrap,jquery&theme=dark)](https://github.com/devsharif)
<br/>
[![Data & Infra](https://skillicons.dev/icons?i=postgres,mysql,mongodb,redis,rabbitmq,kafka,docker,kubernetes,nginx,git,github,vscode,visualstudio,postman,azure&theme=dark)](https://github.com/devsharif)

![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=flat&logo=keycloak&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)
![EF Core](https://img.shields.io/badge/EF_Core-512BD4?style=flat&logo=dotnet&logoColor=white)
![MediatR CQRS](https://img.shields.io/badge/CQRS_MediatR-512BD4?style=flat&logo=dotnet&logoColor=white)
![Hangfire](https://img.shields.io/badge/Hangfire-0A0A0A?style=flat&logo=dotnet&logoColor=white)
![SignalR](https://img.shields.io/badge/SignalR-512BD4?style=flat&logo=dotnet&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=github-actions&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat&logo=microsoft-sql-server&logoColor=white)

</div>

<table>
<tr>
<td width="50%" valign="top">

**Backend**
- ASP.NET Core Web API / MVC / Minimal APIs
- Clean Architecture, DDD, CQRS + MediatR
- EF Core, Dapper, FluentValidation
- Keycloak / Identity / JWT / OAuth2 / OIDC
- Hangfire, Quartz, HostedServices

</td>
<td width="50%" valign="top">

**Distributed Systems & DevOps**
- RabbitMQ (exchanges, DLQ, retries, outbox)
- Redis cache, SignalR real-time
- Docker multi-stage + Compose stacks
- Nginx, GitHub Actions, Seq / Serilog
- Health checks, global error handling

</td>
</tr>
<tr>
<td width="50%" valign="top">

**Frontend**
- Angular 2x+, TypeScript, RxJS
- AngularJS legacy migration
- ERP / dashboard / reporting UIs
- HTML / CSS / Bootstrap, Chart.js

</td>
<td width="50%" valign="top">

**Data**
- SQL Server, PostgreSQL, MySQL
- MongoDB, Redis
- Migrations, seeding, auditing
- Reconciliation-safe payment flows

</td>
</tr>
</table>

---

## Architecture Blueprint

Standard layout for every serious backend:

```
src/
├── Domain/            # entities, value objects, domain events, interfaces
├── Application/       # CQRS handlers, DTOs, validators, pipelines, specs
├── Infrastructure/    # EF Core, RabbitMQ, Redis, Keycloak, email/SMS, jobs
└── WebApi/            # controllers / minimal APIs, middleware, versioning
```

```mermaid
flowchart LR
  Client[Angular / SPA] --> Gateway[API Gateway + Keycloak Auth]
  Gateway --> API1[Core API<br/>.NET + EF Core]
  Gateway --> API2[Domain Services<br/>.NET + CQRS]
  API1 <--> MQ[(RabbitMQ<br/>events + commands)]
  API2 <--> MQ
  MQ --> Worker[Workers<br/>Hangfire / Consumers]
  API1 --> SQL[(SQL Server / Postgres)]
  API2 --> SQL
  API2 --> Cache[(Redis)]
  Worker --> Mongo[(MongoDB / Logs)]
  API1 -.-> Docker[Docker + Compose<br/>CI/CD via Actions]
  API2 -.-> Docker
```

**Engineering defaults:** SOLID · idempotent consumers · versioned REST · EF migrations · Serilog + Seq · audit trails · `api + db + rabbitmq + keycloak + redis` up in one command.

---

## Selected Work

| Domain | Highlights |
|---|---|
| **ERP System** | Inventory, sales / purchase, HR & payroll, accounts · role-based access · reporting + audit trails |
| **Diagnostic Management** | Patient registration, test booking, lab workflow, report delivery, billing |
| **Payment Gateways** | Checkout, callbacks / webhooks, reconciliation, failure retries |
| **SU Boilerplate** | Full-featured .NET starter — Clean Architecture, auth / roles, CRUD scaffolding, notifications |
| **Extensions & Tooling** | `AngularProjectGenerator` one-click scaffold · `js-media-selector` · WinForms utilities |
| **NuGet Packages** | `SUAspNetCore.Notifier` — server-side toasts for ASP.NET Core · [nuget.org/profiles/devsharif](https://www.nuget.org/profiles/devsharif) |

→ Full index: [github.com/devsharif?tab=repositories](https://github.com/devsharif?tab=repositories)

<details>
<summary><b>SU Boilerplate — visual preview (10 screens)</b></summary>
<br/>
<p align="center">
  <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/1.png" width="49%"></img> <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/2.png" width="49%"></img> <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/3.png" width="49%"></img> <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/4.png" width="49%"></img> <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/5.png" width="49%"></img> <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/6.png" width="49%"></img> <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/7.png" width="49%"></img> <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/8.png" width="49%"></img> <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/9.png" width="49%"></img> <img src="https://raw.githubusercontent.com/devsharif/devsharif/main/project/boilerplate/10.png" width="49%"></img>
</p>
</details>

---

## Analytics

<div align="center">

![Followers](https://img.shields.io/github/followers/devsharif?style=flat&label=followers&color=58a6ff)
![Stars](https://img.shields.io/github/stars/devsharif?style=flat&label=stars&color=58a6ff)
![Repos](https://img.shields.io/github/repo-size/devsharif/devsharif?style=flat&label=profile-repo&color=58a6ff)

<br/>

![Streak](https://streak-stats.demolab.com?user=devsharif&theme=tokyonight&hide_border=true)

![Contributions](https://ghchart.rshah.org/58a6ff/devsharif)

<sub>Contribution graph + streak are live. Detailed language mix is covered in <b>Core Stack</b> above.</sub>

</div>

---

<div align="center">

**Let's build systems that scale.**

📧 **dev.sharifullah@gmail.com** · 💼 [linkedin.com/in/sharifullah](https://linkedin.com/in/sharifullah) · 📦 [nuget.org/profiles/devsharif](https://www.nuget.org/profiles/devsharif)

<sub>Clean input → solid architecture → shippable output.</sub>

</div>
