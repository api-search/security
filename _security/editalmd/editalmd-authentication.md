---
anonymous_access: true
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: EditalMD API
  slug: editalmd-api
  spec_type: OpenAPI
  url: https://editalmd.com/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Editalmd Authentication
name_suffix: Authentication
oauth_flows: []
overview: EditalMD declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: EditalMD
provider_slug: editalmd
scheme_count: 4
schemes:
- description: Public, no credential. Search (GET /api/busca), tender sheets (GET /api/compra/{id}), CNAE dictionary, health, discovery documents and feeds are free and unauthenticated. Documents of tenders published 30+ days ago are free samples on the same anonymous surface.
  id: public
  type: none
- create: POST /api/dono
  description: 'Owner token sent as Authorization Bearer. Created by POST /api/dono with no signup; the response also returns the whsec_ webhook signing secret. Only a hash of the token is stored server-side. Gates the alert, watcher and owner-state routes (auth: owner in llms.txt).'
  id: owner-token
  scheme: bearer
  token_prefix: edm_
  type: http
- create: POST /api/credito
  description: Prepaid-credit bearer token, sent as Authorization Bearer (or the X-Credito header). Bought once via POST /api/credito?usd={1|5|10|25} paid with x402; returned exactly once; debits any paid route across all the operator's products ("vale em todos os produtos da casa"). Not an account - a pure bearer.
  id: credit-token
  scheme: bearer
  token_prefix: cred_
  type: http
- description: Per-request machine payment. A paid route called without payment answers HTTP 402 with an accepts[] offer; the client pays (USDC) and repeats the request with the X-PAYMENT header. No registration. Every paid delivery returns x-editalmd-recibo and x-editalmd-sha256 headers and a receipt at GET /api/recibo/{id}.
  id: x402
  scheme: x402
  type: payment
slug: editalmd-authentication
source_filename: editalmd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: EditalMD Authentication Profile\ngenerated: '2026-09-05'\nmethod: searched\nsource: https://editalmd.com/api/\ndocs: https://editalmd.com/llms.txt\nnote: >-\n  The OpenAPI declares no securitySchemes; the auth model is documented in the self-describing /api/ index\n  (auth block), llms.txt and llms-full.txt. There are no accounts anywhere: every credential is a no-signup\n  bearer token or a per-request x402 payment.\nschemes:\n  - id: public\n    type: none\n    description: >-\n      Public, no credential. Search (GET /api/busca), tender sheets (GET /api/compra/{id}), CNAE dictionary,\n      health, discovery documents and feeds are free and unauthenticated. Documents of tenders published 30+\n      days ago are free samples on the same anonymous surface.\n  - id: owner-token\n    type: http\n    scheme: bearer\n    token_prefix: edm_\n    description: >-\n      Owner token sent as Authorization Bearer. Created by POST /api/dono with no signup; the response also\n \
  \     returns the whsec_ webhook signing secret. Only a hash of the token is stored server-side. Gates the\n      alert, watcher and owner-state routes (auth: owner in llms.txt).\n    create: POST /api/dono\n  - id: credit-token\n    type: http\n    scheme: bearer\n    token_prefix: cred_\n    description: >-\n      Prepaid-credit bearer token, sent as Authorization Bearer (or the X-Credito header). Bought once via\n      POST /api/credito?usd={1|5|10|25} paid with x402; returned exactly once; debits any paid route across\n      all the operator's products (\"vale em todos os produtos da casa\"). Not an account - a pure bearer.\n    create: POST /api/credito\n  - id: x402\n    type: payment\n    scheme: x402\n    description: >-\n      Per-request machine payment. A paid route called without payment answers HTTP 402 with an accepts[]\n      offer; the client pays (USDC) and repeats the request with the X-PAYMENT header. No registration.\n      Every paid delivery returns x-editalmd-recibo\
  \ and x-editalmd-sha256 headers and a receipt at\n      GET /api/recibo/{id}.\nwebhook_signing:\n  scheme: standard-webhooks\n  secret_prefix: whsec_\n  headers: [webhook-id, webhook-timestamp, webhook-signature]\n  algorithm: HMAC-SHA256 of \"id.timestamp.body\" with the base64-decoded secret, signature as \"v1,<base64>\"\n  rotation: POST /api/dono/segredo - previous secret still signs for 24 hours\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/editalmd/refs/heads/main/authentication/editalmd-authentication.yml
summary_line: 4 schemes
tags:
- GovTech
- Public Procurement
- Brazil
- PNCP
- Legal & Compliance
- Business Intelligence
- Company Data
- CNPJ
- CNAE
- SICAF
- Document Extraction
- Agent-Native
- MCP
- x402
- Machine-Payable
---
