# Acadamic-Research-Agentic-Banking-Assistant
An AI-powered banking assistant built using LangGraph, Groq LLM, and SQLite. The assistant can handle banking queries such as account balance checks, transaction history, mini statements, and fund transfers using agentic tool calling.

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
