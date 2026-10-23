# SOC L1 Phishing Email Triage Lab

### Alert Received
A user reported suspicious email: "Your account will be closed!"

### 1. What I Checked
- **Email Header:** SPF = FAIL, Reply-To different from From
- **Suspicious Link:** http://secure-login-verify-01.com
- **VirusTotal:** 8/92 engines flagged as phishing
- **AbuseIPDB:** IP 192.168.100.5 reported 45 times for phishing

### 2. My Verdict
**CONFIRMED MALICIOUS - Phishing Attempt**

### 3. What I Did (SOC L1 Response)
1. Blocked the malicious domain on firewall
2. Told user to delete email and not click
3. Reset user's password
4. Created ticket: INC-2026-001
5. Added IOC to blacklist

### 4. Tools I Used
Wireshark, VirusTotal, AbuseIPDB, Email Header Analyzer

### 5. Skills Shown
Log analysis, IOC extraction, OSINT, Incident Response Documentation

---
**Analyst:** Norman Emongais | SOC L1 | Busia, Kenya
