# Good and bad summary examples

Use these examples to calibrate what a correct output looks like.

---

## Example 1 — Business report (good summary)

**Document excerpt (abridged):**
> "Q3 2026 results showed revenue of $4.2 million, up 18% year-on-year.
> Operating costs increased by 6% due to new hires. The board approved
> expansion into three new markets: Brazil, India, and Germany. Product B
> was discontinued after declining sales for two consecutive quarters.
> The next board meeting is scheduled for 15 January 2027."

**Good summary (7 lines):**
```
This document is the Q3 2026 financial and strategic report for the company.
Revenue reached $4.2 million, an 18% increase compared to the same quarter last year.
Operating costs rose 6% because of new staff hired during the quarter.
The board approved expansion into Brazil, India, and Germany.
Product B has been discontinued following two quarters of declining sales.
The next board meeting is scheduled for 15 January 2027.
No further decisions or action items are recorded in the report.
```

---

## Example 2 — Academic article (good summary)

**Document excerpt (abridged):**
> "This study examined the effect of sleep deprivation on short-term memory
> in adults aged 18–35. Participants who slept fewer than six hours showed
> a 23% reduction in recall accuracy on standardised tests. The authors
> recommend that workplace wellness programmes include sleep-hygiene
> education."

**Good summary (4 lines):**
```
This document is a research study on sleep deprivation and short-term memory in young adults.
Participants sleeping fewer than six hours showed a 23% drop in memory recall accuracy.
The study population was adults aged 18 to 35.
The authors recommend adding sleep-hygiene education to workplace wellness programmes.
```

---

## Example 3 — Bad summary (violations marked)

**Bad output:**
```
This report covers Q3 results.                          ← too vague for line 1
The company is doing well overall.                      ← opinion not in document
Revenue was strong thanks to a booming economy.         ← "booming economy" not in document
Competitors may be affected by the same trends.         ← outside speculation
The next quarter will likely be better.                 ← prediction not in document
```

**Why it fails:**
- Line 1 does not state what the document is about specifically enough.
- Lines 2–5 add opinions, outside knowledge, and speculation not found in
  the source document.

---

## Example 4 — Unreadable document (correct response)

**Situation:** The user says "summarize this PDF" but no file is attached
or the file cannot be opened.

**Correct agent response:**
```
I cannot read the document you mentioned. Please paste the text directly
into the chat or share a file I can open, and I will summarize it for you.
```

This is not a summary — it is an honest refusal. The skill requires that
the agent read the actual content before summarizing.
