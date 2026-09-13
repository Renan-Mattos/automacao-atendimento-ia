# Automação de Atendimento com IA

Projeto de automação de atendimento desenvolvido com n8n, Google Gemini e integração com Gmail.

## Objetivo

Criar um fluxo automatizado capaz de receber mensagens de clientes, compreender suas necessidades, manter o contexto da conversa e realizar a qualificação de leads interessados em solicitar um orçamento.

## Arquitetura

```text
Cliente
   ↓
Webhook
   ↓
Organização dos dados
   ↓
AI Agent + Google Gemini
   ↓
Memória conversacional
   ↓
Qualificação do cliente
   ↓
Solicitação de orçamento
   ↓
Workflow de notificação
   ↓
Gmail
