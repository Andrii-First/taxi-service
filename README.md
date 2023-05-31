# taxi-service

Project description:
- Simple web-application that supports Authentication, registration and other CRUD methods.

Features:
- registration like a Driver;
- Authentication as a Driver;
- create/update/remove(soft delete) of Driver;
- create/update/remove(soft delete) of Manufacturer;
- create/update/remove(soft delete) of Car;
- display list of all Drivers;
- display list of all Manufacturers;
- display list of all Cars;
- add/remove driver from car;
- display list of all Drivers of Car;
- display list of all Cars driven by authorised Driver;
- logout;

Project structure:
main:
-java.taxi:
    -controllers - contains all controllers.
    -dao - dao layer of project. All sql query's is here. 
    -exception - custom exception for project.
    -lib - contains injector.
    -model - models of Driver, Manufacturer, Car.
    -service - service layer of project. No sql query's. All business logic is here.
    -util - contains connection to DB.
    -web.filter - contains filter for authorised/not authorised Drivers.
-resources:
    -init_db.sql - used to initialize proper tables;
-webapp:
    -WEB-INF - contains all JSP pages.
    -web.xml file

In this project were used:
    - Injector
    - Servlets
    - Filter
    - SQL
    
!!!!To START!!!!
- use query from init_db.sql to initialise tables in your SQL DataBase
- configure ConnectionUtil from util directory to get connection to your DB.
- use Tomcat 9.0.75 to run project.