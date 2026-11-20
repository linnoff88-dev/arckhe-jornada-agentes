# Jornada dos Agentes â€” do chat ao criador de agentes

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


**ðŸ‡§ðŸ‡· [PortuguÃªs](README.md) Â· ðŸ‡ºðŸ‡¸ [English](README.en.md) Â· ðŸ‡ªðŸ‡¸ [EspaÃ±ol](README.es.md)**

[![Do chat ao criador de agentes](guia/assets/banner.jpg)](https://inematds.github.io/jornada-agentes/guia/)

## O que Ã©

Este repositÃ³rio reÃºne os exercÃ­cios da sÃ©rie INEMA "Do chat ao criador de agentes". SÃ£o quatro sequÃªncias, em ordem: usar o agente no terminal, montar um assistente pessoal pelo Telegram, colocar tarefas numa fila que roda sozinha e automatizar redes sociais com aprovaÃ§Ã£o sua. Serve para quem jÃ¡ usa o chat da IA e quer que ela trabalhe por conta prÃ³pria. Cada exercÃ­cio tem um "pronto quando" que diz se vocÃª terminou. VocÃª precisa de um computador, do terminal e do Claude Code ou do Codex.

## ðŸ“– Guia de uso

Guia completo (landing + passo a passo): **https://inematds.github.io/jornada-agentes/guia/**

## As 4 sequÃªncias

A ordem importa: sem a sequÃªncia 1, as outras nÃ£o ficam de pÃ©. Sem milagre: o sistema precisa rodar correto antes de rodar sozinho.

| # | SequÃªncia | ExercÃ­cios | Base |
|---|---|---|---|
| 1 | Do chat para o terminal (OSWork) | [exercicios/01-oswork.md](exercicios/01-oswork.md) | [curso](https://inematds.github.io/oswork-quick/) Â· [Ã¡rea](https://eventos.inema.pro/oswork/) |
| 2 | Crie o seu Jarvis (INTELECTO) | [exercicios/02-jarvis.md](exercicios/02-jarvis.md) | [INTELECTO](https://inematds.github.io/intelecto/) Â· [curso](https://inematds.github.io/intelecto-curso/) Â· [Ã¡rea](https://eventos.inema.pro/jarvis/) |
| 3 | Filas de agentes (inemaccbot) | [exercicios/03-filas.md](exercicios/03-filas.md) | [guia](https://inematds.github.io/inemaccbot/guia/) Â· [curso](https://eventos.inema.pro/inemaccbot.html) |
| 4 | Redes sociais no automÃ¡tico | [exercicios/04-redes.md](exercicios/04-redes.md) | [reel7etapas](https://inematds.github.io/reel7etapas/guia/) Â· [promoavatar](https://inematds.github.io/promoavatar/guia/) Â· [promoavatar3](https://inematds.github.io/promoavatar3/guia/) Â· [finviral](https://inematds.github.io/finviral/guia/) Â· [saudeviral](https://inematds.github.io/saudeviral/guia/) Â· [advviral](https://inematds.github.io/advviral/guia/) |

PÃ¡gina da sÃ©rie: https://eventos.inema.pro/do-chat-ao-agente/

## Fila caseira

`ferramentas/fila-caseira.sh` Ã© uma fila mÃ­nima para entender a ideia antes do inemaccbot: cada arquivo em `entrada/` vira uma tarefa, a resposta vai para `feito/`, o erro vai para `falhou/`, e uma rodada interrompida retoma de onde parou.

```bash
mkdir -p fila/entrada
echo "Resuma em 5 linhas o que Ã© uma fila de tarefas." > fila/entrada/01.md
echo "Liste 3 riscos de deixar um agente rodando sozinho." > fila/entrada/02.md
./ferramentas/fila-caseira.sh fila          # motor padrÃ£o: claude
./ferramentas/fila-caseira.sh fila codex    # ou o Codex
```

## VÃ­deos

Cinco vÃ­deos (abertura + um por sequÃªncia), cada um com a sua pÃ¡gina explicativa em [serie/](https://inematds.github.io/jornada-agentes/serie/jornada-ia/) (PT/EN/ES). Roteiros: [videos/roteiros.md](videos/roteiros.md).

## Estrutura

```
exercicios/            exercÃ­cios em PT (en/ e es/ traduzidos)
ferramentas/           fila-caseira.sh
guia/                  pÃ¡gina do guia (PT, en/, es/)
videos/roteiros.md     roteiros dos 5 vÃ­deos
```

---

Tudo aberto e gratuito no **[INEMA.CLUB](https://inema.club)**.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>