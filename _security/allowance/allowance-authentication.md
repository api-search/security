---
api_key_in:
- header
api_specs:
- filename: allowance-openapi-original.json
  format: json
  label: Allowance API
  slug: allowance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allowance/refs/heads/main/openapi/allowance-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Allowance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Allowance secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Allowance
provider_slug: allowance
scheme_count: 2
schemes:
- description: API key with prefix alw_. Contact hello@useallowance.com for early access.
  in: header
  name: ApiKeyAuth
  parameter: X-Allowance-Key
  sources:
  - openapi/allowance-openapi-original.json
  type: apiKey
- description: OAuth2 authorization code flow (planned — not yet active)
  flows:
  - authorizationUrl: https://useallowance.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://useallowance.com/oauth/token
  name: OAuth2
  sources:
  - openapi/allowance-openapi-original.json
  type: oauth2
slug: allowance-authentication
source_filename: allowance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/allowance-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Allowance-Key\n  description: API key with prefix alw_. Contact hello@useallowance.com for early access.\n  sources:\n  - openapi/allowance-openapi-original.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://useallowance.com/oauth/authorize\n    tokenUrl: https://useallowance.com/oauth/token\n    scopes: 3\n  description: OAuth2 authorization code flow (planned — not yet active)\n  sources:\n  - openapi/allowance-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allowance/refs/heads/main/authentication/allowance-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Payments
- Agentic Payments
- AI Agents
- Virtual Cards
- Fintech
- Model Context Protocol
- Consumer Trust
- Spending Controls
- AP2
---
