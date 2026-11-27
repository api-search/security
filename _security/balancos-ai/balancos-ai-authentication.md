---
anonymous_access: false
api_key_in: []
api_specs:
- filename: balancos-ai-bcb-api-openapi.yml
  format: yaml
  label: Balanços.AI BCB API
  slug: balancos-ai-bcb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/balancos-ai/openapi/balancos-ai-bcb-api-openapi.yml
- filename: balancos-ai-cvm-api-openapi.yml
  format: yaml
  label: Balanços.AI CVM API
  slug: balancos-ai-cvm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/balancos-ai/openapi/balancos-ai-cvm-api-openapi.yml
- filename: balancos-ai-empresas-api-openapi.yml
  format: yaml
  label: Balanços.AI Empresas API
  slug: balancos-ai-empresas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/balancos-ai/openapi/balancos-ai-empresas-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Balanços.AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Balanços.AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Balanços.AI
provider_slug: balancos-ai
scheme_count: 1
schemes:
- bearerFormat: bal_live token
  description: 'Authorization header with Bearer token. Token format: bal_live_<43 chars>.'
  errors:
  - code: chave_invalida
    description: Bearer token missing, malformed, invalid or revoked.
    status: 401
  example: Bearer bal_live_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
  headerName: Authorization
  scheme: bearer
  tokenLocation: header
  type: http
slug: balancos-ai-authentication
source_filename: balancos-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://balancos.ai/api/docs\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Authorization header with Bearer token. Token format: bal_live_<43 chars>.\"\n    bearerFormat: \"bal_live token\"\n    tokenLocation: header\n    headerName: Authorization\n    example: \"Bearer bal_live_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\"\n    errors:\n      - status: 401\n        code: chave_invalida\n        description: \"Bearer token missing, malformed, invalid or revoked.\"\n"
source_yaml_url: https://artifacts.apis.io/balancos-ai/authentication/balancos-ai-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Brazil
- Public Data
- Financial Statements
---
