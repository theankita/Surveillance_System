# Platform Surveillance System

## Overview

Platform Surveillance System is a Python-based system monitoring and automation tool that periodically collects information about system resources and running processes and stores the information in log files.

The application monitors CPU usage, RAM consumption, disk utilization, network statistics, and active processes. Logs are automatically generated at user-defined intervals using a scheduler.

This project demonstrates the practical use of Python automation, process monitoring, system administration, scheduling, and log generation.

---

## Features

* Automatic system monitoring
* Periodic log generation
* CPU usage monitoring
* RAM usage monitoring
* Disk usage reporting
* Network statistics collection
* Running process monitoring
* Process details logging
* Scheduled execution using time intervals
* Automatic log file creation with timestamps

---

## Technologies Used

### Programming Language

* Python

### Libraries & Modules

* psutil
* schedule
* os
* sys
* time

### Concepts

* Process Monitoring
* System Administration
* Task Scheduling
* Log Generation
* Automation Scripting
* Resource Monitoring

---

## Project Structure

```bash
Surveillance_System/
│
├── Surveillance.py
│
README.md
```

---

## Workflow

Start Application
↓
Accept Command-Line Arguments
↓
Schedule Monitoring Task
↓
Collect System Information
↓
Generate Log File
↓
Store Process Details
↓
Repeat at Specified Interval

---

## Monitored Information

### CPU Monitoring

The application collects current CPU utilization using:

```python
psutil.cpu_percent()
```

### Memory Monitoring

The application collects RAM usage statistics using:

```python
psutil.virtual_memory()
```

### Disk Monitoring

Disk partition usage is monitored using:

```python
psutil.disk_partitions()
psutil.disk_usage()
```

### Network Monitoring

Network traffic statistics are collected using:

```python
psutil.net_io_counters()
```

Information recorded:

* Bytes Sent
* Bytes Received

### Process Monitoring

The application scans active processes and records:

* Process ID (PID)
* Process Name
* Username
* Process Status
* Process Start Time
* CPU Usage Percentage
* Memory Usage Percentage

---

## Log File Generation

A timestamped log file is automatically created.

Example:

```text
2026-06-01_18-30-45.log
```

The log file contains:

* System Report
* CPU Usage
* RAM Usage
* Disk Usage
* Network Statistics
* Process Information

---

## Command-Line Usage

### Help

```bash
python Surveillance.py --h
```

### Usage Information

```bash
python Surveillance.py --u
```

### Execute Monitoring

```bash
python Surveillance.py 5 Logs
```

Where:

* 5 = Monitoring interval in minutes
* Logs = Directory used to store generated log files

---

## Sample Output

```text
--------------------------------------------------
---------- Platform Surveillance System ----------
--------------------------------------------------

Platform Surveillance System started successfully

Directory created with name : Logs

Time interval in minutes : 5

Press Ctrl + C to stop the execution
```

---

## Learning Outcomes

This project demonstrates:

* Python Automation
* Process Monitoring
* System Resource Tracking
* Log File Generation
* Task Scheduling
* Command-Line Programming
* Operating System Utilities
* System Administration Concepts

---

## Future Improvements

* Email Log Delivery
* PDF Report Generation
* Real-Time Dashboard
* CPU and Memory Usage Alerts
* Database Storage for Logs
* Web-Based Monitoring Interface
* Multi-System Monitoring

---

## Author

### Ankita Dnyanoba Shinde

GitHub:
https://github.com/theankita

**Project Type:** Python Automation & System Monitoring Project
