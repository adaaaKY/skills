# persona-builder

A Claude Code skill that generates rich, structured UX personas as Markdown documents — ready to feed into design analysis, critique, or heuristic evaluation.

## What it does

The skill interviews you with focused questions, then produces a detailed persona document covering:

- Demographics and psychographics
- Goals, motivations, and definition of success
- Pain points, frustrations, and current workarounds
- Tech behavior, device usage, and digital fluency
- AI tool usage and comfort level
- Mental models and product expectations
- Trust signals and abandonment triggers
- Social media behavior and social proof sensitivity
- Accessibility and situational constraints
- Actionable design implications

Personas are concrete and specific — no generic filler. Every field is grounded in the product context you provide.

## How to trigger it

Use any of these phrases in Claude Code:

- `"create a persona"`
- `"build a persona for [user type]"`
- `"define my target user"`
- `"who is my user?"`
- `"I need a persona for [product]"`
- `"make a persona"`
- `"create a user profile"`

Also triggers automatically when you ask to analyze a design flow "for [type of user]" and no persona document exists yet.

## How it works

1. **Interview** — Claude asks one question at a time to gather product context, user archetype, and primary goal. Optional enrichment questions follow if needed.
2. **Generate** — A full persona document is produced using a structured template.
3. **Review** — You confirm or edit until the persona is right.
4. **Save** — Optionally save to a `.md` file in your project (e.g. `persona-marcus-webb.md`).
5. **Next steps** — Optionally pass the persona into a design flow analysis or create a second persona for comparison.

## Installation

Copy the `persona-builder/` folder into your Claude Code skills directory:

```
~/.claude/skills/persona-builder/SKILL.md
```

Or, if you're using a project-level skills setup, place it under `.claude/skills/` in your project root.

## Example output

```markdown
# Persona: Sarah Chen, 34
**Archetype:** The Efficiency Maximizer
**Product Context:** Grocery delivery app

---

## At a Glance
> "I just need it to remember what I always buy and stop asking me the same questions every week."

| Field | Detail |
|---|---|
| Age | 34 |
| Location | Chicago, IL |
| Occupation | Marketing manager |
| Life Stage | Parent of a toddler |
...
```

## License

MIT
