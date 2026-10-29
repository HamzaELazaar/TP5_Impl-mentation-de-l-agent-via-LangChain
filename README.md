# Agentic AI with LangChain & LangGraph

A hands-on notebook exploring AI agents using LangChain, LangGraph, and Ollama.

---

## Table of Contents

1. [Overview](#overview)
2. [Objectives](#objectives)
3. [Concepts Covered](#concepts-covered)
4. [Technologies](#technologies)
5. [Tools Implemented](#tools-implemented)
6. [Project Structure](#project-structure)
7. [Prerequisites](#prerequisites)
8. [Installation](#installation)
9. [Configuration](#configuration)
10. [Usage](#usage)
11. [Example Usage](#example-usage)
12. [Security](#security)
13. [Troubleshooting](#troubleshooting)
14. [Author](#author)
15. [License](#license)

---

## Overview

This project is an educational Jupyter Notebook that demonstrates how to build an **AI agent** using **LangChain**, **LangGraph**, and a locally hosted **Ollama** language model.

The notebook walks through the complete lifecycle of an agentic system: defining custom tools, connecting a local language model, letting the agent reason and select the appropriate tool for a given user request, and persisting conversation state across sessions using PostgreSQL checkpointing.

The project is designed for learning purposes and relies on demonstration data for its tools. It can be extended to connect to real APIs and data sources.

---

## Objectives

The main goals of this project are:

- Understand how modern AI agents differ from simple LLM calls.
- Learn how to define custom tools with the `@tool` decorator.
- Observe how an agent autonomously selects a tool based on user intent.
- Practice stateful conversation management using LangGraph.
- Persist agent memory using PostgreSQL checkpointing.
- Run everything locally with Ollama (no external API keys required).

---

## Concepts Covered

| Concept | Description |
|---|---|
| AI Agents | Building reasoning agents with LangChain |
| Custom Tools | Defining tools with the `@tool` decorator |
| Tool Calling | Agent-driven execution of tools |
| Local LLM | Ollama-hosted model (e.g., `llama3`, `mistral`) |
| State Management | LangGraph conversation state |
| Persistence | PostgreSQL checkpointing |
| Configuration | Loading environment variables with `python-dotenv` |

---

## Technologies

- **Python 3.10+**
- **LangChain** — Agent framework
- **LangGraph** — Stateful agent orchestration
- **Ollama** — Local LLM runtime
- **PostgreSQL** — Checkpoint persistence
- **Jupyter Notebook** — Interactive development environment
- **python-dotenv** — Environment variable management

---

## Tools Implemented

The agent has access to three custom tools:

| Tool | Purpose | Data Source |
|---|---|---|
| Search | Returns sample news-search results | Demonstration data |
| Weather | Returns weather information for a city | Demonstration data |
| Employee Information | Returns sample employee records | Demonstration data |

> Note: The search, weather, and employee tools use demonstration data unless connected to real data sources.

---

## Project Structure
