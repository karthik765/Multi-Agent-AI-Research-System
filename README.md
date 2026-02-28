Deep Research: Multi-Agent AI Research System
This repository hosts a sophisticated multi-agent system designed to automate the entire research lifecycle—from initial planning and web searching to comprehensive report writing and automated email delivery. The system coordinates several specialized AI agents to ensure high-density information gathering and professional synthesis.

🚀 System Workflow
The ResearchManager acts as the central nervous system, orchestrating the following asynchronous pipeline:

Search Planning: The PlannerAgent breaks down a complex query into a strategic set of web search terms to ensure breadth and depth.

Information Gathering: The SearchAgent executes live web searches, stripping away "fluff" to create concise, information-dense summaries.

Synthesis & Reporting: The WriterAgent consumes the gathered data to produce a detailed, 1000+ word professional report in Markdown format.

Automated Delivery: The EmailAgent converts the final report into a clean HTML format and dispatches it via the SendGrid API.

Interactive Interface: A Gradio-powered UI allows users to trigger research tasks and track the "trace" of the AI's logic in real-time.

🛠️ Technical Stack
Core Orchestration: Python with asyncio for high-performance, concurrent agent execution.

Large Language Model: Powered by OpenAI GPT-4o-mini for efficient reasoning and text generation.

Web Interface: Gradio for a responsive, sky-themed user experience.

Infrastructure & Tools:

Pydantic: For strict data validation and structured agent outputs.

SendGrid: For reliable automated email delivery.

Dotenv: For secure management of API keys and environmental variables.

📦 Project Structure
deep_research.py: The entry point for the Gradio web application.

research_manager.py: The primary class coordinating the agent interactions.

planner_agent.py: Defines search strategies and reasoning steps.

search_agent.py: Handles web search tool integration and summarization.

writer_agent.py: Manages the generation of structured, long-form reports.

email_agent.py: Manages HTML conversion and SendGrid communication.

📈 Future Enhancements
Vector Database Support: Integrating RAG (Retrieval-Augmented Generation) for long-term memory.

Multi-Source Search: Expanding beyond standard web searches to include academic papers or specific news APIs.

Interactive Editing: Allowing users to modify the search plan before the agents begin data collection.
