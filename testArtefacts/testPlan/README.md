# Test plan

## 1. Introduction

The Mortgage Calculator is a web application designed to assist users in calculating mortgage payments based on loan amount, interest rate, and loan term. The application aims to provide accurate and reliable calculations in a user-friendly manner.

Mortgage Calculator typically includes the following functions:

1. **Loan Amount**: This function allows the user to input the total amount they wish to borrow for their mortgage.

2. **Interest Rate**: The interest rate function enables the user to enter the annual interest rate associated with their mortgage.

3. **Loan Term**: This function allows the user to specify the duration of the loan in years or months.

4. **Monthly Payment Calculation**: The Mortgage Calculator calculates the monthly payment based on the loan amount, interest rate, and loan term provided by the user.

5. **Amortization Schedule**: The calculator generates an amortization schedule, which displays a detailed breakdown of the monthly payment, including the principal amount, interest payment, and remaining loan balance over the loan term.

6. **Additional Payments**: Some Mortgage Calculators provide the option to include additional payments, such as lump-sum payments or increased monthly payments, to see their impact on the loan repayment schedule and overall interest savings.

7. **Affordability Analysis**: This function helps users determine how much they can afford to borrow based on their income, expenses, and debt-to-income ratio.

8. **Total Interest Calculation**: The calculator computes the total amount of interest paid over the life of the loan, giving users an understanding of the long-term cost of the mortgage.

9. **Comparison Tool**: a comparison feature that allows users to input multiple loan scenarios, compare their monthly payments, interest costs, and loan terms, aiding in decision-making.

10. **Refinancing Analysis**: For existing mortgages, the calculator may include a refinancing analysis function, enabling users to evaluate the potential savings and benefits of refinancing their loan.

## 2. Test Objectives

1. Validate the accuracy of mortgage payment calculations by comparing the results with manual calculations using predefined test scenarios.
Example: Verify that for a loan amount of $200,000, an interest rate of 4%, and a 30-year loan term, the calculated monthly payment is approximately $954.83.

2. Evaluate the usability and functionality of the user interface by performing exploratory testing and assessing the intuitiveness of the application's features.
Example: Verify that all input fields are clearly labeled and user-friendly, allowing users to easily enter loan details and obtain accurate results.

3. Verify the input validation and error handling mechanisms by intentionally providing invalid or out-of-range input values and ensuring appropriate error messages are displayed.
Example: Confirm that when entering a negative loan amount, the application displays an error message indicating that the loan amount must be a positive value.

4. Assess the performance and responsiveness of the application by simulating concurrent user interactions and measuring the response times for various calculations.
Example: Measure the application's response time for calculating mortgage payments with multiple simultaneous user requests and ensure it remains within acceptable limits (e.g., under 2 seconds).

5. Validate the compatibility of the application across different browsers and devices to ensure a consistent user experience.
Example: Test the Mortgage Calculator on popular web browsers such as Chrome, Firefox, and Safari, as well as on different mobile devices running iOS and Android operating systems.

## 3. Test Scope

**In scope**: Calculation accuracy, user interface functionality, input validation, error handling, performance, and compatibility.

**Out of scope**: Integration with external systems, security testing, and backend database validation.

1. **Calculation Accuracy**: The scope includes verifying the accuracy of mortgage payment calculations performed by the calculator. This involves validating that the calculated monthly payments align with the expected results based on predefined test scenarios and manual calculations.

2. **User Interface Functionality**: The scope encompasses testing the functionality and usability of the user interface components of the mortgage calculator. It involves validating that all UI elements are functional, responsive, and provide the intended user experience. This includes verifying the proper functioning of input fields, buttons, dropdowns, and any interactive elements.

3. **Input Validation**: The scope covers testing the validation mechanisms for user inputs. It includes ensuring that the calculator handles invalid or out-of-range values appropriately, displaying error messages when required, and preventing incorrect inputs from affecting the calculation results.

4. **Error Handling**: The scope includes testing how the mortgage calculator handles errors and exceptions. This involves validating that error messages are displayed in case of unexpected scenarios or incorrect inputs, providing clear instructions for resolution, and ensuring that the application gracefully recovers from errors without crashing or compromising the user experience.

5. **Performance**: The scope encompasses evaluating the performance and responsiveness of the mortgage calculator. This involves measuring and validating the system's response times for different calculations, ensuring that it remains within acceptable limits even under peak load or stress conditions. It also includes assessing resource utilization, such as CPU and memory usage, to identify any performance bottlenecks.

6. **Compatibility**: The scope covers testing the compatibility of the mortgage calculator across different browsers, devices, and operating systems. It involves verifying that the calculator functions correctly and displays appropriately on various platforms, ensuring a consistent user experience for a wide range of users.

## 4. Test Approach

Test approach described in the [Test Strategy](https://github.com/Akaiinuu/mainPage/blob/main/testArtefacts/testStrategy/README.md).

## 5. Test Environment

### 5.1 Operation system 

* Windows 10 (64-bit)

* macOS Mojave (10.14)

* Ubuntu Linux (20.04)

### 5.2. Browsers

* Google Chrome (version 92)

* Mozilla Firefox (version 90)

* Safari (version 14.1)

### 5.3. Mobile devices

* iPhone 12 (iOS 15)

* Samsung Galaxy S20 (Android 11)

### 5.4. Testing tools 

* Test automation framework: Selenium WebDriver (Java), RestAssured (Java), Junit (version 5)

* Test management tool: JIRA, TestRail, Confluence

* Bug tracking tool: JIRA

* Performance testing tool: Apache JMeter

### 5.5 Test data

Test data is stored in the TestRail

* Valid loan amounts with varying values

* Valid interest rates with different rates

* Different loan terms (in years and months)

* Invalid input data for testing validation

### 5.6. Dependencies

External API for fetching real-time interest rates (API documentation and endpoints will be provided separately)

Database server (MySQL) for storing user preferences and configurations

### 5.7. Test environment setup

1. Install the latest versions of the specified operating systems on dedicated test machines.

2. Install and configure the required browsers with the specified versions.

3. Set up the mobile devices with the specified operating system versions.

4. Install and configure the necessary testing tools (Selenium WebDriver, JIRA, Bugzilla, JMeter) on the designated test machines.

5. Ensure the availability of the external API for fetching real-time interest rates.

6. Set up the MySQL database server with the required schema and configurations.


## 6. Test Execution

### 6.1. Test case execution

* The test cases will be executed using a combination of manual and automated testing approaches.

* Test cases will be executed in a sequential manner, ensuring any dependencies are considered.

* The testing team, will be responsible for executing the test cases.

### 6.2. Test execution process

* Begin by reviewing the test cases and test scenarios to ensure a clear understanding of the expected results.

* Execute each test case step-by-step, following the defined test procedures and guidelines.

* Record the actual results, observations, and any deviations encountered during test execution.

* Compare the actual results with the expected results to determine the pass/fail status of each test case.

* If automated testing is involved, execute the automation scripts and analyze the generated test reports.

### 6.3 Defect reporting

* Any defects encountered during test execution should be promptly reported using the designated defect tracking tool (e.g., JIRA).

* Testers should provide detailed defect reports, including steps to reproduce, expected and actual results, and severity/priority classification.

* The assigned defect owner should review and validate the reported defects, provide necessary clarifications, and track their resolution.

### 6.4. Test progress tracking

* Test progress should be tracked regularly to monitor the status of test execution.

* Testers should update the test case execution status, indicating whether a test case is executed, passed, failed, or blocked.

* Test progress reports should be prepared and shared with the relevant stakeholders at defined intervals to provide visibility into the testing progress.

### 6.5. Test logs and results documentation

* Test execution logs should be maintained to document the details of executed test cases, including test case ID, steps, and actual results.

* Any deviations, observations, or issues encountered during test execution should be logged appropriately.

* Test results, including the pass/fail status of each test case, should be documented for future reference and analysis.

### 6.6 Test coverage analysis

* Regularly analyze the test coverage to ensure that all critical functional areas are adequately tested.

* Evaluate the percentage of test cases executed, coverage by functional modules, and coverage by risk priority to assess the level of testing completeness.

* Identify any gaps in the test coverage and take necessary actions to ensure comprehensive testing

## 7. Schedule

### 7.1. Test phases and milestones

* Unit Testing Phase: Start Date - [Insert Start Date], End Date - [Insert End Date]

* Integration Testing Phase: Start Date - [Insert Start Date], End Date - [Insert End Date]

* System Testing Phase: Start Date - [Insert Start Date], End Date - [Insert End Date]

* User Acceptance Testing (UAT) Phase: Start Date - [Insert Start Date], End Date - [Insert End Date]

### 7.2 Test iterations

Iteration 1: Start Date - [Insert Start Date], End Date - [Insert End Date]

* Objective: Perform initial functional testing and identify critical defects.

* Scope: Focus on basic mortgage calculations, input validation, and basic user interface interactions.

* Deliverables: Test cases, defect reports, and test execution logs.

Iteration 2: Start Date - [Insert Start Date], End Date - [Insert End Date]

* Objective: Perform in-depth testing and verify complex mortgage scenarios.

* Scope: Cover advanced mortgage calculations, edge cases, error handling, and integration with external systems.

* Deliverables: Test cases, defect reports, and test execution logs.

### 7.3. Test activities timeline

* Test Planning: Start Date - [Insert Start Date], End Date - [Insert End Date]

* Test Case Preparation: Start Date - [Insert Start Date], End Date - [Insert End Date]

* Test Execution: Start Date - [Insert Start Date], End Date - [Insert End Date]

* Defect Management: Start Date - [Insert Start Date], End Date - [Insert End Date]

* Test Reporting: Start Date - [Insert Start Date], End Date - [Insert End Date]

### 7.3. Resource allocation

Testers:

[Insert Name 1]: Dedicated full-time to testing activities throughout the project.

[Insert Name 2]: Part-time involvement during specific testing phases.

Test Automation Engineer:

[Insert Name]: Responsible for developing and maintaining automated test scripts.

Testing Tools and Equipment:

[Insert Tool 1]: Used for test case management and defect tracking.

[Insert Tool 2]: Used for test automation and performance testing.

### 7.5. Dependencies

* Availability of the Test Environment: Ensure the test environment is set up and ready by [Insert Start Date].

* Application Builds: Coordinate with the development team to receive the application builds for testing according to the defined schedule.

* Test Data: Ensure relevant and appropriate test data is available prior to the start of each testing phase.

### 7.6. Test effort estimation

* Unit Testing Phase: [Insert Estimated Effort]

* Integration Testing Phase: [Insert Estimated Effort]

* System Testing Phase: [Insert Estimated Effort]

* UAT Phase: [Insert Estimated Effort]

### 7.7. Contingency plan

* Allocate buffers in the schedule to accommodate unexpected issues or delays that may arise during testing.

* Regularly monitor the progress and address any deviations from the planned schedule promptly.

* Maintain open communication channels with stakeholders to ensure alignment and manage expectations regarding the schedule

## 8. Test Deliverables

Test Plan document, Test Cases document, Test Execution Reports, Defect Reports.

## 9. Risk Mitigation

1. Inaccurate calculations leading to incorrect mortgage payments. Mitigation: Conduct thorough calculation validation against predefined test scenarios and manual calculations.

2. Poor performance and slow response times. Mitigation: Perform performance testing under load and stress conditions to identify bottlenecks and optimize application performance.

3. Compatibility issues across different browsers and devices. Mitigation: Test the application on multiple browsers and devices to ensure consistent functionality and user experience.


## 10. Exit Criteria

Criteria for test completion: Execution of all test cases, resolution of critical and high-severity defects, and meeting the predefined test objectives.



















