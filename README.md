# Student-Manager-Web-App

## About
This is a JSP and Servlet web application project that connects to a MySQL database allowing users to perform CRUD operations on students. The project has been developed using MVC architecture with DAO design pattern.

A web browser submits a request to our servlet controller, which utilizes a helper class called 'StudentDbUtili'. This class communicates with the database, retrieves the data, and then the controller forwards the data to a JSP page, serving as the view. Finally, the view is sent back to the browser.
In this application, the class named 'StudentDbUtili' acts as a Data Access Object (DAO), which is a commonly used pattern in programming to separate the data access logic from the rest of the application. By employing the DAO pattern, the code becomes more modular and maintainable.

![Student-Manager MVC Architecture](https://github.com/RandulaTharaka/Student-Manager-Web-App/assets/60685092/2ab0e990-7d2b-4a50-889e-abbeb820c873)

## Built With

## Prerequisites
Following applications must be installed in your system in oder to run this project.
- Java 11
- Apache Tomcat Server 8.5
- MySQL 8.0 and Workbench

## Installation 
1. Clone the repository<br>
   git clone ____________________
2. Create the MySQL user account<br>
   Open MySQL workbench and go to File -> Open SQL Script. Then open the '01-create-user.sql' file located in 'sql-scripts' folder in the repository and click execute button in the workbench.
3. Create the Database<br>
   Go to File -> Open SQL Script in MySQL workbench. Then open the '02-students.sql' file located in 'sql-scripts' folder in the repository and click execute button in the workbench.
4. Import the project in Eclipse<br>
   Go to File -> Open projects from File System. Then click 'Directory' button and select the 'student-manager-web-app' folder in the repository. Then click 'Finish' button.
5. Run the project<br>
   Right click on the project and select 'Run As' -> 'Run on Server'. Then select 'Tomcat v8.5 Server' and click 'Next' button. In the next wizard click 'Browse' and select Tomcat 8.5 installation directory in your file system and click 'Finish' button.

If you encounter any errors after installing the project, please review the following for possible solutions.
   - Make sure that your JDBC driver (mysql-connector-j-) version matches the version of your MySQL server.
   - Resolve any unbounded libraries in the project build path.
   - Verify that the context.xml file is properly configured and make any necessary adjustments.
   - Make sure that you have provided valid admin port number for Tomcat server.
