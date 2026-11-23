::: {align="center"}
# ∑ CalcSpace

### All-in-One Calculator Website

**Every calculation, one space.**

A modern, colorful and responsive calculator platform built with **Java
25** and **Spring Boot**.

`<br>`{=html}

![Java](https://img.shields.io/badge/Java-25-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring
Boot](https://img.shields.io/badge/Spring_Boot-3.5.7-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-Build-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![Status](https://img.shields.io/badge/Project-Academic-7C3AED?style=for-the-badge)
:::

------------------------------------------------------------------------

## 👨‍🎓 Project Information

  Field                    Details
  ------------------------ ---------------------------------------------
  **Project**              CalcSpace -- All-in-One Calculator Website
  **Developer**            Md. Mashrafi Rahman
  **Student ID**           IT24034
  **Course**               Software Engineering and Project Management
  **Project Background**   First project developed using Spring Boot
  **Backend**              Java 25, Spring Boot 3.5.7, Spring Web
  **Frontend**             HTML5, CSS3, JavaScript
  **Build Tool**           Maven
  **Web Server**           Spring Boot Embedded Tomcat

## ✨ About CalcSpace

CalcSpace brings **30 calculators** together in one easy-to-use website.
Instead of visiting multiple websites for everyday calculations, users
can find calculators by category, search for a specific tool, enter
values and view the result through an interactive interface.

This is my **first Spring Boot project**, developed for the **Software
Engineering and Project Management** course. The project gave me
practical experience in building and running a Java-based web
application.

## 🧮 Calculator Collection

  -----------------------------------------------------------------------
  Category                            Included calculators
  ----------------------------------- -----------------------------------
  **Math & Everyday**                 Basic, Percentage, Discount, Tip,
                                      Bill Splitter, Average

  **Health & Fitness**                BMI, BMR, Calorie, Healthy Weight,
                                      Water Intake

  **Finance**                         Loan EMI, Simple Interest, Compound
                                      Interest, Salary, Tax

  **Date & Time**                     Age, Date Difference, Event
                                      Countdown

  **Student**                         GPA, CGPA

  **Unit Converter**                  Temperature, Length, Weight, Speed,
                                      Data Storage

  **Fun & Lifestyle**                 Love, Friendship, Mood, Stress
  -----------------------------------------------------------------------

## 🚀 Features

-   🎨 Modern, colorful interface
-   📱 Responsive layout for mobile, tablet and desktop
-   🔎 Search calculators by name
-   🗂️ Browse calculators by category
-   🧾 Interactive input forms
-   ⚡ Instant result display
-   ☕ Spring Boot application backend
-   🩺 REST API health endpoint

## 🧰 Technology Stack

  Technology          Role
  ------------------- -----------------------------------------------
  Java 25             Main programming language
  Spring Boot 3.5.7   Backend application framework
  Spring Web          Web and REST endpoint support
  Maven               Build and dependency management
  HTML5               Web page structure
  CSS3                Styling and responsive layout
  JavaScript          Calculator interactions and calculation logic
  Embedded Tomcat     Runs the Spring Boot web application

## 🔄 Application Flow

The following diagram illustrates the typical user journey through
CalcSpace.

``` mermaid
flowchart TD
    A([Open CalcSpace]) --> B[Load Home Page]
    B --> C{Choose how to find a calculator}
    C -->|Browse| D[Select a Category]
    C -->|Search| E[Search by Calculator Name]
    D --> F[Select a Calculator]
    E --> F
    F --> G[Open Calculator Form]
    G --> H[Enter Required Values]
    H --> I{Are the inputs valid?}
    I -->|No| J[Show Validation Message]
    J --> H
    I -->|Yes| K[Perform Calculation]
    K --> L[Display Result]
    L --> M{Calculate Again?}
    M -->|Yes| H
    M -->|No| B
```

## 🏗️ High-Level Application View

``` mermaid
flowchart LR
    U[User] --> UI[Browser Interface]
    UI --> SEARCH[Search and Category Selection]
    SEARCH --> FORM[Calculator Input Form]
    FORM --> JS[JavaScript Calculation Logic]
    JS --> RESULT[Result Display]

    UI <--> SB[Spring Boot Application]
    SB --> TOMCAT[Embedded Tomcat]
    SB --> HEALTH[REST Health Endpoint]
```

*This is a conceptual view of the application based on its described
technology and features.*

## 📅 Project Gantt Chart

The chart below is an **illustrative development plan** for this
academic project, not a record of verified completion dates. Adjust the
dates to match your actual project timeline if required for course
submission.

``` mermaid
gantt
    title CalcSpace — Illustrative Development Plan
    dateFormat YYYY-MM-DD
    axisFormat %d %b

    section Planning
    Define scope and calculator categories :a1, 2026-11-24, 2d
    Identify requirements and features    :a2, after a1, 2d

    section Design
    Plan UI and responsive layout          :b1, after a2, 3d
    Design application flow                :b2, after a2, 2d

    section Development
    Set up Spring Boot and Maven           :c1, after b1, 2d
    Build calculator interface             :c2, after c1, 4d
    Implement calculator interactions      :c3, after c2, 5d
    Add categories, search and filtering   :c4, after c2, 3d

    section Testing
    Test calculator inputs and results    :d1, after c3, 3d
    Check responsive behaviour            :d2, after c4, 2d
    Fix issues and refine UI               :d3, after d1, 2d

    section Delivery
    Prepare README and project files       :e1, after d3, 2d
    Final review and demonstration         :e2, after e1, 1d
```

## 🖥️ Getting Started

### Prerequisites

Make sure you have the following installed:

-   **JDK 25**
-   **IntelliJ IDEA**
-   Internet connection for the first Maven dependency download

> **Note:** A separate Tomcat installation is not required. Spring Boot
> runs with its embedded Tomcat server.

### Run in IntelliJ IDEA

1.  Download and extract the project ZIP.

2.  Open **IntelliJ IDEA**.

3.  Select **File → Open**.

4.  Choose the extracted `AllInOneCalculator` project folder.

5.  Wait for IntelliJ IDEA to import the Maven project and download
    dependencies.

6.  Find `AllInOneCalculatorApplication.java`.

7.  Click the green **Run** icon beside the main application class.

8.  Open your browser and visit:

    **http://localhost:8080**

### Run from Mac / Linux Terminal

Open Terminal in the project root folder and run:

``` bash
./mvnw spring-boot:run
```

If the project does not contain the Maven Wrapper, use:

``` bash
mvn spring-boot:run
```

### Run from Windows Terminal

``` bat
mvnw.cmd spring-boot:run
```

Then open **http://localhost:8080** in your browser.

## 📁 Typical Project Structure

The exact package and folder names may differ in the supplied project
ZIP.

``` text
AllInOneCalculator/
├── src/
│   └── main/
│       ├── java/
│       │   └── .../
│       │       └── AllInOneCalculatorApplication.java
│       └── resources/
│           ├── static/
│           ├── templates/
│           └── application.properties
├── pom.xml
└── README.md
```

## 🎯 Learning Outcomes

By developing CalcSpace, I gained practical experience with:

-   Creating and running a Spring Boot application
-   Understanding a Maven-based Java project
-   Working with frontend and backend components
-   Building a responsive web interface
-   Implementing interactive calculator features
-   Organizing a project from planning through development and testing

## 🔮 Future Improvements

Potential improvements for future versions:

-   User registration and login
-   Calculation history
-   MySQL database integration
-   User-specific saved calculations
-   Admin dashboard
-   Additional calculators and customization options

## 👨‍💻 Author

**Md. Mashrafi Rahman**\
**Student ID:** IT24034\
**Course:** Software Engineering and Project Management

------------------------------------------------------------------------

::: {align="center"}
**CalcSpace --- Every calculation, one space.**

*An academic project and my first step into Spring Boot development.*
:::
