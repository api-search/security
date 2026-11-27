---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: contracko-com-authentication-api-openapi.yml
  format: yaml
  label: Contracko Authentication API
  slug: contracko-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contracko-com/openapi/contracko-com-authentication-api-openapi.yml
- filename: contracko-com-contract-types-api-openapi.yml
  format: yaml
  label: Contracko Contract Types API
  slug: contracko-com-contract-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contracko-com/openapi/contracko-com-contract-types-api-openapi.yml
- filename: contracko-com-parsing-api-api-openapi.yml
  format: yaml
  label: Contracko Parsing API
  slug: contracko-com-parsing-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contracko-com/openapi/contracko-com-parsing-api-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Contracko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contracko secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Contracko
provider_slug: contracko-com
scheme_count: 2
schemes:
- description: Contracko integration API key. Issue keys from Settings → Integrations → API keys.
  in: header
  name: ContrackoApiKey
  parameter: x-contracko-api-key
  sources:
  - openapi/contracko-com-openapi.yml
  type: apiKey
- bearerFormat: opaque
  description: 'Pass your Contracko integration API key as a bearer token: `Authorization: Bearer <key>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/contracko-com-openapi.yml
  type: http
slug: contracko-com-authentication
source_filename: contracko-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://contracko.com/api/developers/llms.txt\ndocs: https://contracko.com/developers/api/parsing/reference\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ContrackoApiKey\n  type: apiKey\n  in: header\n  parameter: x-contracko-api-key\n  description: Contracko integration API key. Issue keys from Settings → Integrations\n    → API keys.\n  sources:\n  - openapi/contracko-com-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: 'Pass your Contracko integration API key as a bearer token: `Authorization:\n    Bearer <key>`.'\n  sources:\n  - openapi/contracko-com-openapi.yml\nkey_scopes:\n  note: API keys carry scopes, returned by GET /health (operationId health) in `scopes`.\n    See scopes/contracko-com-scopes.yml.\n  docs: https://contracko.com/api/developers/llms.txt\nmcp_server:\n  endpoint: https://app.contracko.com/mcp\n  schemes:\n\
  \  - type: oauth2\n    note: Browser sign-in (OAuth) is the recommended connection; Read and Write are\n      separate permissions approved at connect time; reconnecting rotates the grant.\n  - type: http\n    scheme: bearer\n    note: Dedicated MCP API key created in Settings → Integrations → API keys, sent\n      in the Authorization Bearer header. Only owners and admins can create, change\n      or revoke API keys.\n  source: https://contracko.com/docs/mcp-server\n"
source_yaml_url: https://artifacts.apis.io/contracko-com/authentication/contracko-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Contract Management
- Legal Tech
- Artificial Intelligence
- Document Parsing
- Data Extraction
- E-Signature
- MCP
---
