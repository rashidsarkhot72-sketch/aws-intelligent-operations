\# ⚙️ AWS Intelligent Operations



\## Incident Monitoring \& Auto-Remediation Dashboard



AWS Intelligent Operations is a self-built cloud operations project that demonstrates \*\*EC2 monitoring, incident detection, automated remediation, SNS notifications, and operational dashboarding\*\*.



The project is designed around a common cloud operations use case: detecting high CPU utilization on an EC2 instance and triggering an automated response.



\---



\## 🎯 Objective



The main objective of this project is to build a simple AWS operations monitoring system that can:



\- Monitor EC2 infrastructure

\- Detect high CPU incidents

\- Track incidents

\- Trigger automated EC2 remediation

\- Send notifications through SNS

\- Display CPU usage and incident history on a dashboard



\---



\## 🏗️ AWS Services Used



| AWS Service | Purpose |

|---|---|

| Amazon EC2 | Runs the monitored server |

| Amazon CloudWatch | Monitors EC2 CPU utilization |

| AWS Lambda | Handles automation and remediation logic |

| Amazon SNS | Sends incident notifications |

| Amazon API Gateway | Provides APIs for dashboard data |

| IAM | Controls permissions between AWS services |

| HTML / JavaScript | Builds the monitoring dashboard |



\---



\## 🔄 Project Workflow



```text

EC2 Server

&#x20;   ↓

CloudWatch Monitoring

&#x20;   ↓

High CPU Detected

&#x20;   ↓

Incident Detection

&#x20;   ↓

Auto-Remediation

&#x20;   ↓

EC2 Reboot Initiated

&#x20;   ↓

SNS Notification

&#x20;   ↓

Dashboard



📊 Dashboard



The dashboard provides visibility into:



EC2 server status

CloudWatch monitoring status

Auto-remediation status

SNS notification status

Total incidents

Detected incidents

Auto-remediated incidents

Current CPU utilization

CPU usage history

70% critical CPU threshold

Recent incident history

🚨 CPU Monitoring



The dashboard displays EC2 CPU utilization using a 0–100% scale.



A red dashed line represents the:



Critical CPU Threshold = 70%



This makes it easy to identify when CPU utilization reaches the configured critical monitoring level.



🔧 Auto-Remediation



When a high-CPU incident is detected, the automation workflow can initiate an EC2 reboot as the remediation action.



The dashboard records the incident and displays the remediation status.



Example:



High CPU

&#x20;  ↓

Incident Detected

&#x20;  ↓

Remediation Triggered

&#x20;  ↓

EC2 Reboot Initiated

🔔 Notifications



Amazon SNS is used as part of the incident notification workflow.



This allows operational alerts to be sent when infrastructure incidents occur.



🖥️ Dashboard Screenshot



The dashboard shows the current system health, CPU monitoring information, and recent incidents.



Screenshots are available in the screenshots folder.



📁 Project Structure

aws-intelligent-operations/

│

├── index.html

├── README.md

├── .gitignore

│

└── screenshots/

&#x20;   ├── 01-dashboard-overview.png

&#x20;   └── 02-cpu-monitoring-70-threshold.png

🚀 How to Run

1\. Clone the repository

git clone https://github.com/rashidsarkhot72-sketch/aws-intelligent-operations.git

2\. Open the project

cd aws-intelligent-operations

3\. Open the dashboard



Open:



index.html



in a web browser.



The dashboard connects to the configured API Gateway endpoints to retrieve incident and CPU information.



🔐 Security



The project uses AWS IAM permissions for service access.



Sensitive credentials, API keys, environment files, and local configuration files should not be committed to GitHub.



The .gitignore file is included to prevent common sensitive or unnecessary files from being committed.



📚 Key Learnings



Through this project, I practiced:



AWS EC2 monitoring

Amazon CloudWatch

AWS Lambda automation

Amazon SNS notifications

API Gateway integration

IAM permissions

Incident management

Automated remediation

CPU monitoring

Dashboard development

Git and GitHub project documentation

💼 Real-World Relevance



This project demonstrates concepts commonly used in cloud operations, infrastructure monitoring, incident management, automation, and production support environments.



It is a self-built project inspired by real-world AWS cloud operations use cases.



👨‍💻 Author



Rashid Sarkhot

