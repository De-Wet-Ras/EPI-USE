# Employee Sorter Project

## Overview
The Employee Sorter Project is a Java application designed to process employee and relationship data, construct a hierarchy, and submit the processed data to a server. This README explains how to set up, run, and use the application, as well as its file structure for users accessing it from GitHub.

---

## Prerequisites

### 1. **Java Development Kit (JDK)**
To run this project, you need a Java Development Kit (JDK). Examples of supported versions:
- **JDK 17 (LTS)**
- **JDK 11 (LTS)**

[Download JDK](https://www.oracle.com/java/technologies/javase-downloads.html)

Ensure the `java` and `javac` commands are available in your terminal or command prompt after installation.

### 2. **NetBeans IDE** (Recommended)
This project is designed to work seamlessly with NetBeans IDE.
- [Download NetBeans](https://netbeans.apache.org/download/)

**Alternative IDEs:**
- IntelliJ IDEA
- Eclipse

Command-line builds are also supported.

### 3. **SQLite Database Driver**
The SQLite JDBC driver is already included in the project’s `lib` folder, so no additional setup is needed.

---

## Instructions to Run the Project

### 1. **Clone the Repository**
1. Open a terminal or command prompt.
2. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your-username/employee-sorter.git
   ```
3. Navigate into the project directory:
   ```bash
   cd employee-sorter
   ```

### 2. **Open the Project in NetBeans**
1. Launch NetBeans IDE.
2. Go to `File -> Open Project`.
3. Navigate to the folder where you cloned the repository.
4. Select the project folder and click `Open`.

### 3. **Configure the Application**
The project requires a `config.properties` file to be properly configured with API endpoints and a candidate token. Verify the following fields in the file:
```properties
employee_url=<API URL for employee data>
relationship_url=<API URL for relationship data>
submit_url=<API URL for submitting data>
candidate_token=<Your Candidate Token>
batch_size=100
```

### 4. **Run the Main Class**
1. In NetBeans, locate the `EmployeeSorterDeWetRasFinal` class.
2. Right-click on the file and select `Run File` to start the application.

The program will process employee and relationship data and submit it to the specified server. Console logs will display the progress and outcomes of each step.

---

## Project Structure
- **`src/`**: Contains all Java source code files.
- **`lib/`**: Includes external dependencies, such as the SQLite JDBC driver.
- **`config.properties`**: A configuration file for specifying API endpoints and authentication details.
- **`employee_relationships.db`**: The SQLite database file (created automatically during runtime).
- **`README.md`**: Documentation for understanding and using the project.

---

## Notes for GitHub Users
1. Ensure your local Java environment meets the requirements specified in the prerequisites section.
2. Update the `config.properties` file with the correct API endpoints and token before running the project.
3. Report issues or request enhancements via the [GitHub Issues](https://github.com/your-username/employee-sorter/issues) page.

---

## Contribution Guidelines
We welcome contributions to this project! To contribute:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Description of changes"
   ```
4. Push your branch to your fork:
   ```bash
   git push origin feature-name
   ```
5. Submit a pull request to the main repository.

---

