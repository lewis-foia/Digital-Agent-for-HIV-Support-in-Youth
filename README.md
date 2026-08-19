# AI-Powered Digital Agent for HIV Support in Youth (Proof-of-Concept)

## Project Overview

This project introduces a compassionate digital assistant designed specifically for young people living with HIV. Beyond just answering questions, this tool serves as a bridge to reliable health information, providing a private and supportive space where users can seek guidance without fear of judgment.

### Why This Matters
For many young people, navigating HIV care can be overwhelming and isolating. This AI agent simplifies that journey by offering instant access to verified medical facts and practical support tools. By making health information conversational and accessible, we aim to empower youth to take charge of their health, improve treatment adherence, and reduce the stigma often associated with seeking help.

## Execution Environment

### Google Colab (Recommended)
This project is optimized to run on **Google Colab**. Using Colab allows you to run the code in the cloud without needing a powerful computer or complex local setups. 

### Local Execution
If you choose to run this project on your own computer, please note that it requires:
*   Specific hardware (a dedicated GPU is recommended for faster processing).
*   Manual installation of all Python libraries and system packages.
*   Proper configuration of your local environment to handle machine learning tasks.

## Group Members

*   Hélio Simango
*   José Fumo
*   Lewis Foia
*   Frenk Muianga

## Setup and Installation

To run this project, you need to install the following dependencies:

```bash
pip install cohere sentence-transformers faiss-cpu
```

## Knowledge Base

The agent relies on a knowledge base derived from `hiv_faq.txt`. This file contains frequently asked questions and answers related to HIV, which are used for retrieval-augmented generation.

## Large Language Model (LLM)

This project uses the Cohere Command A 03 2025 model. You will need a Cohere API key to use the model. Please replace the placeholder in the code with your actual API key.

## Usage

### Ask the Agent

You can interact with the agent by calling the `ask_agent` function to get supportive answers to HIV-related questions.

### Schedule an Appointment

The agent includes a tool to help you remember your next clinic visit:

```python
def schedule_appointment(date):
    return f"Appointment scheduled for {date}. Please remember to attend and bring your treatment records."
```

### Interactive Chat Loop

You can start a live conversation with the bot by running the `chat_loop()` function. Type `quit`, `exit`, or `stop` to end the session.
```
