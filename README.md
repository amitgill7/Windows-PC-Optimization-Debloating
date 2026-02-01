# Windows PC Optimization & Debloating Lab 💻

## Overview
This lab documents the manual optimization and deep cleaning of a Windows 11 system without the use of third-party automation tools. All changes were performed using native Windows utilities, PowerShell commands, system configuration tools, and registry settings to improve performance, reduce background processes, and enhance system responsiveness.

---

## Objectives
- Reduce RAM and CPU usage
- Remove unnecessary preinstalled applications
- Optimize startup and background services
- Improve boot time and system responsiveness
- Enhance system privacy and control over updates
- Demonstrate understanding of Windows system internals

---

## Tools Used
- Windows Task Manager
- PowerShell (Administrator)
- Services.msc
- Task Scheduler
- Disk Cleanup
- System Configuration (msconfig)
- Registry Editor
- Windows Settings

---

## System Information
- Operating System: Windows 11
- Permissions: Administrator
- Optimization Type: Manual system tuning

---

## Methodology

### Step 1: Baseline System Analysis
- Recorded CPU usage, memory usage, and background process count using Task Manager
- Captured screenshots of system state before optimization
<img width="926" height="560" alt="image" src="https://github.com/user-attachments/assets/2cac594b-a9a7-4fc9-ac7c-cd9c9303769f" />
<img width="926" height="567" alt="image" src="https://github.com/user-attachments/assets/61f803ed-7c55-432a-960d-b3610c4cacf9" />

---

### Step 2: System Safety Measures
- Verified Windows version and administrator access
- Created a system restore point before applying changes
<img width="852" height="480" alt="image" src="https://github.com/user-attachments/assets/30a06551-d684-49ab-b21f-802ad2fc3821" />

---

### Step 3: Check Windows Update Status
- Windows updates patch known vulnerabilities:
- Helps rotects against malware, ransomware, and exploits:
<img width="1200" height="634" alt="image" src="https://github.com/user-attachments/assets/b5e0682c-9ce6-43d3-a83a-ef31506a4a0f" />

---

### Step 4: Removing Preinstalled Applications (Debloating)
- Used PowerShell to list installed UWP applications:
- Removed non-essential apps:
- Verified removal and ensured essential system apps remained intact
<img width="1118" height="839" alt="image" src="https://github.com/user-attachments/assets/991f2039-56e2-4dae-be98-ec267db43d79" />
<img width="1629" height="886" alt="image" src="https://github.com/user-attachments/assets/151e9bed-56e6-4041-ace3-6c80bdd03b4d" />

---

## Step 5: Startup Program Optimization
- Reviewed startup applications using Task Manager
- Disabled unnecessary startup programs
- Reduced boot-time load
<img width="802" height="454" alt="image" src="https://github.com/user-attachments/assets/5b725a42-5d6b-4ab3-b994-f54d6902adc6" />

---

## Step 6: Windows Service Optimization

### Objective
- Identified non-essential services using services.msc
- Changed startup type for selected services to Manual or Disabled
- Ensured critical system services remained untouched

### Services Modified
- **Connected User Experiences and Telemetry (Diagnostic Tracking Service)** – Disabled  
- **Windows Search** (optional) – Set to Manual or Disabled    

### Result
- Reduced background service activity
- Improved overall system responsiveness
<img width="1040" height="587" alt="image" src="https://github.com/user-attachments/assets/19b30e2f-3070-4d24-bf21-5477d7d37236" />
<img width="1040" height="588" alt="image" src="https://github.com/user-attachments/assets/eb012d21-b9f5-43ca-b1ed-1f289d6f3ebe" />

---

## Step 7: Scheduled Task Cleanup
- Opened Task Scheduler
- Disabled unnecessary telemetry and data collection tasks
- Reduced background task execution
<img width="779" height="656" alt="image" src="https://github.com/user-attachments/assets/8e668250-3102-4899-9ba2-c6b1c8666a61" />

---

## Step 8: Performance & Visual Tweaks
- Opened **System Properties → Performance Options**
- Disabled unnecessary animations and visual effects
- Applied **High Performance** power plan

### Result
- Faster UI response
- Improved system performance, especially on startup and multitasking
<img width="836" height="603" alt="image" src="https://github.com/user-attachments/assets/46874558-e78a-4502-ba5c-b45dba6702a2" />
<img width="1059" height="349" alt="image" src="https://github.com/user-attachments/assets/e3eb599b-2a9d-4ed6-ae2d-7df7ac72741d" />

---

## Step 9: Storage & Memory Optimization
- Performed Disk Cleanup
- Cleared temporary files
- Verified reduced disk usage
<img width="464" height="455" alt="image" src="https://github.com/user-attachments/assets/0a367f0f-990c-407c-a861-1bbb1d7629a4" />
<img width="1121" height="635" alt="image" src="https://github.com/user-attachments/assets/f4b71ad6-7fe2-4274-be87-72d474662414" />

---

## Step 10: Privacy & Telemetry Reduction
- Disabled advertising ID and tracking features
- Limited diagnostic data collection via Windows Settings
- Applied registry-based telemetry restrictions
<img width="1386" height="908" alt="image" src="https://github.com/user-attachments/assets/bdaa09cc-8ab9-4d37-82b5-271fe1e18418" />

## Step 11: Final Results & Before/After Comparison
- After applying all optimizations (bloatware removal via PowerShell, disabling non-essential services, cleaning up scheduled tasks/telemetry, and any additional tweaks like privacy settings or startup management), here's the impact on system performance.
<img width="1022" height="762" alt="image" src="https://github.com/user-attachments/assets/59f0dc84-c238-4909-9f6c-424a3f6984dd" />
<img width="1031" height="765" alt="image" src="https://github.com/user-attachments/assets/092efd0d-d0f9-41fa-bf79-0e945e11fe52" />

---

### Before Optimization : 
Before: ~9% CPU, 149 processes, small spikes visible*

### After Optimization :  
After: 2% CPU, only 57 processes, ultra-flat graphs*


#### Summary
- Process count dropped by over 60%, directly from removing bloat and disabling telemetry/maintenance tasks — this reduces context switching and minor CPU wake-ups.
- CPU utilization is now consistently lower at idle, with almost no spikes.
- Memory stayed impressively low (2.3 GB idle is top-tier for Windows 11 with 32 GB total).
- On high-end hardware like the Ryzen 9800X3D, the system feels "overkill smooth" — perfect for gaming/productivity with zero background interference.
- Trade-offs: None noticeable in daily use; lost features (e.g., some UWP apps, full telemetry) were intentional and replaced with alternatives where needed.



