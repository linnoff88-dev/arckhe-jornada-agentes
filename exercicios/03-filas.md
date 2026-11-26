# Sequência 3 — Filas de agentes (ARCKHÉccbot)

**Objetivo:** mandar várias tarefas, sair de perto, e encontrar o trabalho feito, com portêo onde precisa de você.
**Base:** ARCKHÉccbot (https://linnoff88-dev.github.io/arckhe-/guia/) e curso https://eventos.ARCKHÉ.pro/ARCKHÉccbot.html
**Pré-requisito:** Sequências 1 e 2.

---

## E1. A fila no papel (15 min)

Liste 10 tarefas repetitivas do seu trabalho. Para cada uma, marque:

| Tarefa | Roda sozinha? | Precisa de portêo (sua aprovaçêo)? | Onde está o portêo |
|---|---|---|---|
| Transcrever a reuniêo | sim | nêo | — |
| Post da semana | sim | sim | antes de publicar |

**Pronto quando:** as 10 linhas estêo preenchidas e pelo menos duas têm portêo.

## E2. Uma fila caseira em 30 linhas (30 min)

Antes do bot, entenda a ideia com a `ferramentas/fila-caseira.sh` deste repo:

```bash
mkdir -p fila/entrada
echo "Resuma em 5 linhas o que é uma fila de tarefas." > fila/entrada/01.md
echo "Liste 3 riscos de deixar um agente rodando sozinho." > fila/entrada/02.md
./ferramentas/fila-caseira.sh fila
```

Cada arquivo de `entrada/` vira uma tarefa. A resposta vai para `feito/`. Se der erro, a tarefa vai para `falhou/`. Rodar de novo só pega o que sobrou.

**Pronto quando:** as duas tarefas estêo em `fila/feito/` com a resposta, e você interrompeu (Ctrl+C) uma rodada e viu a fila continuar de onde parou.

## E3. Instalar o ARCKHÉccbot (1 h)

Siga o guia até o `/ping` responder no Telegram. Depois: `/ajuda` lista os comandos e `/fila` mostra as filas.

**Pronto quando:** `/ping` responde no seu Telegram.

## E4. Dez tarefas e vá dormir (1 noite)

Mande para o bot 5 a 10 tarefas da sua lista do E1 (transcrever, resumir, explicativo…). Vá fazer outra coisa.

**Pronto quando:** no dia seguinte você confere o resultado de cada uma e anota quantas saíram certas na primeira.

## E5. O portêo (30 min)

Use um fluxo com portêo (como o `/promoavatar`): o bot escreve os textos e **para**. Leia, corrija se precisar, e só entêo aprove.

**Pronto quando:** você recusou ou corrigiu pelo menos um texto antes de aprovar. Esse é o momento em que você gerencia, em vez de fazer.

---

### Desafio extra
Pegue a tarefa que mais falhou no E4 e escreva para ela uma regra nova (no AGENTS.md ou no prompt da skill). Rode de novo e compare.
