# Plans Folder

This folder contains action plans created by the AI Employee for processing tasks.

## Plan Format
Each plan follows this structure:

```markdown
---
created: 2026-02-20T21:37:00Z
status: completed
author: claude_code
target: [file_name]
risk: [low|medium|high]
success_criteria: [description]
---

# Plan: [Brief Description]

## Objective
[Brief description of what needs to be accomplished]

## Steps
1. [ ] Step 1
2. [ ] Step 2
3. [ ] Step 3

## Risk Assessment
- **Risk Level**: [low/medium/high]
- **Mitigation**: [how risks are handled]

## Success Criteria
- [ ] [specific measurable outcome]
- [ ] [specific measurable outcome]

## Execution Commands
```bash
# Commands to execute the plan
```
```

## Processing Steps
1. AI Employee creates plan based on Needs_Action item
2. Plan is reviewed and approved
3. Plan is executed
4. Results are logged and files are moved to Done
5. Dashboard is updated with completion status

## Examples
- Plan for processing client invoice files
- Plan for categorizing and storing resumes
- Plan for scheduling meetings from agenda files
- Plan for processing research documents

## Plan History
- plan_001_test_file_3.md - Completed: System validation test
- plan_002_client.txt.md - Completed: Simple text message processing
- plan_003_app.txt.md - Completed: Casual greeting message processing
- plan_004_test_file.txt.md - Completed: System validation test
- plan_005_test_file_2.txt.md - Completed: System validation test
```