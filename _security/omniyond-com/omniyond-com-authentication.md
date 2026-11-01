---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: omniyond-com-mcp-api-openapi.yml
  format: yaml
  label: omniyond-com MCP API
  slug: omniyond-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omniyond-com/openapi/omniyond-com-mcp-api-openapi.yml
- filename: omniyond-com-scheduler-api-openapi.yml
  format: yaml
  label: omniyond-com Scheduler API
  slug: omniyond-com-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omniyond-com/openapi/omniyond-com-scheduler-api-openapi.yml
- filename: omniyond-com-utility-api-openapi.yml
  format: yaml
  label: omniyond-com Utility API
  slug: omniyond-com-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omniyond-com/openapi/omniyond-com-utility-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Omniyond Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: omniyond-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: omniyond-com
provider_slug: omniyond-com
scheme_count: 2
schemes:
- bearerFormat: omni_*
  description: Prepaid-credit API key. Create one in the Omniyond dashboard.
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/omniyond-com-openapi.yml
  - openapi/omniyond.yaml
  type: http
- description: 'x402 pay-per-call. Omit the API key to receive a `402` with payment

    requirements in the `payment-required` response header, then pay and

    resend with the `X-PAYMENT` header. USDC on Base.'
  in: header
  name: x402
  parameter: X-PAYMENT
  sources:
  - openapi/omniyond-com-openapi.yml
  - openapi/omniyond.yaml
  type: apiKey
slug: omniyond-com-authentication
source_filename: omniyond-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/omniyond-com-openapi.yml, openapi/omniyond.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: omni_*\n  description: Prepaid-credit API key. Create one in the Omniyond dashboard.\n  sources:\n  - openapi/omniyond-com-openapi.yml\n  - openapi/omniyond.yaml\n- name: x402\n  type: apiKey\n  in: header\n  parameter: X-PAYMENT\n  description: |-\n    x402 pay-per-call. Omit the API key to receive a `402` with payment\n    requirements in the `payment-required` response header, then pay and\n    resend with the `X-PAYMENT` header. USDC on Base.\n  sources:\n  - openapi/omniyond-com-openapi.yml\n  - openapi/omniyond.yaml\n"
source_yaml_url: https://artifacts.apis.io/omniyond-com/authentication/omniyond-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI
- API
- Pay-per-use
- Scheduling
- Automation
---
