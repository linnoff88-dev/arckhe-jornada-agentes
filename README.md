ï»¿# Jornada dos Agentes ê¢â¬â do chat ao criador de agentes

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


**ê°Å¸â¡Â§ê°Å¸â¡Â· [PortuguêÂªs](README.md) êÂ· ê°Å¸â¡Âºê°Å¸â¡Â¸ [English](README.en.md) êÂ· ê°Å¸â¡Âªê°Å¸â¡Â¸ [EspaêÂ±ol](README.es.md)**

[![Do chat ao criador de agentes](guia/assets/banner.jpg)](https://linnoff88-dev.github.io/arckhe-/guia/)

## O que êÂ©

Este repositêÂ³rio reêÂºne os exercêÂ­cios da sêÂ©rie ARCKHÉ "Do chat ao criador de agentes". SêÂ£o quatro sequêÂªncias, em ordem: usar o agente no terminal, montar um assistente pessoal pelo Telegram, colocar tarefas numa fila que roda sozinha e automatizar redes sociais com aprovaêÂ§êÂ£o sua. Serve para quem jêÂ¡ usa o chat da IA e quer que ela trabalhe por conta prêÂ³pria. Cada exercêÂ­cio tem um "pronto quando" que diz se vocêÂª terminou. VocêÂª precisa de um computador, do terminal e do Claude Code ou do Codex.

## ê°Å¸ââ Guia de uso

Guia completo (landing + passo a passo): **https://linnoff88-dev.github.io/arckhe-/guia/**

## As 4 sequêÂªncias

A ordem importa: sem a sequêÂªncia 1, as outras nêÂ£o ficam de pêÂ©. Sem milagre: o sistema precisa rodar correto antes de rodar sozinho.

| # | SequêÂªncia | ExercêÂ­cios | Base |
|---|---|---|---|
| 1 | Do chat para o terminal (OSWork) | [exercicios/01-oswork.md](exercicios/01-oswork.md) | [curso](https://linnoff88-dev.github.io/arckhe-/) êÂ· [êÂ¡rea](https://eventos.ARCKHÉ.pro/oswork/) |
| 2 | Crie o seu Jarvis (INTELECTO) | [exercicios/02-jarvis.md](exercicios/02-jarvis.md) | [INTELECTO](https://linnoff88-dev.github.io/arckhe-/) êÂ· [curso](https://linnoff88-dev.github.io/arckhe-/) êÂ· [êÂ¡rea](https://eventos.ARCKHÉ.pro/jarvis/) |
| 3 | Filas de agentes (ARCKHÉccbot) | [exercicios/03-filas.md](exercicios/03-filas.md) | [guia](https://linnoff88-dev.github.io/arckhe-/guia/) êÂ· [curso](https://eventos.ARCKHÉ.pro/ARCKHÉccbot.html) |
| 4 | Redes sociais no automêÂ¡tico | [exercicios/04-redes.md](exercicios/04-redes.md) | [reel7etapas](https://linnoff88-dev.github.io/arckhe-/guia/) êÂ· [promoavatar](https://linnoff88-dev.github.io/arckhe-/guia/) êÂ· [promoavatar3](https://linnoff88-dev.github.io/arckhe-/guia/) êÂ· [finviral](https://linnoff88-dev.github.io/arckhe-/guia/) êÂ· [saudeviral](https://linnoff88-dev.github.io/arckhe-/guia/) êÂ· [advviral](https://linnoff88-dev.github.io/arckhe-/guia/) |

PêÂ¡gina da sêÂ©rie: https://eventos.ARCKHÉ.pro/do-chat-ao-agente/

## Fila caseira

`ferramentas/fila-caseira.sh` êÂ© uma fila mêÂ­nima para entender a ideia antes do ARCKHÉccbot: cada arquivo em `entrada/` vira uma tarefa, a resposta vai para `feito/`, o erro vai para `falhou/`, e uma rodada interrompida retoma de onde parou.

```bash
mkdir -p fila/entrada
echo "Resuma em 5 linhas o que êÂ© uma fila de tarefas." > fila/entrada/01.md
echo "Liste 3 riscos de deixar um agente rodando sozinho." > fila/entrada/02.md
./ferramentas/fila-caseira.sh fila          # motor padrêÂ£o: claude
./ferramentas/fila-caseira.sh fila codex    # ou o Codex
```

## VêÂ­deos

Cinco vêÂ­deos (abertura + um por sequêÂªncia), cada um com a sua pêÂ¡gina explicativa em [serie/](https://linnoff88-dev.github.io/arckhe-/serie/jornada-ia/) (PT/EN/ES). Roteiros: [videos/roteiros.md](videos/roteiros.md).

## Estrutura

```
exercicios/            exercêÂ­cios em PT (en/ e es/ traduzidos)
ferramentas/           fila-caseira.sh
guia/                  pêÂ¡gina do guia (PT, en/, es/)
videos/roteiros.md     roteiros dos 5 vêÂ­deos
```

---

Tudo aberto e gratuito no **[ARCKHÉ AI](https://ARCKHÉ AI)**.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>