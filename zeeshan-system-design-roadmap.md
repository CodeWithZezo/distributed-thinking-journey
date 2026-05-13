# 🏗️ HLD + LLD System Design Roadmap (Weekends)

> **For:** Zeeshan Saleem
> **Duration:** 8 weekends (parallel with distributed thinking roadmap)
> **Market target:** Pakistani/Indian companies (Careem, Zameen, Bazaar, Bykea, Foodpanda, Daraz, Systems Limited, Devsinc, Folio3, Arbisoft, Tintash, etc.)
> **Goal:** Pass system design + LLD rounds in mid-tier company interviews
> **Approach:** Pure thinking + paper designs, no projects

---

## 📑 Table of Contents

### 📋 Intro Sections
- [Why This Roadmap Hits Different](#-why-this-roadmap-hits-different)
- [8-Weekend Overview](#-8-weekend-overview)
- [Weekend Structure](#-weekend-structure)
- [Notes System](#-notes-system)
- [Pakistani Market Specifics](#-pakistani-market-specifics-important)

### 🗓️ WEEKEND 1: Foundations
- [Saturday (Day 1) — HLD Framework & Approach](#saturday--hld-framework--approach)
  - [The Universal HLD Framework](#the-universal-hld-framework-1-hour)
  - [Non-Functional Requirements Concept](#concept-non-functional-requirements-15-min)
  - [Case Study: Foodpanda Backend](#case-study-45-min)
  - [Exercise: Design ATM System](#exercise-design-atm-system-hld-style-1-hour)
- [Sunday (Day 2) — OOP Refresh + SOLID](#sunday--oop-refresh--solid)
  - [OOP Pillars Re-Examined](#oop-pillars-re-examined-1-hour)
  - [SOLID Principles Deep](#solid-principles-deep-15-hours)
  - [Exercise: SOLID Smell Hunt](#exercise-solid-smell-hunt-1-hour)

### 🗓️ WEEKEND 2: Databases + Design Patterns (Creational)
- [Saturday (Day 3) — Database Design for Interviews](#saturday--database-design-for-interviews)
  - [The Database Decision Framework](#the-database-decision-framework-1-hour)
  - [Schema Design Principles](#schema-design-principles-1-hour)
  - [Exercise: Design Foodpanda Order DB](#exercise-design-foodpanda-order-db-15-hours)
- [Sunday (Day 4) — Creational Design Patterns](#sunday--creational-design-patterns)
  - [1. Singleton](#1-singleton-15-min)
  - [2. Factory Method](#2-factory-method-15-min)
  - [3. Abstract Factory](#3-abstract-factory-15-min)
  - [4. Builder](#4-builder-15-min)
  - [5. Prototype](#5-prototype-10-min)
  - [Exercise: When to Use Which?](#exercise-when-to-use-which-45-min)

### 🗓️ WEEKEND 3: Caching + Structural Patterns
- [Saturday (Day 5) — Caching for HLD Interviews](#saturday--caching-for-hld-interviews)
  - [When to Mention Caching](#when-to-mention-caching-in-interview-30-min)
  - [Cache Layers In Real Systems](#cache-layers-in-real-systems-45-min)
  - [Cache Invalidation Strategies](#cache-invalidation-strategies-30-min)
  - [CDN Concept](#cdn-concept-30-min)
  - [Exercise: Add Caching to Foodpanda](#exercise-add-caching-to-foodpanda-15-hours)
- [Sunday (Day 6) — Structural Design Patterns](#sunday--structural-design-patterns)
  - [1. Adapter](#1-adapter-20-min)
  - [2. Facade](#2-facade-20-min)
  - [3. Decorator](#3-decorator-20-min)
  - [4. Proxy](#4-proxy-15-min)
  - [5. Composite](#5-composite-15-min)
  - [6. Bridge](#6-bridge-10-min)
  - [Exercise: Design Library Management LLD](#exercise-design-library-management-lld-15-hours)

### 🗓️ WEEKEND 4: Load Balancing + Behavioral Patterns
- [Saturday (Day 7) — Load Balancing + Queues in HLD](#saturday--load-balancing--queues-in-hld)
  - [Load Balancer Concept](#load-balancer-concept-45-min)
  - [Health Checks](#health-checks-15-min)
  - [Queues Refresh for HLD](#queues-refresh-for-hld-1-hour)
  - [Exercise: Add LB + Queue to ATM System](#exercise-add-lb--queue-to-atm-system-15-hours)
- [Sunday (Day 8) — Behavioral Design Patterns](#sunday--behavioral-design-patterns)
  - [1. Observer](#1-observer-25-min)
  - [2. Strategy](#2-strategy-25-min)
  - [3. Command](#3-command-20-min)
  - [4. State](#4-state-20-min)
  - [5. Template Method](#5-template-method-15-min)
  - [6. Chain of Responsibility](#6-chain-of-responsibility-15-min)
  - [7. Iterator](#7-iterator-5-min)
  - [Exercise: Design Vending Machine LLD](#exercise-design-vending-machine-lld-2-hours)

### 🗓️ WEEKEND 5: URL Shortener (HLD) + Parking Lot (LLD)
- [Saturday (Day 9) — URL Shortener Full HLD](#saturday--url-shortener-most-asked-hld-question)
  - [Step 1: Requirements](#step-1-requirements-15-min)
  - [Step 2: Capacity Estimation](#step-2-capacity-estimation-15-min)
  - [Step 3: API Design](#step-3-api-design-15-min)
  - [Step 4: Data Model](#step-4-data-model-20-min)
  - [Step 5: High-Level Architecture](#step-5-high-level-architecture-20-min)
  - [Step 6: Deep Dives](#step-6-deep-dives-30-min)
  - [Step 7: Scale + Failures](#step-7-scale--failures-20-min)
- [Sunday (Day 10) — Parking Lot LLD](#sunday--parking-lot-lld)
  - [Requirements](#requirements-15-min)
  - [Class Design](#class-design-15-hours)
  - [Key Design Decisions To Articulate](#key-design-decisions-to-articulate)
  - [Sequence Diagrams](#sequence-diagram-vehicle-enters)

### 🗓️ WEEKEND 6: Twitter Feed (HLD) + Splitwise (LLD)
- [Saturday (Day 11) — Twitter/Instagram Feed](#saturday--twitterinstagram-feed-hard-hld)
  - [Why This Is Hard](#why-this-is-hard)
  - [Requirements + Capacity](#requirements-15-min-1)
  - [The Fan-out Problem](#the-fan-out-problem-45-min)
  - [Architecture](#architecture-30-min)
  - [Trade-offs To Articulate](#trade-offs-to-articulate-30-min)
- [Sunday (Day 12) — Splitwise LLD](#sunday--splitwise-lld)
  - [Requirements](#requirements-15-min-2)
  - [Class Design](#class-design-15-hours-1)
  - [Algorithm: Simplify Debts](#algorithm-simplify-debts-important)

### 🗓️ WEEKEND 7: Uber/Careem (HLD) + Chess (LLD)
- [Saturday (Day 13) — Ride-Sharing System (Uber/Careem)](#saturday--ride-sharing-system-ubercareem)
  - [Why Best Question For Pak Market](#why-this-is-the-best-question-for-pak-market)
  - [Requirements + Capacity](#requirements-20-min)
  - [Core Components](#core-components-45-min)
  - [The Matching Problem](#the-matching-problem-45-min)
  - [Real-Time Location Updates](#real-time-location-updates-30-min)
  - [Surge Pricing](#surge-pricing-15-min)
- [Sunday (Day 14) — Chess Game LLD](#sunday--chess-game-lld)
  - [Requirements](#requirements-15-min-3)
  - [Class Design](#class-design-2-hours)
  - [Key Design Decisions](#key-design-decisions)
  - [Patterns Used](#patterns-used)

### 🗓️ WEEKEND 8: Mock Interviews + Synthesis
- [Saturday (Day 15) — HLD Mock Interview Marathon](#saturday--hld-mock-interview-marathon)
  - [Mock 1: Notification System](#mock-1-design-a-notification-system-that-handles-1m-notificationsday)
  - [Mock 2: Bykea's Backend](#mock-2-design-bykeas-backend-motorcycle-ride-sharing-in-pakistan)
  - [Mock 3: Library Management](#mock-3-design-a-library-management-system)
  - [Self-Review Checklist](#self-review-checklist)
- [Sunday (Day 16) — LLD Mock + Final Synthesis](#sunday--lld-mock--final-synthesis)
  - [LLD Mock Interview](#lld-mock-interview-2-hours)
  - [Final Synthesis Document](#final-synthesis-document-2-hours)
  - [LinkedIn Capstone Post](#linkedin-capstone-post)

### 🎯 End Sections
- [Post-Roadmap Outputs](#-post-roadmap-outputs)
- [Master Resource List](#-master-resource-list)
- [Realistic Expectations](#-realistic-expectations)
- [Pehla Step Aaj](#-pehla-step-aaj)
- [Job Hunt Strategy (Bonus)](#-job-hunt-strategy-bonus)

---

## 🎯 Why This Roadmap Hits Different

Pichle "thinking roadmap" mein tum **distributed systems concepts** seekh rahe ho.
Yahan **interview-specific structure** seekhoge — *kaise* socho, *kaise* communicate karo, *kaise* sound senior in 45 minutes.

**Pakistani market reality check:**
- Companies FAANG-level system design questions nahi poochti
- Lekin **fundamentals** strict hain — capacity estimation, DB choice, API design
- **LLD zyada important** mid-tier companies mein — kyunki actual codebase pe kaam karna hai
- **Trade-off articulation** = senior signal

---

## 📅 8-Weekend Overview

| Weekend | HLD Focus | LLD Focus |
|---|---|---|
| 1 | Framework + Approach | OOP refresh + SOLID |
| 2 | Database design + APIs | Design patterns (creational) |
| 3 | Caching + CDN | Design patterns (structural) |
| 4 | Load balancing + Queues | Design patterns (behavioral) |
| 5 | URL Shortener (full design) | Parking Lot LLD |
| 6 | Twitter/Instagram feed | Splitwise LLD |
| 7 | Uber/Careem | Chess/Tic-tac-toe LLD |
| 8 | Mock interviews + synthesis | Mock interviews |

---

## ⏰ Weekend Structure

**Saturday (3-4 hours):** HLD focus
- 1 hour: Concept/framework learning
- 1 hour: Case study analysis
- 1-2 hours: Design exercise on paper

**Sunday (2-3 hours):** LLD focus
- 1 hour: Pattern/principle learning
- 1-2 hours: Design exercise (class diagrams)

**Total weekend commitment:** 5-7 hours
**Total over 8 weekends:** ~50 hours

---

## 📝 Notes System

```
system-design-journey/
├── weekend-1/
│   ├── hld-framework.md
│   ├── lld-oop-refresh.md
│   └── exercises.md
├── weekend-2/
... so on
└── interview-prep/
    ├── hld-cheatsheet.md
    ├── lld-cheatsheet.md
    └── company-questions/
        ├── careem-style.md
        ├── zameen-style.md
        └── daraz-style.md
```

---

## 🇵🇰 Pakistani Market Specifics (Important!)

### Companies & Their Style

**Careem** (Dubai-based, hires from Pak/India)
- LLD heavy: design ride-matching service
- HLD: focus on real-time location, surge pricing
- Trade-offs in latency vs accuracy

**Bazaar, Bykea, Foodpanda**
- Practical system design — order management, delivery tracking
- Database design weight zyada
- "Why did you choose X?" questions

**Daraz (Alibaba ecosystem)**
- E-commerce focused — cart, checkout, inventory
- Capacity estimation important
- DB sharding questions

**Systems Limited, Devsinc, Folio3, Arbisoft, Tintash**
- More LLD weight than HLD
- Clean code principles emphasized
- Design patterns explicitly asked

**Remote (Toptal, Turing, contract platforms)**
- Mixed style, often US-influenced
- Both HLD + LLD with trade-offs
- Communication skills matter zyada

### What They DON'T Usually Ask
- Designing Google-scale systems (search engine, gmail)
- Deep distributed consensus questions
- Cassandra/HBase internals
- Custom protocol design

### What They DO Ask
- "Design Uber for one city"
- "Design Foodpanda backend"
- "Design library management system"
- "Design ATM"
- "Design online voting system"

---

# 🗓️ WEEKEND 1: Foundations

## Saturday — HLD Framework & Approach

### The Universal HLD Framework (1 hour)

Memorize this 7-step structure. Apply to **every** HLD question:

```
1. Requirements (5 min)
   - Functional (features)
   - Non-functional (scale, latency, availability)
   - Out of scope (what you WON'T design)

2. Capacity Estimation (5 min)
   - Users (DAU, MAU)
   - Read/write ratio
   - Storage needs
   - Bandwidth needs

3. API Design (5 min)
   - Endpoints
   - Request/response shape
   - Idempotency
   - Authentication

4. Data Model (10 min)
   - Tables/collections
   - Relationships
   - Indexes
   - Choice: SQL vs NoSQL (with reason)

5. High-Level Architecture (10 min)
   - Components diagram
   - Data flow
   - Where each piece lives

6. Deep Dives (10 min)
   - Interviewer picks 1-2 areas
   - Trade-offs articulated

7. Scale + Failures (10 min)
   - Bottlenecks
   - How to scale each component
   - What can break
```

### Drill: Memorize "5-5-5-10-10-10-10" timing breakdown

### Concept: Non-Functional Requirements (15 min)

These 4 are asked in **every** interview:
- **Scalability** — how many users? Reads? Writes?
- **Availability** — 99.9%? 99.99%? Acceptable downtime per year?
- **Consistency** — strong? Eventual? Acceptable lag?
- **Latency** — p50, p95, p99 — kya target hai?

### Case Study (45 min)

**Analyze: How Foodpanda backend likely works**

Think through:
- User places order → restaurant gets notification → rider matched → delivery → payment
- Components: API gateway, order service, restaurant service, rider service, payment service
- Where's the database? Where's the cache?
- What if restaurant is offline?
- What if rider doesn't accept?

**Write 1-page analysis** in apne words.

### Exercise: Design ATM System (HLD style) (1 hour)

**Don't jump to code. Use the 7-step framework.**

Requirements clarification:
- What operations? (withdraw, deposit, balance, transfer)
- Multi-bank support?
- Cash management?
- Receipts?

Capacity:
- How many transactions per ATM per day?
- Network reliability?

API:
- Auth, withdraw, balance APIs
- What goes over network to bank server?

Data model:
- Account, Transaction, Card tables

Architecture:
- ATM client → ATM server → Bank backend
- Where transactions logged?

Failures:
- Network down during transaction?
- Cash dispenser jam?
- Card swallowed?

**Save your design as `weekend-1/atm-hld.md`**

---

## Sunday — OOP Refresh + SOLID

### Why This Matters

LLD interview ka 70% sirf **clean OOP + SOLID** hai. Tumne JS/TS likha hai, lekin OOP discipline shaky ho sakti hai (profile observation).

### OOP Pillars Re-Examined (1 hour)

Don't memorize definitions. Understand **why each exists**.

**1. Encapsulation**
- Sirf "private variables" nahi
- Real meaning: implementation details hide, contract expose
- Why: change implementation without breaking callers

**2. Inheritance**
- "is-a" relationship
- **Most overused** OOP feature
- Composition > Inheritance (often)

**3. Polymorphism**
- Same interface, different implementations
- Why interfaces exist
- Strategy pattern ka foundation

**4. Abstraction**
- Hide complexity, expose essence
- Different from encapsulation (subtle distinction)

### Self-Quiz
1. Composition vs Inheritance — kab kya?
2. Abstract class vs Interface (TypeScript/Java context)?
3. "Favor composition over inheritance" — kyun?

### SOLID Principles Deep (1.5 hours)

Har principle ke saath:
- 1-line definition
- 1 code smell jo violate kare
- 1 refactored version

**S — Single Responsibility**
- "Ek class, ek reason to change"
- Smell: God class with 20 methods doing unrelated things
- Example: `User` class jo authenticate, save, email send, log generate — sab kare

**O — Open/Closed**
- "Open for extension, closed for modification"
- Smell: `if-else` chain for types
- Example: PaymentProcessor that has switch case for each payment method

**L — Liskov Substitution**
- "Subclass replace parent without breaking"
- Smell: `Square extends Rectangle` (classic violation)
- Why: setting width on square breaks rectangle contract

**I — Interface Segregation**
- "Many small interfaces > one big"
- Smell: `IPrinter` jo print, scan, fax, copy sab kare
- Better: separate `IPrint`, `IScan`, etc.

**D — Dependency Inversion**
- "Depend on abstractions, not concrete"
- Smell: `OrderService` directly creates `MySQLOrderRepo`
- Better: `OrderService(repo: IOrderRepo)` — inject dependency

### Exercise: SOLID Smell Hunt (1 hour)

Apne purane projects (AuthFlow, Notemark) ka koi 1 file kholo. Find:
- 1 SRP violation
- 1 OCP violation
- 1 DIP violation

**Likho:**
- Smell kahan hai
- Kyun problem hai
- Kaise refactor karoge

**Save as `weekend-1/solid-smells-found.md`**

---

# 🗓️ WEEKEND 2: Databases + Design Patterns (Creational)

## Saturday — Database Design for Interviews

### The Database Decision Framework (1 hour)

In interview, **DB choice 30 seconds mein justify** karna hai. Memorize this tree:

```
Need ACID transactions? → SQL (Postgres/MySQL)
└─ Relations heavy with joins? → SQL
└─ Need read replicas, mature ecosystem? → SQL

Document-shaped data, flexible schema? → MongoDB
└─ Content management, catalogs? → MongoDB

Key-value with simple access? → Redis (cache) or DynamoDB
└─ Session storage, leaderboards? → Redis

Write-heavy, time-series? → TimescaleDB / ClickHouse
└─ Analytics, metrics? → ClickHouse

Search needed? → Elasticsearch (separate from primary)

Default for Pakistani market interview: PostgreSQL
└─ Unless interviewer asks for specific use case
```

### Schema Design Principles (1 hour)

**Normalization vs Denormalization trade-off:**

Normalized (3NF):
- Pros: no duplication, easy updates
- Cons: lots of joins (slow reads)
- Use: write-heavy systems, transactional

Denormalized:
- Pros: fast reads, simple queries
- Cons: duplication, harder updates
- Use: read-heavy systems, analytics

**Indexing Cheatsheet:**
- Index columns in WHERE clauses (frequent)
- Index foreign keys
- Composite index column order: most selective first
- Don't index low-cardinality columns (gender, boolean)
- Every index = slower writes

### Exercise: Design Foodpanda Order DB (1.5 hours)

Tables design karo:
- users
- restaurants
- menu_items
- orders
- order_items
- riders
- payments
- reviews

For each:
- Columns + types
- Primary key
- Foreign keys
- Indexes (justify each)

**Constraint:** PostgreSQL only. Why? — agar interviewer poochay.

**Tricky questions to think about:**
- Order status changes karta hai — history kaise store karo? (status_history table?)
- Menu price change hota hai — purane orders ka price kaise rahe? (snapshot in order_items)
- Restaurant offline ho jaye — kya orders accept ho?

**Save as `weekend-2/foodpanda-schema.md`**

---

## Sunday — Creational Design Patterns

### Why Patterns Matter For LLD Interviews

Pakistani mid-tier companies often **explicitly poochti hain**: "Which design pattern would you use here?"

23 patterns hain. **Tumhe 8-10 deeply samjhne hain.** Today: Creational (5 patterns).

### 1. Singleton (15 min)

**Idea:** Ek hi instance puri app mein.
**Use case:** Database connection pool, logger, config.
**Pitfall:** Global state — testability harm karta hai.

**Pseudo-design:**
```
Class DatabasePool {
  private static instance: DatabasePool
  private constructor() {...}

  static getInstance(): DatabasePool {
    if (!instance) instance = new DatabasePool()
    return instance
  }
}
```

**Interview gotcha:** Singleton in distributed systems doesn't work — multiple instances on multiple servers. They'll test if you know this.

### 2. Factory Method (15 min)

**Idea:** Object creation logic centralized, return type abstract.
**Use case:** Multiple notification types (SMS, Email, Push).

**Example:**
```
NotificationFactory.create("sms") → returns SMSNotifier
NotificationFactory.create("email") → returns EmailNotifier
```

**Why not just new?:** Adding new type doesn't change client code.

### 3. Abstract Factory (15 min)

**Idea:** Factory of factories — related object families.
**Use case:** UI themes — DarkButton + DarkTextbox + DarkDropdown vs Light equivalents.

**Less common in interviews** but know the concept.

### 4. Builder (15 min)

**Idea:** Step-by-step object construction, especially for complex objects.
**Use case:** SQL query builder, HTTP request builder.

**Example pseudo-code:**
```
new PizzaBuilder()
  .size("large")
  .crust("thin")
  .addTopping("cheese")
  .addTopping("mushroom")
  .build()
```

**Interview question:** "Design pizza ordering" — Builder fits perfectly.

### 5. Prototype (10 min)

**Idea:** Clone existing objects rather than create new.
**Use case:** When creation is expensive (DB hit, computation).
**Less asked** — bas concept jaano.

### Exercise: When to Use Which? (45 min)

For each scenario, pick the right pattern + justify:

1. Logger that must be one across the app → ?
2. Different payment processors (Stripe, PayPal, JazzCash) → ?
3. Configuring a complex HTTP request with headers, query params, body, auth → ?
4. UI theme switcher (dark/light) → ?
5. Creating copies of a template document → ?

**Save as `weekend-2/creational-patterns-practice.md`**

---

# 🗓️ WEEKEND 3: Caching + Structural Patterns

## Saturday — Caching for HLD Interviews

### When to Mention Caching in Interview (30 min)

**Don't add cache to every design.** Senior signal = knowing **when not to cache.**

Cache karo jab:
- Read >> write (10:1 ratio ya zyada)
- Same data baar baar maanga jaye
- DB hit expensive ho
- Stale data acceptable ho thodi der

Cache **na** karo jab:
- Write-heavy system
- Strong consistency required
- Data unique per request
- Cache logic > DB logic complexity

### Cache Layers In Real Systems (45 min)

**Reddit ka famous 5-layer cache:**
1. Browser cache
2. CDN cache
3. Reverse proxy cache (Varnish/Nginx)
4. Application cache (Redis/Memcached)
5. Database cache (Postgres shared_buffers)

**Pakistani context:** Most interview questions need **layers 3-4**. CDN sometimes for static assets.

### Cache Invalidation Strategies (30 min)

Memorize this for interviews:

| Strategy | When to use | Pitfall |
|---|---|---|
| TTL only | Acceptable stale data | Race conditions on expire |
| Write-through | Strong consistency need | Slower writes |
| Write-behind | High write throughput | Data loss risk on crash |
| Event-based (invalidate on update) | Moderate consistency | Complex implementation |
| Cache-aside | Most common, flexible | Cache miss penalty |

### CDN Concept (30 min)

For Pak/India market interviews:
- Cloudflare or AWS CloudFront mention karo
- Static assets serve karte hain (images, JS, CSS)
- Video streaming
- "Edge computing" buzzword

**Don't over-explain CDN unless asked deep.**

### Exercise: Add Caching to Foodpanda (1.5 hours)

Pichle weekend ka schema lo. Identify cache opportunities:

1. Restaurant menu — kab cache karo? TTL? Invalidation?
2. User's cart — Redis mein? Why?
3. Restaurant list with filters — cacheable?
4. Order status — should you cache?
5. Search results — kaise cache karo?

**For each: trade-offs likho. Stale data ka impact kya hoga?**

**Save as `weekend-3/foodpanda-caching.md`**

---

## Sunday — Structural Design Patterns

### 1. Adapter (20 min)

**Idea:** Make incompatible interfaces work together.
**Use case:** Third-party library jo different interface use karti hai.

**Example:** Tumhe payment gateway integrate karna hai. JazzCash ka API alag hai, EasyPaisa ka alag. Tum `PaymentAdapter` interface banao, har gateway ka adapter likho.

**Real use in Pakistani context:** Multiple bank APIs adapt karna for fintech.

### 2. Facade (20 min)

**Idea:** Simple interface over complex subsystem.
**Use case:** Order placement involves cart, payment, inventory, notification — facade unko coordinate kare.

**Pseudo-code:**
```
OrderFacade {
  placeOrder() {
    cart.validate()
    inventory.reserve()
    payment.process()
    notification.send()
  }
}
```

**Client just calls `orderFacade.placeOrder()` — complexity hidden.**

### 3. Decorator (20 min)

**Idea:** Add behavior to object dynamically without modifying class.
**Use case:** Middleware in Express, coffee shop add-ons.

**Example:**
```
Coffee → MilkDecorator(Coffee) → SugarDecorator(MilkDecorator(Coffee))
```

Each decorator adds price + description.

**Interview favorite:** Pizza/Coffee/Sandwich problems use this.

### 4. Proxy (15 min)

**Idea:** Surrogate for another object — control access.
**Types:**
- Virtual proxy (lazy loading)
- Protection proxy (access control)
- Remote proxy (RPC stubs)

**Less commonly asked** but know concept.

### 5. Composite (15 min)

**Idea:** Tree structures where individual + composite treated uniformly.
**Use case:** File system (file + folder), UI components, organization hierarchy.

**Example:**
```
Component (interface)
├── File (leaf)
└── Folder (composite — contains list of Components)
```

`folder.getSize()` recursively calls on all children.

### 6. Bridge (10 min)

**Less common** in mid-tier interviews. Skim and move on.

### Exercise: Design Library Management LLD (1.5 hours)

Classic interview question.

Requirements:
- Books, members, librarians
- Borrow, return, reserve
- Late fees
- Search

**Classes you need:**
- Book, BookItem (multiple copies)
- Library, Branch
- Member, Librarian (inheritance from Person?)
- Loan, Reservation
- SearchService

**Patterns to use:**
- Factory for creating different item types (Book, DVD, Magazine)
- Observer for reservation notifications (next weekend)
- Strategy for late fee calculation

**Draw class diagram on paper.**

**Save as `weekend-3/library-lld.md`**

---

# 🗓️ WEEKEND 4: Load Balancing + Behavioral Patterns

## Saturday — Load Balancing + Queues in HLD

### Load Balancer Concept (45 min)

**Where it sits:**
```
Client → DNS → Load Balancer → [App Server 1, 2, 3...]
```

**Algorithms (memorize):**
- Round robin (simple, default)
- Least connections (better for long-running)
- Weighted (some servers more powerful)
- IP hash (sticky sessions)
- Geographic (route to nearest)

**Types:**
- Layer 4 (TCP) — fast, no inspection
- Layer 7 (HTTP) — slower, can route by path/headers

**Mention in interview:**
- "Nginx for L7, AWS ALB for L7, AWS NLB for L4"
- "HAProxy popular open-source"

### Health Checks (15 min)

LB ko pata kaise chale ke server zinda hai?
- Active: LB pings `/health` every X seconds
- Passive: Watches actual responses, marks failed if many errors

**Interview gotcha:** Health check should test **deep health** (DB connection, dependencies) not just "is HTTP responding."

### Queues Refresh for HLD (1 hour)

You've studied queues in distributed thinking roadmap. Yahan **interview articulation** seekho.

**When to mention queue in design:**
- Async processing (email, SMS, notifications)
- Decoupling services
- Rate limiting / smoothing traffic spikes
- Background jobs (report generation)
- Retry mechanism

**Technology mention:**
- Pak/India mid-tier: **Redis (BullMQ) or RabbitMQ** are safe
- Don't mention Kafka unless throughput justifies (100k+ events/sec)
- AWS SQS if cloud-native answer

**Interview-killing phrase:**
> "I'd use a message queue here to decouple X from Y, allowing Y to process asynchronously and providing retry capability if Y is temporarily unavailable."

### Exercise: Add LB + Queue to ATM System (1.5 hours)

Weekend 1 ka ATM design lo. Now add:

1. Where does LB go?
2. How many ATM servers? Where in geography?
3. Which operations should be async (queue)?
4. Transaction logging — sync or async?
5. Daily reconciliation — definitely async, but how?

**Update your weekend-1 design with these layers.**

---

## Sunday — Behavioral Design Patterns

### 1. Observer (25 min)

**Idea:** When one object changes, dependents auto-notified.
**Use case:** Event systems, pub/sub, notifications.

**Example:**
```
OrderSubject → notifies → [EmailNotifier, SMSNotifier, AnalyticsLogger]
```

When order placed, all observers triggered.

**Real world:** Frontend reactivity (React state → re-render), Node.js EventEmitter.

**Interview favorite:** "How would you implement notification system?"

### 2. Strategy (25 min)

**Idea:** Family of algorithms, interchangeable at runtime.
**Use case:** Payment methods, sorting strategies, fee calculation.

**Example:**
```
PaymentContext.setStrategy(new JazzCashStrategy())
paymentContext.processPayment()
```

Switch strategy without changing context.

**Why important:** Open/Closed principle ka practical form.

### 3. Command (20 min)

**Idea:** Encapsulate request as object.
**Use case:** Undo/redo, request queuing, macro recording.

**Example:**
```
class DepositCommand implements Command {
  execute() { account.deposit(amount) }
  undo() { account.withdraw(amount) }
}
```

Editor undo/redo classic example.

### 4. State (20 min)

**Idea:** Object behavior changes when internal state changes.
**Use case:** Order states (placed → confirmed → preparing → out for delivery → delivered).

**Anti-pattern this replaces:** Giant `switch` statement on state.

**Example:**
```
Order in PlacedState → can cancel
Order in DeliveredState → cannot cancel, can return
Same .cancel() call, different behavior based on state.
```

**Interview favorite for:** Vending machines, ATMs, traffic lights.

### 5. Template Method (15 min)

**Idea:** Algorithm skeleton in base class, steps overridden by subclasses.
**Use case:** Different report generators with same structure.

**Example:**
```
Base: generateReport() { fetchData(); formatData(); export(); }
Subclasses override fetchData() and export() differently.
```

### 6. Chain of Responsibility (15 min)

**Idea:** Pass request along chain until handled.
**Use case:** Express middleware, approval workflows.

**Example:**
```
authMiddleware → loggerMiddleware → rateLimitMiddleware → handler
```

Express itself uses this pattern.

### 7. Iterator (5 min)

**Idea:** Sequential access without exposing internals.
**Built into most languages** — `for...of`, `for...in`.
**Skim, move on.**

### Exercise: Design Vending Machine LLD (2 hours)

Use **State pattern** primarily.

States:
- NoCoinState
- HasCoinState
- DispensingState
- SoldOutState

Actions per state:
- insertCoin()
- selectProduct()
- dispense()
- refund()

**Classes:**
- VendingMachine
- State (interface)
- NoCoinState, HasCoinState, DispensingState, SoldOutState (concrete)
- Product
- Inventory

**Draw state transition diagram + class diagram.**

**Save as `weekend-4/vending-machine-lld.md`**

---

# 🗓️ WEEKEND 5: URL Shortener (Full HLD) + Parking Lot LLD

## Saturday — URL Shortener (Most Asked HLD Question)

### Why This Question Is The Classic

Every Pak/India interview at some point asks URL shortener variant:
- Bit.ly clone
- Custom short URLs for marketing
- QR code generators

**Master this one design, you can adapt to many.**

### Apply 7-Step Framework (3 hours total)

#### Step 1: Requirements (15 min)

Functional:
- Shorten long URL → short URL
- Redirect short URL → long URL
- Custom alias (optional)
- Expiration (optional)
- Analytics (clicks count)

Non-functional:
- 100M URLs created/day
- 10:1 read/write ratio
- Latency: redirect < 100ms
- Availability: 99.9%
- URLs cannot be guessable (security)

Out of scope:
- User accounts
- Pricing tiers
- Detailed analytics

#### Step 2: Capacity Estimation (15 min)

- Writes: 100M/day = ~1200/sec average, ~3600/sec peak
- Reads: 1B/day = ~12000/sec average, ~36000/sec peak
- Storage: 100M URLs/day × 500 bytes = 50 GB/day, 18 TB/year
- Bandwidth (read): 12000 × 500 bytes = 6 MB/sec

#### Step 3: API Design (15 min)

```
POST /shorten
Body: { long_url: string, custom_alias?: string, expiry?: timestamp }
Response: { short_url: string }

GET /:short_code
Response: 301 redirect to long_url

GET /:short_code/analytics
Response: { clicks: number, recent_clicks: [...] }
```

#### Step 4: Data Model (20 min)

**Choice: PostgreSQL** (transactional, mature, sufficient for 1200 writes/sec)

```sql
CREATE TABLE urls (
  short_code VARCHAR(10) PRIMARY KEY,
  long_url TEXT NOT NULL,
  created_at TIMESTAMPTZ DEFAULT NOW(),
  expires_at TIMESTAMPTZ,
  click_count BIGINT DEFAULT 0
);
CREATE INDEX idx_expires ON urls(expires_at) WHERE expires_at IS NOT NULL;
```

**Short code generation strategy** (KEY discussion):
- Option A: Hash long URL (MD5 first 7 chars) — collisions possible
- Option B: Auto-increment ID → base62 encode — sequential, guessable
- Option C: Pre-generate pool of unique codes — best for scale
- Option D: UUID first 8 chars — simple, low collision

**Most interview-impressive: Option C**

#### Step 5: High-Level Architecture (20 min)

```
Client → CDN → Load Balancer → App Server (Node.js)
                                    ↓
                                Redis Cache (hot URLs)
                                    ↓
                                PostgreSQL (primary)
                                    ↓
                                Read Replicas (for redirects)
```

**Async pipeline:**
```
App Server → Click Events Queue (BullMQ) → Analytics Worker → Click count update
```

#### Step 6: Deep Dives (30 min)

**Pick 2 to go deep on:**

**Deep Dive 1: Cache Strategy**
- Cache hot URLs in Redis (LRU eviction)
- TTL: 24 hours
- Cache-aside pattern
- Click count NOT in cache (use queue instead)

**Deep Dive 2: Click Counting**
- Don't update DB on every click (DB will die at 36k/sec)
- Queue clicks, batch update every 1 minute
- Analytics service consumes events separately

#### Step 7: Scale + Failures (20 min)

Bottlenecks:
- DB writes: shard by short_code prefix? Probably not needed (1200/sec)
- DB reads: read replicas + cache
- Cache: Redis cluster if memory exceeds 100GB

Failures:
- Redis down → direct DB hit (slower but works)
- DB down → return cached + error log
- App server down → LB removes from pool

**Save your design as `weekend-5/url-shortener-hld.md`**

This is your **portfolio piece** — interviewer-ready.

---

## Sunday — Parking Lot LLD

### Why This Question

Almost every mid-tier company asks. Tests:
- OOP design
- Inheritance vs composition
- Design patterns (Strategy, Factory)
- Real-world thinking

### Requirements (15 min)

- Multi-level parking lot
- Multiple spot types: Compact, Regular, Large, Handicapped, Motorcycle
- Vehicle types: Car, Motorcycle, Truck
- Entry/Exit gates
- Pricing: hourly, daily caps
- Payment: cash, card
- Display: available spots per level

### Class Design (1.5 hours)

```
ParkingLot
├── List<ParkingFloor>
├── List<EntryGate>
├── List<ExitGate>
└── ParkingDisplayBoard

ParkingFloor
├── floorNumber
├── List<ParkingSpot>
└── displayBoard

ParkingSpot (abstract)
├── id, isOccupied, currentVehicle
└── canFitVehicle(Vehicle): boolean

CompactSpot extends ParkingSpot
RegularSpot extends ParkingSpot
LargeSpot extends ParkingSpot
MotorcycleSpot extends ParkingSpot
HandicappedSpot extends ParkingSpot

Vehicle (abstract)
├── licensePlate, type
Car extends Vehicle
Motorcycle extends Vehicle
Truck extends Vehicle

ParkingTicket
├── ticketNumber, vehicleType, entryTime, exitTime
├── spotAssigned, status
└── calculateFee(): number

PaymentStrategy (interface)
├── CashPayment
├── CardPayment
└── OnlinePayment

ParkingRateCalculator (Strategy pattern)
├── HourlyRate
├── DailyRate
└── MonthlyPassRate
```

### Key Design Decisions To Articulate

1. **Why ParkingSpot abstract?**
   - Different fit rules (Motorcycle fits in compact, Truck doesn't)
   - Use Liskov substitution properly

2. **Why Strategy for pricing?**
   - Different lots may have different pricing
   - Easy to add new strategies (Member discount, EV discount)

3. **Why Factory for ticket generation?**
   - Centralized ID generation
   - Could be sequential or UUID

4. **Thread safety:**
   - Multiple entry gates simultaneously checking same spot
   - Use locks / atomic operations
   - Database-level: row locks on spot

### Sequence Diagram: Vehicle Enters

```
Car arrives → EntryGate.checkSpotAvailable(Car)
   → ParkingLot.findSpot(Car)
   → For each Floor, find first available CompactSpot/RegularSpot
   → Lock the spot
   → Generate ParkingTicket
   → Mark spot occupied
   → Open gate
   → Return ticket to user
```

### Sequence Diagram: Vehicle Exits

```
Driver at exit → ExitGate.scanTicket(ticketNumber)
   → Calculate fee using strategy
   → User selects payment method
   → PaymentStrategy.processPayment()
   → On success: mark spot empty, close ticket
   → Open gate
```

**Save as `weekend-5/parking-lot-lld.md`**

This is **another portfolio piece**.

---

# 🗓️ WEEKEND 6: Twitter Feed HLD + Splitwise LLD

## Saturday — Twitter/Instagram Feed (Hard HLD)

### Why This Is Hard

The "celebrity problem" — Imran Khan has 20M followers. If he tweets, do you push to 20M timelines instantly?

### Requirements (15 min)

Functional:
- User posts tweet
- User sees feed (tweets from people they follow)
- Like, retweet, reply

Non-functional:
- 500M DAU
- Average 200 follows per user
- Read >> write (100:1)
- Feed should be < 200ms

### Capacity Estimation (15 min)

- 500M DAU
- Tweets/sec: ~6000 (writes)
- Feed requests/sec: ~600,000 (reads)
- Each user fans-out 200 followers on average

### The Fan-out Problem (45 min)

**Approach 1: Pull Model (Fan-out on read)**
- On feed request, query tweets from all followed users
- Sort, return
- Pros: simple, no precomputation
- Cons: SLOW on read (joins across millions of rows)

**Approach 2: Push Model (Fan-out on write)**
- On tweet, push to all followers' timeline caches
- Read = just fetch precomputed timeline
- Pros: fast reads
- Cons: write amplification (1 tweet → 200 writes)

**Approach 3: Hybrid (Best for Twitter scale)**
- Push for normal users (< 10k followers)
- Pull for celebrities (> 10k followers)
- Merge at read time

**This is "celebrity problem solution" — articulate this in interview = senior signal**

### Architecture (30 min)

```
Client → API Gateway → Tweet Service / Feed Service

Tweet Service:
  → Tweet DB (Postgres or Cassandra)
  → Fan-out Queue (Kafka)
  → Fan-out Workers → Timeline Cache (Redis)

Feed Service:
  → Timeline Cache (Redis) ← reads here mostly
  → If celebrity in follows: fetch from Tweet DB
  → Merge and return
```

### Trade-offs To Articulate (30 min)

- Eventual consistency in feed: acceptable
- Read latency vs write latency: optimize reads
- Storage cost (denormalized timelines) vs computation cost

### Exercise (1 hour)

Same design, but for Instagram feed (with images).

Differences:
- Images much larger than text
- CDN crucial
- Algorithmic feed (not chronological) — how?

**Save as `weekend-6/twitter-feed-hld.md`**

---

## Sunday — Splitwise LLD

### Why This Question

Tests:
- Object modeling for relationships
- Graph algorithms thinking
- Strategy pattern (split types)

### Requirements (15 min)

- Users
- Groups (e.g., "Roommates", "Trip to Naran")
- Add expense, split among users
- Split types: equal, exact amounts, percentage, shares
- Show who owes whom
- Settle up

### Class Design (1.5 hours)

```
User
├── userId, name, email
└── balances: Map<User, BigDecimal>  // negative = I owe them, positive = they owe me

Group
├── groupId, name
├── members: List<User>
└── expenses: List<Expense>

Expense
├── expenseId, description, totalAmount
├── paidBy: User
├── splitStrategy: SplitStrategy
└── splits: List<Split>

Split
├── user, amount

SplitStrategy (interface)
├── EqualSplit
├── ExactSplit
├── PercentageSplit
└── ShareSplit

ExpenseManager (main service)
├── addExpense(Expense)
├── getBalance(User)
├── settleUp(User1, User2)
└── simplifyDebts(Group)
```

### Algorithm: Simplify Debts (Important!)

In group of 5 friends with many transactions, instead of A pays B, B pays C, C pays A — simplify to minimum transactions.

This is a **graph problem** — interviewer love articulating:
- Build debt graph
- Use min-cash-flow algorithm
- Reduce N² transactions to N-1 in best case

### Exercise (1 hour)

Add features:
- Currency support (multi-currency expenses)
- Recurring expenses (rent every month)
- Expense categories with analytics

How does class diagram change?

**Save as `weekend-6/splitwise-lld.md`**

---

# 🗓️ WEEKEND 7: Uber/Careem HLD + Chess LLD

## Saturday — Ride-Sharing System (Uber/Careem)

### Why This Is The Best Question For Pak Market

Careem is from Pakistan. Almost every Pak company asks variant of this.

### Requirements (20 min)

Functional:
- Riders request rides
- Drivers accept rides
- Real-time location tracking
- Fare calculation
- Payment
- Ratings

Non-functional:
- 100k drivers in Karachi (single city scope)
- 1M riders
- Real-time updates (< 1 sec)
- Surge pricing in high demand

### Capacity (15 min)

- 1M DAU rider, 100k drivers
- Peak rides: ~50k/hour = ~14/sec
- Driver location updates: 100k × 1 per 4 sec = 25k/sec
- Storage: rides, locations, payments

### Core Components (45 min)

```
Mobile App (Driver + Rider) ↔ API Gateway

Services:
- User Service (auth, profile)
- Driver Service (online status, location)
- Ride Service (request, match, status)
- Location Service (real-time GPS)
- Pricing Service (fare calc, surge)
- Payment Service
- Notification Service
- Analytics Service
```

### The Matching Problem (45 min)

When rider requests ride, find nearest driver:

**Approach 1: Naive**
- Query all online drivers in city
- Calculate distance to each
- Pick nearest
- **Slow** at 100k drivers

**Approach 2: Geohashing**
- Divide city into grid cells (e.g., 1km × 1km)
- Each driver in one cell
- Rider in cell X → look in cell X + adjacent cells
- Much faster

**Approach 3: QuadTree / R-tree**
- Hierarchical spatial index
- Used by real Uber

**Mention: Redis Geospatial commands** (`GEOADD`, `GEORADIUS`) — built-in support.

### Real-Time Location Updates (30 min)

- Driver app sends GPS every 4 seconds
- Don't write to main DB (too much load)
- Write to Redis Geospatial
- WebSocket from driver app
- WebSocket to rider for "driver coming" updates

### Surge Pricing (15 min)

- Monitor demand-supply in each geo cell
- If demand > supply × threshold → surge multiplier
- Update every 30 seconds
- Display to rider before they book

**Save as `weekend-7/uber-hld.md`**

---

## Sunday — Chess Game LLD

### Why This Question

Tests:
- Complex OOP modeling
- Inheritance hierarchies
- Game state management

### Requirements (15 min)

- 2 players
- 8x8 board
- 6 piece types with different movements
- Check, checkmate, stalemate
- Castling, en passant, promotion (advanced)

### Class Design (2 hours)

```
ChessGame
├── board: Board
├── players: [Player, Player]
├── currentTurn: Player
├── status: GameStatus
├── moves: List<Move>
└── makeMove(Move): boolean

Board
├── cells: Cell[8][8]
└── initialize()

Cell
├── x, y
└── piece: Piece (nullable)

Piece (abstract)
├── color: Color (White/Black)
├── isKilled: boolean
└── canMove(start: Cell, end: Cell, board: Board): boolean  // abstract

King extends Piece
Queen extends Piece
Bishop extends Piece
Knight extends Piece
Rook extends Piece
Pawn extends Piece

Move
├── start: Cell, end: Cell
├── pieceMoved: Piece
├── pieceKilled: Piece (nullable)
└── isCheck, isCheckmate, isCastling, isEnPassant
```

### Key Design Decisions

1. **Why Piece abstract with `canMove` method?**
   - Each piece has unique movement rules
   - Polymorphism in action

2. **How to detect Check?**
   - After each move, check if opponent's King is attackable by any of your pieces
   - Iterate all your pieces, call `canMove(piece.cell, king.cell, board)`

3. **How to detect Checkmate?**
   - King is in check + no valid move can remove the check
   - Try all possible moves of king and other pieces, check if any leaves king safe

4. **Castling rules** (complex):
   - Neither King nor Rook has moved
   - No pieces between them
   - King doesn't pass through attacked squares

### Patterns Used

- **Strategy** — different piece movements
- **Observer** — could notify UI on board change
- **Command** — could record moves for undo/replay

**Save as `weekend-7/chess-lld.md`**

---

# 🗓️ WEEKEND 8: Mock Interviews + Synthesis

## Saturday — HLD Mock Interview Marathon

### The Drill (4 hours)

**3 mock interviews, 45 minutes each + 15 min self-review**

Use voice recorder. Imagine interviewer in front of you.

**Mock 1: "Design a notification system that handles 1M notifications/day"**

Walk through 7 steps out loud:
1. Requirements
2. Capacity
3. API
4. Data model
5. Architecture
6. Deep dives (push notifications, retry, dedupe)
7. Scale + failures

**Mock 2: "Design Bykea's backend"** (motorcycle ride-sharing in Pakistan)

Similar to Uber but consider:
- Smaller bikes, no surge pricing
- Cash-heavy (less card)
- Specific to Pakistan geo

**Mock 3: "Design a library management system"**

This is more LLD-leaning but in HLD format:
- Multi-branch library
- Book reservation system
- Late fee management

### Self-Review Checklist

After each mock, check:
- ✅ Did I clarify requirements before designing?
- ✅ Did I do capacity estimation with real numbers?
- ✅ Did I justify DB choice?
- ✅ Did I mention specific technologies (not vague "use a database")?
- ✅ Did I articulate trade-offs?
- ✅ Did I cover failure modes?
- ✅ Was my pace right (not too fast/slow)?

Listen to recording — kahan stuck hue? Kya filler words?

---

## Sunday — LLD Mock + Final Synthesis

### LLD Mock Interview (2 hours)

**3 quick mocks, 30 minutes each:**

**Mock 1: Design Tic-Tac-Toe**
- Board, Player, GameStatus
- Win detection algorithm
- Use State pattern?

**Mock 2: Design Snake and Ladder**
- Board, Player, Dice, Snake, Ladder
- Turn management
- Win condition

**Mock 3: Design ATM** (full LLD this time)
- Card, Account, Transaction
- State pattern for ATM states (Idle, CardInserted, PinEntered, etc.)
- Strategy for transaction types

### Final Synthesis Document (2 hours)

Banao `interview-cheatsheet.md`:

**HLD Cheatsheet:**
- 7-step framework
- Capacity estimation shortcuts
- DB decision tree
- When to use cache, queue, LB
- Common scaling techniques
- Failure modes vocabulary

**LLD Cheatsheet:**
- SOLID quick reference
- Top 10 design patterns with 1-line use cases
- Common LLD questions (Parking, Library, Chess, etc.)
- UML quick reference

**Pakistani Companies Specific:**
- Careem-style questions
- Foodpanda/Bazaar/Bykea common asks
- E-commerce specific (Daraz)
- Banking/Fintech (Easypaisa, Nayapay)

### LinkedIn Capstone Post

> "8 weekends of system design practice — HLD + LLD. From URL shortener to Twitter feed, from parking lot to chess. Now ready for system design interviews. Specifically targeting [companies]. Open to opportunities."

---

# 🎯 Post-Roadmap Outputs

## Knowledge Files
- 8 weekend folders with HLD + LLD designs
- 1 interview cheatsheet
- 6 portfolio-quality designs:
  - ATM (HLD)
  - Foodpanda DB
  - URL Shortener
  - Twitter Feed
  - Uber/Careem
  - Library / Parking Lot / Chess / Splitwise (LLDs)

## Skills Acquired
- ✅ 7-step HLD framework second nature
- ✅ Top 10 design patterns confidently
- ✅ SOLID principles fluent
- ✅ Trade-off articulation
- ✅ 45-min interview pace
- ✅ Pakistani company-specific examples

## Interview Readiness
- ✅ Can design Careem-style ride-sharing
- ✅ Can design Foodpanda-style food delivery
- ✅ Can design URL shortener / Pastebin variants
- ✅ Can design any standard LLD (parking, library, ATM)
- ✅ Can defend choices with trade-offs

---

# 📚 Master Resource List

## Books
- **System Design Interview** by Alex Xu (Vol 1 & 2) — buy or download
- **Designing Data-Intensive Applications** by Kleppmann — reference
- **Head First Design Patterns** — for LLD patterns (excellent for beginners)

## YouTube Channels
- **Gaurav Sen** (Indian, very Pak/India relevant)
- **System Design Interview** channel
- **ByteByteGo** (Alex Xu's channel)
- **Tech Dummies** (Narendra L)
- **Concept && Coding** (Shrayansh) — Indian LLD focused

## Websites
- **systemdesignprimer** on GitHub (free, comprehensive)
- **highscalability.com** (case studies)
- **InterviewBit** (problems)
- **LeetCode discuss** — system design posts

## Practice Communities
- LinkedIn — follow @sysdesign people
- Pakistani Dev Slack communities
- Discord servers for Pakistani devs

---

# ⚠️ Realistic Expectations

## What This Roadmap Won't Do
- Make you Google L6 ready (different scale)
- Give you years of production experience
- Replace actual work experience

## What This Roadmap WILL Do
- Get you through Careem/Bazaar/Daraz/Foodpanda interviews
- Make you confident in mid-tier Pakistani/Indian companies
- Give you structured thinking for any new system
- Set foundation for FAANG prep later if you go that route

---

# 🚀 Pehla Step Aaj

1. **Save this file** + create GitHub repo `system-design-journey`
2. **8 folders banao** (weekend-1 to weekend-8)
3. **Pichli wali distributed thinking roadmap saath rakho** — dono ek doosre ko complement karte hain
4. **Schedule fix karo:**
   - Mon-Fri: Distributed thinking (2-3 hours)
   - Sat-Sun: System design (5-7 hours)
   - **Sunday evening:** Both off, recharge

5. **First weekend (Weekend 1) ka pehla 30 minutes:**
   - 7-step framework yaad karo
   - Apply karo to "Design Bykea" — 1 paragraph apne words mein abhi likho, baghair kuch padhe
   - Weekend 1 ke baad us paragraph pe wapas aao — compare karo

---

# 💼 Job Hunt Strategy (Bonus)

While you do this 8-weekend roadmap:

**Week 2:** Update LinkedIn — add "Studying distributed systems + system design"
**Week 4:** Post about a design you did (URL shortener) — get attention
**Week 6:** Reach out to 5 Pakistani senior engineers for advice (DMs)
**Week 8:** Start applying to Careem, Bazaar, Daraz, Bykea, Foodpanda

**Lahore-specific:**
- Tintash, Arbisoft, Folio3, Devsinc, Systems Limited
- Visit their offices if possible
- Attend Pak dev meetups (PakDev Slack)

---

**Bhai 8 weekends. ~50 hours. Pakistani mid-tier companies tumhare paas aayengi.**

**Bilkul realistic plan hai. Lage raho.** 💪🇵🇰

*Roadmap created: 12 May 2026 for Zeeshan Saleem*
*Companion to: Distributed Systems Thinking Roadmap*
