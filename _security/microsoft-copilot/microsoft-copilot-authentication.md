---
api_key_in: []
api_specs:
- filename: microsoft-copilot-change-notifications-api-openapi.yml
  format: yaml
  label: Microsoft Copilot Change Notifications API
  slug: microsoft-copilot-change-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/openapi/microsoft-copilot-change-notifications-api-openapi.yml
- filename: microsoft-copilot-chat-api-openapi.yml
  format: yaml
  label: Microsoft Copilot Chat API
  slug: microsoft-copilot-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/openapi/microsoft-copilot-chat-api-openapi.yml
- filename: microsoft-copilot-interaction-export-api-openapi.yml
  format: yaml
  label: Microsoft Copilot Interaction Export API
  slug: microsoft-copilot-interaction-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/openapi/microsoft-copilot-interaction-export-api-openapi.yml
- filename: microsoft-copilot-retrieval-api-openapi.yml
  format: yaml
  label: Microsoft Copilot Retrieval API
  slug: microsoft-copilot-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/openapi/microsoft-copilot-retrieval-api-openapi.yml
- filename: microsoft-copilot-search-api-openapi.yml
  format: yaml
  label: Microsoft Copilot Search API
  slug: microsoft-copilot-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/openapi/microsoft-copilot-search-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Copilot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Copilot secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization using Microsoft identity platform (Azure AD). Requires a Microsoft 365 Copilot license for each user accessing Copilot API functionality.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-copilot-openapi.yml
  type: oauth2
slug: microsoft-copilot-authentication
source_filename: microsoft-copilot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-copilot-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 5\n  description: OAuth 2.0 authorization using Microsoft identity platform (Azure AD). Requires\n    a Microsoft 365 Copilot license for each user accessing Copilot API functionality.\n  sources:\n  - openapi/microsoft-copilot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/authentication/microsoft-copilot-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Agents
- AI Assistant
- Artificial Intelligence
- Chatbot
- Copilot
- Extensibility
- Generative AI
- Microsoft-365
- Productivity
---
