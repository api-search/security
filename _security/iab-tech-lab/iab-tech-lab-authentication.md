---
anonymous_access: true
api_key_in: []
api_specs:
- filename: iab-tech-lab-opendirect-1-5-1-swagger.yaml
  format: yaml
  label: OpenDirect API
  slug: opendirect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml
- filename: iab-tech-lab-agentic-advertising-api-openapi.yaml
  format: yaml
  label: IAB Agentic Advertising API
  slug: agentic-advertising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-agentic-advertising-api-openapi.yaml
- filename: iab-tech-lab-seller-agent-openapi.json
  format: json
  label: Seller Agent API
  slug: seller-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-seller-agent-openapi.json
- filename: iab-tech-lab-buyer-agent-openapi.json
  format: json
  label: Buyer Agent API
  slug: buyer-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-buyer-agent-openapi.json
auth_types:
- apiKey
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Iab Tech Lab Authentication
name_suffix: Authentication
oauth_flows:
- implicit (illustrative example in the OpenDirect contract)
overview: IAB Tech Lab secures its APIs with apiKey, http-bearer, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit (illustrative example in the OpenDirect contract) flow(s).
provider_name: IAB Tech Lab
provider_slug: iab-tech-lab
scheme_count: 5
schemes:
- bootstrap: first operator key minted out-of-band with `ad-seller create-operator-key` (printed once); later keys via POST /auth/api-keys with an operator credential
  description: Static API key presented as a bearer token; accepted on any endpoint. Anonymous requests are allowed on most buyer-facing reads and receive public-tier data only.
  header: 'Authorization: Bearer <api_key>'
  name: seller-agent bearer
  roles:
  - buyer — tiered data access (seat / agency / advertiser pricing), no control-plane rights
  - operator — required for admin REST routes and admin MCP tools over HTTP (anonymous -> 401, buyer key -> 403)
  scheme: bearer
  sources:
  - https://iabtechlab.github.io/seller-agent/api/authentication/
  - openapi/iab-tech-lab-seller-agent-openapi.json (Authentication tag: /auth/api-keys)
  type: http
- description: Same keys and roles as the bearer form; when both headers are present whichever is found first is validated.
  header: X-Api-Key
  in: header
  name: seller-agent X-Api-Key
  sources:
  - https://iabtechlab.github.io/seller-agent/api/authentication/
  type: apiKey
- description: Local stdio MCP access is trusted like the CLI and requires no header; HTTP MCP transports use the bearer / X-Api-Key operator key for admin tools.
  name: seller-agent MCP stdio
  sources:
  - https://iabtechlab.github.io/seller-agent/api/mcp/
  type: none
- description: '"Example of one of OAuth 2.0 authorization flow that can be used according to specification." The OpenDirect 1.5.1 contract leaves the authorization server, flow and scopes to each implementing seller.'
  flows:
  - authorizationUrl: https://opendirect.example.com/connect/authorize
    flow: implicit
    scopes: 1
  name: OauthSecurity
  sources:
  - openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml
  type: oauth2
- description: api.iabtechlab.com advertises /docs/oauth behind /login; the mechanism could not be read without a subscription.
  name: Supply Chain API (gated)
  sources:
  - https://api.iabtechlab.com/ (nav link /docs/oauth -> 302 /login)
  type: unknown
slug: iab-tech-lab-authentication
source_filename: iab-tech-lab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml (securityDefinitions) upgraded with https://iabtechlab.github.io/seller-agent/api/authentication/ and https://iabtechlab.github.io/seller-agent/api/mcp/\ndocs: https://iabtechlab.github.io/seller-agent/api/authentication/\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  - oauth2\n  oauth2_flows:\n  - implicit (illustrative example in the OpenDirect contract)\nschemes:\n- name: seller-agent bearer\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <api_key>'\n  description: Static API key presented as a bearer token; accepted on any endpoint. Anonymous requests are allowed on most buyer-facing reads and receive public-tier data only.\n  roles:\n  - buyer — tiered data access (seat / agency / advertiser pricing), no control-plane rights\n  - operator — required for admin REST routes and admin MCP tools over HTTP (anonymous -> 401, buyer key -> 403)\n  bootstrap:\
  \ 'first operator key minted out-of-band with `ad-seller create-operator-key` (printed once); later keys via POST /auth/api-keys with an operator credential'\n  sources:\n  - https://iabtechlab.github.io/seller-agent/api/authentication/\n  - openapi/iab-tech-lab-seller-agent-openapi.json (Authentication tag: /auth/api-keys)\n- name: seller-agent X-Api-Key\n  type: apiKey\n  in: header\n  header: X-Api-Key\n  description: Same keys and roles as the bearer form; when both headers are present whichever is found first is validated.\n  sources:\n  - https://iabtechlab.github.io/seller-agent/api/authentication/\n- name: seller-agent MCP stdio\n  type: none\n  description: Local stdio MCP access is trusted like the CLI and requires no header; HTTP MCP transports use the bearer / X-Api-Key operator key for admin tools.\n  sources:\n  - https://iabtechlab.github.io/seller-agent/api/mcp/\n- name: OauthSecurity\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://opendirect.example.com/connect/authorize\n\
  \    scopes: 1\n  description: >-\n    \"Example of one of OAuth 2.0 authorization flow that can be used according to specification.\" The\n    OpenDirect 1.5.1 contract leaves the authorization server, flow and scopes to each implementing seller.\n  sources:\n  - openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml\n- name: Supply Chain API (gated)\n  type: unknown\n  description: api.iabtechlab.com advertises /docs/oauth behind /login; the mechanism could not be read without a subscription.\n  sources:\n  - https://api.iabtechlab.com/ (nav link /docs/oauth -> 302 /login)\nnote: >-\n  The securitySchemes block of the seller-agent OpenAPI is empty — the auth described above comes from the\n  provider's documentation, not the contract. The seller-agent additionally performs OAuth 2.1 PKCE\n  against FreeWheel (ad-server side, `ad-seller freewheel-login`), which is outbound and not part of its own API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/authentication/iab-tech-lab-authentication.yml
summary_line: apiKey/http-bearer/oauth2 · 5 schemes
tags:
- Company
- Advertising
- AdTech
- Standards
- Programmatic
- Real-Time Bidding
- Consent
- Privacy
- Video Ads
- Agentic Advertising
- Non-Profit
---
