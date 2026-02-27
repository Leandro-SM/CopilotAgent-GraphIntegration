# CopilotAgent-GraphIntegration

[![PowerShell](https://custom-icon-badges.demolab.com/badge/PowerShell-5391FE?logo=powershell-white&logoColor=fff)](#)

Utilizar Copilot e Microsoft Graph API para distribuição de mensagens através de um agente de IA para:

    -Enumeração de usuários

    -Criação automática de chats 1:1

    -Envio programático de mensagens

    -Integração com agentes conversacionais (compatíveis com o Microsoft Teams)

    -Estrutura para disparo de mensagens em lote


## Estrutura  
```bash
Azure AD -> App Registrado
        │
        │ OAuth 2.0 (Client Secret)
        ▼
Microsoft Graph API (Powershell)
        │
        ├── Listagem de Usuários (Get)
        ├── Criação de Chat 1:1 (Create)
        └── Envio de Mensagens (Automate)
                │
                ▼
        Microsoft Teams
                │
                ▼
      Agente (Copilot / App)
```
