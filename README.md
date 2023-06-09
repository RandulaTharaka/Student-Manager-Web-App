# Student-Manager-Web-App
![repo-size](https://img.shields.io/github/repo-size/RandulaTharaka/Student-Manager-Web-App) 
![top-language](https://img.shields.io/github/languages/top/RandulaTharaka/Student-Manager-Web-App) 
![last-commit](https://img.shields.io/github/last-commit/RandulaTharaka/Student-Manager-Web-App) 

## Description
This is a JSP and Servlet web application project that connects to a MySQL database allowing users to perform CRUD operations on student records. The project has been developed using MVC architecture with DAO design pattern. Additionally, JSP Standard Tag Library (JSTL) and JSP Scriplets have been utilized for render the View. 

Following image depicts the MVC architecture with DAO design pattern used in the Student-Manager application. 

![Student-Manager MVC Architecture](https://github.com/RandulaTharaka/Student-Manager-Web-App/assets/60685092/2ab0e990-7d2b-4a50-889e-abbeb820c873)

A web browser submits a request to the servlet controller, which utilizes a helper class called 'StudentDbUtili'. This class communicates with the database, retrieves the data back to the controller, and then the controller forwards the data to a JSP page, serving as the view. Finally, the view is sent back to the browser.
In this application, the class named 'StudentDbUtili' acts as a Data Access Object (DAO), which is a commonly used pattern in programming to separate the data access logic from the rest of the application. By employing the DAO pattern, the code becomes more modular and maintainable.

### Built With
| <img align= "left" style="padding-right" width="30px" alt="html-icon" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" /> | <img align= "left" style="padding-right" width="30px" alt="css-icon" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" /> | <img align= "left" style="padding-right" width="30px" alt="java-icon" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" /> | <img align= "left" style="padding-right" width="30px" alt="mysql-icon" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" /> | <img align= "left" style="padding-right" width="30px" alt="tomcat-icon" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tomcat/tomcat-original.svg" /> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| HTML                                                                                                                                                       | CSS                                                                                                                                                     | Java                                                                                                                                                     | MySQL                                                                                                                                                       | Tomcat                                                                                                                                                         | 
</br>
          
## Prerequisites
Following applications must be installed in your system in oder to run this project.
- Java 11
- Apache Tomcat Server 8.5
- MySQL 8.0 and Workbench
- Eclipse IDE

## Installation 
1. Clone the repository<br>
   `git clone https://github.com/RandulaTharaka/Student-Manager-Web-App.git`
   
2. Create the MySQL user account<br>
   Open MySQL workbench and go to File -> Open SQL Script. Then open the '01-create-user.sql' file located in 'sql-scripts' folder in the repository and click execute button in the workbench.
   
3. Create the Database<br>
   Go to File -> Open SQL Script in MySQL workbench. Then open the '02-students.sql' file located in 'sql-scripts' folder in the repository and click execute button in the workbench.
   
4. Import the project in Eclipse<br>
   Go to File -> Open projects from File System. Then click 'Directory' button and select the 'student-manager' folder in the repository. Then click 'Finish' button.
   
5. Run the project<br>
   Right click on the project and select 'Run As' -> 'Run on Server'. Then select 'Tomcat v8.5 Server' and click 'Next' button. In the next wizard click 'Browse' and select Tomcat 8.5 installation directory in your file system and click 'Finish' button. </br>
   
- If you encounter any errors after installing the project, please review the following for possible solutions.
   - Make sure that your JDBC driver (mysql-connector-j-) version matches the version of your MySQL server.
   - Resolve any unbounded libraries in the project build path.
   - Verify that the context.xml file is properly configured and make any necessary adjustments.
   - Make sure that you have provided valid admin port number for Tomcat server.
