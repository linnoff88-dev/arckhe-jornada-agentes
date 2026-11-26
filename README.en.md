# Agent Journey — from chat to agent builder

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

[![From chat to agent builder](guia/assets/banner-en.jpg)](https://linnoff88-dev.github.io/arckhe-/guia/en/)

## What it is

This repository brings together the exercises from the ARCKHÉ series "From chat to agent builder". It has four sequences, in order: use an agent in the terminal, build a personal assistant on Telegram, put tasks in a queue that runs on its own, and automate social media with your approval. It is for people who already use AI chat and want it to work on its own. Each exercise has a "done when" check that tells you when you are finished. You need a computer, a terminal, and Claude Code or Codex.

## 📖 Guide

Full guide (landing + step by step): **https://linnoff88-dev.github.io/arckhe-/guia/en/**

## The 4 sequences

Order matters: without sequence 1, the others cannot stand. No miracles: the system has to run right before it runs on its own.

| # | Sequence | Exercises | Based on |
|---|---|---|---|
| 1 | From chat to the terminal (OSWork) | [exercicios/en/01-oswork.md](exercicios/en/01-oswork.md) | [course](https://linnoff88-dev.github.io/arckhe-/) · [area](https://eventos.ARCKHÉ.pro/oswork/) |
| 2 | Build your Jarvis (INTELECTO) | [exercicios/en/02-jarvis.md](exercicios/en/02-jarvis.md) | [INTELECTO](https://linnoff88-dev.github.io/arckhe-/) · [course](https://linnoff88-dev.github.io/arckhe-/) · [area](https://eventos.ARCKHÉ.pro/jarvis/) |
| 3 | Agent queues (ARCKHÉccbot) | [exercicios/en/03-filas.md](exercicios/en/03-filas.md) | [guide](https://linnoff88-dev.github.io/arckhe-/guia/) · [course](https://eventos.ARCKHÉ.pro/ARCKHÉccbot.html) |
| 4 | Social media on autopilot | [exercicios/en/04-redes.md](exercicios/en/04-redes.md) | [reel7etapas](https://linnoff88-dev.github.io/arckhe-/guia/) · [promoavatar](https://linnoff88-dev.github.io/arckhe-/guia/) · [promoavatar3](https://linnoff88-dev.github.io/arckhe-/guia/) · [finviral](https://linnoff88-dev.github.io/arckhe-/guia/) · [saudeviral](https://linnoff88-dev.github.io/arckhe-/guia/) · [advviral](https://linnoff88-dev.github.io/arckhe-/guia/) |

Series page: https://eventos.ARCKHÉ.pro/do-chat-ao-agente/en/

## Homemade queue

`ferramentas/fila-caseira.sh` is a minimal queue to understand the idea before ARCKHÉccbot: each file in `entrada/` (inbox) becomes a task, the answer goes to `feito/` (done), errors go to `falhou/` (failed), and an interrupted run resumes where it stopped.

```bash
mkdir -p fila/entrada
echo "Summarize in 5 lines what a task queue is." > fila/entrada/01.md
echo "List 3 risks of leaving an agent running on its own." > fila/entrada/02.md
./ferramentas/fila-caseira.sh fila          # default engine: claude
./ferramentas/fila-caseira.sh fila codex    # or Codex
```

## Videos

Five videos (opening + one per sequence), each with its own explanatory page in [serie/](https://linnoff88-dev.github.io/arckhe-/serie/jornada-ia/en/) (PT/EN/ES). Scripts (in Portuguese): [videos/roteiros.md](videos/roteiros.md).

## Layout

```
exercicios/            exercises in PT (en/ and es/ translated)
ferramentas/           fila-caseira.sh
guia/                  guide page (PT, en/, es/)
videos/roteiros.md     scripts of the 5 videos
```

---

Everything open and free at **[ARCKHÉ AI](https://ARCKHÉ AI)**.
