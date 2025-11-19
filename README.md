# Azure-AI-Foundry — Build an AI Agent with Azure AI Agent Service

A hands-on demonstration showcasing expertise in Azure AI Foundry, Azure AI Agent Service, and Python-driven AI tooling.
This exercise guides users through developing a simple yet powerful AI agent capable of analyzing data and generating charts using the built-in Code Interpreter tool.

📘 Overview

In this exercise, you will:

Create an Azure AI Foundry project

Use the Azure AI Agent Service SDK (Python)

Build an AI Agent that can analyze uploaded data

Use the Code Interpreter tool to dynamically generate Python code

Run statistical calculations and produce text-based charts

Interact with the agent via a stateful thread-based conversation loop

🚀 Key Features

🔹 Azure AI Agent creation with GPT-4o

🔹 Automatic data file upload & handling

🔹 Dynamic Python execution for analytics

🔹 Conversation-thread memory support

🔹 CLI-based interactive agent client

🔹 Full project cleanup instructions included

🏗️ Project Structure
Azure-AI-Foundry/
│
└── Python/
    ├── agent.py               # Main agent application
    ├── data.txt               # Sample dataset
    ├── .env                   # Local environment config
    ├── requirements.txt       # Dependencies

📦 Installation & Setup
1. Clone Repository in Azure Cloud Shell
rm -r ai-agents -f
git clone https://github.com/MicrosoftLearning/mslearn-ai-agents ai-agents

2. Navigate to the Lab Directory
cd ai-agents/Labfiles/02-build-ai-agent/Python
ls -a -l

3. Create Virtual Environment & Install Dependencies
python -m venv labenv
./labenv/bin/Activate.ps1
pip install -r requirements.txt azure-ai-projects azure-ai-agents

4. Configure Environment

Edit .env:

Set your_project_endpoint

Set MODEL_DEPLOYMENT_NAME=gpt-4o


🧠 Building the AI Agent

The workflow includes:

Connecting to Azure AI Foundry using the SDK

Uploading data.txt

Creating a CodeInterpreterTool

Initializing an AI agent with statistical analysis instructions

Creating a thread for interactive chat

Running prompts & viewing responses

Cleaning up the agent and thread

Code snippets include imports, authentication, data upload, agent creation, prompt execution, error handling, message retrieval, and cleanup logic.

▶️ Running the App
1. Sign in to Azure
az login

2. Run the Application
python agent.py

Example prompts:
What's the category with the highest cost?
Create a text-based bar chart showing cost by category
What's the standard deviation of cost?


Enter quit to exit the app.
Afterward, the script outputs the full conversation history.

🧹 Cleanup Instructions

To avoid unnecessary Azure costs:

Open the Azure Portal

Locate the resource group used in this exercise

Select Delete resource group

Confirm deletion

🤝 Contributing

This repository is for demonstration and learning purposes.
Feel free to fork, adapt, or incorporate into your own Azure AI projects.
