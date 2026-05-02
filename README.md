# casual-human-voice

A Claude skill for writing that sounds like a real person talking, not a language model trying to be helpful. General-purpose casual voice — flexes from texts to captions to personal blog posts to emails to friends.

## What this skill does

Strips out the AI tells (em dashes, curly quotes, "delve," neat bullet lists, generic positivity) and replaces them with the things that make writing sound human: concrete details, comma splices, sentence fragments, jokes inside sentences, and a willingness to commit to a feeling instead of hedging everything.

The voice adapts to the medium. A text about losing your keys is loose and frustrated. A caption about your dog is warm and a little dumb. A reflection on a hard day is quiet and specific. The skill is one voice with multiple settings, not a single fixed persona.

## Installation

### Option 1: Claude Code

Clone into your `~/.claude/skills/` directory:

```bash
git clone https://github.com/Object-ions/casual-human-voice-skill.git
```

The skill will be auto-discovered on next launch.

### Option 2: Claude Projects (claude.ai)

1. Open the project where you want the skill active
2. Upload `skills/casual-human-voice/SKILL.md` to the project's knowledge/files section
3. Reference it in the project's custom instructions if needed

### Option 3: Drop into any Claude-aware folder

Copy `skills/casual-human-voice/SKILL.md` into whatever folder structure your tooling expects. The frontmatter at the top makes it self-describing.

## Usage

Trigger the skill with phrases like:

- "write this like a human"
- "make it casual"
- "more conversational"
- "like i'm texting a friend"
- "less AI"

For formal contexts (client emails, compliance docs, professional writing), the skill auto-disables — see the "When This Skill Does NOT Apply" section in `SKILL.md`.

## Example outputs

The voice flexes by medium. Same input, different settings:

**Input:** "I had a long day at work and ended up burning dinner."

**As a text:**

> long day. tried to cook, set off the smoke alarm, ordered thai instead. great success.

**As a caption:**

> made dinner. dinner is now charcoal. we're getting takeout.

**As a personal blog post / journal entry:**

> Long day. The kind where you finish and realize you haven't really thought about anything outside of work in nine hours. I tried to cook because I had this idea that making dinner would feel grounding, and instead the smoke alarm went off and I just stood there for a second wondering if this was the universe being funny.

Same voice, different volume. That's the whole skill.

## Repo structure

```
casual-human-voice/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── CHANGELOG.md
├── .gitignore
└── SKILL.md
```

## Contributing

Issues and PRs welcome. If a specific AI-tell keeps slipping past the skill, or the medium-calibration feels off for a context you use a lot, open an issue with an example.

See [CONTRIBUTING.md](./CONTRIBUTING.md) for details.

## License

MIT — see [LICENSE](./LICENSE).
