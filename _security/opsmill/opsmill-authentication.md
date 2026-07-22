---
api_key_in:
- header
api_specs:
- filename: opsmill-infrahub-openapi-original.json
  format: json
  label: Infrahub REST API
  slug: infrahub-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-infrahub-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opsmill Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpsMill secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpsMill
provider_slug: opsmill
scheme_count: 2
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/opsmill-infrahub-openapi-original.json
  type: http
- in: header
  name: APIKeyHeader
  parameter: X-INFRAHUB-KEY
  sources:
  - openapi/opsmill-infrahub-openapi-original.json
  type: apiKey
slug: opsmill-authentication
source_filename: opsmill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/opsmill-infrahub-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/opsmill-infrahub-openapi-original.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-INFRAHUB-KEY\n  sources:\n  - openapi/opsmill-infrahub-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/authentication/opsmill-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Infrastructure Saas
- Network Automation
- Source Of Truth
- Data Management
- GraphQL
- DevOps
- Configuration Management
- AIOps
- Open Source
---
