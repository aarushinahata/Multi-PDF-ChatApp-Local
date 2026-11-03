# Multi-PDFs ChatApp

A local Streamlit app for searching the contents of multiple PDF documents. PDF text is processed on your computer; no Gemini API key or internet connection is needed for document search.

## Features

- **Local PDF processing:** Extracts and searches text on your computer without sending documents to Gemini or requiring an API key.
- **Question-based passage search:** Ask a question and see the most relevant text found in the uploaded PDFs.
- **Source references:** Each result includes the PDF filename and page number.
- **Prepared sample answers:** Five questions about the bundled *Augmented LLMs.pdf* return concise answers cited to page 1.
- **Sample PDF download:** Download *Augmented LLMs.pdf* directly from the app sidebar.
- **Honest answers:** General questions return relevant excerpts from the document, not AI-generated reviews or summaries.

## Installation

Install the requirements:

```powershell
pip install -r requirements.txt
```

Run the app from this folder:

```powershell
streamlit run chatapp.py
```

## Usage

1. Upload one or more PDFs in the sidebar.
2. Click **Submit & Process**. The app extracts and organizes the PDF text locally so it can be searched; this step does not create an AI-written review or send the PDF to Gemini.
3. Ask a question about the uploaded PDF. The app searches its text and shows the most relevant passages with the source filename and page number.
4. The app returns relevant text from the PDF rather than generating an AI-written summary. For the bundled *Augmented LLMs.pdf*, five prepared questions also have concise answers with a page citation.
5. Use **Download Augmented LLMs PDF** in the sidebar to download the sample PDF.

Scanned/image-only PDFs may not contain extractable text and therefore may not be searchable.

## License

Distributed under the MIT License. See `LICENSE` for more information.
