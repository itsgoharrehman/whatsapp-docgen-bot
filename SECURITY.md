# Security Policy

## Supported Versions

| Version | Supported | Description |
| :--- | :--- | :--- |
| `1.0.x` | Yes | Current stable release branch (`main`) |
| `< 1.0.0` | No | Legacy versions |

## Document Generation Security Scope

whatsapp-docgen-bot processes arbitrary user text into binary document structures. Security invariants include:
* **Memory Bounding**: Document rendering engines enforce strict limits on total slide count (`MAX_SLIDES_PER_DECK`) and page count (`MAX_PDF_PAGES`) to prevent memory exhaustion attacks.
* **Sanitized Layout Injection**: Dynamic inputs rendered to PDF/PPTX formats must prevent binary payload injection and template breakout.
* **Credential Isolation**: Groq API keys and WhatsApp session tokens must remain strictly in process memory and never be serialized into generated document metadata.

## Reporting a Vulnerability

If you discover a vulnerability or denial-of-service vector in the document rendering engine, report it privately:

* **Security Contact**: Gohar Rehman
* **Email**: `goharrehmanfsd260@gmail.com`
* **Response SLA**: Initial acknowledgement within 48 hours; resolution timeline provided within 7 days.

Please do not open public GitHub issues or discussions regarding undisclosed vulnerabilities.