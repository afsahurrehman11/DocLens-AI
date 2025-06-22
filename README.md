# DocuLens AI – Retrieval-Augmented Generation (RAG) Agent

## Description

**DocuLens AI** is your AI agent powered by Retrieval-Augmented Generation (RAG). Upload any PDF, ask your question, and DocuLens AI dives into your document to deliver precise, lightning-fast answers. No jargon, no fuss—just clear insights for beginners and experts alike, all driven by a robust RAG engine.

## Features

- **PDF Reader**: Quickly loads and reads your PDF files.
- **Smart Splitting**: Breaks text into small pieces for fast search.
- **Deep Understanding**: Uses top embeddings to know what your text means.
- **Quick Search**: Finds the right parts instantly with a fast index.
- **AI Answers**: Uses a powerful LLM to craft clear responses.
- **Memory Tracking**: Remembers your previous questions for follow-ups.
- **On-Topic Only**: Sticks to your PDFs and politely declines unrelated questions.

## How It Works

1. **Load PDF**: The AI reads and extracts text from your PDF.
2. **Split Text**: Text is chopped into bite-size chunks.
3. **Create Embeddings**: Chunks become vectors to capture their meaning.
4. **Build Index**: A FAISS index makes searching super quick.
5. **Answer Query**: When you ask, the AI finds the best chunks and asks the LLM.
6. **Generate Reply**: The LLM gives a clear answer, using only your PDF.
7. **Remember History**: Past questions help the AI stay on track.

## Usage

Start the script, type your question, and see the answer from your PDF. If you ask something outside the PDF, DocuLens AI will say:

> "I can only answer questions about the documents provided."

## Testing

Tested with:

- **Tech Manual**: A detailed machine guide.
- **Sales Report 2024**: Monthly numbers for clear examples.

## Sample Interaction

- **You**: "Who made the compressor?"
- **DocuLens AI**: "The compressor is made by ELGi (see page 1, ‘About ELGi’)."

## Setup Instructions

1. **Clone Repo**
   ```bash
   git clone https://github.com/afsahurrehman11/DocuLens-AI
   cd doculens-ai
   ```
2. **Install Tools**
   ```bash
   pip install -r requirements.txt
   ```
3. **Add Your API Key**
   - Set your LLM API key in the environment (e.g., `export API_KEY=your_key`).
4. **Add a PDF**
   - Place your PDF in the project folder.
5. **Run the Agent**
   ```bash
   python main.py
   ```




