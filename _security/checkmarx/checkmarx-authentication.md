---
api_key_in: []
api_specs:
- filename: 34965-8158-rest-api.html
  format: yaml
  label: Checkmarx SAST API
  slug: checkmarx-sast-api
  spec_type: OpenAPI
  url: https://checkmarx.com/resource/documents/en/34965-8158-rest-api.html
- filename: checkmarx-sca-openapi.yml
  format: yaml
  label: Checkmarx SCA API
  slug: checkmarx-sca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-sca-openapi.yml
- filename: checkmarx-one-openapi.yml
  format: yaml
  label: Checkmarx One API
  slug: checkmarx-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-one-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Checkmarx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkmarx secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Checkmarx
provider_slug: checkmarx
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained via client credentials from the Checkmarx One IAM service
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/checkmarx-one-openapi.yml
  - openapi/checkmarx-sast-openapi.yml
  - openapi/checkmarx-sca-openapi.yml
  type: http
slug: checkmarx-authentication
source_filename: checkmarx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkmarx-one-openapi.yml, openapi/checkmarx-sast-openapi.yml, openapi/checkmarx-sca-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained via client credentials from the Checkmarx One\n    IAM service\n  sources:\n  - openapi/checkmarx-one-openapi.yml\n  - openapi/checkmarx-sast-openapi.yml\n  - openapi/checkmarx-sca-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/authentication/checkmarx-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Security
- Code Analysis
- DevSecOps
- SAST
- Security Testing
- Vulnerability Scanning
---
