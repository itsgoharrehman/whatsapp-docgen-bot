## Summary of Changes

Describe the proposed changes, architecture impact, and reason for the modification.

## Security Checklist

Before submitting this pull request, verify each of the following security invariants:

- [ ] **Memory Bounding**: Verified that document generation changes enforce memory bounds and do not cause memory leaks during large rendering tasks.
- [ ] **No Hardcoded Credentials**: Verified that no WhatsApp session tokens or Groq API keys are committed.
- [ ] **Schema Validation**: Verified that any new skill validates LLM-generated JSON before passing it to document renderers.
- [ ] **Output Tested**: Verified successful generation of sample PDF and PPTX files.

## Testing Performed

Detail the local tests or manual verification steps conducted.