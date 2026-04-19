---
title: ⚡️ Управление версиями. Git.
summary: Информация об управлении версиями. Git.
date: 2026-02-14
authors:
  - me
tags:
  - Hugo Blox
  - Jupyter
  - Open Science
  - Tutorials
cover:
  # image: cover.jpg  # Auto-detected from cover image in this folder
  icon:
    name: "📔"
image:
  caption: "Image credit: [HugoBlox](https://hugoblox.com)"
  focal_point: Center
  placement: 1
content_meta:
  trending: true
---
{{< toc mobile_only=true is_open=true >}}

> [!TIP]
> **Git — это не просто резервное копирование.** Git позволяет экспериментировать без страха сломать работающий код. Создали ветку — сломали? Удалили ветку, и ничего не случилось.

- **Полная история** – Каждая строчка кода имеет автора, дату и причину изменения.
- **Без папок `_v2_final`** – Больше никогда не создавайте копии проекта с именами `script_final_3_реально_последнее`.
- **Работайте параллельно** – 10 разработчиков спокойно правят один проект. Ветки не пересекаются, пока вы сами их не сольёте.
- **Откат в один клик** – Ошиблись? `git revert` — и всё снова работает.

## Основные команды Git

| Команда | Что делает |
| :--- | :--- |
| `git init` | Создать новый репозиторий в текущей папке |
| `git clone <url>` | Скачать готовый репозиторий с GitHub/GitLab |
| `git status` | Посмотреть, какие файлы изменены |
| `git add <file>` | Подготовить файл к коммиту |
| `git commit -m "сообщение"` | Сохранить снимок изменений |
| `git push` | Отправить коммиты на удалённый сервер |
| `git pull` | Забрать свежие изменения с сервера |
| `git log --oneline` | Показать историю коммитов кратко |

## Как начать использовать Git

1. **Установите Git.**  
   – Windows: [git-scm.com](https://git-scm.com)  
   – macOS: `brew install git`  
   – Linux: `sudo apt install git`

2. **Представьтесь системе.** Git подписывает каждый ваш коммит:
   ```bash
   git config --global user.name "Ваше Имя"
   git config --global user.email "you@example.com"
