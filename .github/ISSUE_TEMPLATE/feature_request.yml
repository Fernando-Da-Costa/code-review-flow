---
name: "Solicitação de funcionalidade"
description: "Sugira uma nova funcionalidade ou melhoria para o projeto."
title: "[Feature] <Título da funcionalidade>"
labels: [feature, needs-review]
assignees: ''
---

## 🎯 Descrição
Descreva claramente o que você deseja implementar ou melhorar.

## 📋 Checklist Técnico
- [ ] Item 1
- [ ] Item 2

## 💡 Motivação
Explique por que essa funcionalidade é útil ou necessária.

## 🔗 Relacionamentos
Se aplicável, relacione com PRs ou outras issues.


# README.md
# Code Review Flow 🚀

Este projeto implementa um fluxo automatizado de revisão de Pull Requests utilizando:
- GitHub Projects (Kanban)
- GitHub Actions (automatizações)
- Slack (notificações)

## Fluxo
1. Dev abre um PR → é automaticamente rotulado como `needs-review`
2. O PR aparece no board (coluna "Aguardando revisão")
3. Um revisor se atribui ao PR e move para "Em revisão"
4. Após revisão, move para "Aprovado" ou "Mudanças solicitadas"
5. Após aprovação e CI OK, pode ser feito o merge

## Requisitos
- Pelo menos 1 aprovação obrigatória no PR
- Testes e lint devem passar
- PRs são rastreados em um Project Board Kanban

## Configurações necessárias
- Criar secret `SLACK_WEBHOOK_URL` com o webhook do Slack
- Editar `.github/CODEOWNERS` para sua equipe real
- Customizar scripts `npm run lint` e `npm test` conforme seu stack

## Labels usadas
- `needs-review`
- `in-review`
- `changes-requested`
- `approved`

## Project Board
Configure um Project (beta) com colunas e automações:
- Aguardando revisão ← `needs-review`
- Em revisão ← `in-review`
- Mudanças solicitadas ← `changes-requested`
- Aprovado ← `approved`

---