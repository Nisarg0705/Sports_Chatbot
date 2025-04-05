# Sports_Chatbot
# pathway
ML Hackathon (Pathway)
Libraries used:
1.	libmagic
2.	openai==1.68.2
3.	langgraph 
4.	langchain-community 
5.	langchainhub 
6.	pathway[all]
7.	os
8.	langchain_core.prompts
9.	langchain_core.pydantic_v1
10.	langchain_openai
11.	typing
12.	time
13.	json
14.	pydantic
15.	pathway
16.	langchain_community.vectorstores
17.	pathway.xpacks.llm.vector_store
18.	patway.xpacks.llm
19.	pathway.udfs
20.	warnings
21.	re
22.	urllib.parse
23.	langchain_community.document_loaders
24.	requerts
25.	openai
26.	bs4
27.	pandas
28.	pathway
29.	pathway.stdlib.indexing
30.	pathway.stdlib.indexing.bm25
31.	pathway.xpacks.llm.document_store
32.	pathway.xpacks.llm.question_answering
33.	langchain_community.vectorstores
34.	langchain
35.	langchain_core.output_parsers
36.	typing_extensions
37.	langgraph.graph
38.	gradio
39.	difflib
40.	langchain_openai
41.	langchain_core.prompts



**Requirements to be followed:
1. Please run the google colab on Edge microsoft.
2. If the code does not work then kindly check the Internal testing code block.
3. Before running the code please enter all your api keys.
4. Pleases wait at least 3-4 minutes for the reponse to generate.
5. Also the UI is made at the end of the code once you run on colab.
**   





Code Explanation:
1.	Library Installation and Setup:
o	All required libraries are installed and upgraded as needed.
o	Necessary dependencies for web scraping, API calls, and large language models (LLMs) are ensured to be available.
2.	Environment Configuration:
o	The operating system environment is set up.
o	API keys for OpenAI, Google API (GOOGLE_API_KEY), and CX_ID for Google Search are configured.
3.	Webpage Content Scraping with LangChain:
o	A Python script is developed to scrape and store webpage content using the LangChain library.
4.	Server Configuration:
o	Pathway host and port are assigned for hosting services.
5.	Search Query Refinement:
o	User-provided queries are refined to improve accuracy and efficiency.
o	Social media results are filtered out to focus on relevant web searches.
o	ChatGPT is utilized to transform natural language queries into concise and precise search queries.
6.	Fetching Search Results via Google API:
o	The Google Search API fetches results based on the refined query.
o	Time restrictions and filtering conditions are applied.
o	The google_search function retrieves relevant links and snippets and does the web scrapping.
7.	Retrieval-Augmented Generation (RAG) Pipeline Implementation:
o	A RAG pipeline is built using LangChain, integrating a retrieval mechanism with ChatGPT to enhance query responses.
8.	Grading Function for Query Evaluation:
o	LangChain and ChatGPT evaluate user queries using a binary (“yes” or “no”) system.
o	This helps filter out irrelevant information.
9.	Enhancing RAG for Improved Accuracy:
o	The RAG model is further refined to improve the accuracy of responses by incorporating relevant retrieved information.
10.	Hallucination Detection in LLM Responses:
o	A function is developed to assess whether the LLM’s response contains relevant or fabricated information.
11.	Sufficiency Assessment for LLM Responses:
o	The adequacy of the LLM’s response is evaluated using GPT-based grading.
12.	Query Rewriting for Improved Retrieval:
o	A query rewriting function enhances search accuracy and retrieval efficiency for vector-based searches.
13.	GraphState Definition for Structured Outputs:
o	A GraphState ensures that dictionary keys follow a specific format for structured and consistent responses.
o	
14.	Answer Generation via GPT:
o	The refined query is processed by GPT to generate the required response. Also the user is asked if they require commentary or not.
15.	Query Feasibility Check for AI Responses:
o	A function determines whether AI can answer the query.
o	If the query pertains to events before October 2023, the system responds with “yes”; otherwise, it proceeds differently.
o	
16.	Decision-Making for LLM vs. Web Scraping:
o	A function determines whether to rely on LLM-generated responses or perform data scraping based on the nature of the query.
17.	Comprehensive RAG Pipeline for Query Handling:
o	The final RAG pipeline is structured to handle:
	Data Scraping & Creation
	Document Retrieval
	Query Transformation
	Answer Generation
	Hallucination & Relevance Grading
18.	Workflow Nodes for Query-Based Decision-Making:
o	LangGraph-based workflow nodes are added for efficient decision-making.
19.	Integration with Web Scraper API:
o	If a query requires scraping, it is processed through scraperapi, and the extracted text is returned.
20.	Input Processing & Result Generation:
o	User inputs are processed, and relevant results are generated.
21.	LLM Agent for Sports Commentary Summarization:
o	The LLM agent processes a text file containing sports updates and generates a summary using GPT.
22.	Web Scraping of Live Commentary:
o	A Python script scrapes sports commentary from a given URL and saves the extracted data.
23.	Real-Time Commentary Updates:
o	The commentary is updated periodically to reflect the latest developments.
24.	User Interface (UI) with Gradio:
o	A UI is developed using Gradio to enable user interaction.
o	The system takes user input and generates the required output dynamically.

This structured pipeline ensures efficient search, retrieval, and response generation while minimizing misinformation and maximizing relevance.



Advantage of our solution:
1.The existing framework of OpenAI we have bettered it by using GoogleSearch Engine + RAG and OpenAI.
2.The commentry features works well and to ask for it the user needs to ask the query about live commentry in a particular match.
3.Giving correct up to date results (example if user asks RCB net run rate then 2.137 but the actual is 2.26 which is provided by our code). 
4.Getting information of any debut player is difficult to receive by using api key calling but in our case it is giving correct info.  






