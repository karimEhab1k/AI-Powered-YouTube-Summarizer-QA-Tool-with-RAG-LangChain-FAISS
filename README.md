# AI-Powered-YouTube-Summarizer-QA-Tool-with-RAG-LangChain-FAISS

This project builds a tool that lets you ask questions about a YouTube video and get answers drawn from its transcript, instead of watching the whole thing.

## How It Works

1. **Load the transcript** from a YouTube video.
2. **Process the text** by splitting it into smaller chunks.
3. **Create embeddings**, which are numerical representations of each chunk's meaning.
4. **Store them in a vector database** (FAISS) so similar content can be found quickly.
5. **Retrieve the relevant chunks** when you ask a question, and pass them to an LLM that writes the answer or summary.

## Tools Used

- **LangChain**: connects the pieces together
- **An LLM**: generates summaries and answers
- **FAISS**: fast similarity search, which also helps pinpoint which part of the video covers a topic
- **Streamlit**: a simple web interface (the project files suggest Gradio is used instead, which does the same job)

## Why It Matters

Long videos are slow to search manually. This tool turns dense transcripts into concise summaries and makes it easy to find specific segments, so video content becomes much more accessible.
