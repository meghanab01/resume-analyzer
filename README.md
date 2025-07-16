# Resume Analyzer

A lightweight resume analyzer built using **Google’s Gemini 2.5 Flash** and **Gradio** in a single Jupyter notebook. It compares resumes with job descriptions and gives AI-powered feedback including match score, strengths, missing skills, and improvement suggestions.

## Features

- Upload resumes in **PDF** or **DOCX** format
- Extracts **LinkedIn URLs**
- Uses **Gemini API** to analyze resume content against any job description
- Returns:
  - Match Score (0–100)
  - Top 3 Strengths
  - Missing Qualifications
  - Suggestions to improve the resume
- Simple and interactive **Gradio interface**

## How to Run

1. Install the requirements:
```bash
pip install -r requirements.txt
```

2. Create a `.env` file with your Gemini API key:

```bash
GOOGLE_API_KEY=your_api_key_here
```

3. Open the Jupyter notebook and run it.

## Tech Stack

- Python
- Gradio
- Google Generative AI (Gemini-2.5-Flash)
- PDF Processing:
  - pdfplumber (primary)
  - PyPDF2 (fallback)
  - python-docx (for Word files)
