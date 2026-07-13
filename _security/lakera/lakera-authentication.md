---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lakera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lakera secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lakera
provider_slug: lakera
scheme_count: 1
schemes:
- description: 'Bearer token issued in the Lakera dashboard. Header format: `Authorization: Bearer ${LAKERA_GUARD_API_KEY}`. Self-hosted deployments may run without authentication.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lakera-openapi.yml
  type: http
slug: lakera-authentication
source_filename: lakera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lakera-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token issued in the Lakera dashboard. Header format: `Authorization:\n    Bearer ${LAKERA_GUARD_API_KEY}`. Self-hosted deployments may run without authentication.'\n  sources:\n  - openapi/lakera-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakera/refs/heads/main/authentication/lakera-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Security
- LLM Security
- Prompt Injection
- Guardrails
- Red Teaming
- GenAI
- API
---
