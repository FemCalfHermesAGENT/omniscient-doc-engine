# omniscient-doc-engine

Intelligent document reader, editor, and handler with Claude-level understanding. PDF, Word, Markdown, LaTeX, OCR, and structured extraction.

## Features

- **Multi-format parsing**: PDF, Word (.docx), Markdown, LaTeX, and more
- **OCR capabilities**: Extract text from scanned documents and images
- **Structured extraction**: Pull tables, forms, key-value pairs, and semantic content
- **Document editing**: Programmatic editing with format preservation
- **AI-powered understanding**: Integration with LangChain and LlamaIndex for RAG pipelines

## Installation

```bash
pip install -r requirements.txt
```

## Project Structure

```
src/
├── parsers/        # Document format parsers (PDF, DOCX, MD, LaTeX)
├── editors/        # Document editing and manipulation
└── extractors/     # Structured data extraction (tables, forms, OCR)
examples/           # Usage examples and notebooks
```

## Quick Start

```python
from src.parsers.pdf_parser import PDFParser

parser = PDFParser("document.pdf")
text = parser.extract_text()
tables = parser.extract_tables()
```

## License

MIT
