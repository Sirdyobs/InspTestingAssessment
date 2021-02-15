# InspTestingAssessment
Assessment for Inspired Testing

This project covers UI tesisting and API testing and it is created from lessons learn't from a number of project I have worked on.

# Concepts Included

Page Object Model
Web page interaction methods
API interaction methods
External Test Configuration

# Tools Used

Maven
Java
Testng
Selenium Web Driver
Extent Report

# Requirements

Maven 3 or higher
Chrome driver
Java 1.8

# Project Folder Structure

  src/main/java
    Package Base
      Base Class - contains properties and methods that form the foundation of the project
    Package Config
      config file - contains configuration parameters of the project. This is were you specify browser and the url you testing on. can add other parameters
    Package Model
      Address Class - Address is the member of User class. Since address is defined by more than one parameter, I decide to create an object that will define the address
      Company Class - Also, Company is a member of user class. Since it is defined by more than one parameters, I decided to create an object to define the company.
      Geo Class - Also, Company is a member of Address class. Since it defined by more than one parameters, I created an object to define the parameters of geo locations.
      User Class - Main object, the above mentioned a members of this class wich needed to be mapped to their values.
      CreateJsonfromClasses - This class converts the User class into a json object using Object Mapper class found from jackson data-bing
    Package PageProp
      Home - Contains element locators for the homepage
      LoginPage - Contains element locators for login page
      TransactionProp - Contains element locators for Transactions page
      UserAPI - Contains URI to user resources
      Welcome - Contains element locators for welcome page
    Package Data
      banking.json file - defines a test data in json format for the UI testing of banking app.
      Banking activity.xlsx - define a test data in excel sheet for the UI testing of the banking app
    Packege Utility  
      APIUtility - defines all the operations/methods used to test the APIs
      GeneralUtility - defines methods that are not specific the core of the project but are building blocks to achieve certain tasks.
      SeleniumDriverUtility - defines all the methods used to interact with the web page, contains reporting mechanisms about webpage results.
  
  src/test/java
    Package Test
      TestI - defines test for API functionality
      TestII - defines tests for web app functionality
    Package TestCases
      APIUsers - defines logic to test the Users API
      Deposit - Defines logic to test the deposit functionality
      Login - defines logic to test the Login functionality
      Transaction - defines logic to test the Transaction functionality
      Withdraw - defines logic to test the withdraw functionality
 
# Usage

To execute the project:
  Clone or download the project from https://github.com/Sirdyobs/InspTestingAssessment.git
  Navigate to the project folder
  Assuming maven is installed, run mvn clean install
  
  
# Reporting

After first execution, a folder "Reports" will be created inside the project folder
A extent report named "InspTesting-Assessment.html" will be generated.
 
      
  
  


