# Contributing to whatsapp-docgen-bot

Thank you for your interest in contributing. We welcome contributions that expand document templates, improve typography, or enhance rendering performance.

## Skill Module Guidelines
When contributing to document rendering skills (`src/skills/`):
1. **Schema Compliance**: All document layouts must define a strict schema in `schema.js` validating LLM-generated structures before rendering.
2. **Memory Bounds**: Ensure all render streams release resources upon completion or failure.
3. **Zero Hardcoded Styles**: Use modular style palettes defined in skill configurations.

## Contribution Workflow
1. Fork and clone:
   ```bash
   git clone https://github.com/<your-username>/whatsapp-docgen-bot.git
   cd whatsapp-docgen-bot
   ```
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Test PDF and PPTX outputs locally against sample payloads.
4. Submit a Pull Request completing the mandatory security checklist in `.github/PULL_REQUEST_TEMPLATE.md`.