---
api_key_in:
- header
api_specs:
- filename: dedaluslabs-dedalus-api-api-openapi.yml
  format: yaml
  label: Dedalus Labs Dedalus API API
  slug: dedaluslabs-dedalus-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-dedalus-api-api-openapi.yml
- filename: dedaluslabs-health-api-openapi.yml
  format: yaml
  label: Dedalus Labs Health API
  slug: dedaluslabs-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-health-api-openapi.yml
- filename: dedaluslabs-machine-lifecycle-api-openapi.yml
  format: yaml
  label: Dedalus Labs Machine Lifecycle API
  slug: dedaluslabs-machine-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-machine-lifecycle-api-openapi.yml
- filename: dedaluslabs-marketplace-api-openapi.yml
  format: yaml
  label: Dedalus Labs Marketplace API
  slug: dedaluslabs-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-marketplace-api-openapi.yml
- filename: dedaluslabs-private-api-openapi.yml
  format: yaml
  label: Dedalus Labs private API
  slug: dedaluslabs-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-private-api-openapi.yml
- filename: dedaluslabs-v1-api-openapi.yml
  format: yaml
  label: Dedalus Labs V1 API
  slug: dedaluslabs-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-v1-api-openapi.yml
- filename: dedaluslabs-webhooks-api-openapi.yml
  format: yaml
  label: Dedalus Labs Webhooks API
  slug: dedaluslabs-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/openapi/dedaluslabs-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dedaluslabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dedalus Labs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dedalus Labs
provider_slug: dedaluslabs
scheme_count: 2
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/dedaluslabs-agents-openapi-original.json
  - openapi/dedaluslabs-machines-openapi-original.yml
  type: http
- description: Dedalus API key. Alternative to Bearer token.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/dedaluslabs-machines-openapi-original.yml
  type: apiKey
slug: dedaluslabs-authentication
source_filename: dedaluslabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dedaluslabs-agents-openapi-original.json, openapi/dedaluslabs-machines-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dedaluslabs-agents-openapi-original.json\n  - openapi/dedaluslabs-machines-openapi-original.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Dedalus API key. Alternative to Bearer token.\n  sources:\n  - openapi/dedaluslabs-machines-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dedaluslabs/refs/heads/main/authentication/dedaluslabs-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Agents
- MCP
- LLM
- Inference
- Gateway
- Compute
- Sandbox
- Developer Tools
---
