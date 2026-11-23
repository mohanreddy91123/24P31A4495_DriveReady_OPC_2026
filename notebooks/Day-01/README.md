# Day 1 – Introduction to AutoCare AI

## Project Overview

AutoCare AI is an AI-powered Vehicle Service Management Assistant designed to help car, bike and scooter owners with vehicle maintenance information, service enquiries and appointment assistance.

## Topics Covered

- Groq API Integration
- LangChain and ChatGroq
- LLM Initialization using GPT-OSS 120B
- System Prompt Engineering
- Building a Basic AI Chatbot
- Testing Customer Queries
- Prompt Injection
- Prompt Guard Demonstration

## Implementation

- Connected the Groq API using Google Colab Secrets.
- Initialized the GPT-OSS 120B language model using ChatGroq.
- Created a custom system prompt for AutoCare AI.
- Developed the `ask()` function to interact with the chatbot.
- Tested vehicle maintenance and service-related questions.
- Tested safety-related queries, including unusual brake noises.
- Tested service booking and pricing enquiries.
- Implemented a Prompt Guard demonstration to detect potentially malicious prompts.

## Safety Features

- Does not provide confirmed mechanical diagnoses.
- Recommends consulting a qualified mechanic for serious vehicle problems.
- Avoids inventing service prices.
- Does not guarantee appointment availability without a booking integration.
- Uses Prompt Guard as an additional prompt-injection detection layer.

## Technologies Used

- Python
- Google Colab
- LangChain
- Groq API
- GPT-OSS 120B
- Meta Llama Prompt Guard 2 (22M)

## Current Limitations

- Real-time appointment booking is not yet integrated.
- Vehicle maintenance recommendations are general and should be checked against the manufacturer's service schedule.
- Customer database and automated reminders are planned for future development.

## Status

**Day 1 – Completed.**
