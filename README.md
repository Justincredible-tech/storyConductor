# Story Conductor

A context-driven protocol for AI-assisted long-form writing.

## The Problem

Writing novels with LLMs is hard. They forget character details, drop plot threads, and hallucinate facts mid-story. Every new session risks continuity errors.

## The Solution

**The Story Conductor Protocol** treats your novel like a software codebase. It enforces a structured "story database" that the AI must read before writing and update after every scene.

### Key Features

- **Lore-Lock System** - Forces the AI to explicitly load relevant context before generating any prose
- **Fact Harvesting** - Automatically extracts and saves new details after each writing session
- **Ripple Effect Protocol** - Tracks continuity changes and flags scenes that need revision
- **Session Recovery** - Allows any AI instance to pick up exactly where the last one left off

## Quick Start

1. Create a `.story-system/` folder in your project
2. Set up the required files (characters, locations, outline, style guide)
3. Copy the system prompt from `storyConductor.md` into your AI session
4. Start writing with persistent context

## File Structure

```
.story-system/
├── thome.md            # Core premise, themes, logline
├── style.md            # Voice, tense, POV, constraints
├── characters/         # One file per character
├── locations/          # One file per setting
├── outline.md          # Master chapter/scene ledger
├── ripples.md          # Continuity change log
└── active-work/        # Current writing workspace
```

## Compatible With

- Claude
- ChatGPT
- Gemini
- DeepSeek
- Any LLM that accepts system prompts

## Documentation

See [storyConductor.md](storyConductor.md) for the complete protocol and system prompt.

## License

MIT
