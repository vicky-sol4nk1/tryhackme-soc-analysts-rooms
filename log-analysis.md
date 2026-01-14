

### 1. What Are Logs? (Core Concept)
- Logs = **Digital footprints** or records of events/activities in systems, applications, networks, and security devices.
- They capture **who**, **what**, **when**, **where**, and **how** something happened.
- Essential for: Monitoring, Detection, Investigation, Forensics, Compliance, Threat Hunting, Incident Response.

### 2. Why Logs Matter in SOC (L1 Role)
- Detect anomalies / malicious behavior early
- Investigate alerts & incidents
- Hunt for threats proactively
- Meet regulatory requirements (GDPR, PCI-DSS, etc.)
- Correlate events across sources in SIEM
- Reconstruct attack timeline (attack chain)

### 3. Common Types of Logs (Most Important for L1 SOC)
- **System Logs** — OS-level events (Windows Event Logs: System, Application, Security)
- **Security Logs** — Authentication, privilege use, policy changes (e.g., Event ID 4624 = successful login)
- **Application Logs** — App-specific events/errors (e.g., IIS, SQL Server)
- **Firewall Logs** — Allowed/denied connections, rules triggered
- **Web Server Logs** — HTTP requests (access logs), errors (e.g., Apache/Nginx/IIS)
- **Authentication Logs** — Login success/failure (e.g., RDP, VPN, AD)
- **DNS Logs** — Queries/responses → detect C2, data exfil, tunneling
- **Email Logs** — Sent/received, spam/phishing attempts
- **Proxy Logs** — Web browsing activity (e.g., URLs, categories, bytes transferred)
- **Cloud Logs** — AWS CloudTrail, Azure Activity Logs, GCP Audit Logs

### 4. Log Formats (Common Ones You’ll See)
- **Syslog** — Standard format (RFC 5424), used by Linux/network devices (priority, facility, message)
- **JSON** — Structured, easy to parse (modern SIEM favorite)
- **CEF** (Common Event Format) — ArcSight standard, key-value pairs
- **LEF** — Log Event Format (some vendors)
- **Plain Text** — Unstructured (older apps)
- **CSV** — Comma-separated (exported logs)
- **Windows Event Logs** — .evtx binary format (use Event Viewer or PowerShell to read)

### 5. Log Management & Tools (Demo Focus: Loggly)
- **Loggly** (cloud-based log management & analytics by SolarWinds)
  - Collect logs from many sources (agents, syslog forwarding, API)
  - Search using keywords, fields, wildcards
  - Filter by time, source IP, event ID, user, etc.
  - Create **dashboards** for real-time monitoring
  - Set up **alerts** (e.g., notify on multiple failed logins)
  - Visualize trends (e.g., login spikes)


Watch previous days (1–10) in the playlist for foundational topics (networking, OS basics, threats, etc.). Day 11 builds toward SIEM & monitoring in later sessions.

If you want notes expanded on a specific part (e.g., more on Event IDs, Loggly queries, or comparison with Splunk/ELK), let me know! Keep grinding — you're on Day 11 of becoming an L1 SOC pro. 💪
