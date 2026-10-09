# Spring Core Demo

A simple Java Maven project demonstrating **Spring Core concepts using XML-based configuration and Setter Dependency Injection**.

## Project Overview

This project demonstrates how the Spring IoC container creates and manages a Java object (Spring Bean) and injects property values through setter methods.

## Technologies Used

- Java
- Spring Framework 6.2.8
- Spring Context
- Apache Maven
- XML Configuration
- Visual Studio Code

## Concepts Covered

- Inversion of Control (IoC)
- Spring Beans
- XML-based Configuration
- Dependency Injection
- Setter Injection
- ApplicationContext
- Bean retrieval using `getBean()`

## Project Structure

```text
SpringCoreDemo/
├── pom.xml
├── .gitignore
└── src/
    └── main/
        ├── java/
        │   └── com/
        │       └── demo/
        │           ├── App.java
        │           └── Student.java
        └── resources/
            └── applicationContext.xml
```

## How It Works

1. Maven downloads the required Spring dependencies specified in `pom.xml`.
2. `Student.java` defines the student properties and setter methods.
3. `applicationContext.xml` defines the Spring bean and its property values.
4. `App.java` loads the XML configuration using `ClassPathXmlApplicationContext`.
5. The application retrieves the bean using `getBean()` and displays the student details.

## How to Run

### Prerequisites

- Java Development Kit (JDK)
- Apache Maven

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/Janardhan493/SpringCoreDemo.git
   ```

2. Navigate to the project directory:

   ```bash
   cd SpringCoreDemo
   ```

3. Compile the project:

   ```bash
   mvn clean compile
   ```

4. Run the application:

   ```bash
   mvn org.codehaus.mojo:exec-maven-plugin:3.5.0:java "-Dexec.mainClass=com.demo.App"
   ```

## Expected Output

```text
Student ID: 101
Student Name: Janardhan
Course: Java Full Stack
```

## Learning Outcome

This project provides practical experience with Spring Core, XML-based bean configuration, Setter Dependency Injection, and the Spring IoC container.
