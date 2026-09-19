# Mohamed Ali Trabelsi

**Fullstack engineer** — I design product interfaces and the systems behind them.

I care about how a screen *feels* (hierarchy, spacing, motion, empty and error states) as much as how a request travels (gateway → service → data → events). Most of my work is production web, mobile, and APIs. Details stay with the teams; **skills and patterns** are what I share here.

---

## How I design software

```
  Web  ·  Mobile
        │
        ▼
  API Gateway  /  BFF
        │
   ┌────┼────────────┐
   ▼    ▼            ▼
 Auth   Domain     Workers
 (IAM)  services   (queues)
   │      │            │
   └──────┴─────┬──────┘
                ▼
         SQL  ·  Document DB
```

**Clients** are component-driven UIs on a design system, not one-off pages.  
**The edge** is a gateway or BFF: routing, auth, aggregation for web and mobile.  
**The core** is bounded services (identity vs domain), not a single ball of controllers.  
**Async** work goes on a message broker when the user should not wait.

---

## Frontend & UI engineering

I treat UI as a **system**: tokens, composition, and states — not a pile of screens.

- **Design system** — colors, type, spacing, and components reused across web and mobile
- **Composition** — small presentational pieces assembled into features (atomic / compound components)
- **Container vs presentational** — data and side effects stay out of visual components
- **States as design** — loading, empty, error, success; not only the happy path
- **Motion with purpose** — feedback and hierarchy, not decoration
- **Responsive & accessible enough to ship** — layout, contrast, focus, tap targets

**Stack I use in product UI:** TypeScript, React, Flutter, mobile (TypeScript and native), Tailwind / component libraries, design tokens.

---

## Backend & platform

- **Modular services** — controller → application → domain → persistence
- **API Gateway** — single entry for clients; services stay internal
- **IAM as its own context** — identity, sessions, tokens; not mixed into every feature
- **Repository / adapter** — business rules do not talk to the database driver
- **Pub/sub** — queues for work that is async or cross-service (e.g. RabbitMQ)
- **Contract-first HTTP** — REST resources, validation, consistent errors
- **Automated checks** — unit where it pays; **E2E** (Playwright) against real environments

**Stack I use in backends:** NestJS / Node, Java services, REST, MongoDB, SQL, Docker.

---

## Patterns I actually use

| Concern | Pattern |
|---|---|
| Product UI | Design system, composition, container / presentational |
| Client–server | BFF or API Gateway in front of services |
| Decomposition | Microservices with clear bounded contexts |
| Identity | Dedicated IAM, token-based access |
| Persistence | Repository, migrations, SQL + document where each fits |
| Coupling | Events / message queue instead of sync chains |
| Quality | E2E on recette/dev, not only local happy paths |

I do not label work “DDD / hexagonal / CQRS” unless that was the real architecture. Interviews should match the README.

---

## Stack (at a glance)

**UI** · TypeScript · React · Flutter · SwiftUI  
**API** · NestJS · Node · Java  
**Data** · PostgreSQL / MySQL · MongoDB  
**Async** · RabbitMQ  
**Quality** · Playwright · Docker

---

## What I look for

Teams that ship **interfaces people enjoy** and **backends that stay understandable** — fullstack seats where design and architecture are the same job.

---

[GitHub](https://github.com/MohamedAliTrabelsiSE)
