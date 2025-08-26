## Repository Description

**spring-tx-board-demos**
This repository is a collection of Spring Boot demo projects, all integrated with the [spring-tx-board](https://github.com/Mamun-Al-Babu-Shikder/spring-tx-board) tool.

The purpose of this repo is to **demonstrate, experiment, and observe** transaction behavior in Spring using **spring-tx-board**.
Each project may cover a specific transaction scenario (propagation, isolation, rollbacks, multi-datasource, etc.) or simply serve as a **contributor’s playground** for testing and showcasing transaction monitoring.

This repo is intended for:

* Learning how Spring manages transactions in different cases
* Experimenting with **spring-tx-board** features
* Serving as a central hub for multiple contributors to add their own demos

---

## 📂 Folder Structure

```
spring-tx-board-demos/
│── README.md                     # Overview + contribution guide
│── common-config/                # (Optional) Shared configs/utilities
│
├── demos/
│   ├── basic-transactions/       # Example demo: Simple commit/rollback
│   ├── propagation-demo/         # Example demo: Propagation behaviors
│   ├── isolation-demo/           # Example demo: Isolation levels
│   ├── rollback-scenarios/       # Example demo: Rollbacks & exceptions
│   ├── multi-datasource-demo/    # Example demo: Multi-datasource transactions
│   ├── user-demo-<name>/         # Contributor-added demo project
│   │   ├── src/main/java/...  
│   │   └── pom.xml / build.gradle
│   │
│   └── ... (more user projects)
│
└── pom.xml / build.gradle        # Parent build file (manages deps for all demos)
```

---

### Contribution Flow

* Each demo project lives in its own folder under `/demos`.
* Contributors can add **their own demo project** (e.g., `user-demo-alice`, `payment-service-demo`, etc.).
* All projects must integrate **spring-tx-board** to provide consistent transaction observation.
* The repo uses a **parent build** maven so dependencies are centrally managed.

