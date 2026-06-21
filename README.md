# Acadamic-Research-Agentic-Banking-Assistant
An AI-powered banking assistant built using LangGraph, Groq LLM, and SQLite. The assistant can handle banking queries such as account balance checks, transaction history, mini statements, and fund transfers using agentic tool calling.

## LLM used:

This project uses the `openai/gpt-oss-120b` model hosted through Groq API for natural language understanding, reasoning, and agentic tool execution.

## Environment Setup

Set your Groq API key as:

GROQ_API_KEY

Do not hardcode API keys in the notebook.

## Objectives:
Understand how Agentic AI can automate core banking operations
Design tool-based systems for LLM interaction with structured data
Build agents that interpret user queries and invoke appropriate tools
Develop orchestration workflows between agents, tools, and databases
Implement secure transaction handling with basic validations
Generate structured outputs such as mini statements
Handle filtered queries like debit/credit transaction views
Add post-processing guardrail
Test and validate the system using real-world scenarios

## Problem Statement:
Banks and financial institutions handle a large volume of customer requests related to account information, transactions, and fund transfers. These interactions are often initiated through chat, mobile apps, or support channels and involve repetitive yet critical operations.

Currently, many banking support processes are manual, fragmented, and query-driven, leading to several challenges:

Delayed response times for customer requests
Inconsistent handling of similar queries across channels
Over-reliance on human intervention for routine operations
Limited ability to process natural language queries efficiently
Lack of seamless integration between user interactions and backend systems
A significant portion of customer requests typically falls into the following categories:

Information retrieval, such as checking account balance or viewing transactions
Transaction operations, such as transferring funds between accounts
Filtered queries, such as viewing only debit or credit transactions
Statement generation, such as requesting a mini statement of recent activities
However, most existing systems lack the capability to:

Automatically understand and interpret user queries from natural language inputs
Dynamically select and execute appropriate backend operations (tools)
Provide consistent, accurate, and real-time responses
Seamlessly integrate conversational AI with structured banking data
The goal is to design and develop an AI-Based Agentic Banking System that can:

Interpret user queries and map them to appropriate banking operations
Enable intelligent agents to interact with tools for balance checks, transactions, and transfers
Support filtered views of transaction data (debit/credit)
Generate structured outputs such as mini statements
Provide a unified, automated, and efficient banking assistance experience

## Workflow Diagram:

<img width="569" height="256" alt="image" src="https://github.com/user-attachments/assets/d8982699-8c57-4ca8-ac71-fbd77608fb6c" />

## SQLite Database Tables:
SQLite is a C library that provides a lightweight disk-based database that doesn't require a separate server process and allows accessing the database using a nonstandard variant of the SQL query language. Some applications can use SQLite for internal data storage.

SQLite3 specifically refers to the third version of SQLite.
Design a structured database to support all banking operations and tool interactions.

CUSTOMERS: Stores basic customer details such as customer ID, name, and contact information (email).

ACCOUNTS: Maintains account-specific data including account ID, linked customer ID, and current balance.

TRANSACTIONS: Records all debit and credit transactions with details like transaction ID, account ID, amount, type, and timestamp.

These tables enable efficient data retrieval, transaction processing, and support all agent-driven banking functionalities.

## Designing Tools:
1. Design and implement all the necessary backend tools (functions/APIs) required to support banking operations.

2. This includes creating tools for balance checking, viewing transactions, transferring funds, filtering debit/credit transactions, and generating mini statements.

3. Ensure that each tool interacts correctly with the underlying database and includes essential validations such as sufficient balance checks and valid beneficiary handling.

4. The focus is on building reliable, reusable, and well-structured tools that can be invoked by the agent during execution.

## Building Agent, Testing, & Gradio Implementation
1. Design and implement the agent orchestration workflow to handle user queries and invoke appropriate tools dynamically.

2. This includes building an intelligent agent capable of interpreting user intent, selecting the correct tool, managing multi-step operations (such as validation before transfer), and formatting responses.

3. Also, test the complete system using sample user queries to validate accuracy, correctness, and robustness of the workflow.

4. Ensure the system handles edge cases such as insufficient balance, invalid inputs, and unsupported queries effectively, providing a smooth and reliable user experience.
