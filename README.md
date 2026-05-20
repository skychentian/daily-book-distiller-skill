# Daily Book Distiller Skill

A public, sanitized AI-agent skill for daily book recommendation and high-density reading cards.

It recommends **exactly one book** based on an agent's available memory, user profile, current priorities, and recent context, then distills the book into a concise reading card:

- What problem the book really answers
- The author's core argument
- The most counterintuitive insight
- A simple thought-structure map
- 2-3 restrained applications to the user

## Privacy

This repo is sanitized for public use.

It does **not** contain:

- Private user names
- Personal memory entries
- Business/customer details
- API keys or credentials
- Private workspace paths

The skill only describes the reusable workflow.

## How to use

Copy `daily-book-distiller/SKILL.md` into your agent's skill directory, or package it using your agent's skill tooling.

For Hermes Agent / Claude-style skills, the required structure is:

```text
daily-book-distiller/
└── SKILL.md
```

## Suggested scheduled prompt

```text
Every day, recommend and distill exactly one book for the user.

Requirements:
1. Use the daily-book-distiller skill.
2. Choose one book only, not a reading list.
3. Use available memory/profile/recent context when selecting the book.
4. Keep the book's own ideas as the main body.
5. Add only 2-3 user-specific applications at the end.
6. Avoid repeated books if history is available.
```

## License

MIT
