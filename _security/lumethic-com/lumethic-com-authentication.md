---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: lumethic-com-api-keys-api-openapi.yml
  format: yaml
  label: Lumethic API Keys API
  slug: lumethic-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumethic-com/openapi/lumethic-com-api-keys-api-openapi.yml
- filename: lumethic-com-marketplace-api-openapi.yml
  format: yaml
  label: Lumethic Marketplace API
  slug: lumethic-com-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumethic-com/openapi/lumethic-com-marketplace-api-openapi.yml
- filename: lumethic-com-public-access-api-openapi.yml
  format: yaml
  label: Lumethic Public Access API
  slug: lumethic-com-public-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumethic-com/openapi/lumethic-com-public-access-api-openapi.yml
- filename: lumethic-com-requests-api-openapi.yml
  format: yaml
  label: Lumethic Requests API
  slug: lumethic-com-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumethic-com/openapi/lumethic-com-requests-api-openapi.yml
- filename: lumethic-com-tags-api-openapi.yml
  format: yaml
  label: Lumethic Tags API
  slug: lumethic-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumethic-com/openapi/lumethic-com-tags-api-openapi.yml
- filename: lumethic-com-verifications-api-openapi.yml
  format: yaml
  label: Lumethic Verifications API
  slug: lumethic-com-verifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumethic-com/openapi/lumethic-com-verifications-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Lumethic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumethic secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lumethic
provider_slug: lumethic-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token from POST /v1/accounts/login
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lumethic-com-openapi.json
  type: http
- description: 'API key from POST /v1/apikeys/. Format: ask_<43 url-safe characters>'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/lumethic-com-openapi.json
  type: apiKey
slug: lumethic-com-authentication
source_filename: lumethic-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lumethic-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token from POST /v1/accounts/login\n  sources:\n  - openapi/lumethic-com-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key from POST /v1/apikeys/. Format: ask_<43 url-safe characters>'\n  sources:\n  - openapi/lumethic-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lumethic-com/authentication/lumethic-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- PhotoVerification
- ImageAuthentication
- AI Detection
- ForensicAnalysis
- MediaIntegrity
---
