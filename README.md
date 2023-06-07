# Jmeter_Connection_Configuration_with_Database_for_Volume_testing

## Project Steps:
- Thread Group->Add->Config Element->JDBC Connection Configuration
                                    - Variable Name: myConnection
- Database URL: jdbc:mysql://localhost:3306
- JDBC Driver Class: com.mysql.jdbc.Driver
- Username: root
- Put the mysql-connector-java-5.1.48.jar in lib folder
- Thread Group->Add->Sampler->JDBC Request
                             - Variable Name: myConnection
- Query: SELECT * FROM table_name
- Create new users
- Select new users


## Technology Used
- JMeter
- Jdk-11
- XAMPP
- SQLyog

## Scenerio
Do volume testing by connecting jmeter with database

## How to run this project
- Clone this project
- Save the .jmx file in bin folder of Apche Jmeter
- Run the .jmx file on jmeter

**Fos 10 second Ramp-up period and 167 users, volume testing is unsuccessful.Screenshot is added below:**
![Screenshot (411)](https://github.com/suptimusfika/Jmeter_Connection_Configuration_with_Database_for_Volume_testing/assets/48064134/193231a6-a035-46d8-8fc7-1701b7068976)

**Fos 30 second Ramp-up period and 167 users, volume testing is unsuccessful.Screenshot is added below:**
![Screenshot (412)](https://github.com/suptimusfika/Jmeter_Connection_Configuration_with_Database_for_Volume_testing/assets/48064134/02b24810-7a25-4ddd-836d-80d24bc93742)

**Fos 60 second Ramp-up period and 167 users, volume testing is unsuccessful.Screenshot is added below:**
![Screenshot (410)](https://github.com/suptimusfika/Jmeter_Connection_Configuration_with_Database_for_Volume_testing/assets/48064134/37da46aa-d6fc-4db4-92a8-f99e9d73c9de)

**Fos 60 second Ramp-up period and 100 users, volume testing is successful.Screenshot is added below:**
![Screenshot (409)](https://github.com/suptimusfika/Jmeter_Connection_Configuration_with_Database_for_Volume_testing/assets/48064134/cb851253-1360-48a4-b6d8-19cd87f23b16)

## You can see when we have decrease the volume of data, then volume testing was successful
