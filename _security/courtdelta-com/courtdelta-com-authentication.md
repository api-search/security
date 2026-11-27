---
anonymous_access: true
api_key_in:
- cookie
api_specs:
- filename: courtdelta-com-attorney-cta-api-openapi.yml
  format: yaml
  label: Court Delta Attorney Cta API
  slug: courtdelta-com-attorney-cta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-attorney-cta-api-openapi.yml
- filename: courtdelta-com-calendar-api-openapi.yml
  format: yaml
  label: Court Delta Calendar API
  slug: courtdelta-com-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-calendar-api-openapi.yml
- filename: courtdelta-com-case-lookup-public-api-openapi.yml
  format: yaml
  label: Court Delta Case Lookup Public API
  slug: courtdelta-com-case-lookup-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-case-lookup-public-api-openapi.yml
- filename: courtdelta-com-case-summary-api-openapi.yml
  format: yaml
  label: Court Delta Case Summary API
  slug: courtdelta-com-case-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-case-summary-api-openapi.yml
- filename: courtdelta-com-citation-check-api-openapi.yml
  format: yaml
  label: Court Delta Citation Check API
  slug: courtdelta-com-citation-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-citation-check-api-openapi.yml
- filename: courtdelta-com-court-date-lookup-api-openapi.yml
  format: yaml
  label: Court Delta Court Date Lookup API
  slug: courtdelta-com-court-date-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-court-date-lookup-api-openapi.yml
- filename: courtdelta-com-courthouse-info-api-openapi.yml
  format: yaml
  label: Court Delta Courthouse Info API
  slug: courtdelta-com-courthouse-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-courthouse-info-api-openapi.yml
- filename: courtdelta-com-expunction-options-api-openapi.yml
  format: yaml
  label: Court Delta Expunction Options API
  slug: courtdelta-com-expunction-options-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-expunction-options-api-openapi.yml
- filename: courtdelta-com-license-points-api-openapi.yml
  format: yaml
  label: Court Delta License Points API
  slug: courtdelta-com-license-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-license-points-api-openapi.yml
- filename: courtdelta-com-public-api-openapi.yml
  format: yaml
  label: Court Delta Public API
  slug: courtdelta-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-public-api-openapi.yml
- filename: courtdelta-com-settings-api-openapi.yml
  format: yaml
  label: Court Delta Settings API
  slug: courtdelta-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-settings-api-openapi.yml
- filename: courtdelta-com-subscribe-api-openapi.yml
  format: yaml
  label: Court Delta Subscribe API
  slug: courtdelta-com-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/courtdelta-com/openapi/courtdelta-com-subscribe-api-openapi.yml
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Court Delta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Court Delta secures its APIs with none and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Court Delta
provider_slug: courtdelta-com
scheme_count: 4
schemes:
- description: Every endpoint in /openapi.json is callable anonymously (case and citation lookup, court-date lookup, calendar export, expunction routing, licence points, courthouse info, alert subscription). The free MCP server at https://mcp.courtdelta.com/mcp is also unauthenticated.
  name: none
  sources:
  - https://app.courtdelta.com/auth.md
  type: none
- description: Browser session cookie issued after signing in with a one-time code emailed to a registered attorney or admin address. NOT obtainable programmatically — there is no password, bearer token, or API-key equivalent. GET /api/case-summary returns 401 for attorney-owned records; the docs say to treat that as "this particular record is private".
  in: cookie
  name: SessionCookie
  parameter: attorney_session
  sources:
  - openapi/courtdelta-com-openapi.yml
  - https://app.courtdelta.com/auth.md
  type: apiKey
- description: The optional paid MCP endpoint https://mcp.courtdelta.com/mcp/pro charges per call in USDC on Base mainnet via x402; an unpaid call returns an MCP error with code 402 carrying the price and payment requirements. Docs state this is payment, not authentication — no credential exists.
  name: x402-payment
  sources:
  - https://app.courtdelta.com/auth.md
  type: payment
- description: A private ops API key exists only for internal endpoints on api.courtdelta.com (case lookup, documents, leadgen, scrape); these return 401 and docs state there is no way for third parties to obtain a key.
  name: private-ops-key
  sources:
  - https://app.courtdelta.com/auth.md
  type: apiKey
slug: courtdelta-com-authentication
source_filename: courtdelta-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://app.courtdelta.com/auth.md\ndocs: https://app.courtdelta.com/auth.md\nsummary:\n  types:\n  - none\n  - apiKey\n  api_key_in:\n  - cookie\n  public_surface_auth: none\n  note: \"Docs state: \\\"No authentication is required for anything you can use. There is no OAuth flow, no token endpoint, and no authorization server.\\\" The only declared scheme is a browser session cookie for attorney-owned records, not obtainable programmatically.\"\nschemes:\n- name: none\n  type: none\n  description: Every endpoint in /openapi.json is callable anonymously (case and citation lookup, court-date lookup, calendar export, expunction routing, licence points, courthouse info, alert subscription). The free MCP server at https://mcp.courtdelta.com/mcp is also unauthenticated.\n  sources:\n  - https://app.courtdelta.com/auth.md\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: attorney_session\n  description: Browser session\
  \ cookie issued after signing in with a one-time code emailed to a registered attorney or admin address. NOT obtainable programmatically — there is no password, bearer token, or API-key equivalent. GET /api/case-summary returns 401 for attorney-owned records; the docs say to treat that as \"this particular record is private\".\n  sources:\n  - openapi/courtdelta-com-openapi.yml\n  - https://app.courtdelta.com/auth.md\n- name: x402-payment\n  type: payment\n  description: The optional paid MCP endpoint https://mcp.courtdelta.com/mcp/pro charges per call in USDC on Base mainnet via x402; an unpaid call returns an MCP error with code 402 carrying the price and payment requirements. Docs state this is payment, not authentication — no credential exists.\n  sources:\n  - https://app.courtdelta.com/auth.md\n- name: private-ops-key\n  type: apiKey\n  description: A private ops API key exists only for internal endpoints on api.courtdelta.com (case lookup, documents, leadgen, scrape); these return\
  \ 401 and docs state there is no way for third parties to obtain a key.\n  sources:\n  - https://app.courtdelta.com/auth.md\noauth_discovery:\n  published: false\n  note: Docs state /.well-known/openid-configuration, /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource are intentionally absent and return 404.\n"
source_yaml_url: https://artifacts.apis.io/courtdelta-com/authentication/courtdelta-com-authentication.yml
summary_line: none/apiKey · 4 schemes
tags:
- Company
- Legal
- Court Records
- Case Tracking
- Notification
- North Carolina
- MCP
---
