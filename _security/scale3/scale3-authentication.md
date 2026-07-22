---
api_key_in:
- header
api_specs:
- filename: scale3-blockchain-intelligence-openapi.yml
  format: yaml
  label: Scale3 Blockchain Intelligence API
  slug: scale3-blockchain-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale3/refs/heads/main/openapi/scale3-blockchain-intelligence-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scale3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scale3 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scale3
provider_slug: scale3
scheme_count: 1
schemes:
- description: API key generated from the Scale3 Autopilot Intel tab (Enterprise license required). Requests must also send the header x-user-agent with value s3l-web-client.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/scale3-blockchain-intelligence-openapi.yml
  type: apiKey
slug: scale3-authentication
source_filename: scale3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/scale3-blockchain-intelligence-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key generated from the Scale3 Autopilot Intel tab (Enterprise license required).\n    Requests must also send the header x-user-agent with value s3l-web-client.\n  sources:\n  - openapi/scale3-blockchain-intelligence-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scale3/refs/heads/main/authentication/scale3-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Blockchain
- Web3
- Node Monitoring
- Observability
- Infrastructure
- Validators
- DevOps
- Alerting
- LLM Observability
---
