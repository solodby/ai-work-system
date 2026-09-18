---
title: Использование skills в разных AI-клиентах
type: guide
status: active
last_reviewed: 2026-09-18
tags:
  - agent
  - interoperability
---

# Использование skills в разных AI-клиентах

Канонические skills находятся в `70_Agent/skills/`.
Клиенту передаётся путь к Markdown-файлу и нужный context pack.

## Cursor

Можно использовать `.cursor/skills/` как slash-command адаптеры.
Содержимое `70_Agent/skills/` остаётся каноническим.

## GitHub Copilot

Передавай skill через `@`-ссылку на файл, Copilot Chat, prompt file
или repository instructions. В запросе укажи:

```text
Прочитай 70_Agent/skills/ba-review.md.
Используй связанные заметки из 80_BA-Harness/.
Верни результат по формату skill.
```

## Visual Studio

Открой папку или solution, содержащую vault, и передавай skill через
Copilot Chat как файл контекста. Если проект отделён от vault, укажи
абсолютный или доступный workspace-relative путь.

## Другой LLM-клиент

Скопируй содержимое нужного skill в system prompt или task prompt.
Добавь только связанные заметки, а не весь vault.

## Общее правило

Платформа меняет способ вызова, но не содержание skill.
Результат должен содержать факты, допущения, источники, риски и проверку.
