---
api_key_in: []
api_specs:
- filename: arthur-ai-platform-openapi.json
  format: json
  label: Arthur Platform API
  slug: arthur-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-ai/refs/heads/main/openapi/arthur-ai-platform-openapi.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Arthur Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceAuthorization
- clientCredentials
overview: Arthur AI secures its APIs with oauth2 and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceAuthorization, and clientCredentials flow(s).
provider_name: Arthur AI
provider_slug: arthur-ai
scheme_count: 4
schemes:
- component: Arthur Platform
  flows:
  - authorizationUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/auth
    flow: authorizationCode
    refreshUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token
    tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token
  name: OAuth2AuthorizationCode
  sources:
  - openapi/arthur-ai-platform-openapi.json
  type: oauth2
- component: Arthur Platform (service accounts, M2M)
  flows:
  - flow: clientCredentials
    tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token
  name: ClientCredentials
  sources:
  - https://docs.arthur.ai/docs/authentication.md
  type: oauth2
- component: Arthur Platform (human local flows)
  flows:
  - flow: deviceCode
    tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token
  name: DeviceAuthorization
  sources:
  - https://docs.arthur.ai/docs/authentication.md
  type: oauth2
- component: Arthur Engine / Agent Toolkit
  in: header
  name: ApiKey
  sources:
  - https://docs.arthur.ai/docs/authentication.md
  type: apiKey
slug: arthur-ai-authentication
source_filename: arthur-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/arthur-ai-platform-openapi.json\ndocs: https://docs.arthur.ai/docs/authentication.md\nnote: >-\n  Arthur uses two distinct auth mechanisms. The Arthur Platform API uses OAuth2\n  via Keycloak (issuer https://platform-auth.arthur.ai/realms/arthur): human\n  flows use device authorization, machine-to-machine uses service-account client\n  credentials (tokens auto-refreshed with a 30s leeway). The self-hosted Arthur\n  Engine / Agent Toolkit uses API keys instead.\nsummary:\n  types:\n    - oauth2\n    - apiKey\n  oauth2_flows:\n    - authorizationCode\n    - deviceAuthorization\n    - clientCredentials\n  api_key_scope: Arthur Engine / Agent Toolkit only\nschemes:\n  - name: OAuth2AuthorizationCode\n    type: oauth2\n    component: Arthur Platform\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/auth\n        tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token\n\
  \        refreshUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token\n    sources:\n      - openapi/arthur-ai-platform-openapi.json\n  - name: ClientCredentials\n    type: oauth2\n    component: Arthur Platform (service accounts, M2M)\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token\n    sources:\n      - https://docs.arthur.ai/docs/authentication.md\n  - name: DeviceAuthorization\n    type: oauth2\n    component: Arthur Platform (human local flows)\n    flows:\n      - flow: deviceCode\n        tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token\n    sources:\n      - https://docs.arthur.ai/docs/authentication.md\n  - name: ApiKey\n    type: apiKey\n    in: header\n    component: Arthur Engine / Agent Toolkit\n    sources:\n      - https://docs.arthur.ai/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthur-ai/refs/heads/main/authentication/arthur-ai-authentication.yml
summary_line: oauth2/apiKey · 4 schemes
tags:
- Company
- AI
- AI Governance
- AI Observability
- Machine Learning
- LLM Evaluation
- Model Monitoring
- MLOps
- Guardrails
- Agents
---
