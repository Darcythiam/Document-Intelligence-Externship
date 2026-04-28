# Document Intelligence Externship

This repository contains a curated set of Google Colab notebooks from my document intelligence externship experience with **Outamation**. The project demonstrates an end-to-end document AI workflow for mortgage-style document analysis, including OCR, PDF parsing, structured extraction, retrieval, LLM-based question answering, model comparison, and a Gradio prototype.

The goal of this repository is to provide a technical overview of the work completed during the externship and to show how different document intelligence components can be combined into a practical pipeline.

## Project Highlights

- Compared OCR engines for scanned financial documents.
- Extracted PDF text, bounding boxes, and structured JSON fields.
- Explored document classification and boundary detection.
- Built retrieval pipelines using BM25, vector search, and embeddings.
- Compared Gemini and TinyLlama for mortgage question answering.
- Created a Gradio demo for document upload and Q&A.

## Repository Structure

```text
document-intelligence-externship/
├── notebooks/
│   ├── 01_ocr_engine_comparison_mortgage.ipynb
│   ├── 02_pdf_text_bounding_boxes_json.ipynb
│   ├── 03_document_boundary_detection_classification.ipynb
│   ├── 04_rag_retrieval_experiments.ipynb
│   ├── 05_llm_comparison_mortgage_qa.ipynb
│   └── 06_mortgage_rag_gradio_app.ipynb
├── data/
│   └── README.md
├── outputs/
│   └── README.md
├── certificates/
│   └── README.md
├── requirements.txt
├── .gitignore
└── README.md
```

## Notebook Guide

| Notebook | Purpose |
|---|---|
| `01_ocr_engine_comparison_mortgage.ipynb` | Compares OCR approaches for scanned mortgage documents. |
| `02_pdf_text_bounding_boxes_json.ipynb` | Extracts text, bounding boxes, key fields, and JSON-style outputs. |
| `03_document_boundary_detection_classification.ipynb` | Tests page-level classification and document boundary detection. |
| `04_rag_retrieval_experiments.ipynb` | Experiments with retrieval settings for document question answering. |
| `05_llm_comparison_mortgage_qa.ipynb` | Compares Gemini and TinyLlama on mortgage-related queries. |
| `06_mortgage_rag_gradio_app.ipynb` | Builds an end-to-end Gradio prototype for document Q&A. |

## Running the Notebooks

These notebooks were developed and tested in **Google Colab**.

### Recommended Colab workflow

1. Open a notebook in Google Colab.
2. Upload the required PDF into the Colab runtime or place it in a `data/` folder.
3. Add `GOOGLE_API_KEY` in Colab Secrets for notebooks that use Gemini.
4. Run the notebook cells from top to bottom.

### API Key Setup

For Gemini-based notebooks, the code expects `GOOGLE_API_KEY` from Colab Secrets or environment variables.

In Colab:

1. Click the key icon in the left sidebar.
2. Add a secret named `GOOGLE_API_KEY`.
3. Turn on notebook access.

No API keys are stored in this repository.

## Data Disclaimer

The documents used in this project are for educational and demonstration purposes only and do not contain sensitive personal information. Large document files are not included by default. Add your own test PDFs to the `data/` folder or upload them directly in Colab.

## Certificate

A certificate of completion can be added in the `certificates/` folder. This is optional, but it can help connect the technical work in this repository to the externship experience.

Suggested filename:

```text
certificates/outamation_externship_certificate.pdf
```

## Technical Stack

Python, Google Colab, PyMuPDF, Tesseract OCR, PaddleOCR, EasyOCR, BM25, FAISS, LlamaIndex, Hugging Face models, Gemini, TinyLlama, pandas, and Gradio.

## Main Takeaway

This project shows how OCR, document parsing, retrieval, and LLMs can be combined into a working document intelligence pipeline. The notebooks are intentionally organized as a technical portfolio rather than a production deployment.
