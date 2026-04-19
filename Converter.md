# Converter

Converter is a Streamlit app for converting manuscript files between PDF, DOCX, and EPUB formats.

It is intended as a practical utility for preparing text files for narration, review, or ebook workflows.

## What It Does

- Convert PDF files to DOCX.
- Convert DOCX files to EPUB.
- Convert PDF files to DOCX and then optionally to EPUB.
- Preserve common text styling where possible, including bold and italics.
- Add EPUB metadata such as title and author.
- Optionally include an EPUB cover image.

## Supported Inputs

Converter accepts:

- `.pdf`
- `.docx`

For EPUB covers, supported image uploads depend on the browser and Streamlit environment, but common image formats such as PNG and JPEG are expected.

## Basic Workflow

1. Upload a PDF or DOCX file.
2. If creating an EPUB, enter the title and author.
3. Optionally upload a cover image.
4. Download the generated DOCX and/or EPUB.

## Outputs

Depending on the uploaded file, Converter can produce:

- A DOCX file converted from PDF.
- An EPUB file converted from DOCX.
- An EPUB file generated after converting a PDF to DOCX.

## EPUB Notes

The EPUB output is a practical EPUB 3 package. It is designed to preserve the main text flow and common inline formatting, not to recreate every detail of a source layout.

DOCX headings may be used to split EPUB content into chapters. If the source document has inconsistent heading styles, chapter splitting may be less predictable.

## PDF Notes

PDF conversion is inherently imperfect because PDF is a layout format rather than a document structure format. Converter aims to produce an editable DOCX, but manual cleanup may still be needed, especially for:

- Complex page layouts
- Headers and footers
- Drop caps
- Tables
- Scanned or image-only PDFs
- Unusual fonts or spacing

## Privacy Notes

Converter processes uploaded files for the conversion task. Do not upload files unless you have the right to process them.

## Limitations

- Converter is not OCR software for image-only PDFs unless the deployment environment provides compatible OCR tooling.
- It is not a substitute for manual proofreading after conversion.
- EPUB validation should be performed separately if the file will be distributed commercially.

