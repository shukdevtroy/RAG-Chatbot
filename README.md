# RAG Chatbot with Documentation

This repository contains a Streamlit application that allows users to chat with the documentation of the Streamlit Python library using OpenAI's GPT-3.5-turbo model. Users can upload PDF or DOCX files containing documentation, and the application will index these documents for reference during the chat.

## Retrieval-Augmented Generation (RAG)

This application employs a form of Retrieval-Augmented Generation (RAG) by combining document retrieval and generative response:

1. **Document Retrieval**: Uploaded documents are indexed using a vector store. This allows the application to efficiently retrieve relevant information based on user queries.

2. **Augmented Generation**: When users ask questions, the chat engine retrieves context from the indexed documents and generates responses using the OpenAI model. This enhances the quality and relevance of the answers, as they are informed by the content of the uploaded documents.

## Features

- **Chat Interface**: Engage in a conversation with the Streamlit documentation.
- **Document Upload**: Upload PDF or DOCX files to index documentation for question answering.
- **Save Conversations**: Save your chat history for future reference.
- **Load Previous Conversations**: View and manage your previous chat sessions.
- **Delete Conversations**: Easily remove unwanted conversation histories.

## Requirements

To run this application, you need the following:

- Python 3.8 or higher
- Streamlit
- llama-index
- pdfplumber
- python-docx
- python-dotenv

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/shukdevtroy/RAG-Chatbot.git
   cd shukdevtroy/RAG-Chatbot
   ```

2. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the root directory of the project and add your OpenAI API key:

   ```
   OPENAI_API_KEY=your_openai_api_key
   ```

## Usage

1. Start the Streamlit app:

   ```bash
   streamlit run app4.py
   ```

2. Open your browser and go to `http://localhost:8501`.

3. Enter your OpenAI API key in the sidebar and upload the PDF or DOCX files that contain the Streamlit documentation.

4. Begin chatting by typing your questions in the chat input box.

5. Use the sidebar to manage your conversations, including saving and deleting previous chats.

## Note

- Ensure you have the appropriate permissions to upload the documentation files.
- The application is designed for technical questions specifically related to the Streamlit library.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

If you'd like to contribute to this project, feel free to submit a pull request or open an issue.

## Acknowledgments

- [Streamlit](https://streamlit.io/)
- [OpenAI](https://openai.com/)
- [llama-index](https://github.com/jerryjliu/llama_index)

## Contact

For any questions or inquiries, please reach out at [shudevdatta@gmail.com].



