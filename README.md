# Java Projects Collection

A collection of Java laboratory experiments covering OOP, JDBC, sockets,
RMI, Servlets, JSP, and Apache Tomcat, along with the ShopSphere project.

## 📁 Repository Structure

``` text
java_projects/
│
├── Exp_01_Student_Registration_Form/
│   └── Java-based Student Registration Form application
│
├── Exp_02_Calculator/
│   └── Java Swing calculator built with an MVC structure
│
├── Exp_03_Mysql_Connect(JDBC)/
│   ├── Java JDBC application for connecting to MySQL
│   └── mysql-connector-j-26.7.0/
│       └── MySQL Connector/J library and source distribution
│
├── Exp_04_Server_Client_Basics/
│   └── Java socket-based server-client programs
│
├── Exp_05_RMI/
│   └── Java RMI client-server example
│
├── Exp_06_Apache_Tomcat/
│   └── Apache Tomcat 11 server
│
├── Exp_06_Servlet_Login_App/
│   └── Servlet-based login application
│
├── Exp_07_JSP_Conversion/
│   └── JSP conversion of the servlet login application
│
└── ShopSphere/
    └── Java web e-commerce project
```

## 🚀 Experiments

### Exp_01 — Student Registration Form

A Java registration form application demonstrating:

-   GUI-based form handling
-   User input and event handling
-   Java classes and objects
-   Database/JDBC integration where applicable

------------------------------------------------------------------------

### Exp_02 — Calculator

A Java Swing calculator organized using the Model-View-Controller
pattern. It supports addition, subtraction, multiplication, division, and
percentage operations.

------------------------------------------------------------------------

### Exp_03 — MySQL Connect (JDBC)

Demonstrates database connectivity between Java and MySQL using
**JDBC (Java Database Connectivity)**.

**Technologies:**

-   Java
-   JDBC
-   MySQL
-   MySQL Connector/J

**Typical workflow:**

``` text
Java Application
      ↓
     JDBC
      ↓
MySQL Connector/J
      ↓
    MySQL
```

The project contains source code, compiled classes, and the required
JDBC connector library. The full Connector/J distribution is kept inside
the same experiment folder.

------------------------------------------------------------------------

### Exp_04 — Server Client Basics

Java server-client communication examples demonstrating:

-   Client-server architecture
-   Network communication
-   Sockets
-   Input/output streams
-   Sending and receiving data

Basic architecture:

``` text
Client  ←──── Network Connection ────→  Server
```

------------------------------------------------------------------------

### Exp_05 — RMI

Demonstrates **Java Remote Method Invocation (RMI)**, which allows a Java
program to invoke methods on an object running in another JVM.

**Main concepts:**

-   Remote Interface
-   Remote Object
-   RMI Server
-   RMI Client
-   Remote Method Invocation

**Basic architecture:**

``` text
Client
  │
  │ Remote Method Call
  ↓
RMI Registry
  │
  ↓
Remote Server Object
```

------------------------------------------------------------------------

### Exp_06 — Apache Tomcat

The `Exp_06_Apache_Tomcat` directory contains the Apache Tomcat 11
server, used to run Java web applications such as:

-   Servlets
-   JSP applications
-   Web applications packaged as WAR files

Important directories include:

  Directory   Purpose
  ----------- ------------------------------------------
  `bin`       Startup and shutdown scripts
  `conf`      Server configuration
  `lib`       Server libraries
  `logs`      Server log files
  `temp`      Temporary files
  `webapps`   Deployed web applications
  `work`      Generated/compiled web application files

Typical Servlet application flow:

``` text
Browser
   ↓
Tomcat Server
   ↓
Servlet
   ↓
Java Application Logic
   ↓
Response
   ↓
Browser
```

------------------------------------------------------------------------

### Exp_06 — Servlet Login App

A Maven-based servlet application demonstrating:

-   Servlets and filters
-   Session handling
-   Login and logout flows
-   Application listeners

Build and deploy it to Tomcat using Maven:

``` bash
cd Exp_06_Servlet_Login_App
mvn clean package
```

------------------------------------------------------------------------

### Exp_07 — JSP Conversion

A JSP version of the servlet login application. It demonstrates:

-   JSP pages and JSTL
-   Request handling and form submission
-   Session-based authentication
-   Reusable page fragments such as headers and footers

Build it with Maven:

``` bash
cd Exp_07_JSP_Conversion/servlet
mvn clean package
```

------------------------------------------------------------------------

### ShopSphere

ShopSphere is a Java web e-commerce project. It includes modules for
database access, networking, RMI, a Swing admin application, and a
Servlet/JSP storefront.

------------------------------------------------------------------------

## 🗄️ MySQL Connector/J

The `mysql-connector-j-26.7.0` directory (inside
`Exp_03_Mysql_Connect(JDBC)`) contains **MySQL Connector/J**, the JDBC
driver used by Java applications to communicate with MySQL databases.

It is used by projects such as:

``` text
Java Application
      ↓
JDBC API
      ↓
MySQL Connector/J
      ↓
MySQL Database
```

> Note: This directory is a dependency/library distribution rather than
> a standalone application project.

------------------------------------------------------------------------

## 🛠️ Technologies Used

-   **Java**
-   **JDBC**
-   **MySQL**
-   **MySQL Connector/J**
-   **Java RMI**
-   **Java Sockets**
-   **Servlets**
-   **JSP**
-   **Apache Tomcat**
-   **Maven**
-   **HTML/CSS/JavaScript** where applicable

------------------------------------------------------------------------

## 📚 Purpose of This Repository

This repository serves as a collection of Java development and college
practical projects. It is useful for:

-   Practicing Core Java
-   Learning OOP
-   Practicing JDBC and MySQL connectivity
-   Understanding client-server programming
-   Learning Java RMI
-   Working with Servlets, JSP, and Tomcat
-   Maintaining college laboratory projects
-   Preparing Java projects for future development and placement
    practice

------------------------------------------------------------------------

## ▶️ Getting Started

### Clone the repository

``` bash
git clone https://github.com/gourav-swami/java_projects.git
cd java_projects
```

### Java Projects

Open the required project in an IDE such as:

-   IntelliJ IDEA
-   Eclipse
-   NetBeans
-   VS Code

Make sure Java/JDK is installed and configured.

### JDBC Projects

For MySQL-based projects:

1.  Install MySQL.
2.  Start the MySQL server.
3.  Configure the database credentials in the Java project.
4.  Add MySQL Connector/J to the classpath if required.
5.  Compile and run the application.

### Tomcat Projects

1.  Open `Exp_06_Apache_Tomcat`.
2.  Place the web application in the `webapps` directory if required.
3.  Start Tomcat using the scripts in `bin`.
4.  Open the application through the Tomcat server URL.

------------------------------------------------------------------------

## 👨‍💻 Author

**Gourav Swami**

GitHub: <https://github.com/gourav-swami>

------------------------------------------------------------------------

## 📌 Note

Some folders contain compiled `.class` files, libraries, server files,
or generated files because this repository is also maintained as a
practical/learning workspace.

For production projects, it is generally better to use a build system
such as Maven or Gradle and avoid committing generated build artifacts.
