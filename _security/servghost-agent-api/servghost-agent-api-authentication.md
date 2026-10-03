---
anonymous_access: true
api_key_in: []
api_specs:
- filename: servghost-agent-api-account-api-openapi.yml
  format: yaml
  label: ServGhost Agent API Account API
  slug: servghost-agent-api-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-account-api-openapi.yml
- filename: servghost-agent-api-catalog-api-openapi.yml
  format: yaml
  label: ServGhost Agent API Catalog API
  slug: servghost-agent-api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-catalog-api-openapi.yml
- filename: servghost-agent-api-domains-api-openapi.yml
  format: yaml
  label: ServGhost Agent API Domains API
  slug: servghost-agent-api-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-domains-api-openapi.yml
- filename: servghost-agent-api-locations-api-openapi.yml
  format: yaml
  label: ServGhost Agent API Locations API
  slug: servghost-agent-api-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-locations-api-openapi.yml
- filename: servghost-agent-api-orders-api-openapi.yml
  format: yaml
  label: ServGhost Agent API Orders API
  slug: servghost-agent-api-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-orders-api-openapi.yml
- filename: servghost-agent-api-quote-api-openapi.yml
  format: yaml
  label: ServGhost Agent API Quote API
  slug: servghost-agent-api-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-quote-api-openapi.yml
- filename: servghost-agent-api-servers-api-openapi.yml
  format: yaml
  label: ServGhost Agent API Servers API
  slug: servghost-agent-api-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-servers-api-openapi.yml
- filename: servghost-agent-api-servghost-agent-api-api-openapi.yml
  format: yaml
  label: ServGhost Agent API ServGhost Agent API
  slug: servghost-agent-api-servghost-agent-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-servghost-agent-api-api-openapi.yml
- filename: servghost-agent-api-top-up-api-openapi.yml
  format: yaml
  label: ServGhost Agent API Top Up API
  slug: servghost-agent-api-top-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-top-up-api-openapi.yml
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
- Agent-Native
- MCP
- x402
---
