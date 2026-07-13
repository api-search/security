---
api_key_in:
- header
api_specs:
- filename: uniblock-unified-api-openapi.yml
  format: yaml
  label: Uniblock Unified API
  slug: unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/openapi/uniblock-unified-api-openapi.yml
- filename: uniblock-direct-api-openapi.yml
  format: yaml
  label: Uniblock Direct API
  slug: direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/openapi/uniblock-direct-api-openapi.yml
- filename: uniblock-json-rpc-api-openapi.yml
  format: yaml
  label: Uniblock JSON-RPC API
  slug: json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/openapi/uniblock-json-rpc-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uniblock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uniblock secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uniblock
provider_slug: uniblock
scheme_count: 1
schemes:
- description: Uniblock project API key passed as a header. If no provider-specific authentication is passed in the request, Uniblock will use the credentials stored in the project associated with this API key.
  in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/uniblock-direct-api-openapi.yml
  - openapi/uniblock-json-rpc-api-openapi.yml
  - openapi/uniblock-unified-api-openapi.yml
  type: apiKey
slug: uniblock-authentication
source_filename: uniblock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uniblock-direct-api-openapi.yml, openapi/uniblock-json-rpc-api-openapi.yml,\n  openapi/uniblock-unified-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Uniblock project API key passed as a header. If no provider-specific authentication\n    is passed in the request, Uniblock will use the credentials stored in the project associated\n    with this API key.\n  sources:\n  - openapi/uniblock-direct-api-openapi.yml\n  - openapi/uniblock-json-rpc-api-openapi.yml\n  - openapi/uniblock-unified-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/authentication/uniblock-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Web3
---
