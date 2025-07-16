# OSINT-AI Investigator

**OSINT-AI Investigator** is an extensible open-source intelligence (OSINT) tool powered by AI. It aggregates publicly available information about individuals or organizations based on input such as email addresses, usernames, names, or domains. The system performs data collection from multiple open sources and generates a comprehensive AI-powered summary report.

This tool is designed for cybersecurity professionals, researchers, and hobbyists who seek to automate reconnaissance and risk profiling in a legal, ethical, and modular manner.

---

## Key Features

- Input types supported: email, username, name, domain
- Data collection from multiple OSINT sources:
  - Breached account data (HaveIBeenPwned)
  - Email reputation (EmailRep.io)
  - GitHub profile and activity (GitHub API)
  - Public social media traces (snscrape: X, Reddit, Instagram)
  - Domain ownership and metadata (WHOIS, crt.sh)
  - Device and server discovery (Shodan API)
- AI-generated summary using GPT-4 or local LLM
- Output as JSON or natural language report (Markdown, PDF-ready)
- Easy-to-use REST API interface via FastAPI
- Modular codebase for easy customization and extension

---

## Sample Use Case

1. A user inputs an email address or username.
2. The system queries OSINT sources such as:
   - HaveIBeenPwned (data breach history)
   - EmailRep.io (reputation and risk flags)
   - GitHub (matching accounts, bio, repos)
   - snscrape (posts and profiles on X, Reddit, etc.)
   - WHOIS or Shodan (for associated domains or IPs)
3. Collected data is compiled and passed to a language model (LLM).
4. An AI-generated summary is returned along with raw data and risk indicators.

---

## Roadmap

- [ ] Export reports to PDF and Markdown
- [ ] Add support for facial reverse search (PimEyes/clearbit style)
- [ ] Graph visualization of relationships (Maltego-style)
- [ ] Integration with SpiderFoot or theHarvester
- [ ] Support for domain mutation (e.g. dnstwist)
- [ ] CLI tool version
