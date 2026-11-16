Claude API Foundations

Overview

This repository contains a collection of hands-on projects exploring core Claude API capabilities in Python.

The projects were developed as practical exercises in conversational AI, prompt evaluation, structured outputs, tool use, web search, text editing, extended thinking, and prompt caching.

Together, they demonstrate a progression from basic API interaction to more structured and tool-enabled AI workflows.

Projects Included

1. Multi-Turn Conversation Context

File: Multi-Turn Conversation Context with the Claude API.ipynb

Explores how conversational context is preserved across multiple turns when working with the Claude API.

Key concepts:

Message history

User and assistant roles

Context preservation

Multi-turn interaction patterns

API-based conversation management

2. Structured Topic Extraction

File: Structured Topic Extraction with Prompt Evaluation.ipynb

Demonstrates structured information extraction from text using Claude.

Key concepts:

Structured outputs

Prompt design

Topic extraction

Output consistency

Evaluation of model responses

3. End-to-End Prompt Evaluation

File: End-to-End Prompt Evaluation for Athlete Meal Planning.ipynb

Builds a complete prompt-evaluation workflow using multiple test cases and an LLM-based grader.

The workflow:

Defines test cases

Generates model responses

Scores each response against solution criteria

Calculates average performance and pass rate

Produces a human-readable evaluation report

The final evaluation included three test cases and achieved:

Average score: 9.3/10

Pass rate: 100%

Test scores: 9/10, 9/10, and 10/10

Supporting report: Prompt_Evaluation_Report.pdf

This project demonstrates how AI outputs can be evaluated systematically rather than reviewed only subjectively.

4. Tool Use Workflow

File: Claude_Tool_Use_Date_Time_v1.ipynb

Demonstrates Claude tool use through custom Python functions.

Example capabilities include:

Retrieving date and time information

Performing duration calculations

Storing reminders

Handling multi-step tool execution

Returning tool results to the model

This project illustrates how Claude can interact with external functions instead of relying only on text generation.

5. Text Editor Tool

File: Claude_Text_Editor_Tool_v1.ipynb

Explores AI-assisted file editing and text manipulation.

Key concepts:

Reading text-based files

Editing file contents

Applying targeted changes

Tool-based interaction with local documents

Structured editing workflows

This project demonstrates how language models can support document and code-editing tasks through controlled tools.

6. Web Search Tool

File: Claude_Web_Search_Tool_v1.ipynb

Demonstrates web-enabled Claude workflows.

Key concepts:

Search-assisted responses

External information retrieval

Tool invocation

Search-result integration

Combining model reasoning with retrieved information

This project explores how AI systems can extend beyond static model knowledge by retrieving outside information.

7. Prompt Caching and Tool Schemas

File: Claude_Prompt_Caching_Tool_Schemas_v1.ipynb

Explores prompt caching and structured tool schemas.

Key concepts:

Reusing repeated prompt context

Tool schema design

Structured function definitions

Reducing unnecessary repeated context

More efficient API workflows

This project demonstrates how prompt structure and caching strategies can improve reusable AI workflows.

8. Extended Thinking

File: Claude_Extended_Thinking_Blocks_v1.ipynb

Explores Claude's extended reasoning capabilities.

Key concepts:

More complex reasoning tasks

Extended thinking blocks

Separating final answers from deeper reasoning processes

API handling of reasoning-enabled responses

This project demonstrates how extended reasoning can support more complex analytical tasks.

Technologies Used

Python

Jupyter Notebook

Anthropic Claude API

anthropic Python SDK

python-dotenv

JSON

HTML report generation

Tool schemas and function calling

API Key Handling

API credentials are loaded from environment variables using python-dotenv.

Example:

from dotenv import load_dotenv
import os

load_dotenv()

print(bool(os.getenv("ANTHROPIC_API_KEY")))

API keys are not stored directly in the notebooks.

A local .env file may be used during development, but it should never be committed to source control.

Repository Purpose

This repository is intended to demonstrate practical experience with:

Claude API integration

Prompt engineering

Multi-turn conversational systems

Structured outputs

Prompt evaluation

Tool use

Web-enabled AI workflows

File-editing workflows

Prompt caching

Extended reasoning

Human-readable AI evaluation reporting

The projects emphasize applied experimentation and workflow design rather than production deployment.

Notes

These projects were developed for learning, experimentation, and portfolio demonstration.

Some model outputs may vary slightly between runs because generative AI systems are nondeterministic.

The prompt-evaluation project intentionally demonstrates this by scoring outputs across multiple test cases and producing a structured evaluation report.

Future Expansion

Potential future additions include:

Fine-grained tool streaming

Additional structured-output workflows

More advanced tool orchestration

Expanded automated evaluation

Agentic workflows

Production-oriented error handling

Logging and observability

Status

Current status: Complete portfolio collection

The repository currently includes eight completed Claude API projects covering foundational and intermediate AI application patterns.

These projects serve as the foundation for later work involving retrieval-augmented generation, multimodal AI, code execution, MCP integration, and agentic workflows.
