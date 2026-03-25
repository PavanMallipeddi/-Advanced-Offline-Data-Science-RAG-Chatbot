**📌 Overview**

This project combines semantic search, keyword search, and a local LLM to answer Data Science questions intelligently. It is designed for students, job seekers, and self-learners who want an interactive tutor that works even without internet access (after initial model download).

**✨ Features**

FeatureDetails🔍 Hybrid RetrievalFAISS (semantic) + BM25 (keyword) combined search🤖 Local LLMTinyLlama-1.1B-Chat — no API key needed💬 Chat HistoryLast 3 exchanges used as context for follow-up questions🎯 Quiz ModeRandom concept flashcard for self-testing🖥️ Gradio UIClean browser-based chat interface📚 Knowledge Base16 core Data Science concepts (easily extensible)

**💬 Usage Modes**

Chat Mode (Gradio UI)
Type any Data Science question and receive a structured answer with explanation, example, and key points.

**Quiz Mode (Terminal)**

Ask (or type quiz/exit): quiz
Explain this concept: Cross validation improves model robustness by multiple splits.

**Terminal Chat**

Ask (or type quiz/exit): What is overfitting?

**Known Limitations
**

TinyLlama (1.1B parameters) may produce incomplete or slightly inaccurate answers for complex questions — it is intended for learning, not production use.
Knowledge base is static (no persistent database). Additions require a re-run of the notebook.
Chat history is stored in-memory and resets on kernel restart.
First run requires internet access to download model weights (~600 MB).
