# CopilotAgent-GraphIntegration

[![PowerShell](https://custom-icon-badges.demolab.com/badge/PowerShell-5391FE?logo=powershell-white&logoColor=fff)](#)

Utilizar Copilot e Microsoft Graph API para distribuição de mensagens através de um agente de IA e:

    -Enumeração de usuários

    -Criação automática de chats 1:1

    -Envio programado de mensagens

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

### Requisitos:

**Instale o Powershell na versão 5.1 ou acima**

**Defina a ExecutionPolicy como RemoteSigned ou Bypass:**

    Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser

**Instale os módulos Graph e Graph.Beta**

    Install-Module Microsoft.Graph -Scope CurrentUser -Repository PSGallery -Force
    Install-Module Microsoft.Graph.Beta -Repository PSGallery -Force

