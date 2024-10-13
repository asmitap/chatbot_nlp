## Chatbot

<p>This project is a chatbot system built using various NLP tools like SpaCy, dateparser, ChromaDB, and TinyLLaMA to extract and generate conversational responses. It can extract dates, validate user information, book appointments, and provide answers based on the loaded document content.</p>

### Features
<ul>
<li>Date Extraction: Extract dates from text using SpaCy and convert them into standard date formats using dateparser and parsedatetime.</li>
<li>User Info Validation: Validate phone numbers and email addresses with regular expressions.</li>
<li>Document Embedding and Querying: Load documents, embed them with SentenceTransformers, and store them in ChromaDB for efficient querying.</li>
<li>Chatbot Response Generation: Use TinyLLaMA model to generate responses for user queries.</li>
<li>Appointment Booking: Automatically book appointments based on user input and natural language date parsing.</li>
</ul>

### Libraries Used
<ul>
<li>SpaCy: For natural language processing and entity recognition.</li>
<li>dateparser: For parsing natural language date expressions.</li>
<li>parsedatetime: For handling date and time conversions.</li>
<li>ChromaDB: For storing document embeddings and querying.</li>
<li>SentenceTransformers: For encoding sentences into embeddings.</li>
<li>TinyLLaMA: For generating text responses.</li>
</ul>

### Installation
<ul>
<li>Clone this repository and install the necessary libraries.</li>
<li>git clone https://github.com/asmitap/chatbot.git</li>
<li>cd chatbot</li>
<li>pip install -r requirements.txt</li>

### Make sure to install the required libraries such as:
<ul>
<li>SpaCy</li>
<li>dateparser</li>
<li>parsedatetime</li>
<li>SentenceTransformers</li>
<li>transformers (TinyLLaMA)</li>
<li>chromadb</li>
<li>re (for regex)</li>

### Load the required SpaCy model:
python -m spacy download en_core_web_sm

### Example Interactions
<br>
You: call me<br>
Please provide your name: John<br>
Please provide your phone number: 9876543210<br>
Please provide your email: john@example.com<br>
Thank you, John. We will call you at 9876543210 or email you at john@example.com.<br><br>

You: book appointment for Sunday<br>
Appointment successfully booked for 2024-10-13.<br><br>

You: Explain about Agriculture.<br>
Similarity Score: 61%<br>
Chatbot: Agriculture is the practice of cultivating plants and raising animals...<br><br>
