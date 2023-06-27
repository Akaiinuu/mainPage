# Bug Reports

## 1. SQL injection Vulnerability in Mortgage Calculator

### 1.1. Bug Description

The mortgage calculator application is vulnerable to SQL injection attacks, allowing unauthorized access and manipulation of the underlying database. This security vulnerability poses a significant risk to the confidentiality, integrity, and availability of sensitive user data.

### 1.2. Steps to Reproduce

1. Launch the mortgage calculator application.

2. In the input field for the loan amount, enter the following value: "'; DROP TABLE Users;--".

3. Click on the calculate button.

4. Observe the results and behavior of the calculator.

### 1.3. Expected Result

The mortgage calculator should correctly validate and sanitize user input, preventing any unauthorized SQL commands or injections. The application should display an error message indicating that the input is invalid or reject the input altogether.

### 1.4. Actual Result

Instead of properly validating the input, the mortgage calculator executes the injected SQL command, resulting in the deletion of the "Users" table from the underlying database. This indicates a severe vulnerability that allows unauthorized database manipulation.

### 1.5. Example

1. Loan Amount: "'; DROP TABLE Users;--"

2. Interest Rate: 3.5%

3. Loan Term: 30 years

### 1.6. Actual Output

The mortgage calculator executes the injected SQL command, leading to the deletion of the "Users" table in the database.

### 1.7. Expected Output

The mortgage calculator should detect the SQL injection attempt, display an error message, and prevent any execution of unauthorized SQL commands.

### 1.8. Attachments

* Screenshots or video recordings demonstrating the issue

* Logs or error messages, if applicable

### 1.9. Impact of the Bug

This vulnerability exposes sensitive user data to unauthorized access and manipulation. Attackers can potentially perform malicious activities, such as deleting or modifying data, bypassing authentication, or gaining unauthorized access to the system. The impact includes compromising data integrity, breaching user privacy, and damaging the reputation of the application.

### 1.10. Priority

Considering the severe security implications and the potential for unauthorized access and data loss, this bug should be assigned the highest priority.

### 1.11. Severity

Given the critical nature of the vulnerability and its potential impact on data security, the severity of this bug is rated as critical.

### 1.12. Environment

* Operating System: Windows 10

* Browser: Google Chrome version 96.0.4664.93

* Mortgage Calculator Application Version: 1.2.3

### 1.13. Additional Notes

* The issue was reproduced multiple times with different SQL injection payloads.

* The vulnerability persists across different browsers and operating systems.

## 2. Incorrect Calculation of Monthly Payment in Mortgage Calculator

**Bug Description:** The mortgage calculator is producing incorrect monthly payment values, leading to inaccurate loan estimations for users. This issue affects the reliability and usability of the calculator, potentially causing financial implications for individuals relying on accurate mortgage calculations.

**Steps to Reproduce:**

1. Launch the mortgage calculator application.

2. Enter the following input values:

* Loan Amount: $250,000

* Interest Rate: 4.5%

* Loan Term: 30 years

3. Click on the calculate button.

4. Compare the calculated monthly payment value with the expected value.

**Expected Result:** The mortgage calculator should accurately calculate the monthly payment based on the provided loan amount, interest rate, and loan term. The calculated monthly payment should align with industry-standard formulas and known mortgage calculations.

**Actual Result:** The mortgage calculator produces an incorrect monthly payment value that deviates from the expected and accurate calculation. This discrepancy leads to misleading loan estimations and may result in users making financial decisions based on incorrect information.

**Example:**

* Loan Amount: $250,000

* Interest Rate: 4.5%

* Loan Term: 30 years

**Expected Monthly Payment:** $1,266.71 (approximately)

**Actual Monthly Payment:** $1,432.89 (approximately)

**Attachments:**

* Screenshots or video recordings demonstrating the issue

* Logs or error messages, if applicable

**Impact of the Bug:** The bug impacts the accuracy and reliability of the mortgage calculator, potentially causing financial implications for users. Incorrect monthly payment calculations may lead to borrowers receiving inaccurate loan estimations, affecting their ability to plan and manage their finances effectively.

**Priority:** Considering the impact on financial calculations and the importance of accurate loan estimations, this bug should be assigned a high priority.

**Severity:** Given the potential consequences for users relying on the mortgage calculator, the severity of this bug is rated as high.

**Environment:**

* Operating System: Windows 10

* Browser: Google Chrome version 96.0.4664.93

* Mortgage Calculator Application Version: 1.2.3

**Additional Notes:**

* The issue persists across different browsers and operating systems.

* It is recommended to conduct further investigation and analysis to identify the root cause of the incorrect calculation.

## 3. Error Message Not Displayed in Mortgage Calculator

**Bug Description:** The mortgage calculator fails to display an appropriate error message when invalid input is entered, making it challenging for users to identify and correct their mistakes. This issue hampers the usability and user experience of the calculator, potentially leading to confusion and frustration for users.

**Steps to Reproduce:**

1. Launch the mortgage calculator application.

2. Enter invalid or unsupported input values, such as special characters, alphabets, or negative numbers, in the loan amount, interest rate, or loan term fields.

3. Click on the calculate button or attempt to proceed with the calculation.

4. Observe the behavior and check if an error message is displayed.

**Expected Result:** The mortgage calculator should promptly detect invalid input values and display a clear and informative error message indicating the issue with the input. The error message should guide users on the valid format and range of values for each field.

**Actual Result:** The mortgage calculator does not display any error message when invalid input is entered. Users are not informed about the invalid input, which can lead to confusion and incorrect calculations.

**Example:**

* Loan Amount: $-100,000 (invalid)

* Interest Rate: 3.5%

* Loan Term: 25 years

**Expected Output:** An error message should be displayed, indicating that negative loan amounts are not allowed.

**Actual Output:** No error message is displayed.

**Attachments:**

* Screenshots or video recordings demonstrating the issue

* Logs or error messages, if applicable

**Impact of the Bug:** The absence of error messages for invalid input reduces the usability and user-friendliness of the mortgage calculator. Users may not be aware of their mistakes or understand why the calculation is not producing the expected results. This can lead to frustration, inaccurate calculations, and a negative user experience.

**Priority:** Considering the impact on usability and user experience, this bug should be assigned a moderate priority.

**Severity:** Given the potential confusion and frustration for users, the severity of this bug is rated as moderate.

**Environment:**

* Operating System: Windows 10

* Browser: Google Chrome version 96.0.4664.93

* Mortgage Calculator Application Version: 1.2.3

**Additional Notes:**

The issue should be investigated to determine the cause of the missing error message and implement appropriate error handling and validation mechanisms.


















