---
api_key_in: []
api_specs:
- filename: gojiberry-ai-appexternal-api-openapi.yml
  format: yaml
  label: Gojiberry AI AppExternal API
  slug: gojiberry-ai-appexternal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-appexternal-api-openapi.yml
- filename: gojiberry-ai-campaigns-api-openapi.yml
  format: yaml
  label: Gojiberry AI Campaigns API
  slug: gojiberry-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-campaigns-api-openapi.yml
- filename: gojiberry-ai-contacts-api-openapi.yml
  format: yaml
  label: Gojiberry AI Contacts API
  slug: gojiberry-ai-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-contacts-api-openapi.yml
- filename: gojiberry-ai-lead-source-agents-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lead source agents API
  slug: gojiberry-ai-lead-source-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lead-source-agents-api-openapi.yml
- filename: gojiberry-ai-lists-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lists API
  slug: gojiberry-ai-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lists-api-openapi.yml
- filename: gojiberry-ai-organization-api-openapi.yml
  format: yaml
  label: Gojiberry AI Organization API
  slug: gojiberry-ai-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-organization-api-openapi.yml
- filename: gojiberry-ai-unibox-api-openapi.yml
  format: yaml
  label: Gojiberry AI Unibox API
  slug: gojiberry-ai-unibox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-unibox-api-openapi.yml
- filename: gojiberry-ai-user-api-openapi.yml
  format: yaml
  label: Gojiberry AI User API
  slug: gojiberry-ai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gojiberry Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gojiberry AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gojiberry AI
provider_slug: gojiberry-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter API Key
  name: API-Key
  scheme: bearer
  sources:
  - openapi/gojiberry-ai-external-openapi-original.json
  type: http
slug: gojiberry-ai-authentication
source_filename: gojiberry-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gojiberry-ai-external-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: API-Key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter API Key\n  sources:\n  - openapi/gojiberry-ai-external-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/authentication/gojiberry-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Sales
- Lead Generation
- Sales Intelligence
- AI Agents
- Outbound
- Go-To-Market
- Prospecting
- LinkedIn
- CRM
---
