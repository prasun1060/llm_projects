# Chat With Me - AI Personal Assistant

This project creates an AI chatbot that acts as your personal representative, answering questions about your career, background, skills, and experience based on your LinkedIn profile and personal summary.

## What it does

The chatbot uses OpenAI's API to:
- Read your LinkedIn profile (PDF format)
- Access your personal summary
- Respond to questions as if it were you
- Maintain a professional and engaging conversation style
- Stay in character while representing you to potential clients or employers

## Prerequisites

- Python 3.8+
- OpenAI API key
- Required Python packages (see `pyproject.toml`)

## Setup Instructions

1. **Complete the initial setup** for this repository from the root folder's README file

2. **Download your LinkedIn profile** as a PDF and save it as `linkedin.pdf` in the `resources/` folder

3. **Create a personal summary** by writing a `summary.txt` file in the `resources/` folder with information about yourself

4. **Set up your environment variables**:
   - Create a `.env` file in the project root
   - Add your OpenAI API key: `OPENAI_API_KEY=your_api_key_here`

5. **Install dependencies**:
   ```bash
   uv sync
   ```

## Usage

1. Open the `chat_with_me.ipynb` notebook
2. Run all cells to start the chatbot
3. The chatbot will be available through the Gradio interface
4. Ask questions about your background, skills, or experience

## File Structure

```
chat_with_me/
├── chat_with_me.ipynb      # Main chatbot notebook
├── README.md               # This file
└── resources/              # Required resources folder
    ├── linkedin.pdf        # Your LinkedIn profile (PDF)
    └── summary.txt         # Your personal summary
```

## Features

- **Personalized Responses**: Tailored to your specific background and experience
- **Professional Tone**: Maintains appropriate business communication style
- **Context Awareness**: Uses both LinkedIn profile and personal summary for comprehensive answers
- **Interactive Interface**: Gradio-based web interface for easy interaction
- **Response Evaluation**: Built-in quality assessment of chatbot responses

## Notes

- Ensure your LinkedIn PDF and summary.txt are properly formatted and contain relevant information
- The chatbot will only answer questions it has information about
- Responses are generated using OpenAI's language models
- Keep your API key secure and never commit it to version control