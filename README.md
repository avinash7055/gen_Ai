# PDF Chat Application

A powerful Streamlit-based application that allows users to chat with multiple PDF documents using AI. The application uses advanced natural language processing and machine learning techniques to understand and respond to questions about the content of uploaded PDF files.

## Features

- 📚 Upload and process multiple PDF documents simultaneously
- 💬 Interactive chat interface to ask questions about the documents
- 🤖 AI-powered responses using OpenAI's GPT models
- 🔄 Conversation memory to maintain context
- 🎨 Modern and responsive user interface
- ⚡ Fast and efficient document processing

## Technologies Used

- **Streamlit**: Web application framework
- **LangChain**: Framework for developing applications powered by language models
- **OpenAI**: For embeddings and chat completions
- **FAISS**: For efficient similarity search and clustering
- **PyPDF2**: For PDF text extraction
- **Python-dotenv**: For environment variable management

## Prerequisites

- Python 3.7+
- OpenAI API key
- Internet connection

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-name>
```

2. Install the required packages:
```bash
pip install -r requirements.txt
```

3. Create a `.env` file in the root directory and add your OpenAI API key:
```
OPENAI_API_KEY=your_api_key_here
```

## Usage

1. Start the application:
```bash
streamlit run app.py
```

2. Open your web browser and navigate to the provided local URL (typically http://localhost:8501)

3. Upload one or more PDF documents using the file uploader in the sidebar

4. Click the "Process" button to analyze the documents

5. Start asking questions about the content of your PDFs in the chat interface

## How It Works

1. **Document Processing**:
   - PDFs are uploaded and processed to extract text
   - Text is split into manageable chunks
   - Chunks are converted into embeddings using OpenAI's embedding model

2. **Vector Storage**:
   - Text embeddings are stored in a FAISS vector store
   - This enables efficient similarity search for relevant content

3. **Chat Interface**:
   - User questions are processed and matched with relevant document content
   - The AI model generates responses based on the context
   - Conversation history is maintained for context-aware responses

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- OpenAI for providing the language models
- Streamlit for the amazing web framework
- LangChain for the powerful NLP tools





