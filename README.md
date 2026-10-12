# Multi-Agent-Legal-Risk-Parser

# Multi-Agent Legal Document Extraction & Risk Pipeline

An agentic AI workflow built using LangChain and Google Gemini to automate contract analysis, legal risk detection, and executive redline summary generation.

## 📌 Architecture Overview

Instead of relying on a single prompt, this project uses a sequential 3-stage agentic pipeline to minimize hallucinations and improve analytical precision:

1. **Agent 1: Entity & Clause Extractor**
   * Extracts key structured information (parties, key dates, liability caps, termination clauses) from raw legal agreements.
2. **Agent 2: Risk & Compliance Assessor**
   * Evaluates extracted clauses against risk frameworks, flagging financial exposure, perpetual liabilities, and compliance gaps.
3. **Agent 3: Executive Summarizer**
   * Synthesizes facts and risk assessments into an executive-level Markdown report complete with redline recommendations and risk ratings.

## 🛠️ Tech Stack

* **Language:** Python
* **Orchestration:** LangChain (`langchain-google-genai`, `langchain-core`)
* **LLM Engine:** Google Gemini API (`gemini-3.8-flash`)
* **Environment:** Google Colab
