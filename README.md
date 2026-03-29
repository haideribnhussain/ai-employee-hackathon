# Personal AI Employee - Bronze Tier

> Hackathon 0: Building Autonomous FTEs in 2026
> Built by: Haider

## What is this?
A local-first Personal AI Employee that monitors folders, creates tasks automatically,
and uses Claude Code to process them — all running on your own machine.

## Architecture
\\\
Drop_Here/  (tum file daalte ho)
     |
filesystem_watcher.py  (detect karta hai)
     |
Needs_Action/  (task file automatically banti hai)
     |
Claude Code  (padhta, sochta, kaam karta hai)
     |
Dashboard.md updated + file moves to Done/
\\\

## Tech Stack
- Brain: Claude Code
- Dashboard: Obsidian (Local Markdown)
- Watcher: Python + Watchdog library
- OS: Windows 11

## Folder Structure
\\\
AI_Employee_Vault/
├── Needs_Action/      # Claude ke liye pending tasks
├── Plans/             # Claude ke banaye plans
├── Done/              # Completed tasks
├── Logs/              # Audit trail
├── Pending_Approval/  # Human approval chahiye
├── Approved/          # Human ne approve kiya
├── Rejected/          # Human ne reject kiya
├── Accounting/        # Financial records
├── Briefings/         # CEO briefings
├── Invoices/          # Invoice files
├── Drop_Here/         # Yahan file daalo trigger ke liye
├── Dashboard.md       # Real-time status
└── Company_Handbook.md # AI ke rules
\\\

## Setup Instructions

### Prerequisites
- Python 3.13+
- Node.js v24+
- Claude Code (active subscription)
- Obsidian v1.10.6+

### Installation
\\\powershell
# 1. Clone the repo
git clone https://github.com/haiderlbnhussain/ai-employee-hackathon
cd ai-employee-hackathon

# 2. Install Python dependencies
pip install watchdog

# 3. Start the watcher
python filesystem_watcher.py

# 4. Naye terminal mein Claude Code chalao
claude
\\\

### How to Use
1. Watcher chalao: python filesystem_watcher.py
2. Koi bhi file Drop_Here/ mein daalo
3. Claude Code ko ye prompt do:
   Check Needs_Action folder, process all pending tasks,
   update Dashboard.md, move completed tasks to Done/
4. Claude automatically sab handle kar leta hai!

## Bronze Tier Checklist
- [x] Obsidian vault with Dashboard.md and Company_Handbook.md
- [x] Working File System Watcher script
- [x] Claude Code reading and writing to vault
- [x] Basic folder structure complete
- [x] Audit logs in Logs/ folder

## Security
- Koi credentials code mein nahi hain
- Sab local machine pe run hota hai
- Human approval required for sensitive actions
- Audit logs Logs/ mein save hote hain

## Demo
Watch the AI Employee in action:
1. Drop a file in Drop_Here/
2. Watcher detects it instantly
3. Claude processes the task
4. Dashboard updates automatically

## Hackathon Submission
- Hackathon: Personal AI Employee Hackathon 0
- Tier: Bronze
- Submit: https://forms.gle/JR9T1SJq5rmQyGkGA
