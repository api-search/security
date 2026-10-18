---
anonymous_access: false
api_key_in: []
api_specs:
- filename: credoai-audit-logs-api-openapi.yml
  format: yaml
  label: Credoai Audit Logs API
  slug: credoai-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credoai/refs/heads/main/openapi/credoai-audit-logs-api-openapi.yml
- filename: credoai-shadow-ai-api-openapi.yml
  format: yaml
  label: Credoai Shadow AI API
  slug: credoai-shadow-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credoai/refs/heads/main/openapi/credoai-shadow-ai-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Credoai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Credoai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Credoai
provider_slug: credoai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT access token obtained from [`POST /auth/exchange`](#tag/Auth/operation/CredoAIWeb.Auth.TokenController.exchange).


    Include in the Authorization header: `Authorization: Bearer <token>`'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/credoai-openapi.json
  type: http
slug: credoai-authentication
source_filename: credoai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: derived\nsource: openapi/credoai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT access token obtained from [`POST /auth/exchange`](#tag/Auth/operation/CredoAIWeb.Auth.TokenController.exchange).\n\n    Include in the Authorization header: `Authorization: Bearer <token>`\n  sources:\n  - openapi/credoai-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credoai/refs/heads/main/authentication/credoai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Governance
- Software-as-a-Service
- PaloAlto
---
