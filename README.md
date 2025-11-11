# Metacogna.ai by PratejraTech

**Metacogna.ai** is an AI-native orchestration platform designed to **think about thinking**.  
It helps individuals and teams plan, iterate, and execute complex ideas by combining **meta-cognitive reasoning**, **intelligent orchestration**, and **tool adapters** into a seamless workflow.

Metacogna.ai is built on cutting-edge **LLMOps** and **MLOps** practices, providing both the **structure** of a project manager and the **adaptability** of an AI collaborator.

---

## ✨ Key Features

- **Meta-Cognition at the Core**  
  Every workflow includes *reasoning → critique → refinement* cycles, inspired by Self-Refine and RLHF research.  
  Iteration isn’t optional — it’s the default.

- **Phased Idea Development**  
  Projects are decomposed into **3–6 structured phases**, enumerated into tasks with clear acceptance criteria.  
  Supports both solo workflows and collaborative, cross-functional teams.

- **Plugin-Oriented Architecture**  
  Abstract adapters connect to tools you already use:
  - LLM providers (OpenAI, Anthropic, local LLMs)
  - Design (Figma)
  - Development (v0.dev, Replit, GitHub)
  - PM (Jira, Notion, Trello)
  - Observability (LangSmith, Prometheus)

- **Intelligent Notifications**  
  Event-based and phase-based updates keep you informed.  
  Ask *“What’s next?”* at any time for a compressed **Next Steps summary**.

- **Collaboration via “Pong”**  
  A translation layer that converts business, design, and engineering language across teams.  
  No more lost-in-translation moments — Pong ensures everyone stays aligned.

- **Privacy-First Design**  
  - **Paid tier:** strict workspace isolation, no data training.  
  - **Free tier:** anonymized “data exhaust” improves system recommendations.  

---

## 🧩 Architecture Overview

Metacogna.ai follows a **microservice + orchestrator** model:

- **Gateway API** – entry point, auth, rate limits  
- **Orchestrator** – LangGraph-style flow control, state machine  
- **Planner** – LLM-based reasoning, phase decomposition  
- **Recommender/Evaluator** – verifies plans, benchmarks against top repos, ROAI calculations  
- **Plugin Registry** – abstract adapters for design/dev/PM tools  
- **Build Runner** – executes jobs (design sync, scaffolds, testing)  
- **Notifications** – milestone + guidance engine  
- **Collab-Pong** – cross-role communication translator  
- **Storage** – domain model persistence, artifacts, audit trail  
- **Ops & Monitoring** – LangSmith integration, observability, dashboards  

Each module is **decoupled** via contracts and events. Services can be swapped or extended without disrupting the whole.

---

## 🚀 MVP Roadmap (8 Phases)

1. **Foundations** – Service skeletons, contracts, observability  
2. **Core State** – `.parti` config for acceptance criteria, budgets, providers  
3. **Orchestration** – Idea decomposition + self-refine planning loop  
4. **Task Atomization** – Enumeration into tasks, optional Jira mapping  
5. **Verification** – Recommender engine + ROAI analysis  
6. **Collaboration** – Pong-enabled team translation  
7. **Adapters** – Figma/v0/Replit integrations, build-runner jobs  
8. **Notifications & Privacy** – Rich UX, paid/free privacy policies, release  

---

## 📊 Use Cases

- **Solo Builders**  
  Plan and execute side projects with guided iteration.  
- **Startups**  
  Align business, design, and engineering through a shared, AI-enhanced hub.  
- **Enterprises**  
  Standardize AI project development with privacy-safe, observable workflows.  
- **Research Teams**  
  Experiment with modular LLM orchestration and reinforcement loops.

---

## 🛡️ Philosophy

> *Iteration is king.  
> If in doubt, iterate again.*  

Metacogna.ai is designed to embody a **growth mindset**:  
- Always critique and refine.  
- Benchmark against the best.  
- Integrate human feedback at every step.  
- Never stop learning from usage (data exhaust → better recommendations).  

---

## 🛠️ Tech Stack

- **Frontend:** Next.js 15 (dynamic notebook UI + browser extension)  
- **Backend:** Next.js API routes, orchestrator in LangGraph  
- **Monitoring:** LangSmith for eval & tracing, structured logs  
- **Data:** JSON schema contracts, lightweight storage, optional vector DB  
- **Deployment:** Replit-first microservices, containerizable for cloud  
- **Collab Layer:** Pong agent for translation & mediation  

---

## 📖 Documentation

- [Architecture ADRs](./docs/architecture)  
- [Service Contracts](./docs/contracts)  
- [User Guide](./docs/user-guide.md)  
- [Contributing](./CONTRIBUTING.md)

---

## 🤝 Contributing

We welcome contributions!  
- Fork, branch, and PR your changes.  
- Follow our [contribution guidelines](./CONTRIBUTING.md).  
- Propose new **plugin adapters** or **evaluation methods** via the Plugin Registry.

---

## 📜 License

Metacogna.ai is released under the MIT License. See [LICENSE](./LICENSE) for details.

---

## 🌐 Links

- Website: [https://metacogna.ai](https://metacogna.ai)  
- Docs: [https://docs.metacogna.ai](https://docs.metacogna.ai)  
- Community: [Discord Invite]  

---
