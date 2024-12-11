Employee Sorter Project - README
Overview
This project is a Java application designed to process employee and relationship data, construct a hierarchy, and submit it to a server. It is packaged in a ZIP file for easy distribution and use.

Prerequisites
1. Java Development Kit (JDK)
To run this project, you need a Java Development Kit (JDK).

Recommended versions:

JDK 17 (LTS) or JDK 11 (LTS).
Download JDK

After installing, make sure java and javac commands are available in your terminal or command prompt.

2. NetBeans IDE (Recommended)
This project is designed to be opened and executed using NetBeans IDE.
Download NetBeans
Other IDEs: IntelliJ IDEA, Eclipse, or command-line builds are also compatible.

3. SQLite Database Driver
  The project includes a pre-configured SQLite JDBC driver, so no separate installation is required.

Instructions to Run the Project

1. Unzip the Project
  Extract the ZIP file to a directory of your choice.

2. Open the Project in NetBeans
  Launch NetBeans.
  Go to File -> Open Project.
  Navigate to the folder where the project was extracted.
  Select the project folder and click Open.

3. Check the Configuration
  Locate the config.properties file in the project directory. Ensure the following fields are correctly filled out:
  employee_url=<API URL for employee data>
  relationship_url=<API URL for relationship data>
  submit_url=<API URL for submitting data>
  candidate_token=<Your Candidate Token>
  batch_size=100
  Update the fields as necessary with your API details and token.

4. Run the Main Class
  In NetBeans, locate the EmployeeSorterDeWetRasFinal class.
  Right-click on the file and select Run File to start the application.
5. Submit Data
  The program will fetch employee and relationship data, process it, and submit it to the server.
  Logs will be displayed in the console to show progress and outcomes.

File Structure in the ZIP
  src/: Contains all source code files.
  lib/: Includes the SQLite JDBC driver and other dependencies.
  config.properties: Configuration file for API endpoints and token.
  README.md: This README document.
  employee_relationships.db: The SQLite database file (created automatically on the first run).
  
Notes for Users
  Ensure the config.properties file is properly configured before running the project.
  If errors occur, verify:
  API endpoints are valid and accessible.
  The candidate_token is correct.
  The correct JDK is installed.
  With the ZIP format, all dependencies and configuration are bundled, making it easy to set up and run the project in any compatible environment.
