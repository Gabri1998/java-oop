# DIT043 - Enterprise System Management

A comprehensive Java enterprise management system demonstrating object-oriented programming principles, design patterns, and software architecture.

## Project Overview

This project implements a complete employee and product management system with multiple modules including staff management, inventory control, review systems, and transaction processing.

## Architecture & Design Patterns

### Core Architecture
- **Facade Pattern**: Central `Facade.java` class providing unified interface to complex subsystems
- **Layered Architecture**: Separation of concerns with clear package structure
- **Menu-Driven Interface**: Interactive console-based user interface

### Object-Oriented Principles
- **Inheritance Hierarchy**: Abstract `Employee` class extended by `Intern`, `RegularEmployee`, `Manager`, and `Director`
- **Polymorphism**: Method overriding in employee subclasses and Object class methods
- **Encapsulation**: Private fields with public accessors/mutators
- **Method Overloading**: Multiple methods with same name but different signatures

## Package Structure

### Main Packages
- **`staff/`**: Employee hierarchy and management
- **`products/`**: Item, Review, and Transaction entities
- **`menus/`**: User interface components
- **`enums/`**: Type-safe enumerations
- **`exceptions/`**: Custom exception handling
- **`facade/`**: System entry point and coordination

### Key Components

#### Staff Management
- **Employee Types**: Intern, Regular Employee, Manager, Director
- **Validation**: Department, Degree, and GPA enumerations for data integrity
- **Exception Handling**: Comprehensive invalid employee scenarios

#### Product System
- **Item Management**: Product catalog and inventory
- **Review System**: Customer feedback and ratings
- **Transaction History**: Purchase tracking and reporting

## Enumeration System

- **`Department`**: Organizational units for Director classification
- **`Degree`**: Academic qualifications for Manager roles
- **`GPA`**: Grade point averages for Intern evaluation
- **`EmployeeExceptionCase`**: Standardized exception messages

## Exception Handling

Custom `InvalidEmployeeException` with enum-based error cases provides consistent error management across the application.

## Testing Strategy

Comprehensive test suite organized by epics:
- **Epic 2**: Regular and alternative test scenarios
- **Epic 3**: Core functionality validation
- **Epic 4**: Extended feature testing
- **Epic 5**: System integration tests
- **Epic 6**: Exception handling verification

## Build & Execution

### Prerequisites
- Java JDK 8+
- Maven 3.6+

### Running the Application
```bash
mvn compile
mvn exec:java -Dexec.mainClass="staff.Main"

**Development Practices**
Input/Output Abstraction: Centralized IO.java class for all user interactions

Menu Navigation: Hierarchical menu system for user workflow

Data Validation: Comprehensive input validation and error handling

Code Organization: Logical package structure with clear responsibilities

**Related Practice Projects**
The repository also contains supplementary practice projects:

Temperature Management: Interface implementation exercises

Array Utilities: Data structure practice

Social Media Simulation: User and post management

Membership Systems: Class relationship exercises

**Technical Stack**
Language: Java

Build Tool: Maven

Testing: JUnit

Architecture: Object-Oriented Design with Facade Pattern
