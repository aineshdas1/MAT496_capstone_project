# AI-Powered Recipe & Nutrition Research Assistant

## Overview
This project is an autonomous multi-agent system designed to act as a comprehensive culinary research team. Instead of a simple recipe search, the application orchestrates a team of AI "specialists"—including a Recipe Developer, a Nutritionist, and a Dietary Specialist.

Using LangGraph, the system manages the state between these agents as they:
1.  Analyze a requested food topic.
2.  Generate specific questions based on their persona.
3.  Research the web using Tavily and Wikipedia to find real-time data.
4.  Synthesize their findings into a coherent report.
5.  Visualize the results in a beautiful, Colab-friendly HTML dashboard.

## Reason for picking up this project
This project was chosen to demonstrate the advanced capabilities of **LangGraph** in managing complex, stateful workflows. It directly aligns with the course curriculum by implementing:

* LangGraph (State, Nodes, Edges): To manage the workflow between the Analyst generation phase and the Interview phase.
* Structured Output: Using Pydantic models to ensure the LLM generates strictly formatted personas and search queries.
* Tool Calling & Semantic Search: Integrating `TavilySearch` and `WikipediaLoader` to ground the AI's responses in factual, external data (RAG).
* Prompt Engineering: Designing distinct system prompts for different agent personas (e.g., the tone of a Nutritionist vs. a Chef).

This project solves the problem of "hallucinated recipes" by enforcing a research-first approach, verifying ingredients and facts against web sources before generating the final guide.

## Video Summary Link

Here is the google drive link of the video summary:


video: https://drive.google.com/file/d/1VQVrIj7tS1LPdQbh3jsT4_v-3eEKe2WV/view?usp=sharing

## Plan
I plan to execute these steps to complete my project:

* [DONE] Step 1: Project initialization: Set up dependencies (LangGraph, Tavily), API environment, and imports.
* [DONE] Step 2: Define Data Structures: Create Pydantic models for `FoodAnalyst` personas and `GraphState` management.
* [DONE] Step 3: Agent Development (Analyst Creator): Build the node responsible for generating specific culinary personas based on user input.
* [DONE] Step 4: Tool Integration: Implement `TavilySearch` and `WikipediaLoader` tools and the logic for generating search queries.
* [DONE] Step 5: Graph Logic (Interview Loop): Construct the core `StateGraph` that manages the cycle of questioning, searching, and answering.
* [DONE] Step 6: Reporting Engine: Implement the logic to synthesize distinct agent interviews into a cohesive final guide.
* [DONE] Step 7: Visualization: Develop a Colab-compatible HTML dashboard to render the final output and research statistics.
* [DONE] Step 8: Final Integration & Delivery: Compile all components into a single, executable `recipe_nutrition_analyst.ipynb` notebook and verified functionality.


## Conclusion
I had planned to achieve a system that could autonomously research and present complex food data. I think I have achieved the conclusion satisfactorily. 

The agent successfully breaks down a broad topic (like "Margherita Pizza") into specific sub-domains, gathers factual information from the web, and presents it in a structured format with citations. The addition of the HTML dashboard makes the output user-friendly and visually appealing, demonstrating that LangGraph can be used to build polished, end-to-end applications.
  
