# OSINT-AI Investigator

**OSINT-AI Investigator** is a lightweight tool for collecting open-source intelligence (OSINT) about email addresses and generating an AI-powered summary report. It integrates popular OSINT sources such as HaveIBeenPwned and EmailRep with a language model (OpenAI GPT or local LLM) to deliver a concise risk profile and insight.

---

## Features

- Query data breaches from HaveIBeenPwned
- Check reputation of email addresses via EmailRep
- Generate risk summaries using AI (e.g., GPT-4 or local LLM)
- Simple REST API interface (FastAPI)
- Modular, extensible architecture

---

## Use Cases

- Cybersecurity reconnaissance
- Personal threat assessment
- Red/blue team tooling
- Enrichment for automated alert systems
- OSINT portfolio project

---

## Technologies

- Python 3.10+
- FastAPI
- httpx (for async HTTP requests)
- OpenAI API or local LLM
- Pydantic
- dotenv

---

## Installation

```bash
git clone https://github.com/your-username/osint-ai-investigator.git
cd osint-ai-investigator
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
