# technical-sales-learning
Building technical fluency in software, cloud infrastructure, APIs, AI and developer tools from a GTM perspective.
# Technical Sales Learning

I'm a sales professional building a stronger technical foundation to better understand the products I sell and the engineers, technical leaders, and businesses that use them.

My goal isn't to become a software engineer. It's to develop enough technical fluency to understand how modern software works, ask better questions, communicate credibly with technical buyers, and sell technical products more effectively.

## What I'm Learning

### Software Development
Git, GitHub, repositories, branches, commits, pull requests, and how engineering teams collaborate on software.

### APIs
How different software systems communicate with each other and how API-based products work.

### Cloud & Infrastructure
How modern applications are hosted, deployed, and operated across cloud infrastructure.

### DevOps, SRE & Observability
How engineering teams deploy software, monitor systems, investigate incidents, identify root causes, and maintain reliability.

### AI
LLMs, AI APIs, agents, RAG, embeddings, and how AI is being integrated into modern software.

### Technical GTM
Connecting technical problems to business impact, identifying the right buyers, asking better discovery questions, and communicating technical value clearly.

## Why I'm Doing This

My background is in sales, where I've worked across prospecting, discovery, demos, closing, onboarding, and account management.

As I move deeper into technical software sales, I want to understand more than the sales pitch. I want to understand the technology behind the products, the problems engineering teams are trying to solve, and why those problems matter to the business.

This repository will document that learning process.

## Learning Log

### Day 1 — Git & GitHub Fundamentals
- Git vs. GitHub
- Repositories
- Commits
- Push and pull
- Branches
- Pull requests
- Merging
- Issues
- Forks
- Open-source software

### Day 2 — How Software Works

**Concepts covered:**
- Frontend vs. backend
- Client and server
- Databases
- APIs
- HTTP
- Requests and responses
- JSON
- Authentication vs. authorization
- Libraries and frameworks

**Core mental model:**

User → Frontend → API → Backend → Database → Response

**Sales takeaway:**

Technical fluency isn't about being able to engineer the customer's system. It's about understanding the environment well enough to recognize technical problems, ask intelligent questions, and connect those problems to business impact.

### Day 3 — APIs, HTTP & Integrations

**Concepts covered:**
- APIs and endpoints
- HTTP methods: GET, POST, PUT/PATCH, DELETE
- Requests and responses
- HTTP status codes
- API authentication and API keys
- Rate limits
- Integrations
- Native integrations vs. APIs
- Webhooks

**Core mental model:**

Application → API Request → Endpoint → Backend → Response → Application

**Sales takeaway:**

Understanding APIs helps me go beyond simply asking whether a product "integrates." I can better understand how systems exchange data, what technical requirements a buyer may have, and ask stronger discovery questions around integrations, scale, authentication, and existing workflows.

### Day 4 — Cloud Infrastructure Fundamentals

**Concepts covered:**
- Cloud computing
- AWS, Azure, and GCP
- Servers and virtual machines
- Compute and storage
- Cloud regions and availability zones
- Development, staging, and production environments
- Deployments
- Containers and Docker
- Kubernetes
- Managed services

**Core mental model:**

Code → GitHub → Build/Test → Deploy → Production → Cloud Infrastructure

**Sales takeaway:**

Cloud infrastructure gives companies scalability and flexibility, but growing infrastructure can also introduce complexity, reliability challenges, and operational overhead. Understanding the basic architecture helps me recognize technical pain and ask better questions about reliability, deployments, scale, and engineering time.

### Day 5 — DevOps, SRE & Observability

**Concepts covered:**
- DevOps
- CI/CD
- Site Reliability Engineering (SRE)
- Incidents and downtime
- Reliability
- On-call engineering
- Monitoring vs. observability
- Logs, metrics, and traces
- Telemetry
- Alerts and alert fatigue
- Root cause analysis
- MTTR

**Core mental model:**

Code → CI/CD → Deployment → Production → Incident → Alert → Investigation → Root Cause → Fix → Recovery

**Sales takeaway:**

Detecting that something broke is only part of the problem. Engineering teams also need to understand what happened, identify the root cause, and restore service quickly. Technical discovery should uncover how incidents are detected, how engineers investigate them, how much time and engineering effort that process requires, and what the business impact is.

### Day 6 — Microservices & Distributed Systems

**Concepts covered:**
- Monolithic vs. microservice architectures
- Distributed systems
- Service dependencies
- Upstream and downstream services
- Cascading failures
- Latency
- Timeouts and retries
- Single points of failure
- Redundancy
- Load balancing
- Scalability

**Core mental model:**

User → Service A → Service B → Service C → Database

A problem in one dependency can affect multiple upstream services, making the symptom visible somewhere completely different from the actual root cause.

**Sales takeaway:**

As software becomes more distributed, identifying that something is broken is not necessarily the same as identifying what caused it. Understanding dependencies helps me ask better questions about how engineering teams investigate incidents, trace problems across services, and determine root cause.

### Day 7 — Databases, Caching & Data Flow

**Concepts covered:**
- Databases
- Tables, rows, and columns
- SQL and relational databases
- NoSQL databases
- Database queries
- Indexes
- Reads and writes
- Caching
- Redis
- Cache hits and misses
- Stale data
- Data flow
- Database scaling and performance

**Core mental model:**

User → API → Backend/Services → Cache → Database → Response

Applications depend on data moving efficiently across multiple components. A slowdown at the data layer can surface as API latency or poor application performance even when the user never interacts directly with the database.

**Sales takeaway:**

Database performance is not just an engineering metric. Slow queries, overloaded systems, or inefficient data flows can affect application performance, customer experience, engineering time, and ultimately the business. Understanding the data layer helps me ask better questions about where bottlenecks occur and how teams investigate them.

### Day 8 — Hands-On API Integration

**Concepts applied:**
- REST APIs
- API endpoints
- GET and POST requests
- HTTP responses
- JSON request and response data
- Query parameters
- HTTP status codes
- Response time / latency
- API error handling
- Using Postman to test API requests

**What I did:**

I moved from learning about APIs conceptually to interacting with one directly using Postman and JSONPlaceholder.

I sent GET requests to retrieve data, used query parameters to filter the information returned, sent a POST request with JSON data to simulate creating a new resource, and intentionally made an unsuccessful request to see how the API communicated an error.

This gave me hands-on experience with the request → endpoint → response process and helped me understand how two software systems can exchange information through an API.

**Status codes observed:**
- `200 OK` — Request completed successfully
- `201 Created` — New resource successfully created/simulated
- `404 Not Found` — Requested resource could not be found

**Core mental model:**

Client → HTTP Request → API Endpoint → Server → HTTP Response → JSON → Client

**Sales takeaway:**

Working with an API directly helped me understand that an integration conversation goes beyond asking whether an API exists. Technical buyers may need to understand which endpoints are available, what data can be read or written, how requests are authenticated, what the response format looks like, how errors are handled, what rate limits exist, and whether the API can support their expected volume.

**Practical Project:**

`api-integration-exploration` — Hands-on exploration of API requests, JSON responses, HTTP status codes, query parameters, and integrations using Postman.

### Day 9 — Authentication, Authorization & API Security

**Concepts covered:**
- Authentication vs. authorization
- API keys
- Access tokens and bearer tokens
- OAuth
- Permission scopes
- Role-Based Access Control (RBAC)
- Principle of least privilege
- API credential security
- 401 vs. 403 responses

**Core mental model:**

Authentication → Who are you?

Authorization → What are you allowed to do?

A successful integration needs more than connectivity. Systems also need a secure way to establish identity and control what users or applications are permitted to access.

**Sales takeaway:**

Technical integration conversations can quickly become security conversations. Enterprise buyers may care about how an API authenticates requests, what permissions an integration requires, what data it can access, and whether access follows least-privilege principles. Understanding these concepts helps me recognize security concerns earlier and involve the right technical resources without overstating what I know.

## Projects

I'll add practical projects and technical product breakdowns as I progress.
