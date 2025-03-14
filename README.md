# LangChain AI Doc Assistant

## Overview
LangChain AI Doc Assistant is a Streamlit-based application designed to assist users in querying research documents using AI-powered natural language processing. It enables users to upload PDFs, process them into vector embeddings, and retrieve relevant information using an NVIDIA-powered language model.

## Features
- Upload and process research documents (PDFs).
- Extract and split text into manageable chunks.
- Store document embeddings in an in-memory vector database.
- Query the document using natural language.
- Generate AI-powered responses based on the uploaded document.
- Interactive chat interface with a user-friendly UI.

## Technologies Used
- **LangChain** for document processing and retrieval.
- **Ollama Embeddings** for generating document embeddings.
- **NVIDIA AI Endpoints** for AI-powered chat responses.
- **Streamlit** for the web-based interface.
- **PDFPlumber** for PDF text extraction.

## Installation
To run the application, install the required dependencies:

```bash
pip install -r requirements.txt
```

## File Structure
- `app.py`: Main application file containing Streamlit UI and backend logic.
- `requirements.txt`: List of dependencies for the project.

## Usage
1. Run the Streamlit application:

   ```bash
   streamlit run app.py
   ```

2. Upload a PDF document via the interface.
3. Ask questions related to the document using the chat input.
4. Receive AI-generated answers based on document content.

## Environment Variables
Ensure that you have set up the NVIDIA API key:

```bash
export NVIDIA_API_KEY='your_api_key_here'
```

## How It Works
1. **Document Upload**: Users upload a PDF file.
2. **Text Processing**: The document is split into smaller text chunks.
3. **Embedding Generation**: Each chunk is converted into a vector embedding.
4. **Indexing**: The embeddings are stored in an in-memory vector database.
5. **Querying**: User queries are matched with the most relevant document chunks.
6. **AI Response**: An NVIDIA-powered AI model generates responses based on the retrieved context.

## Future Improvements
- Support for multiple document uploads.
- Persistent vector storage using a database.
- Enhanced UI/UX with better chat interactivity.
- Integration with additional AI models for improved response quality.

