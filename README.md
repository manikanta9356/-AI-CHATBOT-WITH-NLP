COMPANY: CODTECH IT SOLUTIONS

NAME: Gattadi Manikanta

INTERN ID: CT04DM1361

DOMAIN: Python Programming

DURATION: 4 Weeks

MENTOR: NEELA SANTOSH

# AI Chatbot with Natural Language Processing (NLP)

An intelligent AI-powered chatbot capable of understanding and responding to human language using Natural Language Processing (NLP) techniques. This project demonstrates how conversational AI can be developed using modern NLP frameworks and machine learning models.

## Features

- Intent recognition and entity extraction
- Context-aware responses
- Pre-trained language models (e.g., spaCy, BERT, or GPT-based)
- Web-based chat interface (optional)
- Continuous learning and custom training support
- Modular architecture for easy integration with APIs and databases

## Technologies Used

- **Python 3.x**
- **Natural Language Toolkit (NLTK)** / **spaCy** / **transformers**
- **Flask / FastAPI** (for the backend API)
- **HTML/CSS/JavaScript** (for frontend if applicable)
- **Scikit-learn / TensorFlow / PyTorch** (for model training)
- **MongoDB / SQLite** (optional for storing conversation history)

## Getting Started

### Prerequisites

Make sure you have Python installed. Install dependencies with:

```bash
pip install -r requirements.txt
Running the Application
Start the backend server:

bash
Copy
Edit
python app.py
If using a web interface, open index.html in your browser or run the frontend development server.

Example Usage
You can interact with the bot using the command line or a web interface. Sample inputs:

"what is your name": "I am a chatbot.",
    "how are you": "I'm doing well, thank you!",
    "what can you do": "I can answer your queries using NLP.",
    "what is nlp": "NLP stands for Natural Language Processing, a field of AI that deals with human language.",
    "what is python": "Python is a high-level, interpreted programming language known for its readability and simplicity.",
    "what is an internship": "An internship is a short-term work experience that allows students to gain practical skills in a specific field.",
    "what is your purpose": "I'm here to help you complete your internship tasks and answer basic questions.",
    "what is github": "GitHub is an online platform to host and share code using Git version control.",
    "what is machine learning": "Machine learning is a branch of AI that enables systems to learn from data and improve over time.",
    "can you help me": "Of course! Ask me any question related to Python, the internship, or general concepts."

The chatbot parses the input, identifies intent, and generates a relevant response.

## How It Works
Text Preprocessing: Input is tokenized, normalized, and cleaned.

Intent Recognition: Classifies the user’s intent using an NLP model.

Entity Extraction: Detects relevant entities like dates, names, etc.

Response Generation: Chooses or generates an appropriate response.

Context Management: Maintains the context of the conversation.

## Project Structure
graphql
Copy
Edit
ai-chatbot-nlp/
├── app.py               # Main server script
├── chatbot/
│   ├── nlp_model.py     # NLP logic and model
│   ├── intents.json     # Sample intents and patterns
│   └── utils.py         # Helper functions
├── static/              # (Optional) Frontend files
├── templates/           # HTML templates
├── requirements.txt     # Dependencies
└── README.md            # This file
## To-Do
 Add voice input integration

 Deploy on cloud (e.g., Heroku, AWS)

 Improve contextual memory

 Add multilingual support

## how to run

## Install spaCy and the Language Model
Open your terminal (Command Prompt, PowerShell, or a code editor terminal like VS Code), and run:

pip install spacy
Then download the en_core_web_md model (which your code uses):

python -m spacy download en_core_web_md
If the medium model (md) is too large or gives issues, you can use the smaller one:

python -m spacy download en_core_web_sm
And in your code, change this line:

nlp = spacy.load("en_core_web_md")
nlp = spacy.load("en_core_web_sm")
## Save Your Code
Save your chatbot code in a file. For example:

chatbot.py
Make sure your file looks something like this at the top:

import spacy

nlp = spacy.load("en_core_web_md")  # Or 'en_core_web_sm' if needed

Define your FAQ...
Also, fix one small issue in your chat loop:

if user_input.strip() == "exit":
    print("ChatBot: bye! Have a nice day!")  # Manually print goodbye
    break
Because "exit" isn't in your faq dictionary.

## Run Your Code
In the same directory where you saved chatbot.py, run:

python chatbot.py
You should see:

ChatBot: Hello! Ask me something. (Type 'exit' to quit)
You:
Then you can chat with your bot.

## Example Conversation

You: what is your name
ChatBot: I am a chatbot.

You: what is machine learning
ChatBot: Machine learning is a branch of AI that enables systems to learn from data and improve over time.

You: bye
ChatBot: bye! Have a nice day!

You: exit
ChatBot: bye! Have a nice day!
