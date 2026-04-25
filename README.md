# Fintech_AI
This is a multi agent web based application called Fintech AI

Project Structure:
ai_finance_assistant/ 
├── src/ 
│   ├── agents/ 
│   ├── core/ 
│   ├── data/ 
│   ├── rag/ 
│   ├── web_app/ 
│   ├── utils/ 
│   └── workflow/ 
├── tests/
├── config.yaml 
├── requirements.txt 
└── README.md 

Tech Stack to use:
- Streamlit for UI
- Python for backend
- LangGraph, LangChain for AI agents
- other necessary Python libraries

Goals
 - the web application, when started, would load a chat based user interface. User sends query from chat box to the backend and the response will be displayed back in a typical chat based application style.
 - user query is sent to the backend system. The query is received by a Router Agent. This agent is an orchestrator and based on the user query it will identify which Agent should be processing the query.
 - There are 3 agents:
	1. Finance Q&A Agent: Handles general financial education queries 
	2. Portfolio Analysis Agent: Reviews and analyzes user portfolios 
	3. Market Analysis Agent: Provides real-time market insights 
 - each agent will have real-time web based tools to search for any financial information to process the user query.
 - when response is displayed to the user in the chat interface it should displayed both response message, agent used and the sources it used to process the query.