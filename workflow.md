

Complete End-to-End Flow

User opens browser
        │
        ▼
http://localhost:5000
        │
        ▼
home()
        │
        ▼
index.html displayed
        │
        ▼
User types question
        │
        ▼
Send button
        │
        ▼
POST /chat
        │
        ▼
chat()
        │
        ▼
request.json["message"]
        │
        ▼
get_answer(question)
        │
        ▼
OpenAI Embedding
        │
        ▼
Pinecone Search
        │
        ▼
Retrieve PDF Context
        │
        ▼
GPT Generates Answer
        │
        ▼
jsonify(response)
        │
        ▼
Browser receives answer
        │
        ▼
Chatbot displays answer
