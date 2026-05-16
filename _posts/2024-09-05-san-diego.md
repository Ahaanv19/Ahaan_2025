---
layout: post
title:  Final Project CS 113
permalink: /csmiracosta/
toc: true
---


# Final Project: CS 113 Capstone Reflection and Evidence

This final project serves as my formal CS 113 capstone reflection and evidence portfolio. Across my projects, I demonstrated growth in Java, JavaScript, Python, object-oriented programming, API development, deployment, testing, documentation, and full software engineering practices. Most importantly, I built projects that connect computing to real-world and socially meaningful problems such as food insecurity, community logistics, routing, educational systems, and user support workflows.

This portfolio is designed to show how I met the CS 113 learning objectives through authentic project work, documented engineering decisions, and linked repository evidence.

---

## Project Portfolio Overview

### Main Repositories Referenced
- [Ahaan_2025](https://github.com/Ahaanv19/Ahaan_2025)
- [hunger_heroes](https://github.com/Ahaanv19/hunger_heroes)
- [hunger_heroes_backend](https://github.com/Ahaanv19/hunger_heroes_backend)
- [hunger_heroes_backend_spring-](https://github.com/Ahaanv19/hunger_heroes_backend_spring-)
- [SD_Auto_Backend](https://github.com/Ahaanv19/SD_Auto_Backend)
- [SD_Auto_Frontend](https://github.com/Ahaanv19/SD_Auto_Frontend)

### Capstone Theme
My work focused on projects with personal and social relevance, especially:
- food donation and community support systems
- traffic routing and commuter planning
- user workflows such as hall pass systems, assignment systems, and progress/rubric tools
- scalable deployment with Docker, nginx, and backend/frontend integration
- reflective blogging and portfolio documentation to explain not just what I built, but why I built it and what I learned

---

## Final Reflection

Throughout this course, I moved beyond isolated assignments and developed the ability to build complete systems. My projects required me to think like both a programmer and an engineer: planning features, organizing tasks, debugging issues, documenting my work, integrating frontend and backend systems, and reflecting on how computing affects people and communities.

One of the strongest examples of this growth is the transition from early frontend/backend connection work in my blog repository into larger full-stack projects like Hunger Heroes and SD Auto. In those projects, I had to manage real APIs, persistence layers, route logic, user state, authentication, deployment environments, and team-oriented software practices. I also had to reflect on ethics, accessibility, usability, and community impact.

The Java Spring Boot work in `hunger_heroes_backend_spring-` is especially important for CS 113 because it demonstrates college-level backend engineering practices using JPA/Hibernate, REST APIs, entity relationships, repositories, collections, abstraction, inheritance, testing structure, and deployment tooling. My supporting repos strengthen that evidence by showing frontend integration, documentation, debugging reflections, and software lifecycle habits across multiple real projects.

---

# CS 113 Requirement Alignment Chart

## Assessment Key
- **Met** = clear implementation evidence in project code and/or documentation
- **Met + Reflected** = implemented and also explained in blog/documentation
- **Met Across Multiple Projects** = demonstrated in more than one repository

---

| CS 113 Requirement | Status | Project(s) | Evidence Link(s) | How I Met the Requirement |
|---|---|---|---|---|
| **Backend implementation using Java Spring Boot with JPA/Hibernate** | **Met** | hunger_heroes_backend_spring- | [pom.xml](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/pom.xml), [BankJpaRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/bank/BankJpaRepository.java), [RubricRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/onboarding_hacks_rubric/RubricRepository.java), [Rubric.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/onboarding_hacks_rubric/Rubric.java) | This project uses Spring Boot with a Maven build, Spring Data JPA repositories, and JPA entities with annotations such as `@Entity`, `@Table`, `@Id`, `@GeneratedValue`, and repository interfaces extending `JpaRepository`. |
| **3+ data structures appropriately applied** | **Met** | hunger_heroes_backend_spring- | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md), [TasksJpaRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/mortevision/TasksJpaRepository.java), [AdventureApiController.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/rpg/adventure/AdventureApiController.java) | The project documents and uses multiple structures including `ArrayList`, `HashMap`, `HashSet`, `LinkedHashMap`, `ConcurrentHashMap`, queues, and tree/graph-related structures. This exceeds the 3+ minimum. |
| **Collections** | **Met** | hunger_heroes_backend_spring- | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md) | The requirements document explicitly maps collection usage including `ArrayList`, `HashMap`, `HashSet`, `LinkedHashMap`, and `ConcurrentHashMap` to application features. |
| **Lists** | **Met** | hunger_heroes_backend_spring-, SD_Auto_Backend | [AssignmentSubmission.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/assignments/AssignmentSubmission.java), [TasksJpaRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/mortevision/TasksJpaRepository.java) | I used lists in model relationships, repository return types, and ordered task/assignment handling. This demonstrates adding, retrieving, ordering, and iterating over data in service-oriented workflows. |
| **Stacks / Queues** | **Met** | hunger_heroes_backend_spring- | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md), [schema_full.txt](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/schema_full.txt) | The project documents queue and stack-related data structures as part of its internal rubric mapping and application design, including task queues and structured processing flows. |
| **Trees** | **Met** | hunger_heroes_backend_spring- | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md) | The requirements file documents tree structure evidence and references category tree testing. This shows tree-based structure usage in the backend. |
| **Sets** | **Met** | hunger_heroes_backend_spring- | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md) | Sets are used for uniqueness and filtering logic, including validation-style operations and allowed value control. |
| **Dictionaries / Maps** | **Met** | hunger_heroes_backend_spring-, SD_Auto_Backend | [AdventureApiController.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/rpg/adventure/AdventureApiController.java), [api/route.py](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/api/route.py) | I used `Map<String,Object>` in Java API responses and mapping logic, and JSON/dictionary-based APIs in Python backends for structured data exchange. |
| **Graphs** | **Met** | hunger_heroes_backend_spring- | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md) | The project documents graph data structure implementation and graph testing, including BFS/DFS-level evidence through its backend rubric mapping. |
| **2+ algorithms implemented with complexity analysis** | **Met** | hunger_heroes_backend_spring-, Ahaan_2025 | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md), [2025-6-08-homefinal.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-6-08-homefinal.md) | My Spring backend explicitly documents algorithms including binary search, BFS, DFS, and priority scoring, while my blog portfolio also references Big-O and algorithm work completed in notebooks. |
| **Searching** | **Met** | hunger_heroes_backend_spring- | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md) | Search is documented both through search methods in repositories and through the project’s internal evidence of linear and binary search. |
| **Sorting** | **Met** | hunger_heroes_backend_spring-, SD_Auto_Backend | [BankJpaRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/bank/BankJpaRepository.java), [TasksJpaRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/mortevision/TasksJpaRepository.java) | I implemented sorted queries and ordering logic, such as balances descending and tasks by due date ascending, which are practical backend uses of sorting. |
| **Hashing** | **Met** | hunger_heroes_backend, hunger_heroes_backend_spring- | [API_STRUCTURE_GUIDE.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docs/API_STRUCTURE_GUIDE.md), [model/user.py](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/model/user.py) | I implemented password hashing in backend authentication workflows and documented the security model in my API docs. |
| **Algorithm analysis** | **Met + Reflected** | hunger_heroes_backend_spring-, Ahaan_2025 | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md), [2025-6-08-homefinal.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-6-08-homefinal.md) | My project evidence includes Big-O style analysis and explicit algorithm complexity documentation, and my blog work shows that I studied and reflected on algorithmic efficiency. |
| **Complete object-oriented design with abstraction** | **Met** | hunger_heroes_backend_spring- | [Generics.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/hacks/classDataStruct/Generics.java) | I created and used abstract classes and abstract methods to define reusable contracts and behavior. |
| **Encapsulation** | **Met** | hunger_heroes_backend_spring-, SD_Auto_Backend, hunger_heroes_backend | [Rubric.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/onboarding_hacks_rubric/Rubric.java), [RouteUsage model](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/model/subscription.py), [user.py](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/model/user.py) | My models encapsulate state and expose behavior through methods, getters, setters, and controlled persistence logic. |
| **Inheritance** | **Met** | hunger_heroes_backend_spring- | [Teacher.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/identity/Teacher.java) | `Teacher` extends `User`, demonstrating inheritance and specialized behavior in an identity system. |
| **Polymorphism** | **Met** | hunger_heroes_backend_spring- | [Teacher.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/identity/Teacher.java), [Generics.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/hacks/classDataStruct/Generics.java) | Polymorphism appears through inheritance hierarchies and abstract method contracts that allow different subclasses to define specialized implementations. |
| **Design patterns (MVC, Repository, etc.)** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend, SD_Auto_Backend | [RubricController.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/onboarding_hacks_rubric/RubricController.java), [RubricRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/onboarding_hacks_rubric/RubricRepository.java), [__init__.py](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/__init__.py) | My Java backend follows MVC and repository architecture, and my Python backends also separate API, model, and persistence concerns. |
| **Version control** | **Met** | all repos | [Ahaan_2025](https://github.com/Ahaanv19/Ahaan_2025), [hunger_heroes](https://github.com/Ahaanv19/hunger_heroes), [hunger_heroes_backend_spring-](https://github.com/Ahaanv19/hunger_heroes_backend_spring-) | My work is version controlled across multiple repositories with structured commit history and tracked feature development. |
| **Source control, branching, pull requests, merging/integrating** | **Met** | all repos | [Ahaan_2025 issues/PR environment](https://github.com/Ahaanv19/Ahaan_2025), [hunger_heroes project repo](https://github.com/Ahaanv19/hunger_heroes) | My projects were developed through GitHub-based workflows that included issue tracking, commits, merges, and integration across project phases. |
| **Testing** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md), [POSTMAN_TESTING_GUIDE.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docs/POSTMAN_TESTING_GUIDE.md) | My Java project documents JUnit/Mockito-style tests and broad testing coverage, while my Flask backend includes detailed Postman API testing workflows. |
| **JUnit tests for critical functionality (>50% coverage)** | **Met** | hunger_heroes_backend_spring- | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md) | The requirements file explicitly documents 73 tests across 6 files and identifies JUnit/service/data-structure coverage. |
| **Build tools (Maven/Gradle)** | **Met** | hunger_heroes_backend_spring- | [pom.xml](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/pom.xml) | The Java Spring backend uses Maven as a formal build and dependency management tool. |
| **Debugging** | **Met + Reflected** | Ahaan_2025, hunger_heroes_backend, SD_Auto_Backend | [reflection.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-02-26-reflection.md), [san-diego.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2024-09-05-san-diego.md), [API_STRUCTURE_GUIDE.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docs/API_STRUCTURE_GUIDE.md) | My blogs describe debugging workflows involving CORS, API mismatches, logging, and iterative fixing, while my backend docs show structured troubleshooting and error handling. |
| **RESTful API with proper HTTP methods, status codes, and error handling** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend, SD_Auto_Backend | [RubricController.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/onboarding_hacks_rubric/RubricController.java), [AdventureApiController.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/rpg/adventure/AdventureApiController.java), [api/route.py](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/api/route.py) | My APIs use GET, POST, PUT, and other methods appropriately, with structured status codes like 200, 201, 400, 404, and 429, plus error responses for invalid input and missing resources. |
| **Database integration with proper entity relationships and queries** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend, SD_Auto_Backend | [AssignmentSubmission.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/assignments/AssignmentSubmission.java), [schema_full.txt](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/schema_full.txt), [__init__.py](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/__init__.py), [sections.py](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/api/sections.py) | My projects demonstrate real persistence models, JPA relationships (`@ManyToOne`, `@ManyToMany`, join tables), SQLAlchemy configuration, and SQLite-backed CRUD workflows. |
| **Docker deployment with docker-compose configuration** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend, SD_Auto_Backend | [Dockerfile](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/Dockerfile), [docker-compose.yml](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/docker-compose.yml), [Dockerfile Python backend](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/Dockerfile), [docker-compose Python backend](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docker-compose.yml) | I containerized backend services and configured compose-based deployment workflows. |
| **Custom domain with DNS and nginx configuration** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend | [nginx_for_flask_8585](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/nginx_for_flask_8585), [litconnect.stu.nginx_file](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/litconnect.stu.nginx_file) | These configs show deployment behind nginx with domain-based routing and production-oriented reverse proxy configuration. |
| **nginx reverse proxy** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend | [nginx_for_flask_8585](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/nginx_for_flask_8585), [litconnect.stu.nginx_file](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/litconnect.stu.nginx_file) | I configured reverse proxy behavior, headers, forwarded request handling, and CORS-aware deployment. |
| **CI/CD** | **Met** | Ahaan_2025 and site repos | [README.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/README.md) | My site/documentation workflow uses GitHub Pages Actions and automated rebuild/deploy behavior, showing continuous integration and deployment practices in my project ecosystem. |
| **Code comments / JavaDoc comments** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend, SD_Auto_Backend | [TinkleJPARepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/bathroom/TinkleJPARepository.java), [scripts/db_init.py](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/scripts/db_init.py), [user.py](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/model/user.py) | My public-facing classes, repositories, utility code, and models include descriptive comments and docstring-style documentation to explain functionality and engineering intent. |
| **API documentation** | **Met** | hunger_heroes_backend | [POSTMAN_TESTING_GUIDE.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docs/POSTMAN_TESTING_GUIDE.md), [API_STRUCTURE_GUIDE.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docs/API_STRUCTURE_GUIDE.md) | I documented endpoints, request formats, workflows, auth behavior, and testing instructions in detail. |
| **Help system / user guide / help documentation** | **Met** | hunger_heroes_backend, Ahaan_2025 | [API_STRUCTURE_GUIDE.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docs/API_STRUCTURE_GUIDE.md), [POSTMAN_TESTING_GUIDE.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docs/POSTMAN_TESTING_GUIDE.md), [Ahaan_2025 README](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/README.md) | I created documentation that helps users and developers understand setup, features, endpoint usage, and backend behavior. |
| **Blog portfolio documenting design decisions and contributions** | **Met** | Ahaan_2025 | [reflection.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-02-26-reflection.md), [san-diego.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2024-09-05-san-diego.md), [testflocker.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2024-10-24-testflocker.md), [homefinal.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-6-08-homefinal.md) | My blog repository contains retrospectives, backend/frontend setup reflections, algorithm learning, database design, exam reflections, and personal feature writeups that document my growth and technical decisions. |
| **Software engineering practices: planning changes, checklists, tracking progress, writing commented code, help documentation** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend, Ahaan_2025 | [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md), [DATA_INTEGRITY_CHECKLIST.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/DATA_INTEGRITY_CHECKLIST.md), [reflection.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-02-26-reflection.md) | My work shows engineering planning through requirement mapping, checklists, documentation, and reflective process writing. |
| **Software development lifecycle practices** | **Met** | all repos | [Ahaan_2025 README](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/README.md), [hunger_heroes backend repos](https://github.com/Ahaanv19/hunger_heroes_backend), [spring backend repo](https://github.com/Ahaanv19/hunger_heroes_backend_spring-) | My work includes version control, build processes, testing, deployment, documentation, issue tracking, and integration across multiple repositories. |
| **Retrospective engineering practices** | **Met + Reflected** | Ahaan_2025 | [reflection.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-02-26-reflection.md), [sprint2journey.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2024-10-15-sprint2journey.md) | I documented strengths, weaknesses, lessons learned, next steps, and reflective evaluation of my engineering process. |
| **Data types: numbers, strings, booleans, arrays, JSON objects, SQLite tables** | **Met** | all repos | [Game.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/rpg/games/Game.java), [Adventure.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/rpg/adventure/Adventure.java), [sections.py](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/api/sections.py) | My projects use primitive and composite data types in models, APIs, JSON responses, and persistent storage. |
| **Operators: string, mathematical, boolean** | **Met** | Ahaan_2025, hunger_heroes_backend_spring-, SD_Auto_Backend | [homefinal.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-6-08-homefinal.md), [api/route.py](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/api/route.py) | Across notebooks, backend logic, and controllers, I used mathematical calculations, boolean checks, and string processing for real application functionality. |
| **Control structures: iteration, conditions, nested conditions, try/except, .then/.catch** | **Met** | Ahaan_2025, SD_Auto_Backend, hunger_heroes_backend_spring- | [profile.js](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/assets/js/api/profile.js), [route.py](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/api/route.py), [AdventureApiController.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/rpg/adventure/AdventureApiController.java) | My projects demonstrate loops, branching, exception handling, async JavaScript chains, and conditional logic in both frontend and backend code. |
| **Input/Output: HTML5 input, validation, and DOM work** | **Met** | Ahaan_2025, SD_Auto_Frontend | [index.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/index.md), [home.html](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_includes/nav/home.html), [profile.js](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/assets/js/api/profile.js) | I used DOM manipulation, input handling, event listeners, validation patterns, and dynamic page updates in frontend code. |
| **Classes / methods / instantiation / parameters / return values** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend, SD_Auto_Backend | [Game.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/rpg/games/Game.java), [RouteUsage model](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/model/subscription.py), [user.py](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/model/user.py) | My backend projects are built around classes, constructors, methods, object instantiation, and method-based business logic. |
| **Deployment practices: DNS, Docker, docker-compose, nginx** | **Met** | hunger_heroes_backend_spring-, hunger_heroes_backend | [Dockerfile](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/Dockerfile), [docker-compose.yml](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/docker-compose.yml), [nginx_for_flask_8585](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/nginx_for_flask_8585), [litconnect.stu.nginx_file](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/litconnect.stu.nginx_file) | My deployment setup shows real production-oriented hosting and reverse proxy design. |
| **Project impact / authentic real-world problem** | **Met + Reflected** | hunger_heroes, SD_Auto, Ahaan_2025 | [hunger_heroes backend home](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/templates/index.html), [SD_Auto README](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/README.md), [reflection.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-02-26-reflection.md) | Hunger Heroes addresses food insecurity and donation logistics; SD Auto addresses traffic routing and local transportation efficiency. These are meaningful, real-world applications of computing. |
| **Ethical considerations: privacy, security, accessibility, equity** | **Met + Reflected** | hunger_heroes_backend, Ahaan_2025 | [API_STRUCTURE_GUIDE.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docs/API_STRUCTURE_GUIDE.md), [reflection.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-02-26-reflection.md) | I addressed secure auth, hashed passwords, controlled access, CORS handling, and community-centered design concerns. My reflection also discusses how computing systems affect real people. |
| **LinkedIn / professional presentation of work** | **Met** | personal portfolio / final project presentation | N/A in repo issue body | I have presented my work professionally as part of my final project documentation and portfolio growth. This requirement is part of my broader capstone presentation of skills and accomplishments. |

---

# Detailed Evidence by Category

## 1. Java Spring Boot + JPA/Hibernate
The strongest direct evidence for CS 113 college-credit alignment comes from `hunger_heroes_backend_spring-`.

### Key Evidence
- [pom.xml](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/pom.xml)
- [Rubric.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/onboarding_hacks_rubric/Rubric.java)
- [RubricRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/onboarding_hacks_rubric/RubricRepository.java)
- [RubricController.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/onboarding_hacks_rubric/RubricController.java)

### Reflection
This repo demonstrates a true Java backend architecture using Spring Boot, repositories, and entity-based persistence. This was important for me because it moved my work into a more professional backend engineering style. Instead of only building frontend features or small scripts, I had to work with controllers, repositories, entities, object relationships, and HTTP APIs in a structured framework.

---

## 2. Object-Oriented Programming
### Key Evidence
- [Teacher.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/identity/Teacher.java)
- [Generics.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/hacks/classDataStruct/Generics.java)
- [Game.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/rpg/games/Game.java)

### Reflection
OOP became much more meaningful when I used it in real systems. Inheritance was no longer just a classroom idea — it became part of my user model design. Abstraction mattered because it helped organize code and enforce contracts. Encapsulation became necessary for maintainability. Polymorphism helped make my architecture flexible instead of repetitive.

---

## 3. Algorithms and Data Structures
### Key Evidence
- [REQUIREMENTS.md](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/REQUIREMENTS.md)
- [BankJpaRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/bank/BankJpaRepository.java)
- [TasksJpaRepository.java](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/src/main/java/com/open/spring/mvc/mortevision/TasksJpaRepository.java)
- [2025-6-08-homefinal.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-6-08-homefinal.md)

### Reflection
I learned that data structures are not just definitions to memorize. They directly affect performance, clarity, and scalability. Using collections, maps, sets, queues, and algorithmic thinking in real code helped me understand why computer science matters in actual software systems.

---

## 4. Full Software Development Lifecycle
### Key Evidence
- [Ahaan_2025 README](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/README.md)
- [POSTMAN_TESTING_GUIDE.md](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/docs/POSTMAN_TESTING_GUIDE.md)
- [Dockerfile](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/Dockerfile)
- [docker-compose.yml](https://github.com/Ahaanv19/hunger_heroes_backend_spring-/blob/0acdd6a38f608f6ff6929ad849a78ecb1a8c148f/docker-compose.yml)

### Reflection
One of the biggest ways I grew was by learning that writing code is only one part of software engineering. Planning, testing, deploying, documenting, debugging, and revising are all part of producing a functioning project. My repositories show that I learned how to build not just code, but a process.

---

## 5. Documentation and Reflection
### Key Evidence
- [2025-02-26-reflection.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-02-26-reflection.md)
- [2024-09-05-san-diego.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2024-09-05-san-diego.md)
- [2024-10-24-testflocker.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2024-10-24-testflocker.md)
- [2025-6-08-homefinal.md](https://github.com/Ahaanv19/Ahaan_2025/blob/af1ed34f1da7d3d8ee3e9087bbdbab6a5d143e30/_posts/2025-6-08-homefinal.md)

### Reflection
My blog portfolio is important because it shows that I can explain my thinking, not just code silently. This matters for college-level work because strong engineering includes communication, reflection, and the ability to justify design choices.

---

## 6. Personal and Social Relevance
### Hunger Heroes
- [Backend home page](https://github.com/Ahaanv19/hunger_heroes_backend/blob/52de39a86e669ba644ff33bbd5f37667f6816efa/templates/index.html)

### SD Auto
- [SD Auto Backend README](https://github.com/Ahaanv19/SD_Auto_Backend/blob/b71610f767a23013dd2321cf441633e8994341a6/README.md)

### Reflection
I intentionally worked on projects that connect computing to actual community needs. Hunger Heroes focuses on food donation systems, logistics, safety, and support for people in need. SD Auto focuses on route efficiency, traffic analysis, and better commuter planning. These projects helped me understand that computing has ethical, civic, and human consequences.

---

## Why This Portfolio Deserves CS 113 Credit

I believe this body of work demonstrates competency in all CS 113 learning objectives because it shows:
- real Java Spring Boot backend engineering
- object-oriented design at the class and system level
- use of data structures and algorithms in authentic projects
- REST API development with persistence and error handling
- deployment with Docker, nginx, and production-style configuration
- testing and debugging workflows
- extensive documentation and reflective writing
- meaningful application of computing to real-world problems

This is not a single isolated assignment. It is a portfolio of sustained growth across multiple projects that together demonstrate my readiness for college-level computer science credit.

---

## Final Statement

This issue serves as my formal CS 113 capstone evidence submission. The linked repositories, files, and reflections show how I met the learning objectives through applied software engineering, documented reasoning, and authentic project development. I am proud of the range of work represented here because it reflects not just what I built, but how I grew into a more complete computer science student and engineer.

Thank you for reviewing my final project and CS 113 evidence portfolio.
