Features
Interactive Knowledge Base Management
Add URLs dynamically for web content
Default knowledge source: MCP vs A2A Protocol article
Persistent vector database storage using LanceDB
Session state tracking prevents duplicate URL loading
Transparent Reasoning Process
Real-time display of the agent's thinking steps
Side-by-side view of reasoning and final answer
Clear visibility into the RAG process
Advanced RAG Capabilities
Vector search using OpenAI embeddings for semantic matching
Source attribution with citations
Agent Configuration
Gemini 2.5 Flash for language processing
OpenAI embedding model for vector search
ReasoningTools for step-by-step analysis
Customizable agent instructions
Default knowledge source: MCP vs A2A Protocol article
Prerequisites
You'll need the following API keys:

Google API Key
Sign up at aistudio.google.com
Navigate to API Keys section
Create a new API key
OpenAI API Key
Sign up at platform.openai.com
Navigate to API Keys section
Generate a new API key
How to Run
Clone the Repository:

git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
cd rag_tutorials/agentic_rag_with_reasoning
Install the dependencies:

pip install -r requirements.txt
Run the Application:

streamlit run rag_reasoning_agent.py
Configure API Keys:

Enter your Google API key in the first field
Enter your OpenAI API key in the second field
Both keys are required for the app to function
Use the Application:
Default Knowledge Source: The app comes pre-loaded with the MCP vs A2A Protocol article
Add Knowledge Sources: Use the sidebar to add URLs to your knowledge base
Suggested Prompts: Click the prompt buttons (What is MCP?, MCP vs A2A, Agent Communication) for quick questions
Ask Questions: Enter queries in the main input field
View Reasoning: Watch the agent's thought process unfold in real-time in the left panel
Get Answers: Receive comprehensive responses with source citations in the right panel
How It Works
The application uses a sophisticated RAG pipeline with Agno v2.0:

Knowledge Base Setup
Documents are loaded from URLs using Agno's Knowledge class
Text is automatically chunked and embedded using OpenAI's embedding model
Vectors are stored in LanceDB for efficient retrieval
Vector search enables semantic matching for relevant information
URLs are tracked in session state to prevent duplicate loading
Agent Processing
User queries trigger the agent's reasoning process
ReasoningTools help the agent think step-by-step
The agent searches the knowledge base for relevant information
Gemini 2.5 Flash generates comprehensive answers with citations
Streaming events provide real-time updates on reasoning and content
UI Flow
Enter API keys → Knowledge base loads with default MCP vs A2A article → Use suggested prompts or ask custom questions
Reasoning process displayed in left panel, answer generation in right panel
Sources cited for transparency and verification
All events streamed in real-time for better user experience
