# Day 3 – ScamShield: AI Scam & Phishing Detection Agent

## Project Overview
Day 3 focuses on improving ScamShield using LangChain and Groq. The goal is to organize the AI interaction using prompt templates, conversation history, output parsers, and basic agent functionality.

ScamShield helps users understand potentially fraudulent messages and provides safety recommendations.

## Technologies Used
- Python
- Google Colab
- LangChain
- LangChain-Groq
- Groq API
- CSV

## Concepts Implemented

### 1. LangChain Integration
Installed and imported LangChain and LangChain-Groq to connect the Groq language model with the application.

### 2. LLM Initialization
Initialized the Groq language model using `ChatGroq` and configured it with the selected model and temperature.

### 3. Chat Prompt Template
Created a structured prompt using `ChatPromptTemplate` to define ScamShield's role, rules, and expected responses.

### 4. Conversation History
Used `MessagesPlaceholder` to maintain previous user and assistant messages. This allows ScamShield to remember relevant details during a conversation.

### 5. Output Parser
Used `StrOutputParser` to convert the model response into a readable string.

### 6. LangChain Chain
Connected the prompt, language model, and output parser using the LangChain pipeline:

`Prompt → LLM → Output Parser`

Used `chain.invoke()` to send user messages for analysis.

### 7. CSV-Based Testing
Created a CSV test dataset containing sample questions and expected keywords.

Implemented a test function to:
- Read test cases from a CSV file.
- Send each test message to ScamShield.
- Compare the response with the expected keyword.
- Display PASS or FAIL results.

### 8. Basic Agent Implementation
Used LangChain's `create_agent` to create a basic ScamShield agent with a system prompt.

This demonstrates the basic agent structure. The current version does not use external tools for live URL reputation checks.

## Sample Test Cases
- Identify a suspicious electricity disconnection message.
- Analyze a message claiming a lottery prize.
- Detect requests for ATM PIN or OTP details.
- Distinguish ordinary informational messages from suspicious messages.
- Provide safety recommendations for potentially fraudulent messages.

## Learning Outcomes
- Understood the fundamentals of LangChain.
- Learned how to initialize an LLM using ChatGroq.
- Created reusable prompt templates.
- Implemented conversation history.
- Built an LLM processing chain.
- Tested AI responses using CSV test cases.
- Explored basic agent creation using LangChain.

## Future Improvements
- Integrate URL reputation checking using a threat-intelligence API.
- Add a user-friendly interface.
- Support analysis of email, SMS, and WhatsApp message text.
- Improve scam classification and testing with a larger dataset.
- Generate detailed scam analysis reports.


