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
<img width="975" height="548" alt="image" src="https://github.com/mjahan11/system-log-analysis-diagnostic-reporting/blob/main/loganalsis1.jpg" />



## Troubleshooting Workflow

## Example Diagnostic Scenario

## SQL Skills Demonstrated

## Project Structure

## Key Outcome

## Disclaimer


