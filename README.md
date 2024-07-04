# Multiple PDF Chat with Gemini

This Streamlit application allows users to chat with multiple PDF documents using Google's Gemini AI model. It extracts text from uploaded PDFs, processes it, and enables users to ask questions about the content.

## Features

- Upload multiple PDF files
- Extract and process text from PDFs
- Split text into manageable chunks
- Create vector embeddings using Google's Generative AI
- Store embeddings using FAISS for efficient retrieval
- Ask questions about the PDF content using natural language
- Get detailed answers powered by Google's Gemini Pro model

## Installation

1. Install the required dependencies:
   pip install -r requirements.txt

2. Set up your Google API key:
- Create a `.env` file in the project root
- Add your Google API key: `GOOGLE_API_KEY=your_api_key_here`

## Usage

1. Run the Streamlit app:
streamlit run app.py
2. Use the sidebar to upload PDF files.

3. Click "Submit & Process" to extract and process the PDF content.

4. Once processing is complete, type your questions in the main text input to get answers based on the PDF content.

## How it Works

1. PDF Upload: Users can upload multiple PDF files through the Streamlit interface.
2. Text Extraction: The app extracts text from the uploaded PDFs.
3. Text Chunking: Extracted text is split into smaller, manageable chunks.
4. Embedding Creation: Google's Generative AI creates embeddings for each text chunk.
5. Vector Storage: FAISS is used to efficiently store and retrieve vector embeddings.
6. Question Answering: User questions are processed using a conversational chain with Google's Gemini Pro model.
7. Response Generation: Relevant information is retrieved, and a detailed answer is generated based on the PDF content.

## Dependencies

- streamlit
- google-generativeai
- python-dotenv
- langchain
- PyPDF2
- faiss-cpu
- langchain_google_genai

## License

This project is open-source and available under the MIT License.

## Acknowledgments

- Google Generative AI for providing the Gemini model
- Streamlit for the web application framework
- FAISS for efficient similarity search capabilities

