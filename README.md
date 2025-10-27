🧾 Digital Forensics File Analyzer
🔍 A Python-based tool for file integrity verification using MD5 & SHA256 hashing
🧠 Overview

The Digital Forensics File Analyzer is a Python-based project that automates file integrity verification.
It scans folders, computes MD5 and SHA256 hashes for every file, and logs all results into a SQLite database and a CSV report.

This project demonstrates real-world digital forensics techniques and Python automation used in cybersecurity investigations.

⚙️ Features

✅ Recursively scans folders for all files
✅ Calculates MD5 and SHA-256 cryptographic hashes
✅ Stores analysis results in SQLite3 database
✅ Exports a clean CSV forensic report
✅ Records file size and timestamp automatically
✅ Demonstrates integration of hashing, databases, and Python scripting — key for cybersecurity & forensic analysis

🧰 Tech Stack
Component	Tool / Technology
Language	Python 3
Operating System	Kali Linux / Windows
Database	SQLite3
Libraries Used	hashlib, os, sqlite3, datetime, csv
Output Format	CSV + PDF
🧩 Project Structure
Digital-Forensics-File-Analyzer/
│
├── create_db.py                         # Creates SQLite database & table
├── file_analyzer.py                     # Main file analyzer script
├── forensics.db                         # SQLite database storing file records
├── forensic_report.csv                  # Generated forensic report (exported)
├── test_files/                          # Sample files used for analysis
│   ├── file1.txt
│   └── file2.txt
├── README.md                            # Project documentation (this file)
└── Digital_Forensics_Project_Report.pdf  # Professional project report (final)

🚀 Usage
1️⃣ Setup

Clone the repository and navigate to the project folder:

git clone https://github.com/sanjana06-dotcom/Digital-Forensics-File-Analyzer.git
cd Digital-Forensics-File-Analyzer

2️⃣ Create Database
python3 create_db.py

3️⃣ Run the Analyzer
python3 file_analyzer.py


When prompted, enter the folder path to analyze, for example:

/home/sanjana/ForensicsFileAnalyzer/test_files

4️⃣ View Results
🔹 In Database:
sqlite3 forensics.db
.mode column
.headers on
SELECT * FROM file_analysis;

🔹 In CSV File:
cat forensic_report.csv

🔹 In Excel:

Open forensic_report.csv → Format as table → Export as Forensic_Report.pdf for submission.

🧾 Sample Output
id	file_name	file_path	md5_hash	sha256_hash	file_size	analysis_time
1	file2.txt	/home/sanjana/.../file2.txt	91672565...	8bbac61b...	30	2025-10-27 17:24:10
2	file1.txt	/home/sanjana/.../file1.txt	5d5776f4...	9acd6f78...	22	2025-10-27 17:24:10
🧠 Learnings & Skills Demonstrated

Digital Forensics Fundamentals

File Integrity Verification

Hashing Algorithms (MD5, SHA256)

Python Scripting & File Handling

Database Management using SQLite3

Report Generation (CSV, Excel, PDF)

📘 Documentation

📄 Download Full Project Report (PDF): "https://github.com/sanjana06-dotcom/Digital-Forensics-File-Analyzer/blob/main/Digital_Forensics_Project_Report.pdf"

👩‍💻 Author

Sanjana S
💼 Cybersecurity & Digital Forensics Enthusiast
🔗 LinkedIn Profile: "https://www.linkedin.com/in/sanjana-s-05b041302" 

📧 Add your email or contact if you wish

⭐ Contribute / Support

If you find this project useful:

⭐ Give it a star on GitHub

🔀 Fork it and build your own version

💬 Share it with other cybersecurity learners
