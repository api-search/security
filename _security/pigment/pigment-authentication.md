---
api_key_in: []
api_specs:
- filename: pigment-applicationapi-api-openapi.yml
  format: yaml
  label: Pigment ApplicationApi API
  slug: pigment-applicationapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-applicationapi-api-openapi.yml
- filename: pigment-blocksapi-api-openapi.yml
  format: yaml
  label: Pigment BlocksApi API
  slug: pigment-blocksapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-blocksapi-api-openapi.yml
- filename: pigment-export-api-openapi.yml
  format: yaml
  label: Pigment Export API
  slug: pigment-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-export-api-openapi.yml
- filename: pigment-exportv1-api-openapi.yml
  format: yaml
  label: Pigment ExportV1 API
  slug: pigment-exportv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-exportv1-api-openapi.yml
- filename: pigment-importapi-api-openapi.yml
  format: yaml
  label: Pigment ImportApi API
  slug: pigment-importapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-importapi-api-openapi.yml
- filename: pigment-importconfigurationapi-api-openapi.yml
  format: yaml
  label: Pigment ImportConfigurationApi API
  slug: pigment-importconfigurationapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-importconfigurationapi-api-openapi.yml
- filename: pigment-importv1-api-openapi.yml
  format: yaml
  label: Pigment ImportV1 API
  slug: pigment-importv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-importv1-api-openapi.yml
- filename: pigment-viewapi-api-openapi.yml
  format: yaml
  label: Pigment ViewApi API
  slug: pigment-viewapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-viewapi-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pigment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pigment secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pigment
provider_slug: pigment
scheme_count: 1
schemes:
- bearerFormat: ApiKey
  description: API Key Authorization header using the Bearer scheme.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/pigment-external-api-openapi.json
  type: http
slug: pigment-authentication
source_filename: pigment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/pigment-external-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ApiKey\n  description: API Key Authorization header using the Bearer scheme.\n  sources:\n  - openapi/pigment-external-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/authentication/pigment-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise Software
- Business Planning
- Financial Planning
- FP&A
- Analytics
- EPM
- Data Integration
- MCP
- SCIM
---
