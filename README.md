# Loan Support Chatbot

## Introduction
The Loan Support Chatbot is a Python application designed to assist users with loan-related inquiries. As a loan support chatbot, it helps users determine their eligibility for different types of loans and provides information about the loan application process. Additionally, the chatbot offers guidelines and recommendations to users based on their financial situation. Whether you need information about loan eligibility criteria, documentation requirements, or the application process timeline, the Loan Support Chatbot is here to help you navigate through the loan application process efficiently.

#

## How It Works

1. PDF Initialization: The system initializes by loading a predefined PDF document named 'data.pdf', containing relevant loan information.
2. Text Chunking: The text content of the PDF document is segmented into smaller, manageable chunks for efficient processing.
3. Language Model Integration: Utilizing a language model, the application generates vector representations (embeddings) of the segmented text chunks.
4. Semantic Matching: Upon receiving a user question, the system compares it with the segmented text chunks to identify the most semantically similar content.
5. Response Generation: The identified chunks are passed to the language model, which generates a response based on the relevant loan information extracted from the PDF document.

#

## Dependencies and Installation

To set up the MultiPDF Chat App, adhere to these instructions:

1. Copy the repository to your computer.
2. Install necessary dependencies with the command:
   ```python
   pip install -r requirements.txt
   ```
3. Acquire an API key from OpenAI and insert it into the .env file located in the project directory.
  ```commandline
  OPENAI_API_KEY=your_secrit_api_key
  ```

#

## Usage

To utilize the Loan Support Chatbot, adhere to these steps:

1. Confirm that you have installed the necessary dependencies and included the OpenAI API key in the .env file.
2. Launch the main.py file utilizing the Streamlit CLI. Execute the subsequent command:
   ```
   streamlit run app.py
   ```
   
3. The application interface will open in your default web browser once launched.
4. Follow the instructions provided to load multiple PDF documents into the application.
5. Utilize the chat interface to ask questions in natural language about the loaded PDFs.
