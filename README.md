# ten-line-summarizer

An [Agent Skill](https://agentskills.io) that condenses any document into
**10 lines or fewer** — faithfully, without adding outside information.

---

## What it does

When a user shares a document (pasted text, PDF, Word file, article, report,
or notes) and asks for a summary, the skill instructs the agent to produce a
plain-text summary of up to 10 lines. Each line is one short sentence. The
first line states what the document is about; the remaining lines cover the
key points, conclusions, important numbers, decisions, and action items found
in the document.

The skill enforces three hard rules:

1. **Never exceed 10 lines.**
2. **Never add facts, opinions, or outside knowledge.**
3. **Never summarize a document it cannot read — it must tell the user instead.**

## Who it is for

- University students who need a quick overview before reading in full
- Business owners reviewing long reports or contracts
- Professionals who want a rapid grasp of articles, memos, or meeting notes

## Folder structure

```
ten-line-summarizer/
├── SKILL.md               # Required — metadata and instructions
├── references/
│   └── examples.md        # Good and bad summary examples
├── README.md              # This file
└── LICENSE                # MIT licence
```

## How to install

1. Copy the `ten-line-summarizer/` folder into your skills directory
   (the location depends on your agent client — check its documentation).
2. Restart or reload your agent so it picks up the new skill.
3. Test it by saying: **"Summarize this document"** and pasting any text.

Supported agent clients are listed at
[agentskills.io/clients](https://agentskills.io/clients).

## How to validate

If you have Python and `pip` available, you can validate the skill with the
official reference library:

```bash
pip install skills-ref
skills-ref validate ./ten-line-summarizer
```

The validator checks that:
- `SKILL.md` is present
- The frontmatter is valid YAML
- `name` follows the naming rules (lowercase, hyphens, no consecutive
  hyphens, matches the folder name)
- `description` is within the 1 024-character limit

If you do not have Python, you can check the rules manually:
- Open `SKILL.md` and confirm the frontmatter block is fenced with `---`.
- Confirm `name: ten-line-summarizer` matches the folder name exactly.
- Count the `description` value — it must be 1 024 characters or fewer and
  must not contain bare colons at the start of a line (which would break
  the YAML parser).

## Trigger phrases

The skill is designed to activate when the user says things like:
- "Summarize this document"
- "Give me the short version"
- "TL;DR this in 10 lines"

## License

MIT — see [LICENSE](LICENSE).
