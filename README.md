# Prototype Financial Insights Engine (BCG GenAI Job Simulation)

**Summary:** Backend proof-of-concept that extracts and interprets financial data from SEC filings (10-K/10-Q) using Python + pandas and rule-based logic. Includes a minimal Streamlit demo to simulate chatbot-style Q&A.

## Features
- Parse filings into structured tables
- Compute KPIs (revenue growth, margins, leverage)
- Rule-based answers with sources
- Notebooks + images for portfolio
- Minimal Streamlit demo

## Project Structure
```
.
├── notebooks/
│   └── BCG_GENAI.ipynb
├── images/
│   ├── bcg_genai_pipeline.png
│   ├── bcg_genai_methodology.png
│   ├── bcg_genai_insights_bar.png
│   └── bcg_genai_conclusion_pie.png
├── src/
│   └── app.py
├── requirements.txt
└── .gitignore
```

## Quickstart
```bash
# 1) Create and activate a virtual env (optional but recommended)
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

# 2) Install deps
pip install -r requirements.txt

# 3) Run demo app
streamlit run src/app.py
```

## Notes
- The Streamlit app routes common queries (revenue, margin, debt) to stub functions.
- Replace stubs with your logic from `notebooks/BCG_GENAI.ipynb`.
