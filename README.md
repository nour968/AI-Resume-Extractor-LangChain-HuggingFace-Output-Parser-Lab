# AI-Resume-Extractor-LangChain-HuggingFace-Output-Parser-Lab
This notebook is a hands-on lab designed to explore and experiment with LangChain, a powerful framework for building applications powered by Large Language Models (LLMs). It walks through core LangChain concepts, practical workflows, and real examples of chaining, prompting, document processing, and model integration.
This notebook demonstrates how to build an AI-powered Resume Parser using:

⚡ HuggingFace Transformers

🧩 LangChain Output Parsers

📄 PDF text extraction

🎯 Structured JSON output generation

It allows you to feed any PDF CV/resume, and the system automatically extracts key fields such as:

👤 Full Name

📧 Email

📱 Phone

🛠 Skills

🎓 Education

💼 Experience

🌐 Social links

📝 Summary

All wrapped in a clean, schema-enforced JSON structure.

🚀 Features

Local LLM inference using HuggingFace

Custom OutputParser schema for consistent output

PDF-to-text preprocessing

Strong structured prompting

Extracts the most important CV fields with high accuracy

Fully reproducible inside a single notebook

📂 Notebook Workflow
1️⃣ Install & Import Dependencies

The notebook installs:

pip install langchain langchain-core langchain-community transformers

2️⃣ Authenticate to HuggingFace Hub

Supports running local models with:

from huggingface_hub import login

3️⃣ Load a LLaMA / Qwen / Mistral Model

Uses HuggingFace AutoModelForCausalLM with FP16 + device map auto.

4️⃣ Define the Resume Schema

Using LangChain’s:

StructuredOutputParser
ResponseSchema

5️⃣ Load Resume PDF
from langchain.document_loaders import PyPDFLoader

6️⃣ Build Prompt Template

A clean JSON output is enforced via:

CV_extraction_template

7️⃣ Generate Structured Response

LLM output is cleaned, parsed, and printed.

📦 Requirements
langchain
langchain-community
langchain-core
transformers==4.52.4
huggingface_hub
pypdf
torch


A GPU is recommended for fast inference.

▶️ How to Use

Open the notebook

Upload a PDF CV

Run all cells

Get your structured CV JSON output instantly

🔮 Future Enhancements

Support for DOCX parsing

Integration with ChromaDB for resume search

Multi-language CV extraction

Export to CSV/ATS-friendly format

Add FastAPI endpoint for deployment

⭐ Support

If this notebook helps you, please star the repo ⭐ — it encourages more AI tools like this!
