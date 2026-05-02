# Contributing

Thanks for wanting to improve this skill. A few notes on what's helpful.

## Issues

Open an issue if:

- A specific AI-tell phrase keeps slipping through (em dashes, "delve," curly quotes, generic positivity, etc.) — include the prompt you used and the offending output
- The skill triggers when it shouldn't, or fails to trigger when it should
- The medium-calibration feels off for a context you use often (e.g. "the caption setting still sounds too long")
- A rule contradicts another rule or is unclear

## Pull Requests

PRs welcome for:

- Adding to the AI-tell avoid list
- Refining the description block to improve trigger accuracy
- Adding before/after examples to the README
- New medium calibrations (e.g. "voice notes," "group chat replies")
- Fixing typos or formatting

For larger changes (restructuring rules, changing the voice model, adding new skills), please open an issue first to discuss.

## Skill format

This repo follows the Anthropic Claude skill convention:

- One skill per folder under `skills/`
- Each folder contains a `SKILL.md` with YAML frontmatter (`name`, `description`)
- The `description` field is what Claude uses to decide when to load the skill — keep it specific and trigger-focused

## Style of the skill itself

The skill file is written in clear, structured prose. It is NOT written in the voice it teaches — that would make it harder to read and maintain. The voice belongs in the output, not the instructions.

## Testing changes

Before submitting a PR, test the skill against at least 3 prompts across different mediums:

1. A short text (should come out loose, fragmentary)
2. A longer reflection (should come out sentence-case, more developed)
3. A formal context that should NOT trigger it (e.g. "draft a client email")

Paste the outputs in the PR description so reviewers can sanity-check.
