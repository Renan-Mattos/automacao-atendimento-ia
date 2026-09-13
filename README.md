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
## Funcionamento

O projeto é dividido em dois workflows.

### 1. Atendimento IA

Workflow responsável pelo atendimento inicial ao cliente.

- Recebe mensagens através de Webhook
- Organiza os dados recebidos em JSON
- Processa as mensagens utilizando Google Gemini
- Mantém memória da conversa por sessão
- Identifica a necessidade do cliente
- Realiza a qualificação do atendimento
- Solicita dados para orçamento quando necessário
- Encaminha o lead para o workflow de notificação

### 2. Notificação de Lead

Workflow responsável pelo processamento do lead encaminhado pelo atendimento.

- Recebe os dados do cliente
- Organiza as informações recebidas
- Processa os dados do lead
- Gera uma mensagem com as informações do cliente
- Envia a notificação através do Gmail

## Tecnologias

- n8n
- Google Gemini
- LLMs
- Webhooks
- JSON
- Gmail
- Automação de processos
- Memória conversacional

## Dados coletados

Durante o atendimento, quando o cliente demonstra interesse em solicitar um orçamento, o fluxo pode coletar:

- Nome
- Telefone
- E-mail
- Interesse
- Necessidade

## Estrutura do projeto

automacao-atendimento-ia/
├── README.md
└── workflow/
    ├── atendimento-ia.json
    └── notificacao-lead.json

## Próximos passos

- Integração com WhatsApp
- Persistência dos leads em banco de dados
- Integração com CRM
- Melhorias na qualificação automática
- Monitoramento dos workflows

## Segurança

Os arquivos disponibilizados neste repositório foram preparados para demonstração e portfólio.

Credenciais, chaves de API, senhas e outras informações sensíveis não são incluídas.

## Autor

Renan de Mattos Marcelino
