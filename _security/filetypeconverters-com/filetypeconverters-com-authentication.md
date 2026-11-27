---
anonymous_access: false
api_key_in: []
api_specs:
- filename: filetypeconverters-com-batches-api-openapi.yml
  format: yaml
  label: FileType Converters Batches API
  slug: filetypeconverters-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-batches-api-openapi.yml
- filename: filetypeconverters-com-convert-api-openapi.yml
  format: yaml
  label: FileType Converters Convert API
  slug: filetypeconverters-com-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-convert-api-openapi.yml
- filename: filetypeconverters-com-formats-api-openapi.yml
  format: yaml
  label: FileType Converters Formats API
  slug: filetypeconverters-com-formats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-formats-api-openapi.yml
- filename: filetypeconverters-com-jobs-api-openapi.yml
  format: yaml
  label: FileType Converters Jobs API
  slug: filetypeconverters-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-jobs-api-openapi.yml
- filename: filetypeconverters-com-openapi-json-api-openapi.yml
  format: yaml
  label: FileType Converters Openapi.json API
  slug: filetypeconverters-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-openapi-json-api-openapi.yml
- filename: filetypeconverters-com-pairs-api-openapi.yml
  format: yaml
  label: FileType Converters Pairs API
  slug: filetypeconverters-com-pairs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-pairs-api-openapi.yml
- filename: filetypeconverters-com-usage-api-openapi.yml
  format: yaml
  label: FileType Converters Usage API
  slug: filetypeconverters-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-usage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FileType Converters Authentication
name_suffix: Authentication
oauth_flows: []
overview: FileType Converters declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FileType Converters
provider_slug: filetypeconverters-com
scheme_count: 2
schemes:
- description: Workspace API key presented as a bearer token.
  header: Authorization
  key_prefix: ftc_
  prefix: 'Bearer '
  scheme: bearer
  type: http
- description: Alternate header form of the same workspace API key.
  in: header
  key_prefix: ftc_
  name: X-API-Key
  type: apiKey
slug: filetypeconverters-com-authentication
source_filename: filetypeconverters-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filetypeconverters.com/api/authentication\ndocs: https://filetypeconverters.com/api/authentication\nname: FileType Converters authentication\nsummary: >-\n  Protected /api/v1 endpoints require a workspace API key sent as either\n  `Authorization: Bearer $FTC_API_KEY` or `X-API-Key: $FTC_API_KEY`. Public\n  catalog endpoints need no key. API keys start with `ftc_`; MCP tokens start\n  with `ftc_mcp_`.\nschemes:\n  - type: http\n    scheme: bearer\n    header: Authorization\n    prefix: 'Bearer '\n    key_prefix: ftc_\n    description: Workspace API key presented as a bearer token.\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    key_prefix: ftc_\n    description: Alternate header form of the same workspace API key.\nnotes:\n  - API access requires a Starter, Pro, or Scale plan.\n  - MCP tokens (prefix ftc_mcp_) work on API read or convert routes when the token has the matching permission.\n  - Revoked keys\
  \ stop matching immediately; expired keys return UNAUTHORIZED.\n"
source_yaml_url: https://artifacts.apis.io/filetypeconverters-com/authentication/filetypeconverters-com-authentication.yml
summary_line: 2 schemes
tags:
- File Conversion
- Document Conversion
- PDF
- OCR
- Spreadsheets
- Image
- MCP
- Developer API
- AI Deep Read
- File Format
---
