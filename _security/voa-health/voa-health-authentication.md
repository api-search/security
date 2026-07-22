---
api_key_in: []
api_specs:
- filename: voa-health-rnds-openapi.yml
  format: yaml
  label: Voa RNDS Integration API
  slug: voa-rnds-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voa-health/refs/heads/main/openapi/voa-health-rnds-openapi.yml
- filename: voa-health-identify-openapi.yml
  format: yaml
  label: Voa Integration Identify API
  slug: voa-integration-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voa-health/refs/heads/main/openapi/voa-health-identify-openapi.yml
auth_types: []
description: Voa uses a two-token model. A long-lived Auth Token identifies the integrating partner (dev convenience, sent as the x-voa-token header). For production, that Auth Token is exchanged per-consultation for a short-lived Bearer JWT (POST /integration/identify/) which authorizes iFrame/plugin embedding and all Voa integration API calls, including RNDS. Voa's own server-to-RNDS leg additionally uses ICP-Brasil A1 mutual-TLS (not exposed to API clients).
kind: authentication
layout: security
method: searched
name: Voa Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: VOA Health declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: VOA Health
provider_slug: voa-health
scheme_count: 3
schemes:
- description: Long-lived Auth Token identifying the integrating partner. Used directly in requests during development without per-consultation renewal.
  environment: development
  id: auth-token
  in: header
  name: x-voa-token
  type: apiKey
- bearer_format: JWT
  description: 'Short-lived per-consultation JWT obtained by exchanging the Auth Token via POST https://api.voa.health/integration/identify/. Expiration configurable via the `expiration` field (seconds, e.g. 43200). Sent as Authorization: Bearer <token> on every Voa integration and RNDS request.'
  environment: production
  id: bearer-jwt
  scheme: bearer
  type: http
- client_facing: false
  description: Voa authenticates to the RNDS national bus using the establishment's ICP-Brasil A1 digital certificate (e-CPF or e-CNPJ, .pfx/.p12) over mTLS, obtaining a 30-minute RNDS JWT. Managed by Voa; not exposed to API consumers. A3 (hardware token) certificates are not supported.
  environment: production
  id: rnds-icp-brasil-mtls
  type: mutualTLS
slug: voa-health-authentication
source_filename: voa-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://docs.voa.health/integracao/iframe/autenticacao.md and\n  https://docs.voa.health/integracao/rnds/como-funciona.md — Voa's documented\n  authentication model for the integration/iFrame/plugin and RNDS APIs.\ndescription: >-\n  Voa uses a two-token model. A long-lived Auth Token identifies the\n  integrating partner (dev convenience, sent as the x-voa-token header). For\n  production, that Auth Token is exchanged per-consultation for a short-lived\n  Bearer JWT (POST /integration/identify/) which authorizes iFrame/plugin\n  embedding and all Voa integration API calls, including RNDS. Voa's own\n  server-to-RNDS leg additionally uses ICP-Brasil A1 mutual-TLS (not exposed to\n  API clients).\ndocs: https://docs.voa.health/integracao/iframe/autenticacao\nschemes:\n  - id: auth-token\n    type: apiKey\n    in: header\n    name: x-voa-token\n    environment: development\n    description: >-\n      Long-lived Auth Token\
  \ identifying the integrating partner. Used directly\n      in requests during development without per-consultation renewal.\n  - id: bearer-jwt\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    environment: production\n    description: >-\n      Short-lived per-consultation JWT obtained by exchanging the Auth Token via\n      POST https://api.voa.health/integration/identify/. Expiration configurable\n      via the `expiration` field (seconds, e.g. 43200). Sent as\n      Authorization: Bearer <token> on every Voa integration and RNDS request.\n  - id: rnds-icp-brasil-mtls\n    type: mutualTLS\n    environment: production\n    client_facing: false\n    description: >-\n      Voa authenticates to the RNDS national bus using the establishment's\n      ICP-Brasil A1 digital certificate (e-CPF or e-CNPJ, .pfx/.p12) over mTLS,\n      obtaining a 30-minute RNDS JWT. Managed by Voa; not exposed to API\n      consumers. A3 (hardware token) certificates are not supported.\noauth2:\
  \ false\nnotes:\n  - Rate limits apply per token (1000 req/hour, 10 req/second).\n  - RNDS submission adds 2-5s latency due to the national-bus round trip; async calls recommended.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voa-health/refs/heads/main/authentication/voa-health-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Health
- Healthcare
- Clinical Documentation
- EHR
- FHIR
- RNDS
- Artificial Intelligence
- Brazil
---
