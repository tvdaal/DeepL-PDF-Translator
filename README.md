# DeepL PDF Translator

A tool for translating PDF documents using the DeepL API while preserving formatting and images.

## Features

- Full PDF document translation with preserved formatting
- Support for maintaining images, tables, and other elements
- Translation of all languages supported by the DeepL API
- Automatic handling of large documents

## Requirements

- Python 3.7+
- DeepL API key (you can get a free one at [DeepL Developer](https://www.deepl.com/pro-api))
- Microsoft Word or LibreOffice (for DOCX to PDF conversion)

## Installation

```bash
# Clone the repository
git clone https://github.com/KNXKO/deepl-pdf-translator.git
cd deepl-pdf-translator

# Install dependencies
pip install -r requirements.txt
```

## Usage

### Basic Usage

```bash
python pdf_translator.py path_to_pdf target_language --auth-key YOUR_DEEPL_API_KEY
```

Example:
```bash
python pdf_translator.py translated.pdf SK --auth-key xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
```

### Parameters

- `path_to_pdf`: Path to the PDF file to translate
- `target_language`: Target language code (e.g., SK, EN, DE, FR...)
- `--auth-key`: DeepL API key
- `--output`: (optional) Path to the output file

## Supported Languages

DeepL API supports these language codes:

- BG (Bulgarian)
- CS (Czech)
- DA (Danish)
- DE (German)
- EL (Greek)
- EN (English)
- ES (Spanish)
- ET (Estonian)
- FI (Finnish)
- FR (French)
- HU (Hungarian)
- ID (Indonesian)
- IT (Italian)
- JA (Japanese)
- LT (Lithuanian)
- LV (Latvian)
- NL (Dutch)
- PL (Polish)
- PT (Portuguese)
- RO (Romanian)
- RU (Russian)
- SK (Slovak)
- SL (Slovenian)
- SV (Swedish)
- TR (Turkish)
- UK (Ukrainian)
- ZH (Chinese)

## How It Works

1. The PDF is converted to DOCX format to preserve formatting and images
2. All text elements within the DOCX are translated using the DeepL API
3. The translated DOCX is converted back to PDF

## Future Improvements

- Parallel processing for faster translation
- Translation memory to avoid re-translating repeated phrases
- OCR support for scanned documents
- Better handling of complex nested objects

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the [MIT License](LICENSE).