# Needs_Action Folder

This folder contains items that require AI Employee's attention.

## File Format
Each file should follow this structure:

```markdown
---
type: [email|file|message|task]
from: [sender/source]
subject: [brief description]
priority: [low|medium|high]
status: pending
created: 2026-02-20T00:00:00Z
---

# Content

## Suggested Actions
- [ ] Action item 1
- [ ] Action item 2
```

## Processing Steps
1. AI Employee reads all files in this folder
2. Analyzes content and priority
3. Creates action plan in Plans folder
4. Updates Dashboard with status
5. Moves file to Done when complete

## Priority Guidelines
- **High**: Requires immediate attention (within 1 hour)
- **Medium**: Process within 4 hours
- **Low**: Process within 24 hours

## Examples
- Email from client asking for proposal
- WhatsApp message requesting appointment
- File drop requiring categorization
- Task requiring research or analysis