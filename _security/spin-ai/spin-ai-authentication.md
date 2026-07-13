---
api_key_in:
- header
api_specs:
- filename: spin-ai-openapi.yml
  format: yaml
  label: Spin.AI SpinOne API
  slug: spin-ai-spinone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spin-ai/refs/heads/main/openapi/spin-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spin Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spin.AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spin.AI
provider_slug: spin-ai
scheme_count: 1
schemes:
- description: 'Spin.AI API authentication using the format: SPIN_API X-APP-ID={appIdValue},X-API-KEY={apiKeyValue} Both the Application ID and API Key are generated in the SpinOne administration console under Settings > Integrations > Public API.'
  in: header
  name: spinApiKey
  parameter: Authorization
  sources:
  - openapi/spin-ai-openapi.yml
  type: apiKey
slug: spin-ai-authentication
source_filename: spin-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spin-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: spinApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Spin.AI API authentication using the format: SPIN_API X-APP-ID={appIdValue},X-API-KEY={apiKeyValue}\n    Both the Application ID and API Key are generated in the SpinOne administration console\n    under Settings > Integrations > Public API.'\n  sources:\n  - openapi/spin-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spin-ai/refs/heads/main/authentication/spin-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Backup
- Compliance
- Data Protection
- Ransomware
- SaaS Security
---
