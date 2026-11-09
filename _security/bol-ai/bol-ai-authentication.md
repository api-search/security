---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bol-ai-billing-api-openapi.yml
  format: yaml
  label: Bol.ai Billing API
  slug: bol-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-billing-api-openapi.yml
- filename: bol-ai-bol-api-openapi.yml
  format: yaml
  label: Bol.ai Bol API
  slug: bol-ai-bol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-bol-api-openapi.yml
- filename: bol-ai-mcp-api-openapi.yml
  format: yaml
  label: Bol.ai MCP API
  slug: bol-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-mcp-api-openapi.yml
- filename: bol-ai-me-api-openapi.yml
  format: yaml
  label: Bol.ai Me API
  slug: bol-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-me-api-openapi.yml
- filename: bol-ai-usage-api-openapi.yml
  format: yaml
  label: Bol.ai Usage API
  slug: bol-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bol Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bol.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bol.ai
provider_slug: bol-ai
scheme_count: 1
schemes:
- description: 'Bol.ai API key (bolai_...). Create one in the app: https://bol.ai/app/ — available on the Professional plan or with credits; new accounts include 5 free documents.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/bol-ai-openapi.yml
  type: http
slug: bol-ai-authentication
source_filename: bol-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bol-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'Bol.ai API key (bolai_...). Create one in the app: https://bol.ai/app/ — available\n    on the Professional plan or with credits; new accounts include 5 free documents.'\n  sources:\n  - openapi/bol-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/bol-ai/authentication/bol-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Freight Documents
- Data Extraction
- Bill of Lading
- 3PL
---
