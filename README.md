# AI-Powered Recipe & Nutrition Research Assistant

## Overview
This project is an autonomous multi-agent system designed to act as a comprehensive culinary research team. Instead of a simple recipe search, the application orchestrates a team of AI "specialists"—including a Recipe Developer, a Nutritionist, and a Dietary Specialist.

Using **LangGraph**, the system manages the state between these agents as they:
1.  **Analyze** a requested food topic.
2.  **Generate** specific questions based on their persona.
3.  **Research** the web using Tavily and Wikipedia to find real-time data.
4.  **Synthesize** their findings into a coherent report.
5.  **Visualize** the results in a beautiful, Colab-friendly HTML dashboard.

## Reason for picking up this project
This project was chosen to demonstrate the advanced capabilities of **LangGraph** in managing complex, stateful workflows. It directly aligns with the course curriculum by implementing:

* **LangGraph (State, Nodes, Edges):** To manage the workflow between the Analyst generation phase and the Interview phase.
* **Structured Output:** Using Pydantic models to ensure the LLM generates strictly formatted personas and search queries.
* **Tool Calling & Semantic Search:** Integrating `TavilySearch` and `WikipediaLoader` to ground the AI's responses in factual, external data (RAG).
* **Prompt Engineering:** Designing distinct system prompts for different agent personas (e.g., the tone of a Nutritionist vs. a Chef).

This project solves the problem of "hallucinated recipes" by enforcing a research-first approach, verifying ingredients and facts against web sources before generating the final guide.

## Video Summary Link
[PASTE YOUR YOUTUBE/DRIVE LINK HERE]

## Plan
I plan to execute these steps to complete my project:

* [DONE] **Step 1:** Set up the environment, API keys (OpenAI, Tavily), and define the Pydantic data models for the Food Analysts.
* [DONE] **Step 2:** Create the `GenerateAnalystsState` graph to dynamically create expert personas based on the user's topic.
* [DONE] **Step 3:** Implement the `InterviewState` graph to handle the cyclical process of asking questions and generating search queries.
* [DONE] **Step 4:** Integrate Web Search tools (Tavily & Wikipedia) to provide context for the agents' answers.
* [DONE] **Step 5:** Develop the Reporting engine to compile individual agent interviews into a final comprehensive guide.
* [DONE] **Step 6:** Create a custom HTML rendering engine to display the results as a styled dashboard within the notebook.

  
