# System Design & Low-Level Design (LLD) Learning Project

A comprehensive Java-based learning project covering Object-Oriented Programming (OOP) principles, SOLID design principles, and essential design patterns. This project is structured as a day-by-day curriculum designed to help developers master low-level design concepts and write maintainable, scalable, and extensible code.

## 📋 Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Technology Stack](#technology-stack)
- [Getting Started](#getting-started)
- [Learning Curriculum](#learning-curriculum)
- [Project Organization](#project-organization)
- [Running the Code](#running-the-code)
- [Running Tests](#running-tests)
- [Key Concepts Covered](#key-concepts-covered)
- [Contributing](#contributing)

## 🎯 Overview

This project serves as a comprehensive learning resource for mastering Low-Level Design (LLD) and Object-Oriented Programming concepts. It follows a structured, progressive curriculum that starts with fundamental OOP concepts and gradually moves toward advanced design patterns.

**What is Low-Level Design (LLD)?**

Low-Level Design is a component-level design process that focuses on:
- Detailed implementation of system components
- Organization of code
- Class diagrams with methods and relationships
- Writing maintainable, scalable, and extensible software

**Goals of this Project:**

- Understand the fundamentals of Object-Oriented Programming
- Master SOLID design principles
- Learn essential design patterns
- Write clean, maintainable, and extensible code
- Build a strong foundation for system design interviews and real-world development

## 📁 Project Structure

```
SystemDesign/
├── src/
│   ├── main/
│   │   └── java/
│   │       └── chamankumar/
│   │           └── lld/
│   │               └── oop/
│   │                   ├── common/              # Shared utilities
│   │                   ├── day01/               # Introduction to OOP
│   │                   ├── day02/               # Access Modifiers
│   │                   ├── day03/               # Polymorphism
│   │                   ├── day04/               # Abstraction
│   │                   ├── day05/               # SOLID: SRP & OCP
│   │                   ├── day06/               # SOLID: LID
│   │                   ├── day07/               # Design Pattern: Singleton
│   │                   ├── day08/               # Design Pattern: Builder
│   │                   ├── day09/               # Design Pattern: Prototype/Registry
│   │                   └── day10/               # Design Pattern: Factory
│   └── test/
│       └── java/
│           └── com/
│               └── chamankumar/
│                   └── lld/
│                       └── oop/                 # Test files for each day
├── pom.xml                                      # Maven configuration
└── README.md                                    # This file
```

Each day's folder typically contains:
- `code/` - Implementation examples and exercises
- `notes/` - Lecture notes and documentation (PDFs and Markdown)
- `assignments/` - Practice problems (where applicable)

## 🔧 Prerequisites

Before you begin, ensure you have the following installed:

- **Java Development Kit (JDK) 23** or higher
- **Apache Maven 3.6+**
- **IDE** (IntelliJ IDEA, Eclipse, or VS Code with Java extensions)
- Basic understanding of Java programming

## 💻 Technology Stack

- **Language**: Java 23
- **Build Tool**: Apache Maven
- **Testing Framework**: JUnit 5 (Jupiter)
- **Libraries**:
  - [Lombok](https://projectlombok.org/) - Reduces boilerplate code
  - JUnit 4 & 5 - For unit testing

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <repository-url>
cd SystemDesign
```

### 2. Build the Project

```bash
mvn clean compile
```

### 3. Run Tests

```bash
mvn test
```

### 4. Explore the Code

Navigate through the `src/main/java/chamankumar/lld/oop/` directory to explore different topics.

## 📚 Learning Curriculum

### Day 1: Introduction to Object-Oriented Programming
**Location**: `day01/intro/`

**Topics Covered**:
- Introduction to LLD (Low-Level Design)
- Procedural vs Object-Oriented Programming
- Classes and Objects
- Encapsulation basics
- State and Behavior

**Key Example**: `BankAccount` class demonstrating basic OOP concepts with debit, credit, and transfer operations.

**Learning Outcomes**:
- Understand the difference between procedural and OOP paradigms
- Learn how to model real-world entities as classes
- Grasp the concept of encapsulation and object interactions

---

### Day 2: Access Modifiers
**Location**: `day02/accessmodifiers/`

**Topics Covered**:
- `public`, `private`, `protected`, and package-private access modifiers
- Visibility and encapsulation
- Best practices for access control

**Key Example**: `Student` class with different access levels for fields and methods.

**Learning Outcomes**:
- Understand when to use each access modifier
- Learn how to properly encapsulate class members
- Apply access modifiers to control class visibility

---

### Day 3: Polymorphism
**Location**: `day03/polymorphism/`

**Topics Covered**:
- Method overriding
- Method overloading
- Runtime polymorphism
- Dynamic method dispatch
- Inheritance and polymorphism

**Key Example**: `User`, `Student`, and `Mentor` classes demonstrating polymorphic behavior.

**Learning Outcomes**:
- Understand compile-time vs runtime polymorphism
- Learn to design extensible class hierarchies
- Master method overriding and overloading

---

### Day 4: Abstraction
**Location**: `day04/abstraction/`

**Topics Covered**:
- Abstract classes and methods
- Interfaces
- Abstract vs Concrete classes
- When to use interfaces vs abstract classes

**Key Example**: `PasswordEncoder` interface with multiple implementations (`DefaultEncoder`, `ReverseEncoder`, `SubStringEncoder`).

**Learning Outcomes**:
- Understand abstraction and its benefits
- Learn to design interfaces for flexibility
- Apply abstraction to hide implementation details

---

### Day 5: SOLID Principles - SRP & OCP
**Location**: `day05/solid01SRPandCRP/`

**Topics Covered**:
- **Single Responsibility Principle (SRP)**: A class should have only one reason to change
- **Open/Closed Principle (OCP)**: Open for extension, closed for modification

**Key Example**: `Bird` class evolution showing how to apply SRP and OCP principles.

**Learning Outcomes**:
- Identify violations of SRP and OCP
- Refactor code to follow SOLID principles
- Design classes that are easy to extend without modification

---

### Day 6: SOLID Principles - LID (Liskov Substitution Principle)
**Location**: `day06/solid02/LID/`

**Topics Covered**:
- **Liskov Substitution Principle (LSP)**: Objects of a superclass should be replaceable with objects of its subclasses
- Strategy Pattern
- Interface Segregation
- Composition over Inheritance

**Key Example**: `Bird` hierarchy with `FlyableBird`, `NonFlyableBird`, and different flying behaviors using strategy pattern.

**Learning Outcomes**:
- Understand LSP and its importance
- Learn to design hierarchies that don't violate LSP
- Apply strategy pattern to achieve flexible behavior

---

### Day 7: Design Pattern - Singleton
**Location**: `day07/DPSingleton/`

**Topics Covered**:
- Singleton pattern implementation
- Thread safety considerations
- Double-checked locking
- Alternative implementations (Enum, Inner Static Class)

**Key Example**: `CollectionPool` class demonstrating thread-safe singleton implementation.

**Learning Outcomes**:
- Understand when to use Singleton pattern
- Implement thread-safe singleton
- Recognize trade-offs and alternatives

---

### Day 8: Design Pattern - Builder
**Location**: `day08/Builder/`

**Topics Covered**:
- Builder pattern for complex object construction
- Fluent interface design
- Immutability and validation
- Lombok `@Builder` annotation

**Key Example**: `Student` class with custom builder implementation and `Database` builder for configuration.

**Learning Outcomes**:
- Create objects with many optional parameters elegantly
- Implement fluent interfaces
- Apply builder pattern for complex object construction

---

### Day 9: Design Pattern - Prototype & Registry
**Location**: `day09/PrototypeRegistry/`

**Topics Covered**:
- Prototype pattern for object cloning
- Registry pattern for managing prototypes
- Shallow vs Deep copying
- Generic registry implementations

**Key Example**: `BackgroundRegistry` managing different types of graphical objects with cloning capabilities.

**Learning Outcomes**:
- Understand when to use prototype pattern
- Implement object cloning efficiently
- Design registry systems for prototype management

---

### Day 10: Design Pattern - Factory
**Location**: `day10/Factory/`

**Topics Covered**:
- Simple Factory pattern
- Factory Method pattern
- Abstract Factory pattern
- Decoupling object creation from usage

**Learning Outcomes**:
- Understand different factory pattern variants
- Learn when to use each factory pattern type
- Decouple object creation from client code

---

## 📖 Project Organization

### Code Structure

Each day's code follows a consistent structure:

```
dayXX/
├── code/
│   ├── Main.java              # Entry point demonstrating usage
│   └── [Other classes].java   # Implementation examples
├── notes/
│   ├── DayXXFullFledgeNotes.md    # Detailed notes
│   ├── DayXXClassNotes.pdf        # PDF lecture notes
│   └── optionalToRead.md          # Additional resources
└── assignments/                    # Practice problems (where applicable)
```

### Common Utilities

The `common/` package contains shared utilities:
- `Console.java` - Utility for console output

## ▶️ Running the Code

### Running Individual Examples

Each day has a `Main.java` file that demonstrates the concepts. You can run them using:

```bash
# Compile the project
mvn compile

# Run a specific main class
java -cp target/classes chamankumar.lld.oop.day01.intro.code.Main
```

### Using Your IDE

1. Import the project as a Maven project in your IDE
2. Navigate to the desired day's `Main.java` file
3. Run the main method directly from your IDE

## 🧪 Running Tests

The project includes unit tests for various concepts. Run all tests:

```bash
mvn test
```

Run tests for a specific day:

```bash
mvn test -Dtest=com.chamankumar.lld.oop.day01.intro.BankAccountTest
```

View test reports in `target/surefire-reports/`.

## 🎓 Key Concepts Covered

### Object-Oriented Programming
- ✅ Classes and Objects
- ✅ Encapsulation
- ✅ Inheritance
- ✅ Polymorphism
- ✅ Abstraction

### SOLID Principles
- ✅ **S**ingle Responsibility Principle (SRP)
- ✅ **O**pen/Closed Principle (OCP)
- ✅ **L**iskov Substitution Principle (LSP)
- ✅ Interface Segregation (covered in Day 6)
- ✅ Dependency Inversion (covered through design patterns)

### Design Patterns (Creational)
- ✅ Singleton
- ✅ Builder
- ✅ Prototype
- ✅ Factory (Simple, Method, Abstract)

### Best Practices
- ✅ Code organization and structure
- ✅ Access control and encapsulation
- ✅ Design for maintainability and extensibility
- ✅ Thread safety considerations
- ✅ Fluent interfaces and method chaining

## 📝 Notes and Documentation

Each day includes comprehensive notes:
- **Full Fledge Notes** (`.md`): Detailed explanations with examples
- **Class Notes** (`.pdf`): Lecture slides and diagrams
- **Optional Reading** (`.md`): Additional resources and references

## 🎯 Learning Path Recommendation

1. **Start with Day 1** - Build a solid foundation in OOP basics
2. **Progress sequentially** - Each day builds upon previous concepts
3. **Read the notes** - Review both code and documentation
4. **Complete assignments** - Practice problems reinforce learning
5. **Run and modify code** - Experiment with examples
6. **Write tests** - Test your understanding with unit tests

## 🔍 Code Examples

### Example 1: Bank Account (Day 1)
```java
BankAccount acc1 = new BankAccount(1, "Alice", 1000);
BankAccount acc2 = new BankAccount(2, "Bob", 500);
acc1.transfer(200, acc2);
```

### Example 2: Builder Pattern (Day 8)
```java
Student student = Student.builder()
    .setFname("John")
    .setLname("Doe")
    .setEmail("john@example.com")
    .setAge(25)
    .build();
```

### Example 3: Singleton Pattern (Day 7)
```java
CollectionPool pool = CollectionPool.getInstance();
```

## 🤝 Contributing

This is a learning project. If you'd like to contribute:

1. Follow the existing code structure and naming conventions
2. Add comprehensive comments and documentation
3. Include tests for new examples
4. Update this README if adding new topics

## 📄 License

This project is for educational purposes.

## 🙏 Acknowledgments

This project is part of a comprehensive LLD/OOP learning curriculum. Each day's content is designed to progressively build understanding of object-oriented design principles and patterns.

---

**Happy Learning! 🚀**

*Remember: Good software design is not about knowing all the patterns, but about understanding when and why to use them.*

