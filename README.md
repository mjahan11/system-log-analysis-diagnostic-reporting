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

### Application Server Connection Failure

**Observed Issue:**  
The log analysis identified repeated application-server connection failures associated with error code **E500**.

**Affected Computer:**  
PC-002

**Error Frequency:**  
6 recorded E500 errors

**Error Message:**  
Unable to connect to application server

### Investigation

The SQL analysis showed that PC-002 had the highest number of recorded errors in the current dataset. The recurring E500 errors indicate that the application-server connection issue should be investigated further.

### Troubleshooting Steps

A Desktop Support technician could:

1. Verify the workstation's network connection.
2. Test connectivity to the application server.
3. Verify DNS resolution.
4. Check whether the application server is available.
5. Verify required application services are running.
6. Review Windows Event Viewer for related errors.
7. Review application logs.
8. Test the application from another workstation.
9. Document the findings and troubleshooting performed.
10. Escalate to the network, server, or application team if necessary.

### Diagnostic Conclusion

The SQL analysis does not independently determine the root cause. It helps identify the affected system and recurring error pattern so that the technician can focus the next troubleshooting steps.

## SQL Skills Demonstrated

- SQL Server
- SELECT statements
- WHERE filtering
- GROUP BY
- ORDER BY
- Aggregate functions
- CASE statements
- Date and time functions
- Common Table Expressions (CTEs)
- SQL Views
- Data validation
- Error analysis
- Performance analysis
- Diagnostic reporting

## Project Structure
```text
system-log-analysis-diagnostic-reporting/
│
├── SQL/
│   ├── 01_Create_Database.sql
│   ├── 02_Create_Table.sql
│   ├── 03_Insert_Data.sql
│   ├── 04_Data_Quality_Checks.sql
│   ├── 05_Log_Analysis.sql
│   └── 06_Diagnostic_Reports.sql
│
├── Documentation/
│   └── Troubleshooting_Guide.md
│
├── Screenshots/
│   ├── 02_data_quality_checks.jpg
│   └── 03_recurring_error_codes.png
│
└── README.md
```

## Key Outcome

## Key Outcome

This project demonstrates how SQL can be used as a technical troubleshooting tool in an IT Support environment.

The analysis helps identify recurring errors, affected computers, error patterns, and performance issues so that support technicians can narrow the troubleshooting scope and determine appropriate next steps.

The project also demonstrates the ability to document technical findings and follow a structured troubleshooting and escalation process.

## Disclaimer

This is a portfolio project created for learning and demonstration purposes.

The system logs, computer names, users, error codes, and troubleshooting scenarios are simulated and do not contain real company or customer information.


