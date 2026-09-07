---
anonymous_access: true
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Radar CNPJ API
  slug: radar-cnpj-api
  spec_type: OpenAPI
  url: https://radar-cnpj.com/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Radar Cnpj Authentication
name_suffix: Authentication
oauth_flows: []
overview: Radar CNPJ declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Radar CNPJ
provider_slug: radar-cnpj
scheme_count: 5
schemes:
- description: Public, no credential. Applies to evaluation (POST /api/avaliar), CNPJ lookup, search, export, autocomplete, reference vocabularies, geolocation, discovery documents and the MCP endpoint. Some origin routes may be geo-restricted to Brazil.
  name: none
  type: none
- description: 'Anonymous monitoring session: POST /api/monitor/session returns a uuid sent as the x-radar-session header on all monitor routes. There is no login — whoever holds the uuid owns the session, so it must be treated as a secret.'
  header: x-radar-session
  in: header
  name: session
  type: apiKey
- description: 'Prepaid credit token: POST /api/credito is paid once via x402 and returns a bearer token (cred_ prefix) that debits any paid API in the house. Shown once, not recoverable; not an account — a bearer of balance.'
  header: 'Authorization: Bearer cred_… (or X-Credito)'
  name: credito
  scheme: bearer
  type: http
- description: Operator metrics token (METRICS_TOKEN) as Authorization Bearer on GET /api/metrics for the full 7-day series; without it the endpoint returns a public subset.
  name: token
  scheme: bearer
  type: http
- description: 'x402 micropayment protocol: exhausted quota or a paid operation returns HTTP 402 with accepts[] (USDC on Base); the client pays and repeats the same call with the X-PAYMENT header. Prices: $0.50/watch/30 days beyond the free 10, $0.10 per agent contact.'
  header: X-PAYMENT
  name: x402
  type: payment
slug: radar-cnpj-authentication
source_filename: radar-cnpj-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://radar-cnpj.com/api/ (self-describing auth block) + https://radar-cnpj.com/llms-full.txt\ndocs: https://radar-cnpj.com/llms-full.txt\nnote: >-\n  The OpenAPI declares no securitySchemes; the auth model is documented in the machine-readable\n  /api/ index and llms-full.txt. The core surface (evaluation, lookup, search, geolocation) is\n  anonymous. Paid operations use the x402 HTTP 402 payment protocol (USDC on Base) via the\n  X-PAYMENT header rather than accounts or API keys.\nschemes:\n  - name: none\n    type: none\n    description: >-\n      Public, no credential. Applies to evaluation (POST /api/avaliar), CNPJ lookup, search,\n      export, autocomplete, reference vocabularies, geolocation, discovery documents and the MCP\n      endpoint. Some origin routes may be geo-restricted to Brazil.\n  - name: session\n    type: apiKey\n    in: header\n    header: x-radar-session\n    description: >-\n      Anonymous monitoring\
  \ session: POST /api/monitor/session returns a uuid sent as the\n      x-radar-session header on all monitor routes. There is no login — whoever holds the uuid\n      owns the session, so it must be treated as a secret.\n  - name: credito\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer cred_… (or X-Credito)'\n    description: >-\n      Prepaid credit token: POST /api/credito is paid once via x402 and returns a bearer token\n      (cred_ prefix) that debits any paid API in the house. Shown once, not recoverable; not an\n      account — a bearer of balance.\n  - name: token\n    type: http\n    scheme: bearer\n    description: >-\n      Operator metrics token (METRICS_TOKEN) as Authorization Bearer on GET /api/metrics for the\n      full 7-day series; without it the endpoint returns a public subset.\n  - name: x402\n    type: payment\n    header: X-PAYMENT\n    description: >-\n      x402 micropayment protocol: exhausted quota or a paid operation returns HTTP 402\
  \ with\n      accepts[] (USDC on Base); the client pays and repeats the same call with the X-PAYMENT\n      header. Prices: $0.50/watch/30 days beyond the free 10, $0.10 per agent contact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radar-cnpj/refs/heads/main/authentication/radar-cnpj-authentication.yml
summary_line: 5 schemes
tags:
- Business & Company Data
- Government/Open Data
- Receita Federal
- CNPJ
- Brazil
- Regulatory & Compliance
- KYB
- Search
- Data Enrichment
- Geolocation
- Monitoring & Alerts
- Agent-native
- MCP
- Micropayments
- x402
---
