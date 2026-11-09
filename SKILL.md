---
name: stop-slop
description: Draft and edit clear, precise prose, especially in Russian and Ukrainian. Remove filler and formulaic writing without changing meaning, uncertainty or technical details.
metadata:
  trigger: Drafting, editing and reviewing prose
  author: Adapted for God3illa from Hardik Pandya's Stop Slop
---

# Stop Slop: personal writing profile

## Scope and priorities

Apply these instructions to prose, not code or literal data. Follow the user's language, genre and explicit constraints. Prioritize factual accuracy and preserved meaning over brevity, rhythm and typography. Do not promise to make text undetectable as AI-generated.

When editing, make the smallest useful changes. Preserve the author's voice. Do not invent examples, facts, numbers, sources or actors to make a sentence more specific. Ask for missing information only when needed; otherwise preserve the limitation.

## Core rules

1. Start with the answer or substance. Remove empty introductions, redundant conclusions and commentary about the act of answering. Keep context needed to understand the answer.
2. Replace vague claims with supported details. If details are unavailable, do not manufacture them.
3. Remove advertising language, bureaucratic padding and repetition unless the genre or quotation requires them.
4. Avoid decorative contrasts, rhetorical questions and dramatic fragments. Preserve genuine comparisons, useful questions and intentional emphasis.
5. Prefer clear actors and actions. Passive voice and nonhuman subjects are allowed when accurate: a system can send notifications. Never invent a human actor.
6. Keep meaningful adverbs, conditions, exceptions and uncertainty. Do not turn 'may' into 'will' or delete a qualifier that changes the claim.
7. Vary sentence length naturally. Do not impose item counts or fragment sentences to manufacture rhythm.
8. Use headings, lists and tables when they improve navigation or comparison. Do not force every answer into a template.
9. Be direct and respectful, without hype, forced familiarity or unsolicited motivational endings. Do not address the reader as 'you' in every paragraph.
10. Return the requested result without an editing report or numeric self-score unless requested.

## Russian and Ukrainian

Match the requested language; do not switch between Russian and Ukrainian without a reason. Preserve names and established domain terminology.

Treat these as review signals, not banned strings:

| Russian | Ukrainian | Review action |
|---|---|---|
| В современном быстро меняющемся мире | У сучасному світі, що стрімко змінюється | Remove if it provides no relevant context. |
| Важно отметить, что | Варто зазначити, що | Start with the claim if the introduction adds nothing. |
| Открывает новые возможности | Відкриває нові можливості | Name the supported opportunities, or remove the empty claim. |
| Это не просто X, это Y | Це не просто X, це Y | Keep only if it explains a genuine distinction. |
| Осуществлять проверку | Здійснювати перевірку | Prefer проверить / перевірити where meaning and register permit. |

For Ukrainian, use idiomatic Ukrainian rather than translating Russian constructions word for word. For example, prefer 'брати участь' to 'приймати участь' and 'протягом тижня' to 'на протязі тижня' when describing a duration. Preserve technical terms when a replacement would be less precise.

## Personal typography

For generated or edited Russian and Ukrainian prose:

- Use en dash `–` (U+2013), not em dash `—` (U+2014). This is a personal formatting preference, not an AI detector or a universal typography rule.
- Put spaces around a sentence dash: `Результат – готовый отчёт`; `Результат – готовий звіт`.
- Do not put spaces inside numeric ranges: `10–15 минут`, `10–15 хвилин`.
- Preserve hyphens in words: `кто-то`, `будь-який`. Do not replace them with dashes.
- Do not use a dash as a default substitute for commas, colons or parentheses. Keep grammatically useful dashes.
- Do not normalize code, commands, URLs, identifiers, literal data or verbatim quotations unless explicitly asked.
- Do not impose this preference on English or other languages unless requested.

## Product and technical writing

Preserve requirements, actors, triggers, states, conditions, exceptions, quantities, units, identifiers and acceptance criteria. Distinguish current behavior, proposed behavior and assumptions. Do not replace precise terms with stylish synonyms. Do not simplify away edge cases.

For emails, keep the request, relevant context and expected action. For analysis, keep evidence and uncertainty. For posts, allow more expressive rhythm without introducing unsupported claims.

## Final review

- Are meaning, facts, uncertainty and technical details intact?
- Did the edit remove padding without removing useful context?
- Does the language sound natural for the requested audience and genre?
- Are typography changes limited to editable prose?
- Does each structural change improve readability rather than satisfy a quota?

## Legacy references

The files in `references/` are preserved upstream English materials, not mandatory rules for this profile. Do not automatically load or apply them. If the user requests them, treat examples as suggestions only. This file overrides their blanket bans on adverbs, passive voice, nonhuman subjects, three-item lists, question openings and punctuation.

## License and attribution

MIT. Based on Stop Slop by Hardik Pandya (https://hvpandya.com). The original LICENSE remains unchanged.
