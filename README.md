# Conversational Recommendation Systems: Integrating RAG with NLP for Context-Aware Recommendations

This project is all about helping people find movies or series just by describing what they're in the mood to watch. Instead of choosing from genres or categories, users can type in a short description — like “a light-hearted rom-com set in Europe” — and the system will try to suggest something that fits.

#### Project Goal
The main aim here is to build a smarter recommendation system that can understand what someone really wants to watch — even when the input is vague. To make that happen, the system uses Natural Language Processing (NLP) and a method called Retrieval-Augmented Generation (RAG).
This can be really useful for streaming platforms or shopping websites where understanding the user's intent is important.

### Tools & Technologies
    - Natural Language Processing (NLP)
    - RAG (Retrieval-Augmented Generation)
    - Langchain – A framework for building NLP applications
    - Groq API – Used to access Mixtral LLM Model
    - Pandas – For data handling and preprocessing
    - Wikipedia / Google / Wikidata – As sources to retrieve context

### How It Works
1. Langchain Framework
    - Used to build the core structure and workflow of the language model.
2. Tool Creation
    - Tools like Wikipedia, Google, and Wikidata are added to help fetch relevant information based on user input.
3. Agent Development
    - An agent is created that reads the user’s query and selects the right tool to collect supporting content.
4. API Integration
    - The system connects to the Groq platform to access the Mixtral LLM Model, which processes the data.
5. RAG-Based Query Handling
    - The agent passes the collected context to the model, which then generates recommendations based on that specific query.

### Skills Used
- Pandas for organizing and preparing data
- Langchain for building the recommendation pipeline
- API integration to use external language models
- RAG technique to improve the quality of results
- Tool and Agent creation to dynamically fetch and process user queries

### Example Use Case
If a user types:
"Looking for a thriller series with intense storylines, similar to Breaking Bad."
The system will search related information, find matching titles, and recommend a list of series based on this description.

### Future Improvements
- Add user feedback to improve recommendations
- Expand tool sources (e.g., TMDb, IMDb APIs)
- Include multiple languages for broader support
