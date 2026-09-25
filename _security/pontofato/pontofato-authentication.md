---
anonymous_access: true
api_key_in: []
api_specs:
- filename: pontofato-apis-json-api-openapi.yml
  format: yaml
  label: PontoFato Apis.json API
  slug: pontofato-apis-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-apis-json-api-openapi.yml
- filename: pontofato-buscar-api-openapi.yml
  format: yaml
  label: PontoFato Buscar API
  slug: pontofato-buscar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-buscar-api-openapi.yml
- filename: pontofato-cep-api-openapi.yml
  format: yaml
  label: PontoFato Cep API
  slug: pontofato-cep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-cep-api-openapi.yml
- filename: pontofato-contact-api-openapi.yml
  format: yaml
  label: PontoFato Contact API
  slug: pontofato-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-contact-api-openapi.yml
- filename: pontofato-credito-api-openapi.yml
  format: yaml
  label: PontoFato Credito API
  slug: pontofato-credito-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-credito-api-openapi.yml
- filename: pontofato-empresas-api-openapi.yml
  format: yaml
  label: PontoFato Empresas API
  slug: pontofato-empresas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-empresas-api-openapi.yml
- filename: pontofato-health-api-openapi.yml
  format: yaml
  label: PontoFato Health API
  slug: pontofato-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-health-api-openapi.yml
- filename: pontofato-local-api-openapi.yml
  format: yaml
  label: PontoFato Local API
  slug: pontofato-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-local-api-openapi.yml
- filename: pontofato-mcp-api-openapi.yml
  format: yaml
  label: PontoFato MCP API
  slug: pontofato-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-mcp-api-openapi.yml
- filename: pontofato-metrics-api-openapi.yml
  format: yaml
  label: PontoFato Metrics API
  slug: pontofato-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-metrics-api-openapi.yml
- filename: pontofato-okf-api-openapi.yml
  format: yaml
  label: PontoFato Okf API
  slug: pontofato-okf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-okf-api-openapi.yml
- filename: pontofato-pontofato-api-openapi.yml
  format: yaml
  label: PontoFato Ponto Fato API
  slug: pontofato-pontofato-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-pontofato-api-openapi.yml
- filename: pontofato-proximo-api-openapi.yml
  format: yaml
  label: PontoFato Proximo API
  slug: pontofato-proximo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-proximo-api-openapi.yml
- filename: pontofato-raio-api-openapi.yml
  format: yaml
  label: PontoFato Raio API
  slug: pontofato-raio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-raio-api-openapi.yml
- filename: pontofato-vizinhanca-api-openapi.yml
  format: yaml
  label: PontoFato Vizinhanca API
  slug: pontofato-vizinhanca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-vizinhanca-api-openapi.yml
- filename: pontofato-well-known-api-openapi.yml
  format: yaml
  label: PontoFato .well Known API
  slug: pontofato-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-well-known-api-openapi.yml
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
- Geospatial
- latitude/longitude
- CNPJ
- Receita Federal
- Business Registry
- Location Intelligence
- proximity search
- radius search
- Open Government Data
- Agent-Native
- MCP
- x402-micropayments
---
