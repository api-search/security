---
api_key_in:
- header
api_specs:
- filename: emerge-tools-analysis-api-openapi.yml
  format: yaml
  label: Emerge Tools Analysis API
  slug: emerge-tools-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-analysis-api-openapi.yml
- filename: emerge-tools-apphistory-api-openapi.yml
  format: yaml
  label: Emerge Tools AppHistory API
  slug: emerge-tools-apphistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-apphistory-api-openapi.yml
- filename: emerge-tools-builddetails-api-openapi.yml
  format: yaml
  label: Emerge Tools BuildDetails API
  slug: emerge-tools-builddetails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-builddetails-api-openapi.yml
- filename: emerge-tools-comment-api-openapi.yml
  format: yaml
  label: Emerge Tools Comment API
  slug: emerge-tools-comment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-comment-api-openapi.yml
- filename: emerge-tools-deadcode-api-openapi.yml
  format: yaml
  label: Emerge Tools DeadCode API
  slug: emerge-tools-deadcode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-deadcode-api-openapi.yml
- filename: emerge-tools-getperftest-api-openapi.yml
  format: yaml
  label: Emerge Tools GetPerfTest API
  slug: emerge-tools-getperftest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-getperftest-api-openapi.yml
- filename: emerge-tools-snapshots-api-openapi.yml
  format: yaml
  label: Emerge Tools Snapshots API
  slug: emerge-tools-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-snapshots-api-openapi.yml
- filename: emerge-tools-trace-api-openapi.yml
  format: yaml
  label: Emerge Tools Trace API
  slug: emerge-tools-trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-trace-api-openapi.yml
- filename: emerge-tools-upload-api-openapi.yml
  format: yaml
  label: Emerge Tools Upload API
  slug: emerge-tools-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-upload-api-openapi.yml
- filename: emerge-tools-uploadfromlink-api-openapi.yml
  format: yaml
  label: Emerge Tools UploadFromLink API
  slug: emerge-tools-uploadfromlink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-uploadfromlink-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Emerge Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emerge Tools secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Emerge Tools
provider_slug: emerge-tools
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Token
  sources:
  - openapi/emerge-tools-openapi.json
  type: apiKey
slug: emerge-tools-authentication
source_filename: emerge-tools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/emerge-tools-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Token\n  sources:\n  - openapi/emerge-tools-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/authentication/emerge-tools-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- B2B
- Mobile
- Developer Tools
- App Performance
- Testing
- iOS
- Android
- DevOps
---
