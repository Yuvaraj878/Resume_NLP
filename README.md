## Resume Parser

This Python script extracts structured information such as **Name**, **Email**, **Phone**, **Skills**, **Degree**, **Institution**, and **Work Experience** from PDF resumes using NLP and pattern matching.

### Usage

1. Place your resume PDF file (e.g. `ML_Resume.pdf`) in the same directory as this script.
2. Install required dependencies:
```bash
pip install spacy pdfplumber
python -m spacy download en_core_web_sm
```

4. The extracted resume information will be printed on the console and saved to `parsed_resume.json` in a structured JSON format.

---

The script uses:

- `pdfplumber` for PDF text extraction
- `spaCy` for Named Entity Recognition (Name, Degree, Institution)
- Regex for Email and Phone extraction
- PhraseMatcher for matching predefined skill keywords
- Regex heuristics for extracting work experience sections
