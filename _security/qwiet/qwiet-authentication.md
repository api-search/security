---
api_key_in: []
api_specs:
- filename: qwiet-api-original.yml
  format: yaml
  label: Qwiet API
  slug: qwiet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwiet/refs/heads/main/openapi/qwiet-api-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qwiet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qwiet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qwiet
provider_slug: qwiet
scheme_count: 1
schemes:
- description: 'Use of the Qwiet API requires an access token, which is available via the Qwiet Dashboard (either under [Account Settings](https://app.shiftleft.io/user/profile) or [Integration Tokens](https://app.shiftleft.io/integrations)) or via the `/tokens` endpoints. You can pass an access token to the API using the HTTP `Authorization` Request header as follows:\

    `Authorization: Bearer {access token}`'
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/qwiet-api-original.yml
  type: http
slug: qwiet-authentication
source_filename: qwiet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/qwiet-api-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: |-\n    Use of the Qwiet API requires an access token, which is available via the Qwiet Dashboard (either under [Account Settings](https://app.shiftleft.io/user/profile) or [Integration Tokens](https://app.shiftleft.io/integrations)) or via the `/tokens` endpoints. You can pass an access token to the API using the HTTP `Authorization` Request header as follows:\\\n    `Authorization: Bearer {access token}`\n  sources:\n  - openapi/qwiet-api-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwiet/refs/heads/main/authentication/qwiet-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Application Security
- SAST
- SCA
- Vulnerability Management
- DevSecOps
- Code Analysis
- MCP
---
