# ScamShield – AI Scam & Phishing Detection Agent

## Overview

ScamShield is an AI-powered cybersecurity assistant that analyzes
SMS, WhatsApp messages, and emails to identify potential scams
and phishing attempts.

It uses an LLM, Python tools, URL reputation checking, and
structured output to explain suspicious messages and recommend
safety actions.

## Features

- Scam and phishing message analysis
- Suspicious language and urgency detection
- Automatic URL extraction
- URLhaus malware URL reputation checking
- Safe, Suspicious, and Dangerous classifications
- Explanation of suspicious signals
- Practical safety recommendations
- Pydantic structured output
- Google Sheets analysis logging
- Agent-based tool calling

## Technology Stack

- Python
- Google Colab
- LangChain
- Groq LLM
- Pydantic
- Requests
- URLhaus API
- Google Sheets API
- Pandas

## Project Workflow

1. User provides a message.
2. ScamShield extracts suspicious URLs.
3. URLs are checked against URLhaus.
4. The AI analyzes message content and suspicious signals.
5. Pydantic validates the analysis structure.
6. ScamShield returns a risk assessment and recommendations.
7. Analysis can be saved to Google Sheets when requested.

