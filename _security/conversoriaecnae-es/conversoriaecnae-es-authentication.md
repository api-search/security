---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: conversoriaecnae-es-b-squeda-api-openapi.yml
  format: yaml
  label: Conversor IAE CNAE Búsqueda API
  slug: conversoriaecnae-es-b-squeda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversoriaecnae-es/openapi/conversoriaecnae-es-b-squeda-api-openapi.yml
- filename: conversoriaecnae-es-b2b-api-openapi.yml
  format: yaml
  label: Conversor IAE CNAE B2B API
  slug: conversoriaecnae-es-b2b-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversoriaecnae-es/openapi/conversoriaecnae-es-b2b-api-openapi.yml
- filename: conversoriaecnae-es-c-digos-api-openapi.yml
  format: yaml
  label: Conversor IAE CNAE Códigos API
  slug: conversoriaecnae-es-c-digos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversoriaecnae-es/openapi/conversoriaecnae-es-c-digos-api-openapi.yml
- filename: conversoriaecnae-es-cuenta-api-openapi.yml
  format: yaml
  label: Conversor IAE CNAE Cuenta API
  slug: conversoriaecnae-es-cuenta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversoriaecnae-es/openapi/conversoriaecnae-es-cuenta-api-openapi.yml
- filename: conversoriaecnae-es-fiscal-api-openapi.yml
  format: yaml
  label: Conversor IAE CNAE Fiscal API
  slug: conversoriaecnae-es-fiscal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversoriaecnae-es/openapi/conversoriaecnae-es-fiscal-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Conversor IAE CNAE Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conversor IAE CNAE secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Conversor IAE CNAE
provider_slug: conversoriaecnae-es
scheme_count: 2
schemes:
- description: Clave de API con prefijo `cvr_`. Obtén una gratis en POST /signup.
  docs_text: Todas las peticiones requieren una clave API enviada en la cabecera HTTP X-API-Key . ... La clave se valida en cada petición. Si es inválida o no se incluye, recibirás un error 401 .
  in: header
  key_prefix: cvr_
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/conversoriaecnae-es-openapi.yml
  - https://www.conversoriaecnae.es/api/v1/docs
  type: apiKey
- applies_to: https://www.conversoriaecnae.es/api/mcp/mcp
  description: 'Docs: premium MCP tools require ''Authorization: Bearer cvr_tu_clave_api''; free MCP tools need no key.'
  name: MCP bearer key
  scheme: bearer
  sources:
  - https://www.conversoriaecnae.es/api/v1/docs
  type: http
slug: conversoriaecnae-es-authentication
source_filename: conversoriaecnae-es-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.conversoriaecnae.es/api/v1/docs\ndocs: https://www.conversoriaecnae.es/api/v1/docs\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  key_prefix: cvr_\n  description: Clave de API con prefijo `cvr_`. Obtén una gratis en POST /signup.\n  docs_text: \"Todas las peticiones requieren una clave API enviada en la cabecera HTTP X-API-Key . ... La clave se valida en cada petición. Si es inválida o no se incluye, recibirás un error 401 .\"\n  sources:\n  - openapi/conversoriaecnae-es-openapi.yml\n  - https://www.conversoriaecnae.es/api/v1/docs\n- name: MCP bearer key\n  type: http\n  scheme: bearer\n  applies_to: https://www.conversoriaecnae.es/api/mcp/mcp\n  description: \"Docs: premium MCP tools require 'Authorization: Bearer cvr_tu_clave_api'; free MCP tools need no key.\"\n  sources:\n  - https://www.conversoriaecnae.es/api/v1/docs\n\
  key_lifecycle:\n  issuance: POST /signup (createApiKey) — key delivered by email only, never in the HTTP response (per docs; not called).\n  rotation_revocation: POST /keys (rotateOrRevokeApiKey) — rotate (old key stops working immediately) or revoke; authenticated with the current X-API-Key; 30 requests/hour per IP (OpenAPI description).\n  dashboard: https://www.conversoriaecnae.es/api-dashboard\nnote: Read from docs and OpenAPI only; no authentication or account endpoint was called.\n"
source_yaml_url: https://artifacts.apis.io/conversoriaecnae-es/authentication/conversoriaecnae-es-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Tax
- Spain
- Business Classification
- CNAE
- IAE
- Open Data
- MCP
---
