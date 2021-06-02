<!---
chloeboss/chloeboss is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

#### Author Contact Info
```
 👋 Hi, I’m Chloe Zeng
 📫 chloezeng310@gmail.com
    +64 021 183 2827
    https://www.linkedin.com/in/chloe-zeng/
```

And I have created few projects to show usage of different automation testing tools.

### Repo list


[![Build Status](https://dev.azure.com/chlozeng/MyFirstProject/_apis/build/status/chloeboss.cucumber-bdd-demo?branchName=master)](https://dev.azure.com/chlozeng/MyFirstProject/_build/latest?definitionId=11&branchName=master)
| Repo          | Build Status  |Release Status|
| ------------- | ------------- |------------- |
| [Cucumber web Demo](https://github.com/chloeboss/cucumber-bdd-demo)| [![Build Status](https://dev.azure.com/chlozeng/MyFirstProject/_apis/build/status/chloeboss.cucumber-bdd-demo?branchName=master)](https://dev.azure.com/chlozeng/MyFirstProject/_build/latest?definitionId=11&branchName=master) |<a href="https://dev.azure.com/chlozeng/MyFirstProject/_dashboards/dashboard/0b27603f-ca0a-4ddd-a108-85bae3788ac8"><img src="https://vsrm.dev.azure.com/chlozeng/_apis/public/Release/badge/d03ef986-5372-4396-a097-e68e1d803625/14/14"/>|
| [Cucumber api Demo](https://github.com/chloeboss/cucumber-api-demo)| [![Build Status](https://dev.azure.com/chlozeng/MyFirstProject/_apis/build/status/chloeboss.cucumber-api-demo?branchName=develop)](https://dev.azure.com/chlozeng/MyFirstProject/_build/latest?definitionId=13&branchName=develop) ||
| [Specflow web/api Demo](https://github.com/chloeboss/specflow-demo)| [![Build Status](https://dev.azure.com/chlozeng/MyFirstProject/_apis/build/status/chloeboss.specflow-demo?branchName=master)](https://dev.azure.com/chlozeng/MyFirstProject/_build/latest?definitionId=10&branchName=master)|<a href="https://dev.azure.com/chlozeng/MyFirstProject/_dashboards/dashboard/0b27603f-ca0a-4ddd-a108-85bae3788ac8"><img src="https://vsrm.dev.azure.com/chlozeng/_apis/public/Release/badge/d03ef986-5372-4396-a097-e68e1d803625/15/15"/>|
| [Cypress Demo](https://github.com/chloeboss/cypressTest)| [![Build Status](https://dev.azure.com/chlozeng/MyFirstProject/_apis/build/status/chloeboss.cypressTest?branchName=master)](https://dev.azure.com/chlozeng/MyFirstProject/_build/latest?definitionId=9&branchName=master)|<a href="https://dev.azure.com/chlozeng/MyFirstProject/_dashboards/dashboard/0b27603f-ca0a-4ddd-a108-85bae3788ac8"><img src="https://vsrm.dev.azure.com/chlozeng/_apis/public/Release/badge/d03ef986-5372-4396-a097-e68e1d803625/12/12"/>|
|[Appium Demo](https://github.com/chloeboss/appiumTests)|||


### Cucumber Web/ Api Demo
#### Web part is a _Java Maven_ project which using _Selenium, Junit, Cucumber under Page Object Design Pattern_.
* It can run with different browsers, also provides **_Headless_** option.
  (default by **_chrome_** you can find setting in **_config.properties_**)
* It allows parallel test execution by using _maven-surefire-plugin_
* In `RunCucumber` file, you can run scenarios with a particular tag. like @chrome, @headless, @api, @countdown
* Using `dynamic XPath` and `Wait till` to locate UI elements
* Using `PicoContainer` as Dependency Injection (DI) Containers to Sharing Test Context between Cucumber Step Definitions
* Using `ScenarioContext` & `Java Hash Map`to store and share test date between steps


#### Api
There are multiple options to test Api eg: Postman, Swagger. In this Demo, I am using Rest Assured which is one of the most used library for REST API automation testing.\
* Parallel test execution by using `maven-surefire-plugin`
* Using `PicoContainer` as Dependency Injection (DI) Containers to Sharing Test Context between Cucumber Step Definitions
* Using `ScenarioContext` & `Java Hash Map`to store and share test date between steps
* `Json Schema` validation
* Deserialization with Generics using `io.restassured.mapper.TypeRef` to deserialize the response to a container with a generic type
* Authentication
* Specification Re-use by using  `RequestSpecBuilder` or `ResponseSpecBuilder.`
* Verifying Response Data: status code, status line, cookies, headers, content type and body
* Specifying Request Data: headers, cookies, body and content type.

  
---  
### Specflow
#### Web
* Parallel Execution by Specflow.Nunit
* Customize BoDi container which used in before scenario `Hook`, in this demo, I added `driver`,`pages` to container
* Use _Explicit wait_ to help to _findElement_ call _WebDriverWait_ until the dynamically added element from the script has been added to the DOM
  ```
  WebElement foo = new WebDriverWait(driver, Duration.ofSeconds(3)).until(driver -> driver.findElement(By.name("q")));```
* Tracking log using Nlog, see in folder specflow-uis
* Use "Page Object Model" reason behind is Code becomes less and optimized because of the reusable page methods in the POM classes, also it makes code makes the code cleaner and easy to understand.
* Logging
 * Nlog
* CI - Azure
 * SpecFlow+ LivingDoc

#### Api
* Validate Response using RestSharp
 * Response Status
 * Response Headers
 * Response Body
* Send and verify HTTP request
 * Post/Get/Delete/Put
* Execute request with Powerful Generic Deserialization (more explanations please see below)
* Parallel Execution using Context dependency Injection(see videos)
* Reporting
 * specflow-living doc
* Test Assertion by Specflow.assist CompareToInstance
* Include Authenticators
 * JWT
 * Basic Auth

---
### Cypress

* end-to-end
* Integration testing which only written in
* JavaScript
* Page Object
* Continuous Integration

---
### Appium
* Testing frameworks TestNG\
* All capabilities, playback and delay settings are configurable through config file.\
* Supports video recording of tests\
* Supports capturing screenshots for Android\
* Provides inbuilt assertions to verify the device elements.\
* Supports Android Emulators.









