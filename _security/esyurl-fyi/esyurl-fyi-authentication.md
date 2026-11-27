---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: esyurl-fyi-auth-api-openapi.yml
  format: yaml
  label: esyURL Auth API
  slug: esyurl-fyi-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-auth-api-openapi.yml
- filename: esyurl-fyi-domain-api-openapi.yml
  format: yaml
  label: esyURL Domain API
  slug: esyurl-fyi-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-domain-api-openapi.yml
- filename: esyurl-fyi-groups-api-openapi.yml
  format: yaml
  label: esyURL Groups API
  slug: esyurl-fyi-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-groups-api-openapi.yml
- filename: esyurl-fyi-links-api-openapi.yml
  format: yaml
  label: esyURL Links API
  slug: esyurl-fyi-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-links-api-openapi.yml
- filename: esyurl-fyi-mcp-api-openapi.yml
  format: yaml
  label: esyURL MCP API
  slug: esyurl-fyi-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-mcp-api-openapi.yml
- filename: esyurl-fyi-me-api-openapi.yml
  format: yaml
  label: esyURL Me API
  slug: esyurl-fyi-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-me-api-openapi.yml
- filename: esyurl-fyi-public-api-openapi.yml
  format: yaml
  label: esyURL Public API
  slug: esyurl-fyi-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-public-api-openapi.yml
- filename: esyurl-fyi-render-api-openapi.yml
  format: yaml
  label: esyURL Render API
  slug: esyurl-fyi-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-render-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: esyURL Authentication
name_suffix: Authentication
oauth_flows: []
overview: esyURL secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: esyURL
provider_slug: esyurl-fyi
scheme_count: 2
schemes:
- description: API key `esy_{keyId}_{secret}`, from an operator or from agent self-sign-up (/auth.md)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/esyurl-fyi-openapi.json
  type: http
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/esyurl-fyi-openapi.json
  type: apiKey
slug: esyurl-fyi-authentication
source_filename: esyurl-fyi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/esyurl-fyi-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key `esy_{keyId}_{secret}`, from an operator or from agent self-sign-up (/auth.md)\n  sources:\n  - openapi/esyurl-fyi-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/esyurl-fyi-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/esyurl-fyi/authentication/esyurl-fyi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Short Links
- QR Codes
- AI Agents
- MCP
---
