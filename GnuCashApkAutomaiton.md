# GnuCash Android App Automation
## _Test Strategy, Test Suite, Test Cases_

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

### Introduction
---
Test cases of GnuCash application are divided based on the features present in the app and various system interaction.

- **Install / Upgrade / Compatibility** : Validation of install & uninstall automatically which resulted into compatibility validation as well.

- **Feature Tests** : Validation of different features.

- **Performance** : Validation of time taken by the action to be performed.

- **End User use case** : Feature validation based on user input values in different currency.


### Test Strategy
---
Test Strategy is mainly focused on feature validation and app interaction with end user and system.
- CRUD is used for all basic featured
    * Create : Creation of records.
    * Read : Redability of records.
    * Update : Updation of records.
    * Delete : Deletion of records.

**Framework** : Unified transferrable framework has been prepared based on Page Object Model (POM)

### Famework Highlight
---
- **Extendibility** : Can be used to automate same test case with IOS as well.
- **Unified** : Cases for backend/RestAPI's can be merged with the framework.
- **Logging** : Logging is a separate entity so can be changed to any mechanism
- **Independent identity** : There is no dependency between test cases.
- **Integratable** : Since maven is a well know tool it can be easily integrated with CI/CD.
- **Parallel Run** : Cases can be run parallely just by small tweking.

### Scope to Add
---
- Retry Mechanism.
- IOS app path.
- Customized reporting tool.
- Integration with CI/CD

### Technology Stack
---
- **Language** : Java
- **Build Automation** : Maven
- **Mobile app automation lib** : Appium
- **Test Manager** : TestNG
- **Reporting Framerork** : Extent Reports
- **IDE** : Eclipse

### Prerequistes To Run Tests
---
- Java should be installed on the system and $JAVA_HOME / Maven(mvn) should be configured.
- Change the device name and platfrom version according the device attached to the system.


### Steps to run test
---
```bash
cd <To_The_Directory_Root>
mvn clean test -Dplatform="android"
``` 

### Reports
```bash
cd Reports
```
Check for the Html file.
