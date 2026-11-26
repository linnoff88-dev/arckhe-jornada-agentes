ï»¿# Jornada dos Agentes ê¢â¬â do chat ao criador de agentes

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


**ê°Å¸â¡Â§ê°Å¸â¡Â· [PortuguêÂªs](README.md) êÂ· ê°Å¸â¡Âºê°Å¸â¡Â¸ [English](README.en.md) êÂ· ê°Å¸â¡Âªê°Å¸â¡Â¸ [EspaêÂ±ol](README.es.md)**

[![Do chat ao criador de agentes](guia/assets/banner.jpg)](https://inematds.github.io/jornada-agentes/guia/)

## O que êÂ©

Este repositêÂ³rio reêÂºne os exercêÂ­cios da sêÂ©rie INEMA "Do chat ao criador de agentes". SêÂ£o quatro sequêÂªncias, em ordem: usar o agente no terminal, montar um assistente pessoal pelo Telegram, colocar tarefas numa fila que roda sozinha e automatizar redes sociais com aprovaêÂ§êÂ£o sua. Serve para quem jêÂ¡ usa o chat da IA e quer que ela trabalhe por conta prêÂ³pria. Cada exercêÂ­cio tem um "pronto quando" que diz se vocêÂª terminou. VocêÂª precisa de um computador, do terminal e do Claude Code ou do Codex.

## ê°Å¸ââ Guia de uso

Guia completo (landing + passo a passo): **https://inematds.github.io/jornada-agentes/guia/**

## As 4 sequêÂªncias

A ordem importa: sem a sequêÂªncia 1, as outras nêÂ£o ficam de pêÂ©. Sem milagre: o sistema precisa rodar correto antes de rodar sozinho.

| # | SequêÂªncia | ExercêÂ­cios | Base |
|---|---|---|---|
| 1 | Do chat para o terminal (OSWork) | [exercicios/01-oswork.md](exercicios/01-oswork.md) | [curso](https://inematds.github.io/oswork-quick/) êÂ· [êÂ¡rea](https://eventos.inema.pro/oswork/) |
| 2 | Crie o seu Jarvis (INTELECTO) | [exercicios/02-jarvis.md](exercicios/02-jarvis.md) | [INTELECTO](https://inematds.github.io/intelecto/) êÂ· [curso](https://inematds.github.io/intelecto-curso/) êÂ· [êÂ¡rea](https://eventos.inema.pro/jarvis/) |
| 3 | Filas de agentes (inemaccbot) | [exercicios/03-filas.md](exercicios/03-filas.md) | [guia](https://inematds.github.io/inemaccbot/guia/) êÂ· [curso](https://eventos.inema.pro/inemaccbot.html) |
| 4 | Redes sociais no automêÂ¡tico | [exercicios/04-redes.md](exercicios/04-redes.md) | [reel7etapas](https://inematds.github.io/reel7etapas/guia/) êÂ· [promoavatar](https://inematds.github.io/promoavatar/guia/) êÂ· [promoavatar3](https://inematds.github.io/promoavatar3/guia/) êÂ· [finviral](https://inematds.github.io/finviral/guia/) êÂ· [saudeviral](https://inematds.github.io/saudeviral/guia/) êÂ· [advviral](https://inematds.github.io/advviral/guia/) |

PêÂ¡gina da sêÂ©rie: https://eventos.inema.pro/do-chat-ao-agente/

## Fila caseira

`ferramentas/fila-caseira.sh` êÂ© uma fila mêÂ­nima para entender a ideia antes do inemaccbot: cada arquivo em `entrada/` vira uma tarefa, a resposta vai para `feito/`, o erro vai para `falhou/`, e uma rodada interrompida retoma de onde parou.

```bash
mkdir -p fila/entrada
echo "Resuma em 5 linhas o que êÂ© uma fila de tarefas." > fila/entrada/01.md
echo "Liste 3 riscos de deixar um agente rodando sozinho." > fila/entrada/02.md
./ferramentas/fila-caseira.sh fila          # motor padrêÂ£o: claude
./ferramentas/fila-caseira.sh fila codex    # ou o Codex
```

## VêÂ­deos

Cinco vêÂ­deos (abertura + um por sequêÂªncia), cada um com a sua pêÂ¡gina explicativa em [serie/](https://inematds.github.io/jornada-agentes/serie/jornada-ia/) (PT/EN/ES). Roteiros: [videos/roteiros.md](videos/roteiros.md).

## Estrutura

```
exercicios/            exercêÂ­cios em PT (en/ e es/ traduzidos)
ferramentas/           fila-caseira.sh
guia/                  pêÂ¡gina do guia (PT, en/, es/)
videos/roteiros.md     roteiros dos 5 vêÂ­deos
```

---

Tudo aberto e gratuito no **[INEMA.CLUB](https://inema.club)**.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>