<p align="center">
  <img src="assets/header.png" alt="Mohamed Ali Trabelsi — Fullstack engineer" width="900" />
</p>

<p align="center">
  Hierarchy, spacing, motion, empty and error states —<br />
  the same standard as gateway → service → data → events.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/TypeScript-0b0d11?style=flat-square&logo=typescript&logoColor=3178C6" alt="TypeScript" />
  <img src="https://img.shields.io/badge/React-0b0d11?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Flutter-0b0d11?style=flat-square&logo=flutter&logoColor=02569B" alt="Flutter" />
  <img src="https://img.shields.io/badge/SwiftUI-0b0d11?style=flat-square&logo=swift&logoColor=F05138" alt="SwiftUI" />
  <img src="https://img.shields.io/badge/NestJS-0b0d11?style=flat-square&logo=nestjs&logoColor=E0234E" alt="NestJS" />
  <img src="https://img.shields.io/badge/Java-0b0d11?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/PostgreSQL-0b0d11?style=flat-square&logo=postgresql&logoColor=4169E1" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/MongoDB-0b0d11?style=flat-square&logo=mongodb&logoColor=47A248" alt="MongoDB" />
  <img src="https://img.shields.io/badge/RabbitMQ-0b0d11?style=flat-square&logo=rabbitmq&logoColor=FF6600" alt="RabbitMQ" />
  <img src="https://img.shields.io/badge/Docker-0b0d11?style=flat-square&logo=docker&logoColor=2496ED" alt="Docker" />
  <img src="https://img.shields.io/badge/Playwright-0b0d11?style=flat-square&logo=playwright&logoColor=2EAD33" alt="Playwright" />
</p>

---

<p align="center">
  <img src="assets/architecture.png" alt="Architecture: clients, gateway, IAM, domain services, queues, data" width="900" />
</p>

---

<table>
  <tr>
    <td width="50%" valign="top">

### Interface

UI is a **system**: tokens, composition, states — not a pile of screens.

- **Design system** — color, type, spacing, shared components across web and mobile
- **Composition** — small presentational pieces assembled into features
- **Separation** — data and side effects stay out of visual components
- **States** — loading, empty, error, success are designed, not leftover
- **Motion** — feedback and hierarchy, never decoration
- **Ship bar** — contrast, focus, tap targets, responsive layout

    </td>
    <td width="50%" valign="top">

### Platform

The backend should stay **readable** after the product ships.

- **Layers** — controller → application → domain → persistence
- **Gateway** — one entry for clients; services stay internal
- **IAM** — identity is its own context, not mixed into every feature
- **Adapters** — domain rules do not talk to the database driver
- **Events** — queues for async and cross-service work
- **Contracts** — REST, validation, consistent errors, E2E on real environments

    </td>
  </tr>
</table>

---

### Patterns I actually use

| Layer | What I reach for |
|:---|:---|
| Product UI | Design system · composition · container / presentational |
| Client–server | BFF or API gateway in front of services |
| Decomposition | Microservices with clear bounded contexts |
| Identity | Dedicated IAM · token-based access |
| Persistence | Repository · migrations · SQL + document where each fits |
| Coupling | Message queue instead of synchronous chains |
| Quality | Playwright against recette / dev — not only local happy paths |

I do not label work DDD, hexagonal, or CQRS unless that was the real architecture.

---

<p align="center">
  Looking for fullstack seats where <strong>design and architecture are the same job</strong>.<br />
  <a href="https://github.com/MohamedAliTrabelsiSE">github.com/MohamedAliTrabelsiSE</a>
</p>
