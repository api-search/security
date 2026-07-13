---
api_key_in:
- header
api_specs:
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev Apps API
  slug: aci-dev-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev Functions API
  slug: aci-dev-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev App Configurations API
  slug: aci-dev-app-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev Linked Accounts API
  slug: aci-dev-linked-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aci Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: ACI.dev secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ACI.dev
provider_slug: aci-dev
scheme_count: 1
schemes:
- description: API key for authentication
  in: header
  name: APIKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/aci-dev-openapi.yml
  type: apiKey
slug: aci-dev-authentication
source_filename: aci-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aci-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key for authentication\n  sources:\n  - openapi/aci-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/authentication/aci-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agent Infrastructure
- Agents
- AI
- Artificial Intelligence
- Function Calling
- MCP
- Model Context Protocol
- OAuth
- Open Source
- Tool Calling
- VibeOps
---
