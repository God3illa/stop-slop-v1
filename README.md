# Stop Slop: personal RU/UK profile

A personal adaptation of [Hardik Pandya's Stop Slop](https://github.com/hardikpandya/stop-slop), focused on clear Russian and Ukrainian prose and product/technical writing.

## Model compatibility

The editorial instructions are model-independent: provide them to Claude, Gemini, ChatGPT or Grok as text. No model-specific code is required. This describes how to supply the instructions, not a claim that every model has been tested or will follow every rule equally well.

Distinguish the model from the application running it. The application determines whether it can load files, install skills, persist custom instructions or read a workspace. Do not assume that a model name implies support for automatic discovery of `SKILL.md`, `GEMINI.md` or `AGENTS.md`.

## Goals

Remove filler and formulaic writing without erasing meaning, uncertainty, authorial voice or technical precision. These are editorial preferences, not a validated quality benchmark or an AI-detection bypass.

## Files

- `SKILL.md`: primary, self-contained instructions for any model. Use this as the source of truth.
- `GEMINI.md`: compact, standalone instructions usable with any model. The filename is historical, not a Gemini requirement or restriction. It is not an automatic-loading guarantee.
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

## Universal quick start: Claude, Gemini, ChatGPT and Grok

1. Open `SKILL.md` on GitHub or locally.
2. Copy the Markdown instructions after the YAML metadata block into the chat before your task. Alternatively, use the compact instructions after the separator in `GEMINI.md`.
3. Ask the model to apply them to the supplied text.
4. Check the result against the manual checks below.

Downloading the repository is optional for this copy-and-paste workflow. A repository URL alone does not ensure that the model has read the files. Instructions supplied in one chat should not be assumed to persist in other chats or applications.

Example task after supplying the instructions:

```text
Применяй переданные редакторские правила к этому заданию.
Отредактируй текст. Сохрани смысл, ограничения, термины и степень уверенности.
Используй тире – в обычном русском и украинском тексте.
Покажи только итоговый текст.

[текст]
```

## Persistent setup and file-based workflows

- If your application offers persistent custom or project instructions, place the editorial instructions there within its limits. Check that they apply to the conversation and selected model.
- If file attachments are available, attach `SKILL.md` and explicitly ask the model to read and apply it. Uploading a file does not by itself mean it is treated as standing instructions.
- In a skill-aware agent, install the directory according to that application's documented skill mechanism. Do not assume every Claude, Gemini, ChatGPT or Grok interface supports skills.
- For API workflows, supply the editorial instructions using the instruction role supported by the selected API. This repository provides prompt content, not provider-specific API integration code.
- These preferences do not override higher-priority application instructions or safety requirements. Context limits and application behavior can affect compliance.

## Abacus AI Desktop and other multi-model agents

The same editorial content can be supplied regardless of the selected model. Configure it in the host application; do not rely on the model name or file name to activate it.

For an explicit local-file workflow, clone or download this repository, open or grant access to its directory, then send:

```text
Прочитай SKILL.md в доступной папке stop-slop-v1 и применяй его
как редакторские инструкции для написания и редактирования текстов
в этой сессии. Не загружай references/ автоматически.
Если файл недоступен, сообщи об этом, не утверждай, что прочитал его.
```

Adjust the path to the actual location. Merely downloading the repository does not activate the rules. For automatic or persistent loading, follow the current documentation of your installed application. Recheck the configuration when starting a new session or switching models; do not assume instructions transfer automatically.

## Manual regression checks

These are checks to run, not claims of completed model evaluation. Test each model/application combination separately on both Russian and Ukrainian texts.

1. Input: `Функция временно недоступна.` Keep `временно`: it carries meaning.
2. Input: `Система отправляет уведомление после оплаты.` Keep the accurate nonhuman actor.
3. Input: `Возможно, изменение снизит число ошибок.` Do not turn a hypothesis into a proven result.
4. Editable prose: `Результат — готовый отчёт.` Expected typography: `Результат – готовый отчёт.`
5. Preserve `кто-то`, `будь-який`, command flags, URLs and verbatim quotations.
6. Input with three real requirements: preserve all three; do not delete one for rhythm.
7. Input: `Перевірка триватиме на протязі тижня.` Suggested edit: `Перевірка триватиме протягом тижня.`
8. Input: `Сервис открывает новые возможности.` Do not invent which opportunities; flag the missing detail if the task permits comments.

Compare original and edited text for factual fidelity first, style second. A model saying it read the rules is not a substitute for checking its output. Prompt instructions improve guidance but are not a deterministic typography validator.

## Attribution and license

Original author: [Hardik Pandya](https://hvpandya.com). Personal adaptation for God3illa. MIT; see `LICENSE`.
