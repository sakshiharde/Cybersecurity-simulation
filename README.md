# 🚨 Cybersecurity Intrusion Detection & Log Analysis
Machine-Learning & Rule-Based Threat Detection | SOC-Style Analysis

This project analyzes network session logs and builds a hybrid rule-based + ML intrusion detection system to detect malicious activities such as:

Brute-force login attempts

Off-hour unauthorized access

Suspicious IP behavior

High-risk traffic and anomaly patterns

The goal is to simulate real-world SOC workflows and identify threats using security analytics and machine-learning techniques.

📁 Dataset Overview

Dataset Fields Used:

Feature	Description
session_id	Unique session identifier
network_packet_size	Amount of data transferred in session
protocol_type	Network protocol used (HTTP/HTTPS/FTP etc)
login_attempts	Total login attempts in session
session_duration	Duration of session
encryption_used	Whether encryption was used
ip_reputation_score	Threat score of source IP
failed_logins	Failed login attempts
browser_type	Browser used
unusual_time_access	Off-hour access flag
attack_detected	Target label (1 = attack)

Dataset Size: 9,537 sessions

🎯 Objectives

Analyze login and network behavior to detect anomalies

Identify indicators of compromise (IOCs)

Build predictive ML model to classify attack vs normal session

Create explainable cyber insights & attack patterns

Validate results with SOC-style alerting logic

🔍 Key Insights
Behavior	Cyber Interpretation
High failed logins	Brute-force attack attempt
High login attempts	Credential stuffing
High IP reputation score	Known malicious source
No encryption	Potential MITM / risky request
Off-hours login	Suspicious account behavior
Large packet size	Possible data exfiltration
🧠 Machine Learning
Model Used

Random Forest (class-weighted) to handle imbalance

Result
Metric	Value
Accuracy	0.88 ✅
Focus	Recall & Precision for attack class

Accuracy alone isn't enough in security — high recall ensures attacks aren't missed.

Key Features Identified

failed_logins

login_attempts

ip_reputation_score

unusual_time_access

network_packet_size
