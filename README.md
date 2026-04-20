🛡️ AI-ML Security DFIR Lab
🔍 Overview

This project documents a Digital Forensics and Incident Response (DFIR) investigation enhanced with AI/ML techniques. It shows how machine learning can help in log analysis, anomaly detection, timeline reconstruction, and evidence extraction during a cyber incident.



🎯 Objective
🧑‍💻 Investigate a simulated breach in a corporate environment (RobbCo case study)
🐧 Use Linux forensic tools and logs to reconstruct attacker activity
🤖 Apply AI/ML scripts for anomaly detection and classification
🧠 Validate AI outputs with human forensic analysis


🧰 Tools & Technologies
🐧 Linux (Ubuntu forensic environment)
💻 Bash / Shell utilities
🐍 Python 3
📊 Scikit-learn
📁 Log tools: grep, cat, find, ls
🤖 Scripts:
classify_logs.py
file_anomalies.py
🔎 Investigation Workflow

1. Initial Access
📜 Checked /var/log/auth.log
🚨 Found suspicious login attempts
🎣 Phishing via .ods file
2. Evidence Collection
📂 Analyzed /tmp/ files
👤 Checked /home/j.morgan/ activity
🔑 Reviewed .bash_history


4. Privilege Escalation
🧑‍💻 SSH key injected into r.house
🔓 Unauthorized access confirmed

6. Persistence
🕵️ Reverse shells found
🌐 Hidden monitoring tool (sysmon)



8. Data Exfiltration
📦 Archive found in /dev/shm/
💾 Source code stolen
🧠 AI Role
📊 Log classification
🚨 Anomaly detection
🧩 Behaviour analysis
⏱️ Timeline reconstruction
⚠️ Limitations
📉 AI is probabilistic, not deterministic
❗ False positives exist
🧑 Human validation required
🔍 Explainability is limited
🏁 Conclusion

AI speeds up DFIR investigations but cannot replace human analysts. It should be used as an assistive tool, not a final authority.
