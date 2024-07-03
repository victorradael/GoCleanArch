
# GoCleanArch: A Learning Project for Clean Architecture and Domain-Driven Design

Welcome to GoCleanArch! This project is designed to help you learn and apply the principles of Clean Architecture and Domain-Driven Design (DDD) using the Go programming language. By following along with this project, you'll gain a deep understanding of these powerful design paradigms and learn how to implement them effectively in your software projects.

## Table of Contents

- [Introduction](#introduction)
- [Why Clean Architecture and DDD?](#why-clean-architecture-and-ddd)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Base projects for refactoring](#base-projects-for-refactoring)
- [Bibliography and References](#bibliography-and-references)
    - [Clean Architecture](#clean-architecture)
    - [Domain-Driven Design](#domain-driven-design-ddd)
    - [Pratical Material](#practical-material)

## Introduction

GoCleanArch is a sample project that demonstrates how to build a robust, maintainable, and scalable application using Clean Architecture and Domain-Driven Design principles. This project aims to provide a clear and practical example that you can follow and adapt to your own needs.

## Why Clean Architecture and DDD?

### Clean Architecture

Clean Architecture is a software design philosophy that aims to separate the concerns of different parts of an application. The main goals of Clean Architecture are:

- **Independent of Frameworks**: The architecture does not depend on the existence of some library of feature-laden software. This allows you to use such frameworks as tools rather than constraints.
- **Testable**: The business rules can be tested without the UI, Database, Web Server, or any other external element.
- **Independent of UI**: The UI can change easily, without changing the rest of the system.
- **Independent of Database**: You can swap out Oracle or SQL Server for Mongo, BigTable, CouchDB, or something else. Your business rules are not bound to the database.
- **Independent of any external agency**: In fact, your business rules simply don't know anything at all about the outside world.

### Domain-Driven Design

Domain-Driven Design (DDD) is an approach to software development that emphasizes collaboration between technical and domain experts to iteratively refine a conceptual model that addresses complex domain logic. The key concepts of DDD include:

- **Ubiquitous Language**: Creating a shared language between developers and domain experts to ensure that the domain model is well understood by all stakeholders.
- **Entities and Value Objects**: Differentiating between objects that have a distinct identity and those that are defined solely by their attributes.
- **Aggregates**: Grouping related entities and value objects into a single unit that ensures consistency and encapsulates the business rules.
- **Repositories**: Abstracting the persistence layer to provide a collection-like interface for accessing aggregates.
- **Domain Events**: Representing significant events in the domain that can trigger side effects or actions.

By learning and applying Clean Architecture and DDD, you will be able to build systems that are:

- **Maintainable**: Easier to understand, modify, and extend over time.
- **Testable**: With well-defined boundaries and dependencies, making unit and integration testing more straightforward.
- **Scalable**: Architected to handle growth and changes in requirements with minimal friction.

## Project Structure

This project follows the principles of Clean Architecture and DDD, organizing code into distinct layers with clear responsibilities. The basic structure is as follows:

```
GoCleanArch/
├── cmd/                # Command-line executables
│   └── main.go         # Entry point for the application
├── internal/           # Internal application code
│   ├── domain/         # Domain layer (Entities, Value Objects, Aggregates)
│   ├── usecases/       # Use cases (Application services, Interactors)
│   ├── interfaces/     # Interfaces (Controllers, Gateways, Repositories)
│   └── infrastructure/ # Infrastructure (Database, Web Framework, etc.)
├── pkg/                # Shared utility code
└── README.md           # This file
```

## Getting Started

To get started with GoCleanArch, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/GoCleanArch.git
    cd GoCleanArch
    ```

2. **Install dependencies**:
    Ensure you have Go installed on your machine. Then, run:
    ```bash
    go mod tidy
    ```

3. **Run the application**:
    ```bash
    go run cmd/main.go
    ```

## Usage

This project includes example use cases and domain models that you can explore and modify. Follow the comments and documentation within the code to understand how each part of the application is structured and how they interact with each other.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Base projects for refactoring

- [Api Rest Go (mux)](https://github.com/victorradael/rest_api_go_mux)
- [Api Rest Go (gin)](https://github.com/victorradael/rest_api_go_gin)

## Bibliography and References

### Clean Architecture

#### Philosophies and Concepts

- **Books**
  - Robert C. Martin, *Clean Architecture: A Craftsman's Guide to Software Structure and Design*. [Link](https://www.amazon.com/Clean-Architecture-Craftsmans-Software-Structure/dp/0134494164)

  - Leonardo Giordani, *Clean Architecture in Python*. [Link](https://leanpub.com/clean-architectures-in-python)

- **Articles and Blogs**
  - Robert C. Martin, *The Clean Architecture*. [Link](https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html)


- **Videos**
  - Robert C. Martin, *Clean Architecture with Uncle Bob Martin*. [Link](https://www.youtube.com/watch?v=o_TH-Y78tt4)

### Domain-Driven Design (DDD)

#### Philosophies and Concepts

- **Books**
  - Eric Evans, *Domain-Driven Design: Tackling Complexity in the Heart of Software*. [Link](https://www.amazon.com/Domain-Driven-Design-Tackling-Complexity-Software/dp/0321125215)
  - Vaughn Vernon, *Implementing Domain-Driven Design*. [Link](https://www.amazon.com/Implementing-Domain-Driven-Design-Vaughn-Vernon/dp/0321834577)

- **Articles and Blogs**
  - Eric Evans, *Domain-Driven Design Reference: Definitions and Pattern Summaries*. [Link](https://www.domainlanguage.com/ddd/reference/)
  - Martin Fowler, *The Anatomy of Domain-Driven Design*. [Link](https://martinfowler.com/bliki/DomainDrivenDesign.html)

- **Videos**
  - Eric Evans, *DDD Europe 2020 - Eric Evans Keynote*. [Link](https://www.youtube.com/watch?v=am-HXycfalo&list=PLf9p-N3ltMTvfEj8KNtOomc9algcX0WtG)

### Practical Material

- **GitHub Repositories**
  - *Clean Architecture Template for .NET*. [Link](https://github.com/jasontaylordev/CleanArchitecture)
  - *Awesome Domain-Driven Design*: Curated list of DDD resources. [Link](https://github.com/heynickc/awesome-ddd)

