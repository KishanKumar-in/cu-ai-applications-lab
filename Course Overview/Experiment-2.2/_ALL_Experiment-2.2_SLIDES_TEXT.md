# Experiment-2.2 - All Lecture Slides Text


## Exp 2.2
### Slide 1
- UNIVERSITY INSTITUTE OF
- ENGINEERING
- DEPARTMENT OF ENGINEERING FOUNDATION-2
- PROGRAM
- NAME
- :
- Bachelor
- of Engineering
- SPECIALIZATION
- :
- COMPUTER SCIENCE & ENGINEERING
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 2                   Experiment No.2.2
- Topic
- : Understanding Azure Machine Learning, Generative AI Models, and AI Agent
- Systems
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- To understand the basic concept of Generative Artificial Intelligence and its role in creating new content
- .
- To
- learn the meaning of prompts and understand the difference between system prompts and user prompts
- .
- To
- understand the basic working of Large Language Models, including tokens,
- embedding's,
- transformers, and attention
- .
- To
- explore the concept of Retrieval Augmented Generation and how it improves AI responses
- .

### Slide 3
- Recap
- of Previous Experiment
- Artificial Intelligence enables machines to perform intelligent tasks such as learning, reasoning, decision-making, understanding language, and solving real-world problems.
- Generative AI, NLP, Speech AI, Computer Vision, and OCR help machines create content, process text, understand voice, analyze images, and extract useful information from documents.
- Responsible AI ensures that AI systems are developed and used in a safe, fair, transparent, secure, inclusive, and ethical manner.

### Slide 4
- Topic 1. Generative Artificial
- Intelligence
- Topic 2. Prompts and Prompt
- Types
- Topic 3. Large Language
- Models
- Topic 4. Retrieval Augmented
- Generation
- Topic 5. AI Agents
- Figure-1 :
- Introduction to Generative AI
- Source :
- https://cogentinfo.com/resources/the-role-of-generative-
- ai
- -in-the-modern-workplace#
- Introduction to Generative AI

### Slide 5
- Figure-2:Generative Artificial Intelligence
- Source:
- https://www.webcluesinfotech.com/what-is-generative-ai-everything-you-need-to-know/
- Generative Artificial Intelligence
- Generative Artificial Intelligence is a branch of artificial intelligence that can create new content such as text, images, audio, video, summaries, stories, poems, and computer code
- .
- It is called “generative” because it generates new output based on the input provided by the user
- .
- It
- is widely used in education, business, research, programming, customer support, and content creation.

### Slide 6
- A prompt is the input given to a Generative AI model to receive a response
- .
- A prompt can be a question, command, instruction, statement, or casual message
- .
- A
- clear and specific prompt helps the model generate better and more accurate responses
- .
- Example of a simple prompt:
- Explain Artificial Intelligence in simple words.
- Example of a better prompt:
- Explain Artificial Intelligence in five simple points for beginner-level students.
- Figure-3
- :Prompt Engineering
- Source:
- https://www.linkedin.com/pulse/what-prompt-engineering-why-useful-generative-ai-models-cloudkitect-hbldc/
- Prompts in Generative AI

### Slide 7
- There are two main types of prompts in Generative AI:
- System Prompt:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>A system prompt defines the behavior, role, tone, and rules of the AI model. It is usually written by the application developer.
- Example:
- You are a helpful assistant. Explain all answers in simple and friendly language.
- User Prompt:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>A user prompt is the actual question or instruction given by the user.
- Example:
- Summarize the topic of AI agents in simple language.
- Figure-4
- :Types of Prompts
- Source:
- https://hatchworks.com/blog/gen-
- ai
- /generative-
- ai
- -prompt-guide/
- Types of Prompts

### Slide 8
- A Large Language Model, also called an LLM, is the core technology behind many Generative AI systems
- .
- They
- generate responses by predicting the next most suitable word or token based on the given prompt
- .
- For
- example, if the input is:
- I heard a dog...
- The model may predict:
- bark
- This happens because the model has learned that dogs commonly bark.
- Figure-5
- :Large Language Models
- Source:
- https://otrs.com/blog/
- ai
- -automation/large-language-models-
- llms
- /
- Large Language Models

### Slide 9
- Tokenization is the process of breaking text into smaller units called tokens.
- Tokens may be complete words, parts of words, punctuation marks, or characters.
- Example:
- Sentence:
- I heard a dog bark loudly.
- Tokens:
- I, heard, a, dog, bark,
- loudly
- After
- tokenization, tokens are converted into numerical vectors called
- embedding's.
- Embedding's
- help the model understand the meaning and relationship between words
- .
- For example, the words
- dog
- ,
- puppy
- , and
- cat
- may be closer in meaning than
- dog
- and
- car
- .
- Figure-6
- :Tokenization and Embedding's
- Source:
- https://airbyte.com/data-engineering-resources/tokenization-
- vs
- -
- embeddings
- Tokenization and
- Embedding's

### Slide 10
- A
- transformer helps the model understand relationships between tokens in a sentence
- .
- The transformer uses a technique called attention.
- Attention helps the model focus on important words in the input
- .
- For example, in the sentence:
- I heard a dog bark
- The words
- heard
- and
- dog
- are important for understanding the word
- bark
- .
- Because of attention, the model can understand context and generate meaningful responses.
- Figure-7 :Attention
- Mechanism
- Source:
- https://www.linkedin.com/pulse/attention-mechanism-secret-behind-how-transformers-satishkumar-80cfc/
- Transformer and Attention Mechanism

### Slide 11
- Retrieval Augmented Generation, or RAG, is a technique used to improve AI responses by adding relevant external information.
- In RAG, the AI system first retrieves useful information from documents, databases, emails, websites, or search engines.
- Then the retrieved information is added to the prompt so that the AI model can generate a more accurate answer.
- Example
- :
- User question:
- What is the maximum travel allowance in my company?
- A RAG-based system searches the company policy document and answers using that document.
- Figure-8 :Retrieval Augmented Generation
- Source:
- https://bradsol.com/resources/blogs/retrieval-augmented-generation-rag-for-llms-a-guide-to-enhanced-accuracy-and-trust/
- Retrieval Augmented Generation

### Slide 12
- AI agents are software applications built using Generative AI.
- They can understand instructions, reason over information, use tools, and perform actions
- .
- For
- example, an AI agent can search information, summarize a document, draft an email, update a calendar, or retrieve data from a database
- .
- AI agents have three main components:
- Large Language Model:
- Acts as the brain of the agent.
- Instructions:
- Define the role, behavior, and rules of the agent.
- Tools:
- Help the agent interact with the world and perform actions.
- Figure-9
- :
- AI Agents
- Source:
- https://builder.aws.com/content/30PvUImLL3LehFlOZpZ5SU6Bavn/agentic-ai-series-part-1-what-are-ai-agents-and-why-do-they-matter
- AI Agents

### Slide 13
- A multi-agent system is a system where multiple AI agents work together to complete complex tasks
- .
- Each agent may have a different role or specialization
- .
- For example:
- One agent may collect data.
- Another agent may analyze the data.
- Another agent may prepare a report.
- Another agent may send the report by email.
- Figure-10 :Multi-Agent Systems
- Source:
- https://www.geeksforgeeks.org/artificial-intelligence/multiagent-planning-in-ai/
- Multi-Agent Systems

### Slide 14
- Summary of the
- Experiment
- Generative AI can create new content such as text, images, audio, video, and code
- .
- Prompts are inputs given to AI models, and better prompts produce better responses
- .
- Large Language Models process language using tokens,
- embedding's,
- transformers, and attention mechanisms
- .
- Retrieval Augmented Generation improves AI responses by retrieving relevant external information
- .

### Slide 15
- Next
- Experiment
- T
- opic(s)
- Topic 1:
- Introduction to Text
- Analysis
- Topic 2:
- Tokenization and Text
- Preprocessing
- Topic 3:
- Statistical Text
- Analysis
- Topic 4:
- Semantic Language Models

### Slide 16
- Quiz/ FAQ’s
- What is Generative AI
- ?
- What
- is a prompt
- ?
- What
- is the difference between a system prompt and a user prompt
- ?
- What
- is a Large Language Model
- ?
- What
- is tokenization
- ?
- What
- are
- embedding's?
- What
- is transformer architecture
- ?
- What
- is Retrieval Augmented Generation
- ?

### Slide 17
- R
- eferences/ Articles/ Videos
- Reference / Articles
- Google Cloud – Generative AI Resources
- https://cloud.google.com/ai/generative-ai
- IBM – What is Generative AI?
- https://www.ibm.com/think/topics/generative-ai
- IBM – What is Retrieval Augmented Generation?
- https://www.ibm.com/think/topics/retrieval-augmented-generation
- IBM – What Are AI Agents?
- https://
- www.ibm.com/think/topics/ai-agents
- Videos
- Generative AI Full Course 2026: From LLM Basics to RAG
- https://www.youtube.com/watch?v=ofGKKLVTM9o
- Learn RAG From Scratch – Python AI Tutorial
- https://www.youtube.com/watch?v=sVcwVQRHIc8

### Slide 18
- Additional
- learning
- R
- esources
- Additional Resources for Learning Generative AI
- https://www.skills.google/course_templates/536
- https://
- www.coursera.org/learn/introduction-to-generative-ai
- Additional Resources for Learning RAG and AI Agents
- https://www.ibm.com/think/topics/retrieval-augmented-generation
- https://
- www.ibm.com/think/topics/ai-agents
- Additional Resources for Prompt Engineering
- https://github.com/dair-ai/Prompt-Engineering-Guide

### Slide 19
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 20
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in
