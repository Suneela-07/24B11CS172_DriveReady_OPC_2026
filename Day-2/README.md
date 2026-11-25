# Day 2 – ScamShield: AI Scam & Phishing Detection Agent

## Project Overview
ScamShield is an AI-powered scam and phishing message analysis assistant. It analyzes suspicious messages, identifies possible scam indicators, classifies risk levels, and provides safety recommendations.

Day 2 focuses on building the core logic of ScamShield using Python and the Groq API.

## Technologies Used
- Python
- Google Colab
- Groq API
- OpenAI Python Client
- JSON

## Concepts Implemented

### 1. LLM Integration
Connected the Groq API with Python using the OpenAI-compatible client to send messages and receive AI-generated responses.

### 2. System Prompt
Created a system prompt that defines ScamShield's role, responsibilities, analysis rules, and response format.

### 3. JSON Output and Parsing
Configured the AI to return structured JSON containing:
- Suspicious message classification
- Risk level
- Possible scam type
- Suspicious indicators
- Suspicious URLs
- Recommended action

Used Python's `json` module to parse and handle the structured response.

### 4. Conversation History
Implemented conversation history so ScamShield can maintain context during a conversation. Added a limit to retain recent messages.

### 5. Dictionaries and Functions
Used Python dictionaries to organize suspicious keywords and their indicators. Created reusable functions to analyze messages and identify suspicious patterns.

### 6. Decorators
Implemented a logging decorator to track function calls and their results.

### 7. Error Handling
Added exception handling for API-related errors, such as:
- Rate limit errors
- API connection errors
- Authentication errors

### 8. Interactive Chatbot
Combined the implemented features into an interactive ScamShield chatbot that accepts messages and returns AI-based scam analysis.

## Sample Test Messages
1. "Your electricity connection will be disconnected. Pay immediately."
2. "Your Amazon order has been shipped. Track it using the official app."
3. "You have won 10 lakh rupees. Pay a processing fee to claim it."
4. "Your college exam starts at 9 AM tomorrow."
5. "Your ATM card will expire. Share your PIN to renew it."

## Expected Output
ScamShield analyzes each message and provides a classification, risk level, suspicious indicators, and recommended safety action.

## Learning Outcomes
- Learned to integrate an LLM API with Python.
- Understood structured JSON responses and parsing.
- Practiced dictionaries, functions, and decorators.
- Implemented conversation history.
- Learned basic API error handling.
- Built an interactive AI-based cybersecurity chatbot.

## Note
ScamShield provides AI-based message analysis. It does not independently confirm whether a URL is malicious or verify its live reputation unless connected to an external threat-intelligence service.
