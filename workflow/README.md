# Workflows n8n

Workflows desenvolvidos para um projeto de automação de atendimento com Inteligência Artificial.

## Arquivos

### atendimento-ia.json

Workflow principal responsável pelo atendimento automatizado.

- Recebimento de mensagens via Webhook
- Organização dos dados recebidos
- Processamento da mensagem com Google Gemini
- Memória conversacional por sessão
- Qualificação do atendimento
- Encaminhamento de leads para o fluxo comercial

### notificacao-lead.json

Workflow responsável pelo processamento do lead encaminhado pelo atendimento.

- Recebimento dos dados do cliente
- Organização das informações
- Envio de notificação por e-mail através do Gmail

## Tecnologias

- n8n
- Google Gemini
- Webhooks
- JSON
- Gmail
- LLMs
- Automação de processos
