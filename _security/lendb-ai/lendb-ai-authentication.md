---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: lendb-ai-keys-api-openapi.yml
  format: yaml
  label: LenDb.ai Keys API
  slug: lendb-ai-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lendb-ai/openapi/lendb-ai-keys-api-openapi.yml
- filename: lendb-ai-lenders-api-openapi.yml
  format: yaml
  label: LenDb.ai Lenders API
  slug: lendb-ai-lenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lendb-ai/openapi/lendb-ai-lenders-api-openapi.yml
- filename: lendb-ai-loan-officers-api-openapi.yml
  format: yaml
  label: LenDb.ai Loan Officers API
  slug: lendb-ai-loan-officers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lendb-ai/openapi/lendb-ai-loan-officers-api-openapi.yml
- filename: lendb-ai-match-api-openapi.yml
  format: yaml
  label: LenDb.ai Match API
  slug: lendb-ai-match-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lendb-ai/openapi/lendb-ai-match-api-openapi.yml
- filename: lendb-ai-specialties-api-openapi.yml
  format: yaml
  label: LenDb.ai Specialties API
  slug: lendb-ai-specialties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lendb-ai/openapi/lendb-ai-specialties-api-openapi.yml
- filename: lendb-ai-stats-api-openapi.yml
  format: yaml
  label: LenDb.ai Stats API
  slug: lendb-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lendb-ai/openapi/lendb-ai-stats-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: LenDb.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: LenDb.ai secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LenDb.ai
provider_slug: lendb-ai
scheme_count: 2
schemes:
- description: Free API key, ldb_live_... Optional.
  name: bearerKey
  scheme: bearer
  sources:
  - openapi/lendb-ai-openapi.yml
  type: http
- description: 'Deprecated: the same key as a query parameter. Prefer the Authorization header; keys in URLs end up in logs and history. Not accepted by /mcp.'
  in: query
  name: queryKey
  parameter: api_key
  sources:
  - openapi/lendb-ai-openapi.yml
  type: apiKey
slug: lendb-ai-authentication
source_filename: lendb-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/lendb-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerKey\n  type: http\n  scheme: bearer\n  description: Free API key, ldb_live_... Optional.\n  sources:\n  - openapi/lendb-ai-openapi.yml\n- name: queryKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: 'Deprecated: the same key as a query parameter. Prefer the Authorization header;\n    keys in URLs end up in logs and history. Not accepted by /mcp.'\n  sources:\n  - openapi/lendb-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/lendb-ai/authentication/lendb-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Mortgage
- Loan Officers
- Artificial Intelligence
- Data
---
