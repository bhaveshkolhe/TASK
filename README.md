# Custom Chatbot using LangChain

This project demonstrates how to create a custom chatbot using LangChain, local embeddings with SentenceTransformer, and FAISS vector store. The chatbot extracts data from a website, creates embeddings, and provides answers through a Flask RESTful API using a local language model from Hugging Face.

## Setup

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/my-chatbot.git
    cd my-chatbot
    ```

2. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Flask App**:
    ```bash
    python app.py
    ```

    By default, the app will run on `http://127.0.0.1:5000`.

## Usage

Send a POST request to the `/ask` endpoint with a JSON body containing a `question` field.

### Example Request

```bash
curl -X POST http://127.0.0.1:5000/ask -H "Content-Type: application/json" -d '{"question": "What are the technical courses available?"}'
