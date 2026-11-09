# Stop Slop: personal RU/UK profile

A personal adaptation of [Hardik Pandya's Stop Slop](https://github.com/hardikpandya/stop-slop), focused on clear Russian and Ukrainian prose, Gemini use and product/technical writing.

## Goals

Remove filler and formulaic writing without erasing meaning, uncertainty, authorial voice or technical precision. These are editorial preferences, not a validated quality benchmark or an AI-detection bypass.

## Files

- `SKILL.md`: primary, self-contained writing and editing instructions.
- `GEMINI.md`: compact, standalone instructions to paste into a Gemini workflow or provide with a task. No native skill support is required.
- `references/`: preserved upstream English references. Their blanket prohibitions are not binding on this profile and they should not be loaded automatically.
- `CHANGELOG.md`: upstream history preserved as inherited.
- `LICENSE`: original MIT license, unchanged.

## Main changes from upstream

- Meaning and precision take priority over brevity and rhythm.
- No blanket bans on adverbs, passive voice, nonhuman subjects or three-item lists.
- Russian and Ukrainian review examples, with idiomatic Ukrainian guidance.
- Personal typography: `–` rather than `—` in editable Russian and Ukrainian prose; preserve word hyphens and protect code, commands, URLs, identifiers, data and verbatim quotes.
- Preserve conditions, exceptions, uncertainty and acceptance criteria in product and technical texts.
- No arbitrary scoring threshold or forced reader address.

## Usage

For Gemini, supply the instructions from `GEMINI.md` in your chosen interface, then provide the task and text. Do not assume that sharing the repository URL automatically loads its instructions. For skill-aware tools, use `SKILL.md` according to that tool's instructions. For other LLM workflows, provide `SKILL.md` as editorial guidance.

Example task:

```text
Отредактируй текст по этим правилам. Сохрани смысл, ограничения, термины и степень уверенности. Покажи только итоговый текст.

[текст]
```

## Manual regression checks

These are checks to run, not claims of completed model evaluation.

1. Input: `Функция временно недоступна.` Keep `временно`: it carries meaning.
2. Input: `Система отправляет уведомление после оплаты.` Keep the accurate nonhuman actor.
3. Input: `Возможно, изменение снизит число ошибок.` Do not turn a hypothesis into a proven result.
4. Editable prose: `Результат — готовый отчёт.` Expected typography: `Результат – готовый отчёт.`
5. Preserve `кто-то`, `будь-який`, command flags, URLs and verbatim quotations.
6. Input with three real requirements: preserve all three; do not delete one for rhythm.
7. Input: `Перевірка триватиме на протязі тижня.` Suggested edit: `Перевірка триватиме протягом тижня.`
8. Input: `Сервис открывает новые возможности.` Do not invent which opportunities; flag the missing detail if the task permits comments.

Compare original and edited text for factual fidelity first, style second. Test separately on Russian and Ukrainian, and on each model/workflow you use.

## Attribution and license

Original author: [Hardik Pandya](https://hvpandya.com). Personal adaptation for God3illa. MIT; see `LICENSE`.
