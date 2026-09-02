# Synapse Gest — CRM de Captação

CRM de captação de leads em um único arquivo HTML (kanban por etapa do funil, mensagens prontas por etapa e sincronização automática dos dados com este repositório via API do GitHub).

## Estrutura

- `index.html` — o app inteiro (interface + lógica).
- `synapse-crm-dados.json` — dados dos leads e modelos de mensagem. É lido e atualizado automaticamente pelo app a cada alteração (via commits feitos pelo próprio navegador).

## Como usar

1. Publique este repositório com o GitHub Pages (Settings → Pages → Deploy from branch → `main` → `/ (root)`).
2. Abra a URL gerada pelo GitHub Pages.
3. No app, clique em **"Configurar GitHub"** e informe:
   - Usuário/organização e nome deste repositório
   - Branch (`main`)
   - Caminho do arquivo (`synapse-crm-dados.json`)
   - Um token de acesso pessoal (fine-grained, com permissão apenas de **Contents: Read and write** neste repositório)
4. A partir daí, toda alteração feita no CRM (criar/editar/excluir lead, editar modelo) gera um commit automático neste repositório.
