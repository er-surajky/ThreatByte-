# 🔐 CyberGuard — AI-Powered Cyber Threat Intelligence Platform

<p align="center">
  <strong>Automated Threat Detection • AI-Driven Analysis • Real-Time Cyber Intelligence</strong>
</p>

<p align="center">
  Your Digital Shield Against Emerging Cyber Threats.
</p>

---

## 🌐 Overview

**CyberGuard** is an automated Cyber Threat Intelligence (CTI) and incident intelligence platform designed to collect, process, analyze, and distribute emerging cybersecurity threats.

Powered by **NVIDIA NIM AI and Meta Llama 3.1**, CyberGuard transforms raw cybersecurity reports into structured and actionable intelligence. It continuously monitors trusted security sources to identify emerging zero-day vulnerabilities, ransomware campaigns, data breaches, software exploits, and other significant cyber threats.

The platform combines automated intelligence collection, AI-powered threat analysis, severity classification, mitigation recommendations, Telegram notifications, and an interactive web-based intelligence dashboard.

Its goal is to simplify threat monitoring and help cybersecurity enthusiasts, SOC analysts, security researchers, and IT professionals stay informed about the evolving threat landscape.

---

## 🚀 Live Platform & Resources

| Resource | Access |
|---|---|
| 🌐 Intelligence Dashboard | [Launch CyberGuard](https://mukulgrover.github.io/ThreatByte) |
| 🤖 Telegram Intelligence Bot | [@threatbytebot](https://t.me/threatbytebot) |
| 💻 GitHub Repository | [CyberGuard](https://github.com/mukulgrover/ThreatByte) |
| 🧠 AI Intelligence Engine | [NVIDIA NIM](https://build.nvidia.com/) |
| ⚙️ Automation Workflow | [GitHub Actions](https://github.com/mukulgrover/ThreatByte/blob/main/.github/workflows/daily_briefing.yml) |

---

## ✨ Core Features

### 🧠 1. AI-Powered Threat Intelligence

Uses NVIDIA NIM inference APIs with Meta Llama 3.1 models to transform unstructured cybersecurity reports into structured threat intelligence.

- Automated cybersecurity report analysis.
- CVE identifier extraction.
- Threat actor identification when supported by source reporting.
- Technical root-cause analysis.
- Attack vector identification.
- Affected software and technology extraction.
- AI-generated defensive recommendations.
- Structured threat intelligence generation.

### 🔍 2. Multi-Source Threat Intelligence Collection

Collects cybersecurity intelligence from multiple established security publications and threat research sources.

**Integrated Intelligence Sources:**
- BleepingComputer
- The Hacker News
- Krebs on Security
- Dark Reading
- SecurityWeek
- SANS Internet Storm Center

**Collection Capabilities:**
- RSS feed aggregation.
- Automated report extraction.
- 24-hour intelligence filtering.
- Duplicate report detection.
- Source attribution.
- Structured JSON data generation.

### 🛡️ 3. Threat Severity & Risk Classification

Organizes collected intelligence according to its potential security impact.

| Severity | Description |
|---|---|
| 🔴 Critical | Severe vulnerabilities or threats requiring urgent attention |
| 🟠 High | Significant security risks with potentially serious consequences |
| 🟡 Medium | Threats requiring investigation and appropriate mitigation |
| 🟢 Low | Lower-impact security developments |

Where available, CVSS scores and vulnerability identifiers provide additional context for risk assessment.

### 🤖 4. Automated Telegram Intelligence Bot

CyberGuard provides automated cybersecurity briefings through its Telegram bot.

**Bot:** [@threatbytebot](https://t.me/threatbytebot)

Features:
- Automated daily intelligence bulletins.
- Subscriber registration.
- On-demand threat intelligence.
- Daily security updates at 08:00 AM IST.
- HTML-formatted intelligence reports.

**Available Commands:**

| Command | Function |
|---|---|
| `/start` | Initialize the Telegram bot |
| `/today` | Retrieve the latest intelligence bulletin |
| `/subscribe` | Subscribe to daily updates |
| `/help` | Display available commands |

### 🌐 5. Interactive Cyber Threat Intelligence Dashboard

A centralized web portal for exploring the latest cybersecurity intelligence.

**Dashboard Capabilities:**
- Dark-themed editorial interface.
- Latest cybersecurity threat reports.
- Interactive threat intelligence cards.
- CVE-based search functionality.
- Threat categorization and filtering.
- Historical intelligence archives.
- Technical threat summaries.
- Defensive mitigation checklists.
- Original source references.

### ⚙️ 6. Fully Automated Intelligence Pipeline

Uses GitHub Actions to execute scheduled intelligence operations without requiring a continuously running server.

- Scheduled daily execution.
- Automated threat collection.
- AI-based intelligence enrichment.
- JSON report generation.
- Telegram bulletin distribution.
- Historical archive updates.
- Automated repository updates and deployment.

---

## 🏗️ System Architecture

CyberGuard follows a modular intelligence-processing architecture.

```text
                 AUTOMATED SCHEDULER
                   GitHub Actions
                    08:00 AM IST
                         |
                         v
              THREAT INTELLIGENCE INGESTION
              -----------------------------
              BleepingComputer
              The Hacker News
              Krebs on Security
              Dark Reading
              SecurityWeek
              SANS ISC
                         |
                         v
                 DATA PROCESSING
              -----------------------------
              RSS Feed Parsing
              Report Extraction
              24-Hour Filtering
              Duplicate Detection
              Source Attribution
                         |
                         v
                AI THREAT ANALYSIS
              -----------------------------
                 NVIDIA NIM API
                 Meta Llama 3.1
                         |
              +----------+----------+
              |          |          |
              v          v          v
           CVE        SEVERITY    ATTACK
         EXTRACTION  CLASSIFICATION ANALYSIS
              |          |          |
              +----------+----------+
                         |
                         v
                INTELLIGENCE ENGINE
              -----------------------------
              Threat Summarization
              Technical Analysis
              Mitigation Recommendations
              Structured JSON Generation
                         |
              +----------+----------+
              |                     |
              v                     v
        TELEGRAM BOT           WEB DASHBOARD
        Daily Briefings        Threat Reports
        /today Command         CVE Search
        Subscriber Alerts      Historical Archive
```

---

## 🛠️ Technology Stack

| Category | Technology | Purpose |
|---|---|---|
| Programming Language | Python 3.12 | Backend processing and automation |
| AI Infrastructure | NVIDIA NIM | AI inference and threat analysis |
| AI Model | Meta Llama 3.1 | Intelligence enrichment |
| Web Scraping | BeautifulSoup4 | Web content extraction |
| Feed Aggregation | Feedparser | RSS intelligence collection |
| Frontend | HTML5, CSS3 | Dashboard structure and styling |
| Client-Side Logic | JavaScript ES6+ | Dynamic rendering and search |
| Messaging | Telegram Bot API | Intelligence notifications |
| Automation | GitHub Actions | Scheduled pipeline execution |
| Data Storage | JSON | Threat intelligence and archives |
| Hosting | GitHub Pages | Web dashboard deployment |

---

## 📂 Project Structure

```text
CyberGuard/
│
├── .github/
│   └── workflows/
│       └── daily_briefing.yml
│
├── backend/
│   ├── config.py
│   ├── scraper.py
│   ├── ai_enricher.py
│   ├── telegram_bot.py
│   ├── bot_service.py
│   ├── generator.py
│   └── requirements.txt
│
├── data/
│   ├── latest.json
│   ├── archive.json
│   ├── subscribers.json
│   └── daily/
│
├── frontend/
│   ├── index.html
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── app.js
│
├── index.html
├── .env.example
├── LICENSE
└── README.md
```

---

## ⚡ Installation & Configuration

### Prerequisites

- Python 3.12 or later.
- Git.
- NVIDIA NIM API key.
- Telegram Bot Token (optional, for Telegram integration).

### Step 1 — Clone the Repository

```bash
git clone https://github.com/mukulgrover/ThreatByte.git

cd ThreatByte
```

### Step 2 — Install Dependencies

```bash
pip install -r backend/requirements.txt
```

### Step 3 — Configure Environment Variables

Create a `.env` file in the root directory.

```env
NVIDIA_API_KEY=your_nvidia_api_key
TELEGRAM_BOT_TOKEN=your_telegram_bot_token
TELEGRAM_BOT_USERNAME=threatbytebot
SITE_URL=https://mukulgrover.github.io/ThreatByte
```

**Security Notice:** Never upload your `.env` file, API keys, or Telegram bot credentials to a public repository.

### Step 4 — Execute the Intelligence Pipeline

```bash
python backend/generator.py
```

The pipeline performs threat collection, data processing, AI enrichment, and intelligence report generation.

### Step 5 — Launch the Web Dashboard

```bash
python -m http.server 8080
```

Access the dashboard:

```text
http://localhost:8080/frontend/index.html
```

---

## 🔄 Daily Automation Workflow

CyberGuard uses GitHub Actions to automate its intelligence lifecycle.

| Stage | Operation |
|---|---|
| 01 | Scheduled workflow execution |
| 02 | Collect cybersecurity intelligence |
| 03 | Filter recent reports and remove duplicates |
| 04 | Analyze reports using NVIDIA NIM |
| 05 | Extract CVEs, severity, and technical details |
| 06 | Generate actionable intelligence reports |
| 07 | Publish Telegram intelligence bulletins |
| 08 | Update JSON intelligence archives |
| 09 | Update and deploy the web portal |

**Scheduled Execution:** 08:00 AM IST (02:30 UTC).

---

## 🔐 Security & Operational Considerations

CyberGuard follows security-conscious development practices.

- Secure API credential management.
- Environment-based configuration.
- GitHub Actions Secrets for CI/CD credentials.
- Controlled processing of external intelligence feeds.
- Source attribution for collected reports.
- Protection of Telegram subscriber information.
- Independent verification of AI-generated security assessments.

**Disclaimer:** CyberGuard is an informational threat intelligence platform. AI-generated analysis may contain inaccuracies. All vulnerability information, severity assessments, and mitigation recommendations should be independently validated before being used in production security environments.

---

## 🎯 Use Cases

CyberGuard can support several cybersecurity activities:

- **SOC Monitoring:** Stay informed about emerging security threats.
- **Threat Research:** Explore vulnerabilities, exploits, and ransomware campaigns.
- **Vulnerability Awareness:** Track newly reported CVEs and security advisories.
- **Security Operations:** Review actionable defensive recommendations.
- **Cybersecurity Learning:** Understand current attack trends and defensive strategies.
- **Threat Intelligence Monitoring:** Access consolidated security information from multiple sources.

---

## 🔮 Future Enhancements

Potential improvements to expand the platform's threat intelligence capabilities:

- MITRE ATT&CK framework integration.
- Indicators of Compromise (IOC) extraction.
- STIX/TAXII threat intelligence support.
- Automated vulnerability correlation.
- Threat actor campaign tracking.
- SIEM platform integration.
- Advanced threat intelligence visualization.
- Email-based security notifications.
- Historical threat trend analytics.
- Automated intelligence confidence scoring.

---

## 👨‍💻 Author

**Suraj Kumar Yadav**

Cybersecurity Enthusiast | Threat Intelligence | Security Research

- **GitHub:** [@Suraj Kumar Yadav](https://github.com/er-surajky)
- **LinkedIn:** [Suraj Kumar Yadav](linkedin.com/in/suraj-kumar-yadav-5183ba299/)

---

## 📜 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more information.

---

## ⭐ Support & Contributions

If you find CyberGuard useful:

- ⭐ Star the repository.
- 🍴 Fork the project.
- 🐛 Report bugs and issues.
- 💡 Suggest new features.
- 🤝 Contribute improvements.

Contributions from the cybersecurity community are welcome.

---

<p align="center">
  <strong>CYBERGUARD</strong>
  <br>
  <em>Stay Informed. Stay Secure. Stay Ahead.</em>
  <br><br>
  🔐 Automated Intelligence for a Safer Digital World.
</p>
