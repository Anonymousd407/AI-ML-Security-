# AI-ML-Security-
🛡️ AI Forensics DFIR Lab Notes
🔍 Overview

This project documents a practical Digital Forensics and Incident Response (DFIR) investigation enhanced with AI/ML techniques. It demonstrates how machine learning models can assist in log analysis, anomaly detection, timeline reconstruction, and evidence extraction during a cyber incident.

🎯 Objective
🧑‍💻 Investigate a simulated breach in a corporate environment (RobbCo case study)
🐧 Use Linux forensic tools and logs to reconstruct attacker activity
🤖 Apply AI/ML-assisted scripts for anomaly detection and classification
🧠 Validate AI outputs with human forensic analysis
🧰 Tools & Technologies
🐧 Linux (Ubuntu-based forensic environment)
💻 Bash / Shell utilities
🐍 Python 3
📊 Scikit-learn (machine learning library)
📁 Log analysis tools (grep, cat, find, ls)
🤖 DFIR AI scripts:
classify_logs.py
file_anomalies.py
🔎 Investigation Workflow
1. Initial Access Analysis
📜 Examined /var/log/auth.log
🚨 Identified suspicious login attempts
🎣 Traced phishing-based entry point via malicious .ods file
2. Evidence Collection
📂 Inspected /tmp/ artifacts
👤 Reviewed /home/j.morgan/ user activity
🔑 Analyzed .bash_history for privilege escalation
3. Privilege Escalation
🧑‍💻 Discovered SSH key injection into r.house account
🔓 Confirmed lateral movement via authorized_keys modification
4. Persistence Mechanisms
🕵️ Identified reverse shells (/tmp/.x, /usr/local/bin/sysmon)
🌐 Found disguised monitoring tool with outbound connections
5. Data Exfiltration
📦 Located encoded archive in /dev/shm/
💾 Confirmed stolen proprietary source code and firmware
🧠 AI/ML Role in Investigation
📊 Log classification using supervised ML models
🚨 File anomaly detection using feature-based analysis
🧩 Behavior pattern recognition for suspicious activity
⏱️ Timeline reconstruction support
⚠️ Limitations Observed
📉 AI outputs are probabilistic, not deterministic
❗ False positives in anomaly classification
🧑 Human validation required for all findings
🔍 Explainability remains a challenge in forensic contexts
🏁 Conclusion

This lab demonstrates how AI can significantly accelerate DFIR investigations while reinforcing that human expertise remains essential for validation, legal defensibility, and accurate interpretation of evidenc
