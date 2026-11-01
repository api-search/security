---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Archtools Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: archtools-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: archtools-dev
provider_slug: archtools-dev
scheme_count: 2
schemes:
- description: API Key authentication (recommended)
  in: header
  name: x-api-key
  type: apiKey
- description: x402 crypto payment authentication via USDC on Base
  in: header
  name: X-PAYMENT
  type: custom
slug: archtools-dev-authentication
source_filename: archtools-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://archtools.dev/docs#authentication\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API Key authentication (recommended)\n  - type: custom\n    name: X-PAYMENT\n    in: header\n    description: x402 crypto payment authentication via USDC on Base\n"
source_yaml_url: https://artifacts.apis.io/archtools-dev/authentication/archtools-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Tools
- API
- Automation
- MCP
---
