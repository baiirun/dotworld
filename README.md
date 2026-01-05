# .world

A unified interface for AI agents to understand how you work.

## What is this?

`.world` is a personal operating system for agent-assisted work. It gives agents context about:
- Who you are and how you think
- What you're working on now
- Your projects, domains, and priorities
- How to navigate your digital life

## Setup

```bash
# Clone to your home directory
git clone https://github.com/baiirun/dotworld.git ~/.world

# Edit the files to match your life
```

## Structure

```
~/.world/
├── CLAUDE.md       # Agent instructions: personality, navigation, sources
├── me.md           # Who you are, how you think
├── now.md          # Current focus, priorities, open loops
├── domains/        # Focused contexts (work, personal, projects)
│   ├── work.md
│   ├── personal.md
│   └── *.md        # Add your own domains
└── tasks/          # Task management system (optional)
    └── README.md   # Setup instructions for tasks CLI
```

## How agents use it

Agents read `CLAUDE.md` first. It tells them:
1. Your preferred communication style
2. When to load other files (token-efficient)
3. Where your important resources live
4. What you're actively working on

The goal: agents have enough context to be useful without asking 20 questions.

## Philosophy

- **Minimal by default** — only load what's needed
- **Plain text** — markdown files, no proprietary formats
- **Agent-native** — structured for LLM consumption
- **Yours** — adapt the structure to fit your life

## Tasks System

The `tasks/` directory is where the tasks CLI stores its database.

The CLI itself lives in a separate repo: [dotworld-tasks](https://github.com/baiirun/dotworld-tasks)
