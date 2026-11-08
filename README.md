# SSH Security Monitoring and Brute-Force Detection Using Splunk

## Project Overview

This project demonstrates the use of Splunk Enterprise for monitoring and analysing SSH authentication logs in a Security Operations Centre (SOC) environment.

The objective was to ingest SSH log data into Splunk, analyse authentication activities, identify suspicious login behaviour, investigate potential brute-force attacks and develop an interactive security monitoring dashboard.

The project simulates practical tasks performed by a Tier 1 SOC Analyst during security monitoring and initial threat investigation.

## Project Objectives

- Ingest SSH authentication logs into Splunk Enterprise.
- Create and organise a dedicated Splunk index.
- Analyse successful and failed SSH authentication events.
- Identify frequently targeted usernames.
- Identify IP addresses generating suspicious login activity.
- Investigate repeated authentication failures.
- Detect potential SSH brute-force attempts.
- Build an interactive SOC monitoring dashboard.

## Tools and Technologies

| Tool | Purpose |
|---|---|
| Splunk Enterprise | Log ingestion, searching and analysis |
| SPL | Security event investigation |
| Linux / Ubuntu | Lab environment |
| SSH Logs (JSON) | Security event dataset |
| Splunk Dashboard Studio | Dashboard development |

## Lab Environment

- SIEM Platform: Splunk Enterprise
- Operating System: Ubuntu Server
- Data Format: JSON
- Splunk Index: `ssh_logs`
- Dashboard: SSH Security Monitoring Dashboard

## Project Implementation

### 1. Log Ingestion and Index Management

Created a dedicated Splunk index named `ssh_logs` to store and organise SSH authentication events separately from other security datasets.

Uploaded the SSH JSON dataset into Splunk and verified successful ingestion.

### 2. SSH Log Analysis

Used Splunk Processing Language (SPL) to investigate SSH authentication activities, including:

- Total SSH events.
- Successful authentication attempts.
- Failed authentication attempts.
- SSH activity over time.
- Source IP address analysis.
- Targeted username analysis.

### 3. Brute-Force Investigation

Investigated repeated SSH authentication failures to identify potential brute-force behaviour.

The investigation focused on:

- Repeated login failures.
- Source IP addresses generating multiple attempts.
- Targeted user accounts.
- Authentication activity patterns.
- Possible successful logins following repeated failures.

Repeated failed logins were treated as indicators requiring further investigation rather than automatic proof of an attack.

### 4. Dashboard Development

Developed an interactive SSH Security Monitoring Dashboard using Splunk Dashboard Studio.

The dashboard provides visual monitoring of SSH authentication activities through numerical panels, charts, tables and interactive inputs.

### Dashboard Features

- Total SSH Events
- Successful SSH Logins
- Failed SSH Logins
- SSH Events Over Time
- Top Source IP Addresses
- Top Targeted Usernames
- Successful vs Failed Authentication
- Potential Brute-Force Activity
- SSH Activity by Host
- Time Range Filtering

## Investigation Findings

Document the actual findings from your dataset here.

Examples of findings to report:

1. Number of successful SSH authentication attempts.
2. Number of failed SSH authentication attempts.
3. IP address with the highest number of failed attempts.
4. Most frequently targeted username.
5. Whether repeated authentication failures were observed.
6. Whether suspicious IP addresses eventually achieved successful authentication.

Only include findings verified from your Splunk searches.

## Screenshots and Evidence

The `screenshots/` directory contains visual evidence of the completed project.

It includes the dashboard overview, authentication analysis, IP investigation and potential brute-force detection panels.

## Skills Demonstrated

- SIEM Operations
- Splunk Enterprise Administration
- SPL Search and Data Analysis
- Linux Log Analysis
- SSH Authentication Monitoring
- Security Event Investigation
- Brute-Force Detection
- Dashboard Development
- Basic Threat Detection and Analysis
- Security Reporting

## Conclusion

This project provided practical experience in using Splunk Enterprise to monitor SSH authentication activities and investigate suspicious login behaviour.

It demonstrates the application of SIEM technology in security monitoring, event analysis and initial threat detection within a SOC environment.

## Dataset Attribution

Include the original dataset repository and its applicable licence here.

## Disclaimer

This project was developed in a controlled educational lab environment using sample security logs. It is intended for cybersecurity learning, SIEM practice and portfolio demonstration.
