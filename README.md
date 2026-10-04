# Learning Java 25

📖 **Read the tutorial: [https://stahe.github.io/en-java-oct-2026/](https://stahe.github.io/en-java-oct-2026/)**

This course teaches the [Java](https://dev.java/) 25 language **through examples**: over two hundred programs (320 Java files), commented line by line, with their execution results included. It starts with the basics of the language and covers database access with JDBC and Hibernate, network programming, and web services with Spring Boot.

This is the Java port of the course [Learning C# 14 with .NET 10](https://stahe.github.io/en-csharp-oct-2026/) (October 2026), which itself is a rewrite of a 2008 C# course: same outline, same examples, same overarching theme, but written in modern Java. All programs compile **without errors or warnings** using JDK 25 (`javac -Xlint:all`) and have been run; the results shown in the course are those from these runs.

| C# 14 Course (2026) | Java 25 Course (2026) |
|---|---|
| C# 14, .NET 10 (LTS) | Java 25 (LTS), JDK 25 |
| single-file applications (`dotnet run prog.cs`) | compact source files (`java Prog.java`) |
| `.csproj` projects, `.slnx` solutions, NuGet | Maven projects (`pom.xml`), Maven Central |
| properties, structures, operator overloading | accessors, records, sealed classes, pattern matching |
| LINQ | Stream API |
| delegates and events | functional interfaces, lambdas, listeners |
| `Task`, `async` / `await` | `CompletableFuture`, virtual threads |
| MSTest, Microsoft.Extensions.DependencyInjection | JUnit 6, Spring Framework 7 |
| System.Text.Json | Jackson 3 |
| ADO.NET, MySqlConnector | JDBC, MySQL Connector/J, HikariCP |
| Entity Framework Core | **Hibernate 7** (Jakarta Persistence 3.2) |
| `HttpClient`, `TcpClient` / `TcpListener` | `java.net.http.HttpClient`, `Socket` / `ServerSocket` |
| ASP.NET Core Minimal API | Spring Boot 4 |

## Course Outline

| Chapter | Content |
|---|---|
| Installation | JDK 25, IntelliJ IDEA / VS Code, the `java` and `javac` commands, compact source files, Maven, multi-module projects |
| Language Basics | types, `var`, code blocks, conversions, arrays, operators, `switch` expressions and pattern matching, checked and unchecked exceptions, `try` with resources, enumerations, passing parameters |
| Classes, records, interfaces | classes, inheritance, polymorphism, sealed classes, `equals` / `hashCode` / `compareTo`, interfaces, abstract classes, generics, packages and modules, records, pattern matching on objects, `Optional` |
| Commonly used Java classes | strings, arrays, collections (including sequenced collections), **Stream API** and `Gatherers`, text and binary files (`java.nio.file`), JSON with Jackson 3, regular expressions |
| Layered architectures | [DAO] / [business] / [UI] layers, multi-module Maven projects, **JUnit 6** unit tests, **dependency injection** with Spring |
| Functional interfaces, lambdas, and events | `java.util.function`, lambdas, method references, closures, composition, event listeners, `PropertyChangeSupport` |
| Execution threads | `Thread`, **virtual threads**, `synchronized`, `ReentrantLock`, `Condition`, atomic operations, `Semaphore`, `CountDownLatch`, concurrent collections, `ExecutorService`, fork/join, `ThreadLocal`, `ScopedValue` |
| Asynchronous programming | `CompletableFuture` and virtual threads, composition, exceptions, cancellation and timeouts, progress, asynchronous I/O, `Flow`, structured concurrency (overview) |
| Database Access with JDBC | MySQL, MySQL Connector/J, `DataSource` and HikariCP, parameterized queries and SQL injection, transactions, batches, `CachedRowSet` |
| **Hibernate** | entities, `SessionFactory` / `Session`, CRUD, persistence context, HQL and Criteria API, relationships and lazy loading, migrations, optimistic concurrency, native SQL, `StatelessSession`, Spring ORM, and `@Transactional` |
| Web Programming | TCP/IP, IPv6, `InetAddress`, TCP clients and servers (one virtual thread per client), HTTP, `HttpClient`, SMTP |
| Web Services | REST / JSON with **Spring Boot 4**, Java console clients, JavaScript web client, Node.js client |

## The Common Thread: An Income Tax Calculator in 9 Versions

Throughout the course, version by version, we build an **income tax calculator** application:

- **Version 1**: a single program; **Version 2**: classes and interfaces; **Version 3**: data read from a text or JSON file;
- **versions 4 and 5**: a layered architecture using Maven modules, tested with JUnit and integrated via dependency injection with Spring;
- **versions 6 and 7**: data stored in a MySQL database, read using JDBC and then Hibernate;
- **version 8**: a TCP server for tax calculation and its client;
- **Version 9**: a Spring Boot REST web service, its console client, and its web client.

## Technologies

Java 25 · JDK 25 · Maven 3.9 · IntelliJ IDEA · VS Code · JUnit 6 · Spring Framework 7 · Jackson 3 · MySQL 8 · MySQL Connector/J 9 · HikariCP · Hibernate ORM 7.4 · Jakarta Persistence 3.2 · Spring Boot 4.1 · Laragon

## Prerequisites

- Previous programming experience in any language.
- A [JDK 25](https://adoptium.net) (Eclipse Temurin or another distribution), [Maven](https://maven.apache.org), and an IDE ([IntelliJ IDEA](https://www.jetbrains.com/idea/) or [VS Code](https://code.visualstudio.com) with the Extension Pack for Java); [Laragon](https://laragon.org) for MySQL (chapters on databases). Installation instructions are provided in the course.

## Author

This course and its code were written by **Claude**, the AI from [Anthropic](https://www.anthropic.com) (October 2026), at the request of Serge Tahé, based on his C# 14 course.

Reviewer: [Serge Tahé](https://stahe.github.io)
