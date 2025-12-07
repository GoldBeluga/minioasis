# Minioasis Library System

Minioasis Library System is an open-source project that modernises and rebuilds the core business logic of a [legacy Java-based library application](https://github.com/minioasis/minioasis-library). The new system is rewritten completely in **ASP.NET**, with a clean architecture that separates domain logic, data infrastructure, and UI concerns.

This version focuses on maintainability, testability, and long-term viability as an open-source, self-hosted library management system that small libraries, community groups, schools, or individuals can deploy easily.

## 🧱 Architecture Overview

The system is being rebuilt using a layered, domain-centric architecture:

- **Domain Layer**  
  - Contains pure C# business logic, entities, rules, and service interfaces.  
  - No ASP.NET dependencies. No Telegram/API/UI code.  
  - This makes the project testable and easy to extend.

- **Infrastructure Layer**  
  - Implements persistence using EF Core, repositories, and database access.  
  - Follows interfaces defined in the Domain layer.

- **Web Layer – Blazor Server**  
  - The admin interface is implemented with **Blazor Server**, allowing direct C# calls to domain services without requiring an HTTP API at this stage.  
  - This keeps the system simple while preserving future flexibility.

- **Internal API (Planned)**  
  An API layer will be added later only if needed, for features such as:
  - Telegram bot connectivity  
  - Mobile app support  
  - External integrations  
  - Multi-library deployments  

Because the domain layer is API-ready, adding this will be straightforward.

## 🚀 Project Goals

- Clean, modular rewrite of the legacy Java system  
- Fully open-source and community-maintainable  
- Installation-friendly through Docker  
- Modern technology stack (ASP.NET, EF Core, Blazor Server)  
- Stable core domain logic with clear boundaries  
- Self-hosted deployment for small libraries  
- Optional internal API for automation, bot integration, or expansion

## 👫 Open Source Contributors Welcome

This project is actively seeking contributors to help with:

- Implementing domain logic from the legacy system  
- Expanding Blazor Server admin UI  
- Improving EF Core repositories and data modelling  
- Writing automated tests for domain logic  
- Docker packaging and deployment improvements  
- Documentation and installation guides  
- Feature proposals and UX improvements

We welcome:
- ASP.NET and Blazor developers  
- Students learning backend design  
- Developers familiar with Java/Spring who can help translate logic  
- Contributors interested in clean architecture or DDD patterns  
- Anyone who wants to help build a modern, free, open-source library system

## 🤝 How to Contribute
Feel free to contact me on Discord at `wang10w`
