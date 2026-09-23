---
anonymous_access: true
api_key_in: []
api_specs:
- filename: servghost-agent-api-openapi.yml
  format: yaml
  label: ServGhost Agent API
  slug: servghost-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Servghost Agent Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: ServGhost Agent API declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ServGhost Agent API
provider_slug: servghost-agent-api
scheme_count: 2
schemes:
- bearerFormat: AAAA-BBBB-CCCC-DDDD
  email_required: false
  issuance: Auto-issued on first topup/order POST, or explicitly via POST /api/v1/account
  kyc_required: false
  location: Authorization header
  name: BearerAuth
  scheme: bearer
  type: http
- detail: Discovery/pricing endpoints (GET /api/v1/catalog, /locations, /topup/bonus, /domains/check and POST /api/v1/quote) require no auth.
  name: Anonymous
  type: none
slug: servghost-agent-api-authentication
source_filename: servghost-agent-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: searched\nsource: https://servghost.com/agents\ndocs: https://servghost.com/agents\nsummary: >-\n  Single scheme: HTTP Bearer token. Tokens are auto-issued on the first POST /api/v1/topup or /api/v1/orders\n  (or explicitly via POST /api/v1/account) with no KYC, no email and no signup. Token format is\n  AAAA-BBBB-CCCC-DDDD. Anonymous, unauthenticated access is allowed for discovery endpoints (catalog,\n  locations, quote, topup/bonus, domains/check). MCP mutating tools carry the same token as an account_token\n  argument rather than a connection-level credential.\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: AAAA-BBBB-CCCC-DDDD\n    location: Authorization header\n    issuance: Auto-issued on first topup/order POST, or explicitly via POST /api/v1/account\n    kyc_required: false\n    email_required: false\n  - name: Anonymous\n    type: none\n    detail: Discovery/pricing endpoints (GET /api/v1/catalog,\
  \ /locations, /topup/bonus, /domains/check and POST /api/v1/quote) require no auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/authentication/servghost-agent-api-authentication.yml
summary_line: 2 schemes
tags:
- Cloud Infrastructure
- VPS hosting
- Dedicated Servers
- GPU Compute
- AI Compute
- Domain Registration
- Privacy
- anonymous hosting
- offshore hosting
- Crypto Payments
- agent-native
- MCP
- x402
---
