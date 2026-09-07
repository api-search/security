---
anonymous_access: true
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: PontoFato API
  slug: pontofato-api
  spec_type: OpenAPI
  url: https://pontofato.com/openapi.json
auth_types:
- none
- http-bearer
- x402-payment
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Pontofato Authentication
name_suffix: Authentication
oauth_flows: []
overview: PontoFato secures its APIs with none, http-bearer, and x402-payment across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PontoFato
provider_slug: pontofato
scheme_count: 4
schemes:
- description: Público — CEP lookup, unidades, proximo, buscar, raio, empresas, discovery documents and the MCP server all answer anonymously.
  name: public
  type: none
- bearerFormat: cred_ token (or X-Credito header)
  description: Prepaid credit token issued by POST /api/credito (paid once via x402); debits per call on paid routes (vizinhanca beyond free quota). Sent as Authorization Bearer cred_… or the X-Credito header.
  name: credito
  scheme: bearer
  type: http
- bearerFormat: METRICS_TOKEN
  description: Operator-only token unlocking the financial block on GET /api/metrics.
  name: operator
  scheme: bearer
  type: http
- description: Per-request machine payment. Paid routes answer HTTP 402 with an x402 v1 accepts[] challenge (USDC on Base); pay and repeat the request with the X-PAYMENT header. Probed live on POST /api/credito?usd=1.
  name: x402
  scheme: x402
  type: payment
slug: pontofato-authentication
source_filename: pontofato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://pontofato.com/api/ (self-described index, auth block) + openapi/pontofato-openapi-original.json\ndocs: https://pontofato.com/api/\nnote: >-\n  The OpenAPI declares no securitySchemes — the auth model is documented in the self-described\n  /api/ index instead. Most of the surface is public with no key and no signup. There is no\n  account system: the prepaid credit token is a bearer of balance, not an identity\n  (\"Não é conta: é portador de saldo\").\nsummary:\n  types: [none, http-bearer, x402-payment]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: public\n    type: none\n    description: >-\n      Público — CEP lookup, unidades, proximo, buscar, raio, empresas, discovery documents and\n      the MCP server all answer anonymously.\n  - name: credito\n    type: http\n    scheme: bearer\n    bearerFormat: cred_ token (or X-Credito header)\n    description: >-\n      Prepaid credit token issued by POST /api/credito\
  \ (paid once via x402); debits per call on\n      paid routes (vizinhanca beyond free quota). Sent as Authorization Bearer cred_… or the\n      X-Credito header.\n  - name: operator\n    type: http\n    scheme: bearer\n    bearerFormat: METRICS_TOKEN\n    description: Operator-only token unlocking the financial block on GET /api/metrics.\n  - name: x402\n    type: payment\n    scheme: x402\n    description: >-\n      Per-request machine payment. Paid routes answer HTTP 402 with an x402 v1 accepts[]\n      challenge (USDC on Base); pay and repeat the request with the X-PAYMENT header. Probed\n      live on POST /api/credito?usd=1.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/authentication/pontofato-authentication.yml
summary_line: none/http-bearer/x402-payment · 4 schemes
tags:
- Brazilian CEP
- address geocoding
- IBGE CNEFE
- geospatial
- latitude/longitude
- CNPJ
- Receita Federal
- business registry
- location intelligence
- proximity search
- radius search
- open government data
- agent-native
- MCP
- x402 micropayments
---
