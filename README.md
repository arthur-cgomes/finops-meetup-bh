# Agent FinOps — ClubPetro

Apresentação web utilizada no **Brasil FinOps Foundation Meetup · Belo Horizonte/MG**, em **11 de maio de 2026**.

## Sobre

`index.html` é um arquivo HTML auto-contido que funciona como deck de slides interativo para a palestra **"O futuro da operação Cloud é agêntico"**. A apresentação conta como a ClubPetro construiu um Agent de FinOps apoiado por agentes de Engenharia e SRE, rodando sobre a plataforma open source **OpenClaw** com modelos Claude (Sonnet), integrado à GCP e ao Discord.

## Estrutura dos slides (15 slides)

| # | Seção | Conteúdo |
|---|-------|----------|
| 001 | Hero | Título, stack (OpenClaw · Claude · GCP) e dados do evento |
| 002 | ClubPetro | Apresentação da empresa |
| 003 | Ponto de partida | O cenário antes do Agent — gastos sem revisão, time pequeno, sem cultura de FinOps |
| 004 | Conceito | As três Personas de FinOps (FinOps Engineer, Engenharia, Produto) |
| 005 | Arquitetura | Como o Agent FinOps enxerga o ambiente real na GCP |
| 006 | Agent FinOps | O Agent central e os dois agentes de suporte (Engenharia e SRE) |
| 007 | Skills | Skills instaladas no OpenClaw (finops, gcp-cud-advisor, google-cloud, data-analyst) |
| 008 | Como funciona | Linguagem natural → ação em tempo real via Discord |
| 009 | Como funciona | Exemplos de notificações vivas geradas pelo Agent |
| 010 | Segurança e Infraestrutura | Governança: VM isolada na GCP, Service Accounts read-only, validação humana |
| 011 | Stack e Status | Por que OpenClaw + Claude Sonnet; status piloto em produção |
| 012 | Resultado · Impacto | Ganhos reais de produtividade para FinOps |
| 013 | Resultado · Dashboard | Custo por SKU, distribuição por projeto, evolução por mês e justificativas de desvio em tela única |
| 014 | Encerramento | Considerações finais |
| 015 | Quem fala | Speaker e abertura para perguntas |

## Como usar

Abra `index.html` diretamente no navegador. A navegação é feita com **scroll** (scroll-snap por slide) ou pelas setas do teclado. Nenhuma dependência externa além de fontes do Google Fonts (Inter Tight, Fraunces, JetBrains Mono).

## Docker

O `Dockerfile` incluso permite servir a apresentação via container:

```bash
docker build -t finops-meetup .
docker run -p 8080:80 finops-meetup
```

Acesse em `http://localhost:8080`.

## Stack da apresentação

- HTML/CSS/JS puro, sem frameworks
- Fontes: Inter Tight · Fraunces · JetBrains Mono (Google Fonts)
- Animações CSS com scroll-snap nativo
- Design dark com paleta laranja (#ff6a1a) sobre fundo #0a0a0b

## Evento

**Brasil FinOps Foundation Meetup**
Belo Horizonte, MG · 11 maio 2026 · 18:00 (Brasília) · In-Person
