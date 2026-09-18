---
title: Универсальная работа с агентами
type: guide
status: active
last_reviewed: 2026-09-18
tags:
  - agent
  - interoperability
---

# Универсальная работа с агентами

Основные skills хранятся в `70_Agent/skills/` как обычные Markdown-файлы.
Они не привязаны к Cursor, Copilot, Visual Studio или конкретной модели.

Любой агент может использовать skill, если ему передать:

1. путь к skill;
2. связанные заметки;
3. задачу;
4. ограничения;
5. ожидаемый формат результата.

## Платформенные адаптеры

- `.cursor/skills/` - короткие адаптеры для Cursor;
- GitHub Copilot - использует этот vault через `@`-ссылки, prompt files
  или custom instructions;
- Visual Studio - использует те же файлы через Solution/Workspace context
  и Copilot Chat;
- любой другой LLM - получает skill как Markdown-инструкцию в prompt.

Каноническая версия всегда находится в `70_Agent/skills/`.
Платформенные файлы не должны содержать отдельную противоречащую методику.

## Универсальный способ вызова

```text
Прочитай 70_Agent/skills/ba-review.md.
Прочитай 80_BA-Harness/05_Validation.md
и связанные заметки проекта.
Выполни skill для указанной задачи.
Верни результат в формате, описанном в skill.
```
