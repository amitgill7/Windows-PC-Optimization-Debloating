# Windows PC Optimization & Debloating Lab 💻

## Overview
This lab documents the process of optimizing and deep-cleaning a Windows 10/11 system using both manual techniques and the Chris Titus Tech Windows Utility. The goal was to reduce background processes, lower memory usage, improve system responsiveness, and gain better control over privacy and Windows updates.

---

## Objectives
- Reduce RAM and CPU usage
- Remove unnecessary Windows bloatware
- Optimize startup and background services
- Improve boot time and system responsiveness
- Enhance privacy and telemetry control
- Document measurable before/after results

---

## Tools Used
- Windows Task Manager
- Windows Disk Cleanup
- PowerShell (Administrator)
- Chris Titus Tech Windows Utility (WinUtil)

---

## System Information
- Operating System: Windows 11
- Optimization Method: PowerShell-based system tuning
- Permissions: Administrator

---

## Methodology

### Step 1: Baseline System Analysis
- Recorded memory usage, CPU usage, and background process count using Task Manager
- Captured screenshots of system state before optimization

### Step 2: Utility Execution
- Launched PowerShell as Administrator
- Executed the Chris Titus Windows Utility using:
  ```powershell
  iwr -useb https://christitus.com/win | iex

