# Taxi Service
This project implements a taxi service, with which you can register
and subsequently authenticate as a driver,
after which various functions will be available, such as:  </br>
* Display: 
  * All Drivers
  * All Cars
  * All Manufacturers
  * My Current Cars
* Create:
  * new Driver
  * new Car
  * new Manufacturer
* Add Driver to Car

## Implementation details
Project based on 3-layer architecture:

* Presentation layer (controllers)
* Application layer (services)
* Data access layer (DAO)

## Technologies
* Java 11
* Apache Tomcat (v9.0.55)
* MySQL
* JDBC
* Servlet
* JSP
* JSTL
* HTML, CSS
* Maven

## Recommendation for setup
1. Configure Apache Tomcat
2. Install MySQL and MySQL Workbench
3. Create a schema and all the necessary tables by using the script from resources/init_db.sql in MySQL Workbench
4. In the */util/ConnectionUtil.java*  class change the *"URL"*, *"user"*
   and *"password"* properties to the ones you specified when installing MySQL
5. In *src / main / resources / log4j2.xml* on the line </br> **<File name
   ="LogToFile" fileName="*path*">** you need to change **"*path*"** to your absolute path to the **.log** file
