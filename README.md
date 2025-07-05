# n8n-serpai
Of course! Here is a README.md file based on the provided n8n project image.

n8n AI Agent with SerpAPI & Calculator

This n8n project demonstrates how to build a powerful and extensible conversational AI agent. The agent can understand user queries in a chat interface, use external tools to fetch real-time information or perform calculations, and maintain conversation history to provide contextual responses.

The example in the screenshot shows the agent responding to a query about the weather in Toronto by using the SerpAPI tool to look up the live forecast.

Key Features

Conversational Interface: Start the workflow and interact with it through a simple chat UI.

LLM-Powered Core: Leverages an OpenAI Chat Model as the "brain" for natural language understanding and response generation.

Tool Usage: The agent is equipped with tools to extend its capabilities beyond its training data.

SerpAPI: To search the web for real-time, up-to-date information (e.g., weather, news, stock prices).

Calculator: To perform mathematical calculations.

Conversation Memory: Utilizes a Simple Memory node to remember previous parts of the conversation, allowing for contextual follow-up questions.

Extensible: Easily add more tools to the AI Agent to give it new abilities.

Workflow Breakdown

When chat message received (Trigger): This trigger node initiates the workflow whenever a user sends a message in the chat panel. It captures the user's input.

AI Agent: This is the central orchestrator of the workflow. It receives the user's message from the trigger and decides the best course of action. It coordinates between the language model, memory, and the available tools.

OpenAI Chat Model: Connected to the Chat Model input of the agent, this node acts as the "brain". It processes the user's query, determines their intent, and formulates the final text response.

Simple Memory: Connected to the Memory input, this node stores the history of the chat session. This allows the agent to understand context from previous messages.

SerpAPI & Calculator (Tools): These nodes are connected to the Tool input of the agent. The agent can choose to use one of these tools if the user's query requires it. For example, it will use SerpAPI for a question about current events and Calculator for a math problem.

Nodes Used

When chat message received

AI Agent

OpenAI Chat Model

Simple Memory

SerpAPI

Calculator

Prerequisites

To run this workflow, you will need:

An active n8n instance.

OpenAI API Credentials: You must configure the OpenAI Chat Model node with your API key.

SerpAPI API Credentials: You must configure the SerpAPI node with your API key.

How to Use

Import the workflow into your n8n instance.

Set up your credentials for the OpenAI Chat Model and SerpAPI nodes.

Activate the workflow using the "Inactive" toggle at the top of the screen.

Open the chat interface by clicking on the When chat message received node.

Start asking questions!

Example Queries:

what is the weather forecast for tomorrow in Toronto?

What is the capital of Australia?

what is 125 multiplied by 42?
![Screenshot 2025-07-05 234620](https://github.com/user-attachments/assets/224835ee-13e0-4cc8-b1e5-b5eaef95206e)


