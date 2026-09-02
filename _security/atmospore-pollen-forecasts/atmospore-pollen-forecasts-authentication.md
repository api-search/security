---
api_key_in:
- header
- query
api_specs:
- filename: atmospore-pollen-forecasts-pollen-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Pollen API
  slug: atmospore-pollen-forecasts-pollen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-pollen-api-openapi.yml
- filename: atmospore-pollen-forecasts-pollen-area-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Pollen Area API
  slug: atmospore-pollen-forecasts-pollen-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-pollen-area-api-openapi.yml
- filename: atmospore-pollen-forecasts-pollen-top-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Pollen Top API
  slug: atmospore-pollen-forecasts-pollen-top-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-pollen-top-api-openapi.yml
- filename: atmospore-pollen-forecasts-species-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Species API
  slug: atmospore-pollen-forecasts-species-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-species-api-openapi.yml
auth_types:
- apiKey
description: API-key authentication only. One key, one environment, no OAuth, no OIDC, no scopes and no test/live separation. The same key authenticates REST and the hosted MCP server, though the two carry it differently.
kind: authentication
layout: security
method: searched
name: Atmospore Pollen Forecasts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atmospore Pollen Forecasts secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Atmospore Pollen Forecasts
provider_slug: atmospore-pollen-forecasts
scheme_count: 2
schemes:
- applies_to:
  - getPollenForecast
  - getPollenArea
  - getPollenTop
  description: API key from your Atmospore account settings
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/atmospore-pollen-forecasts-openapi-original.json
  surface: rest
  type: apiKey
- alternative:
    in: query
    parameter: key
  endpoint: https://mcp.atmospore.com/mcp
  format: Bearer ak_...
  in: header
  name: MCPBearer
  parameter: Authorization
  sources:
  - https://mcp.atmospore.com/mcp (live JSON-RPC -32001 error, 2026-08-09)
  - https://atmospore.com/article/mcp
  surface: mcp
  type: apiKey
slug: atmospore-pollen-forecasts-authentication
source_filename: atmospore-pollen-forecasts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/atmospore-pollen-forecasts-openapi-original.json\ndocs: https://atmospore.com/api-docs\ndescription: >-\n  API-key authentication only. One key, one environment, no OAuth, no OIDC, no scopes and no\n  test/live separation. The same key authenticates REST and the hosted MCP server, though the two\n  carry it differently.\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  scopes: false\n  mtls: false\n  environments: 1\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: API key from your Atmospore account settings\n    surface: rest\n    applies_to: [getPollenForecast, getPollenArea, getPollenTop]\n    sources:\n      - openapi/atmospore-pollen-forecasts-openapi-original.json\n  - name: MCPBearer\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Bearer ak_...'\n    surface: mcp\n    endpoint: https://mcp.atmospore.com/mcp\n\
  \    alternative: {in: query, parameter: key}\n    sources:\n      - https://mcp.atmospore.com/mcp (live JSON-RPC -32001 error, 2026-08-09)\n      - https://atmospore.com/article/mcp\nunauthenticated_operations:\n  - operationId: getSpecies\n    path: /v1/species\n    declared: 'security: [] in the OpenAPI'\n    verified: '2026-08-09, HTTP 200 with no credentials'\n    note: Species metadata is fully public and cacheable for 24 hours.\nkey_management:\n  issuance: https://atmospore.com/account\n  signup: https://atmospore.com/register\n  free_tier: 3000 requests/month, no credit card\n  observed_prefix: ak_\n  documented_prefix: atmo_\n  prefix_discrepancy: >-\n    The MCP server's own error message says `Bearer ak_...`, while the setup snippet published at\n    https://atmospore.com/article/mcp says `Bearer atmo_your_key_here`. One of the two is wrong.\n  rotation_policy: not published\n  key_scoping: none (a key is all-or-nothing across every operation)\n  expiry: not published\nfailure_modes:\n\
  \  - {status: 401, condition: no x-api-key header, body: '{\"error\":\"Missing API key. Include x-api-key header.\"}', verified: true}\n  - {status: 403, condition: unknown or malformed key, body: '{\"error\":\"Invalid API key\"}', verified: true, retry: never}\ntransport_security:\n  https_required: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: >-\n    No Strict-Transport-Security header on pollenapi.com or atmospore.com — a plaintext first\n    request is not protected against downgrade. See security/atmospore-pollen-forecasts-domain-security.yml.\ngaps:\n  - Key travels in a header on REST and in an Authorization bearer on MCP with no unified statement anywhere.\n  - No scopes, so an integration cannot be granted read-only or single-operation access — every key is total.\n  - No key rotation, expiry or revocation policy published.\n  - No HSTS on the API host.\n  - Documented and actual key prefixes disagree.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/authentication/atmospore-pollen-forecasts-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Weather
- Pollen
- Allergy
- Environmental Data
- Health
- Geospatial
- Forecasting
- Smart Home
- MCP
- OpenAPI
- Norway
- Climate
---
