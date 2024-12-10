# Chat with Your PDFs (RAG)

This project provides a chatbot application powered by AI that allows users to upload PDF documents and interact with their content in a conversational format. The chatbot leverages advanced language models to retrieve and generate responses based on the information stored in the PDFs. Built with Streamlit, LangChain, and OpenAI, it enables a seamless user experience for document-based question answering.

## Features

- **Upload PDF files**: Supports uploading multiple PDF documents.
- **Text Chunking**: Splits the document into manageable chunks for efficient processing.
- **Vector Store Integration**: Uses Chroma for persistent vector storage to enable fast document retrieval.
- **AI-Powered Responses**: Supports multiple OpenAI models (e.g., `gpt-3.5-turbo`, `gpt-4`).
- **Interactive Chat Interface**: Provides an intuitive chat-like interface for querying documents.

## Installation

### Prerequisites

- Python 3.8 or later
- OpenAI API Key

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/chat-with-pdfs.git
   cd chat-with-pdfs
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file and set your OpenAI API key:
   ```
   OPENAI_API_KEY=your_openai_api_key
   ```

4. Run the application:
   ```bash
   streamlit run app.py
   ```

## Usage

1. Open the application in your browser (typically at `http://localhost:8501`).
2. Upload one or more PDF documents using the sidebar.
3. Select an AI model from the sidebar dropdown menu.
4. Ask questions in the chat input field and receive AI-generated answers based on the content of your PDFs.

## File Structure

- **`app.py`**: Main application file.
- **`db/`**: Directory for storing persistent vector data.
- **`requirements.txt`**: List of required Python packages.

## Key Components

- **PDF Processing**: Utilizes `PyPDFLoader` to read and preprocess PDF documents.
- **Text Splitting**: Splits documents into chunks using `RecursiveCharacterTextSplitter` for efficient embedding and retrieval.
- **Vector Store**: Uses Chroma for storing and querying document embeddings.
- **AI Interaction**: Powered by OpenAI models with customizable prompts.

## Models Supported

- `gpt-3.5-turbo`
- `gpt-4`
- `gpt-4-turbo`
- `gpt-4o-mini`
- `gpt-4o`

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or suggestions.

## Acknowledgments

- [Streamlit](https://streamlit.io/)
- [LangChain](https://langchain.com/)
- [Chroma](https://www.trychroma.com/)
- [OpenAI](https://openai.com/)
