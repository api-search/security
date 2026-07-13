---
api_key_in: []
api_specs:
- filename: merge-hris-api-openapi.yaml
  format: yaml
  label: Merge HRIS API
  slug: hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-hris-api-openapi.yaml
- filename: merge-ats-api-openapi.yaml
  format: yaml
  label: Merge ATS API
  slug: ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-ats-api-openapi.yaml
- filename: merge-accounting-api-openapi.yaml
  format: yaml
  label: Merge Accounting API
  slug: accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-accounting-api-openapi.yaml
- filename: merge-ticketing-api-openapi.yaml
  format: yaml
  label: Merge Ticketing API
  slug: ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-ticketing-api-openapi.yaml
- filename: merge-crm-api-openapi.yaml
  format: yaml
  label: Merge CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-crm-api-openapi.yaml
- filename: merge-file-storage-api-openapi.yaml
  format: yaml
  label: Merge File Storage API
  slug: file-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-file-storage-api-openapi.yaml
- filename: merge-knowledge-base-api-openapi.yaml
  format: yaml
  label: Merge Knowledge Base API
  slug: knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-knowledge-base-api-openapi.yaml
- filename: merge-chat-api-openapi.yaml
  format: yaml
  label: Merge Chat API
  slug: chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-chat-api-openapi.yaml
- filename: merge-agent-handler-api-openapi.yaml
  format: yaml
  label: Merge Agent Handler
  slug: agent-handler
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-agent-handler-api-openapi.yaml
- filename: merge-gateway-api-openapi.yaml
  format: yaml
  label: Merge Gateway
  slug: gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/openapi/merge-gateway-api-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Merge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Merge secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Merge
provider_slug: merge
scheme_count: 1
schemes:
- description: Token-based authentication with required prefix "Bearer"
  name: tokenAuth
  scheme: bearer
  sources:
  - openapi/merge-accounting-api-openapi.yaml
  - openapi/merge-agent-handler-api-openapi.yaml
  - openapi/merge-ats-api-openapi.yaml
  - openapi/merge-chat-api-openapi.yaml
  - openapi/merge-crm-api-openapi.yaml
  - openapi/merge-file-storage-api-openapi.yaml
  - openapi/merge-hris-api-openapi.yaml
  - openapi/merge-knowledge-base-api-openapi.yaml
  - openapi/merge-ticketing-api-openapi.yaml
  type: http
slug: merge-authentication
source_filename: merge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/merge-accounting-api-openapi.yaml, openapi/merge-agent-handler-api-openapi.yaml,\n  openapi/merge-ats-api-openapi.yaml, openapi/merge-chat-api-openapi.yaml, openapi/merge-crm-api-openapi.yaml,\n  openapi/merge-file-storage-api-openapi.yaml, openapi/merge-hris-api-openapi.yaml, openapi/merge-knowledge-base-api-openapi.yaml,\n  openapi/merge-ticketing-api-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  description: Token-based authentication with required prefix \"Bearer\"\n  sources:\n  - openapi/merge-accounting-api-openapi.yaml\n  - openapi/merge-agent-handler-api-openapi.yaml\n  - openapi/merge-ats-api-openapi.yaml\n  - openapi/merge-chat-api-openapi.yaml\n  - openapi/merge-crm-api-openapi.yaml\n  - openapi/merge-file-storage-api-openapi.yaml\n  - openapi/merge-hris-api-openapi.yaml\n  - openapi/merge-knowledge-base-api-openapi.yaml\n  - openapi/merge-ticketing-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/authentication/merge-authentication.yml
summary_line: http · 1 scheme
tags:
- Integrations
- Platform
- Unified API
- Agent Handler
- LLM Gateway
---
