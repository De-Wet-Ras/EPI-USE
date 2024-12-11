# Employee Sorter

A Java application for sorting and managing employee data using APIs and a SQLite database.

---

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Setup Instructions](#setup-instructions)
- [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
- [Features](#features)
- [Notes](#notes)

---

## Overview

This project fetches employee and relationship data from APIs, processes the data to create a hierarchy, and submits the data back to an API. It uses SQLite for intermediate data storage and requires Java to run.

---

## Prerequisites

To run this project, ensure you have the following installed:

- **Java Development Kit (JDK)**: Version 8 or later.
  - Examples: [OpenJDK](https://openjdk.org/) or [Oracle JDK](https://www.oracle.com/java/technologies/javase-downloads.html).
- **SQLite**: Included as part of the JDBC driver used in the project.

---

## Setup Instructions

### Clone the Repository

Clone this repository using the following command:

```bash
git clone https://github.com/De-Wet-Ras/EPI-USE.git
```

### Load the Project

1. Extract the ZIP or ensure the cloned repository is in a folder.
2. Open your preferred IDE (e.g., IntelliJ IDEA, NetBeans, Eclipse).
3. Import the project as a **Maven** or **Gradle** project, or configure dependencies manually.
4. Verify that the `config.properties` file is in the root directory with valid API URLs and credentials.

### Configure the Project

Ensure the `config.properties` file has the following structure and contains valid data:

```properties
employee_url=<API_URL_FOR_EMPLOYEES>
relationship_url=<API_URL_FOR_RELATIONSHIPS>
submit_url=<API_URL_FOR_SUBMISSION>
candidate_token=<YOUR_CANDIDATE_TOKEN>
batch_size=500
```

---

## Running the Application

1. Build the project in your IDE or using a terminal:
   
   ```bash
   javac -d bin src/com/employeesorterdewetrasfinal/*.java
   ```

2. Run the project:
   
   ```bash
   java -cp bin com.employeesorterdewetrasfinal.EmployeeSorterDeWetRasFinal
   ```

3. Monitor the logs in the terminal for progress and errors.

---

## Project Structure

```
EPI-USE/
├── src/
│   └── com/employeesorterdewetrasfinal/
│       ├── EmployeeSorterDeWetRasFinal.java
├── config.properties
├── README.md
└── employee_relationships.db
```

### Key Files

- **`EmployeeSorterDeWetRasFinal.java`**: Main application logic.
- **`config.properties`**: Configuration file for API credentials and URLs.
- **`employee_relationships.db`**: SQLite database file generated during execution.

---

## Features

- Fetch employee and relationship data from APIs.
- Store data in a local SQLite database.
- Generate a hierarchy of employees and submit to the API.
- Error handling for missing data and submission failures.

---

## Notes

- This project assumes valid API credentials and URLs.
- The SQLite database is recreated each time the application runs.
- If any issues occur, check the console logs for detailed error messages.

---
