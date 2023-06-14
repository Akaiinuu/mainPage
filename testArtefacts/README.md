# Test Strategy

## 1. Scope And Overview

### 1.1. Test object

The Mortgage Calculator Web App is a simple yet essential tool designed to assist users in calculating mortgage payments based on the loan amount, interest rate, and loan term. The primary objective of testing this web application is to ensure accurate calculations, proper functionality, and a seamless user experience. The test strategy will focus on validating the core features and ensuring the app performs as intended.

### 1.2. Objective

The key objectives of testing the Mortgage Calculator Web App are as follows:

#### 1.2.1 Functional Testing:

* Verify the accuracy of mortgage payment calculations.
* Validate the functionality of input fields, buttons, and calculations.
* Ensure proper handling of different loan terms, interest rates, and loan amounts.
* Test various scenarios, including positive and negative test cases, boundary values, and edge cases.

#### 1.2.2. Usability Testing:

* Evaluate the user interface for intuitiveness and ease of use.
* Validate the responsiveness of the app across different devices and screen sizes.
* Verify that error messages are clear and informative
* Test the app's compatibility with popular web browsers.

#### 1.2.3. Performance Testing:

* Measure the app's response time under normal and peak load conditions.
* Validate that the app can handle multiple simultaneous calculations without performance degradation.
* Test the app's stability and resource consumption to ensure it can handle expected user traffic.

#### 1.2.4. Security Testing:

* Validate the app's resistance to common security vulnerabilities, such as SQL injection and cross-site scripting.
* Ensure that user inputs are properly validated and sanitized to prevent data breaches or unauthorized access.
* Test authentication mechanisms (if applicable) to ensure secure access to the app.

## 2. Test approach

### 2.1. Testing levels

| Level                                 |                                           Description                                           |                                      Responsible role |
|---------------------------------------|:-----------------------------------------------------------------------------------------------:|------------------------------------------------------:|
| Unit testing.                         |                               Testing all components and modules.                               |                                      Developers team. |
| Integration testing.                  |        Testing how different modules and components work together. API, UI, E2E testing.        |                   Automation QA team. Manual QA team. |
| System testing.                       |                     Testing how all system work. Check different scenarios.                     | Automation QA team. Manual QA team. Performance team. |
| User acceptance testing.              |  Validating the system's suitability for real-world use and its alignment with business needs.  |                         Manual QA team. Stakeholders. |

### 2.1. Testing types

| Type                      |                                                                          Goal                                                                          |                                     Responsible role |
|---------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------:|-----------------------------------------------------:|
| Unit testing.             |               To verify the functionality of individual units or components of the software and ensure they work correctly in isolation.               |                                     Developers team. |
| Smoke testing.            | To perform a quick check of the critical functionalities of the software after a build or deployment, ensuring that major issues are identified early. | Developers team. Automation QA team. Manual QA team. |
| API testing.              |                        To validate that the API functions as intended, adhering to the defined specifications and requirements.                        |                  Automation QA team. Manual QA team. |
| UI testing.               |                                   To verify that users can interact with the application's user interface components                                   |                  Automation QA team. Manual QA team. |
| System testing.           |      To test the entire integrated system and verify that it functions according to the specified requirements and meets the intended user needs.      |                                      Manual QA team. |
| Perfomance testing.       |                                                         To validate Stability and Reliability                                                          |                                    Performance team. |
| Security testing.         |                                         To identify vulnerabilities, weaknesses, and potential security risks                                          |                                       Security team. |
| Regression testing.       |      To ensure that existing functionality is not affected by new changes or bug fixes, maintaining the stability and integrity of the software.       |                  Automation QA team. Manual QA team. |
| Localization Testing.     |    To verify that the software functions correctly when adapted to different languages or cultural requirements, ensuring localization is accurate.    |                                      Manual QA team. |
| Accessibility Testing.    |  To ensure the software is accessible to users with disabilities, adhering to accessibility standards and guidelines, and providing equal usability.   |                                      Manual QA team. |
| User Acceptance Testing.  |       To test the software from the end-user's perspective and validate its usability, ensuring it meets the user requirements and expectations.       |                        Manual QA team. Stakeholders. |

### 2.2. Testing tools and technologies

| Tool or technology  |                                                   Purpose                                                    |                                                                      Responsible role |
|---------------------|:------------------------------------------------------------------------------------------------------------:|--------------------------------------------------------------------------------------:|
| Java.               |                       Programming language for writing code, tests and test framework.                       |                                                  Developers team. Automation QA team. |
| JUnit.              |                               Framework for creating unit-test and auto tests.                               |                                                                   Automation QA team. |
| Selenium.           |                                    Framework for creating UI auto tests.                                     |                                                                   Automation QA team. |
| RestAssured.        |                                    Framework for creating API auto tests.                                    |                                                                   Automation QA team. |
| Allure.             |                                 Framework for creating auto tests’s reports.                                 |                                                                   Automation QA team. |
| Maven.              | Provides a consistent and standardized way to build, package, and manage dependencies of a software project. |                                                  Developers team. Automation QA team. |
| Jira.               |                                            Task management tool.                                             | Automation QA team. Manual QA team. Performance team. Developers team. Security team. |
| TestRail.           |                            Test management tool. Creating and storing test cases.                            |                  Automation QA team. Manual QA team. Performance team. Security team. |
| Confluence.         |                              Creating, storing, maintaining test documentation.                              |                  Automation QA team. Manual QA team. Performance team. Security team. |
| Postman.            |                                            Tool for testing API.                                             |                                                                       Manual QA team. |
| Swagger.            |                               Tool for creating and testing API specification.                               |                                                      Manual QA team. Developers team. |
| Kibana.             |                                     Tool for creating and storing logs.                                      |                                                      Manual QA team. Developers team. |
| MySQL.              |                                                Storing data.                                                 |                                  Developers team. Automation QA team. Manual QA team. |
| Figma.              |                                          Testing moqups and screen.                                          |                                                                       Manual QA team. |
| Browser’s devtools. |                                                 Testing UI.                                                  |                                                   Automation QA team. Manual QA team. |
| TeamCity.           |                                    CI/CD server for executing auto tests.                                    |                                  Developers team. Automation QA team. Manual QA team. |
| GitHub              |                            Hosting platform for version control and collaboration                            |                                  Developers team. Automation QA team. Manual QA team. |

## 2.3. Test environment

### 2.3.1. Stands

| Stand   |        Link         |                                     Responsible role |
|---------|:-------------------:|-----------------------------------------------------:|
| Dev     |     dev.dev.com     |                        Developers team. DevOps team. |
| Test    |    test.test.com    |                                      Manual QA team. |
| Preprod | Preprod.Preprod.com | Automation QA team. Performance team. Security team. |
| Prod    |      prod.com       |                                        Support team. |

### 2.3.2. Test platforms

* Use a range of devices, including desktops, laptops, tablets, and smartphones, to test the app's responsiveness.
* Test across various operating systems, including Windows, macOS, iOS, and Android.
* Utilize different web browsers such as Chrome, Firefox, Safari, and Edge.

## 3. Release control

### 3.1. Release criteria
* All critical test cases related to mortgage payment calculations, input validation, and user interface functionality should pass successfully.

* A minimum test coverage of 90% should be achieved, ensuring that major components and functionalities are thoroughly tested.

* High-severity defects identified during testing should be resolved or have appropriate workarounds in place.

### 3.2. Regression testing

* Conduct comprehensive regression testing to ensure that new feature implementations or code changes do not introduce any regressions in existing functionality.

* Execute a regression test suite that includes critical and high-priority test cases covering key calculation scenarios, input validations, and user interactions.

### 3.3. Version control
* Utilize a version control system (GitHub) to manage code changes and track the history of modifications made to the application.

* Ensure that all code changes are properly documented, reviewed, and committed to the appropriate branches or repositories.

### 3.4. Deployment testing
* Validate the deployment process by simulating a production-like environment and performing end-to-end deployment testing.

* Verify the correct configuration of deployment settings, including database connections, environment-specific configurations, and security settings.

* Ensure smooth database migrations or updates are executed without any data loss or inconsistencies.

### 3.5. Release notes

* Prepare detailed release notes documenting the changes, bug fixes, and enhancements included in the current release.

* Include information about the specific mortgage calculation improvements, UI enhancements, and any known issues or limitations in the release notes.

* Provide instructions or guidelines for users and stakeholders on how to best utilize the new features and report any issues or feedback.

### 3.5. Collaboration with Development and Operations Teams

* Foster close collaboration between the development, testing, and operations teams throughout the release process.

* Conduct regular meetings to align on release timelines, coordinate any required infrastructure changes, and address any deployment-related concerns or dependencies.

### 3.7. Rollback plan

* Define a clear rollback plan in case critical issues or defects are identified after the release.

* Establish criteria for triggering a rollback, such as severe functionality issues impacting user experience or data integrity.

* Document the steps required to revert to the previous stable version of the application and communicate the decision to all relevant stakeholders.

## 4. Risk analysis
Several risks are associated with the testing process. These risks include inaccurate calculations, usability issues, performance bottlenecks, security vulnerabilities, and compatibility challenges. Mitigation strategies for each risk will be implemented, including thorough validation of calculations, usability testing with real users, performance testing under various load conditions, security testing using industry-standard practices, and compatibility testing across different browsers and devices.

| Risk                                        |                                                                                                                                 Description                                                                                                                                  | Impact |                                                                                                                                                                                                                        Mitigation |
|---------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|--------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| Incomplete or Inadequate Test Coverage.     |                                                        If the test coverage is insufficient, there is a risk of missing critical scenarios or functionalities that could lead to undetected defects in the software.                                                         | High.  |                                                                                                                      Requirement Analysis and Traceability. Test Case Design Techniques. Exploratory Testing. Regression Testing. |
| Inaccurate Test Data.                       |                                                   Using inaccurate or incomplete test data can result in ineffective testing and may not reflect real-world usage scenarios, leading to potential issues being overlooked.                                                   | High.  |                                                                                               Data Validation and Verification. Data Generation and Masking. Test Data Refresh and Cleanup. Data Consistency across Environments. |
| Defects Leakage.                            |                                    Despite thorough testing, there is a risk that some defects may go undetected and subsequently reach the production environment, impacting end-users and potentially causing customer dissatisfaction.                                    | High.  |                                             Test Coverage Analysis. Test Case Effectiveness. Defect Tracking and Management. Regression Testing. Continuous Integration and Continuous Delivery (CI/CD). User Acceptance Testing. |
| Time and Resource Constraints.              |  Limited time and resources can pose a risk to comprehensive testing. With tight schedules and limited personnel, there may be pressure to skip certain tests or rush through the testing process, which can result in inadequate coverage and potentially missed defects.   | High.  |                                                                                              Prioritize Testing Efforts. Test Planning and Estimation. Agile Testing Practices. Test Automation. Collaboration and Communication. |
| Environmental Dependencies.                 |    Software systems often rely on external dependencies, such as databases, third-party services, or network infrastructure. Changes or issues with these dependencies can introduce risks during testing, as they may cause failures or inconsistencies in test results.    | High.  | Test Environment Replication. Test Environment Management. Environment Virtualization or Containerization. Environment Independence. Environment Monitoring. Environment Simulations and Mocking. Regular Environment Validation. |
| Communication and Collaboration Challenges. |                                   Lack of effective communication and collaboration among team members, stakeholders, and developers can lead to misunderstandings, delays in issue resolution, and inefficiencies in the testing process.                                   | High.  |                                                                                           Clear Communication Channels. Project Documentation. Agile Practices. Clear Roles and Responsibilities. Training and Skill Development. |
| Scope Creep.                                | Changes in project scope, requirements, or priorities can introduce risks during testing. Late changes or additions to the software can result in inadequate time for testing or the need for regression testing, potentially impacting the overall quality of the software. | High.  |                                                                                        Regularly Communicate and Collaborate with Stakeholders. Prioritize and Manage Change Requests. Clearly Define and Document Project Scope. |
| Tool Limitations.                           |              Testing tools and frameworks may have limitations or compatibility issues, which can affect the effectiveness and efficiency of the testing process. Inadequate tool selection or improper tool configuration can introduce risks during testing.               | High.  |                                                                                                                                     Tool Evaluation and Selection. Regularly Update and Upgrade. Regularly Evaluate Alternatives. |
| Human Error.                                |                     Testers can make mistakes during test case design, execution, or reporting, leading to inaccurate test results or missed defects. Proper training, attention to detail, and quality assurance practices can help mitigate this risk.                     | High.  |                                                                                                                     Training and Skill Development. Standardize Processes and Documentation. Clear and Detailed Test Case Design. |
| Security and Data Privacy Risks.            |                                      During testing, there is a risk of exposing sensitive data or introducing vulnerabilities in the system. It is crucial to handle test data and test environments securely to mitigate these risks                                       | High.  |                                                                             Perform Security Testing. Protect Test Environments. Secure Test Data. Regularly Educate and Train Team Members. Conduct Security Reviews and Audits. |

## 5. Review and approvals

### 5.1. Test plan review

* Before commencing testing, the test plan will undergo a review process involving relevant stakeholders, including the development team, project manager, and business analysts.

* The test plan will be assessed for completeness, alignment with project requirements, and feasibility of proposed testing approaches.

* Feedback and suggestions from reviewers will be incorporated into the test plan to enhance its effectiveness.

### 5.2. Test case review

* Test cases developed for the Mortgage Calculator Web App will undergo a review process to ensure their accuracy, coverage, and adherence to requirements.

* Peers, senior testers, or subject matter experts will review the test cases and provide feedback on their structure, relevance, and expected outcomes.

* The review process aims to identify any gaps, ambiguities, or redundant test cases and make necessary improvements.

### 5.3. Test data review

* The test data used for various test scenarios, including different loan amounts, interest rates, and loan terms, will be reviewed for appropriateness and representativeness.

* The review will involve validating that the test data covers a wide range of values, including edge cases and boundary conditions.

* Feedback from the review process will be considered to refine and enhance the test data set.

### 5.4. Test execution approval

* Before starting the formal test execution phase, the test manager or designated authority will review the test plan, test cases, and associated test data to ensure readiness for execution.

* The approval will be based on factors such as completeness of test coverage, availability of necessary resources, and confirmation of test environment stability.

* Once the approval is granted, the test execution phase can commence.

### 5.5. Defect review and approval

* When defects are discovered during testing, a defect review and approval process will be established.

* Defects will be documented, including their severity, impact, steps to reproduce, and supporting evidence.

* The project stakeholders, including the development team and business representatives, will review the defects and provide their approvals for prioritization and resolution.

### 5.6. Test completion review

* At the end of the testing phase, a review will be conducted to evaluate the completion and effectiveness of the testing activities.

* The test manager, project manager, and key stakeholders will assess whether the defined test objectives have been met and if the exit criteria for testing have been satisfied.

* The review will determine whether the application is ready for release or if additional testing or defect resolutions are required.

## 6. Test Deliverables

The following deliverables will be produced during the testing process:

* Test Plan: A comprehensive document outlining the test approach, objectives, and strategies.
* Test Cases: Detailed test cases covering functional, usability, performance, and security aspects.
* Test Execution Reports: Detailed reports capturing test results, including passed and failed test cases.
* Defect Reports: Log and track any identified defects with clear steps to reproduce and severity levels assigned.
* Test Summary Report: A final report summarizing the testing activities, outcomes, and recommendations.