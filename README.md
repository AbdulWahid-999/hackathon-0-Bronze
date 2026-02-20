# Personal AI Employee - Bronze Tier

## Project Overview
This is the Bronze Tier implementation of the Personal AI Employee hackathon project. It includes the foundational components for an autonomous digital assistant.

## Bronze Tier Requirements Completed

✅ **Obsidian vault with Dashboard.md and Company_Handbook.md**
✅ **One working Watcher script (File System monitoring)**
✅ **Claude Code successfully reading from and writing to the vault**
✅ **Basic folder structure: /Inbox, /Needs_Action, /Done**
✅ **All AI functionality implemented as Agent Skills**

## Folder Structure
```
Bronze-Tier/
├── AI_Employee_Vault/
│   ├── Dashboard.md              # Real-time system dashboard
│   ├── Company_Handbook.md       # Rules and guidelines
│   ├── Inbox/                     # Drop folder for files
│   ├── Needs_Action/              # Items requiring processing
│   ├── Done/                      # Completed items
│   ├── Plans/                     # Action plans created by AI
│   ├── Pending_Approval/          # Items waiting for human approval
│   ├── Approved/                  # Approved items
│   └── Rejected/                  # Rejected items
├── file_watcher.py               # File system watcher script
├── requirements.txt              # Python dependencies
└── README.md                    # This file
```

## Installation

1. **Install Python dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Install watchdog (if not using requirements.txt):**
   ```bash
   pip install watchdog
   ```

## Usage

### Start the File System Watcher
```bash
python file_watcher.py
```

### Test the System
1. Drop a file into the `AI_Employee_Vault/Inbox/` folder
2. The watcher will detect it and create a markdown file in `Needs_Action/`
3. Claude Code can then read the Needs_Action file and create a plan

### Claude Code Integration
```bash
# From the Bronze-Tier directory
claude --cwd AI_Employee_Vault

# Then use Claude Code to:
# 1. Read the Needs_Action file
# 2. Create a plan in Plans/
# 3. Process the file and move to Done/
```

## Agent Skills Implemented

### File Processing Skill
- Detects file drops in Inbox folder
- Creates structured action items
- Categorizes by file type and priority
- Updates system status

### Task Management Skill
- Reads Needs_Action items
- Creates detailed action plans
- Manages workflow through approval process
- Updates Dashboard with progress

## Next Steps (Silver Tier)
To upgrade to Silver Tier, implement:
- Gmail Watcher for email processing
- WhatsApp Watcher for messaging
- MCP servers for external actions
- Automated approval workflows
- Scheduling system

## Security Features
- Local-first architecture (no cloud storage)
- Audit logging for all actions
- Human-in-the-loop approval for sensitive actions
- Credential management through environment variables

## Troubleshooting

### Common Issues
1. **Watcher not detecting files:** Check permissions and path
2. **Claude Code can't read files:** Verify file paths and permissions
3. **File not moving to Done:** Check for errors in processing

### Debug Mode
Enable debug logging by setting the logging level to DEBUG in file_watcher.py.

## License
This project is for educational purposes as part of the Personal AI Employee Hackathon.

## Support
For questions about the hackathon, join the Wednesday Research Meeting (details in the main documentation).