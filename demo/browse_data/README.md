# FinanceBench Data Browser

Static single-page browser for the FinanceBench JSONL dataset. Built with Alpine.js + Tailwind — no build step, no `node_modules`.

## Running

Serve from the **project root** (so the page can reach `../../data/` and `../../pdfs/`):

```bash
cd /path/to/financebench
python -m http.server 8000
```

Then open **http://localhost:8000/demo/browse_data/**

> The page must be served over HTTP — `file://` won't work due to browser fetch restrictions.

## Features

- **Questions view** — browse all 150 benchmark Q&A pairs with filters for company, sector, doc type, year, question type, and reasoning type; full-text search across questions, answers, justifications, and evidence
- **Documents view** — browse all 361 documents with metadata and inline PDF preview
- **Evidence viewer** — each question shows extracted evidence passages with a toggle to open the source PDF embedded directly on the relevant page
