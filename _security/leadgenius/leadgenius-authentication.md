---
api_key_in:
- header
api_specs:
- filename: leadgenius-enrichment-api-openapi.yml
  format: yaml
  label: LeadGenius Enrichment API
  slug: leadgenius-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadgenius/refs/heads/main/openapi/leadgenius-enrichment-api-openapi.yml
auth_types:
- apiKey
description: LeadGenius authenticates every API request with a single account API key sent in the Authorization header using the `Token` scheme. There is no OAuth, no OpenID Connect, no scope surface and no per-request signing. Derived from the captured OpenAPI securitySchemes and upgraded from the published authentication section of the API reference.
kind: authentication
layout: security
method: searched
name: Leadgenius Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeadGenius secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LeadGenius
provider_slug: leadgenius
scheme_count: 1
schemes:
- description: 'LeadGenius uses API keys to allow access to the API. The key must be included in all API requests to the server in a header of the form `Authorization: Token {apikey}`, alongside `Content-Type: application/json`.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/leadgenius-enrichment-api-openapi.yml
  - https://docs.leadgenius.com/#authentication
  type: apiKey
  value_format: Token {apikey}
slug: leadgenius-authentication
source_filename: leadgenius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/leadgenius-enrichment-api-openapi.yml\ndocs: https://docs.leadgenius.com/#authentication\ndescription: >-\n  LeadGenius authenticates every API request with a single account API key sent in the Authorization\n  header using the `Token` scheme. There is no OAuth, no OpenID Connect, no scope surface and no\n  per-request signing. Derived from the captured OpenAPI securitySchemes and upgraded from the\n  published authentication section of the API reference.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  scopes: none\nschemes:\n  - name: TokenAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    value_format: 'Token {apikey}'\n    description: >-\n      LeadGenius uses API keys to allow access to the API. The key must be included in all API\n      requests to the server in a header of the form `Authorization: Token {apikey}`, alongside\n      `Content-Type: application/json`.\n\
  \    sources:\n      - openapi/leadgenius-enrichment-api-openapi.yml\n      - https://docs.leadgenius.com/#authentication\nprovisioning:\n  self_serve: https://app.leadgenius.com/sign-up\n  self_serve_note: >-\n    LeadGenius launched a self-serve API trial in 2026 — registering issues an API key without human\n    interaction. See\n    https://www.leadgenius.com/resources/introducing-the-new-leadgenius-api-experience-real-time-enrichment-zero-bottlenecks\n  sales: sales@leadgenius.com\n  sales_note: >-\n    LeadGenius customers may also contact Sales or their Customer Success rep for an API subscription\n    and key.\n  login: https://app.leadgenius.com/sign-in\nrotation:\n  documented: false\nkey_scoping:\n  documented: false\n  note: A single account-level key; no restricted or publishable key classes are documented.\nerrors:\n  invalid_key:\n    status: 401\n    meaning: Unauthorized -- Your API key is invalid.\nrelated:\n  conventions: conventions/leadgenius-conventions.yml\n  errors:\
  \ errors/leadgenius-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadgenius/refs/heads/main/authentication/leadgenius-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Enrichment
- Lead Generation
- Sales
- Marketing
- B2B Data
- Contact Data
- Firmographics
- Go To Market
- Account Based Marketing
---
