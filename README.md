# System Log Analysis & Diagnostic Reporting

## Overview

This project simulates an IT Support / Desktop Support troubleshooting scenario using SQL Server to analyze system and application logs.

The goal is to identify recurring technical issues, error codes, affected computers, performance problems, response-time issues, and error trends that can help support technicians investigate and troubleshoot incidents.

---

## Objective

The project focuses on:

- Identifying recurring system and application errors
- Analyzing error codes and error frequency
- Identifying affected computers and users
- Investigating response-time and performance issues
- Analyzing error trends by date and time
- Supporting technical troubleshooting and escalation
- Documenting troubleshooting procedures

---

## Technologies

- SQL Server
- SQL Server Management Studio (SSMS)

## Project Architecture

System / Application Logs -->SQL Server--> Data Quality Checks-->Log Analysis-->Diagnostic Reporting-->Troubleshooting Documentation

## Database 

- The project uses a SQL Server database named:
    * IT_Log_Analysis

## Data Quality Checks
Before performing the analysis, SQL queries are used to validate the log data.
<img width="975" height="548" alt="image" src="https://github.com/mjahan11/system-log-analysis-diagnostic-reporting/blob/main/Data-quality%20checks.jpg" />

The project checks for:

- Missing timestamps
- Missing computer names
- Duplicate records
- Invalid response times
- Incomplete log information

### Validation Result

The current dataset contains 20 records. The validation checks identified:

- 0 missing timestamps
- 0 missing computer names
- 0 invalid response times

## Log Analysis

SQL queries were developed to analyze system and application logs and identify recurring technical issues that may require further troubleshooting.

### 1. Total System Errors

The total number of error events was calculated to understand the overall error volume in the dataset.

<img width="975" height="548" alt="image" src="https://github.com/mjahan11/system-log-analysis-diagnostic-reporting/blob/main/loganalsis2.jpg" />

### 2 Errors by Computer

Errors were grouped by computer to identify systems with a higher number of recorded errors.

<img width="975" height="548" alt="image" src="https://github.com/mjahan11/system-log-analysis-diagnostic-reporting/blob/main/loganalsis3.jpg" />



### 3. Recurring Error Codes
Error codes were analyzed to identify recurring technical problems.
<img width="975" height="548" alt="image" src="https://github.com/mjahan11/system-log-analysis-diagnostic-reporting/blob/main/loganalsis1.jpg" />




## Troubleshooting Workflow

## Troubleshooting Workflow

The log analysis is used as an initial diagnostic step to narrow the scope of a technical issue. The following workflow can be used by an IT Support or Desktop Support technician.

### Troubleshooting Steps

1. **Identify the recurring issue**  
   Review the log data to determine the type of problem being reported.

2. **Identify the affected computer or user**  
   Determine which workstation or user is associated with the issue.

3. **Review the error code and message**  
   Examine the error code and message to understand the reported problem.

4. **Check error frequency and timing**  
   Determine whether the issue is isolated or recurring and identify when it occurs.

5. **Verify network connectivity**  
   Test network connectivity, DNS resolution, and access to required resources when applicable.

6. **Check Windows services and applications**  
   Verify that required Windows services and application processes are running.

7. **Review Windows Event Viewer**  
   Check Application, System, and Security logs for related events.

8. **Check user account and permissions**  
   Verify account status, authentication, access permissions, and resource access when applicable.

9. **Test from another workstation**  
   Determine whether the issue is specific to one computer or affects multiple systems.

10. **Document the findings**  
    Record the symptoms, investigation steps, findings, and actions taken.

11. **Escalate when required**  
    Escalate the issue to the appropriate server, network, application, or security team when it cannot be resolved at the support level.

## Example Diagnostic Scenario

## SQL Skills Demonstrated

## Project Structure

## Key Outcome

## Disclaimer


