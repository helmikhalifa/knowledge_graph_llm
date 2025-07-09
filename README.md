# knowledge_graph_llm

🧠✨ Knowledge Graph from Text using Google's Gemini LLM
This project demonstrates how to build a knowledge graph from a given text using Large Language Models (LLMs), specifically Google's Gemini, and visualize it. This can be a foundational step for developing a RAG (Retrieval-Augmented Generation) Agent. 🤖

🖼️ Demo
Below is a visualization of the knowledge graph generated from a text about Mr Bean (Wikipedia: https://en.wikipedia.org/wiki/Mr._Bean). The graph is interactive, and you can explore the relationships between different entities. 🌐

A snapshot of the interactive knowledge graph visualization from gemini_knowledge_graph.html.

⚙️ How it Works
The process of generating the knowledge graph is detailed in the knowledge_graph.ipynb notebook and involves the following steps:

💻 Installation of Libraries: The necessary Python libraries such as langchain, langchain-google-genai, python-dotenv, pyvis, and google-generativeai are installed.

🔑 API Key Setup: Your Google AI Studio API key for Gemini is required. The notebook loads the key from a .env file for security.

🤖 LLM Instantiation: A Gemini model (e.g., "gemini-2.5-pro") is instantiated using ChatGoogleGenerativeAI from the langchain_google_genai library.

📈 Graph Data Extraction: The LLMGraphTransformer is used to process the input text and extract entities (nodes) and their relationships (edges) to form a graph structure.

📊 Graph Visualization: The extracted graph data is visualized using the pyvis library, creating an interactive HTML file (gemini_knowledge_graph.html) that allows for exploration of the knowledge graph.

🚀 Getting Started
To run this project yourself, follow these steps:

Clone the repository:

Bash

git clone https://github.com/helmikhalifa/knowledge_graph_llm.git
cd knowledge_graph_llm
Install the dependencies:

Bash

pip install --upgrade langchain langchain-experimental langchain-google-genai python-dotenv pyvis google-generativeai
Set up your API Key:

Create a .env file in the root directory.

Add your Google AI Studio API key to the .env file:

GOOGLE_API_KEY="YOUR_GEMINI_API_KEY"
▶️ Run the Jupyter Notebook:

Open and run the knowledge_graph.ipynb notebook to generate your own knowledge graph from a text of your choice.

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.
