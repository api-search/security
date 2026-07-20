---
api_key_in: []
api_specs:
- filename: arthur-scope-openapi.json
  format: json
  label: Arthur Scope
  slug: arthur-scope
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthurai/refs/heads/main/openapi/arthur-scope-openapi.json
- filename: arthur-engine-openapi.json
  format: json
  label: Arthur GenAI Engine
  slug: arthur-genai-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthurai/refs/heads/main/openapi/arthur-engine-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Arthurai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ArthurAI secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ArthurAI
provider_slug: arthurai
scheme_count: 2
schemes:
- description: Bearer token authentication with an API key
  name: API Key
  scheme: bearer
  sources:
  - openapi/arthur-engine-openapi.json
  type: http
- flows:
  - authorizationUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token
  name: OAuth2AuthorizationCode
  sources:
  - openapi/arthur-scope-openapi.json
  type: oauth2
slug: arthurai-authentication
source_filename: arthurai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/arthur-engine-openapi.json, openapi/arthur-scope-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: API Key\n  type: http\n  scheme: bearer\n  description: Bearer token authentication with an API key\n  sources:\n  - openapi/arthur-engine-openapi.json\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/auth\n    tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token\n    scopes: 0\n  sources:\n  - openapi/arthur-scope-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthurai/refs/heads/main/authentication/arthurai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Ai Ml
- AI Governance
- AI Observability
- LLM Evaluation
- Model Monitoring
- Guardrails
- MLOps
---
