---
name: ten-line-summarizer
description: >-
  Summarizes any document — pasted text, PDF, Word file, article, report, or
  notes — into a maximum of 10 plain-text lines. Each line is one short
  sentence. The first line states what the document is about; the remaining
  lines cover key points, main conclusions, important numbers, decisions, and
  action items drawn only from the document itself. Use this skill whenever the
  user asks for a short summary, says "summarize this document", "give me the
  short version", or "tldr this in 10 lines". It is NOT for translating,
  editing, or rewriting documents, NOT for generating any content that is not
  in the source material, and NOT for summarizing content the agent cannot
  actually read or access.
license: MIT
---

## When to use this skill

Activate this skill when the user:
- pastes or attaches a document and asks for a summary
- says phrases like "summarize this", "give me the short version", or
  "tldr this in 10 lines"
- wants a quick overview of a long report, article, contract, essay, or set
  of notes

Do NOT activate this skill to translate, edit, rewrite, fact-check, or
extend a document with outside information.

## What to gather first

Before summarizing, confirm you have the following:

1. **The document itself** — pasted text, an uploaded file (PDF, DOCX, TXT,
   etc.), or a URL whose content you can read. If the document cannot be
   read or accessed, tell the user immediately instead of guessing.
2. **An optional focus area** — ask only if the user has not already stated
   one. Examples the user might mention:
   - key dates or deadlines
   - action items or next steps
   - financial figures or statistics
   - decisions made
   If no focus is requested, produce a balanced summary of the whole document.

## Step-by-step process

1. **Read the entire document.** Do not skim. Make sure you can access all
   of it before proceeding.
2. **Identify the document's purpose.** One sentence that captures what the
   document is and what it is trying to communicate.
3. **Extract the most important content.** In priority order:
   - the main argument, finding, or purpose
   - supporting key points
   - important numbers, dates, or names
   - conclusions or recommendations
   - decisions made
   - action items or next steps
4. **Draft up to 10 lines.** Line 1 must state what the document is about.
   Lines 2–10 cover the content identified in step 3, in order of
   importance. Stop when you have captured the essential content or when you
   reach 10 lines, whichever comes first.
5. **Check every line against the source.** Remove or rewrite any line that
   adds facts, opinions, or knowledge not present in the document.
6. **Count the lines.** If you have more than 10, cut the least important
   ones until you are at 10 or fewer.
7. **Output the summary.** Plain text only — no headings, no bullet
   symbols, no numbering, no introduction ("Here is your summary:"), and
   no closing remark.

## Output format

- Plain text, one sentence per line
- 10 lines maximum under all circumstances
- Line 1: a single sentence stating what the document is about
- Lines 2–10: key points, conclusions, numbers, decisions, and action items
  found in the document
- No markdown, no headings, no bullet points, no preamble, no sign-off

See [examples of good and bad summaries](references/examples.md) for
guidance.

## Hard rules — never break these

- Never exceed 10 lines.
- Never add facts, opinions, or outside knowledge not present in the
  document.
- Never rewrite, edit, paraphrase beyond capturing meaning, or translate
  the document.
- If you cannot read or access the document, tell the user clearly instead
  of producing a guess.
- Do not include headings, bullet points, numbered lists, introductions, or
  closing remarks in the output.
