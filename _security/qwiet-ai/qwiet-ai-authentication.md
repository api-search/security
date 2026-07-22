---
api_key_in: []
api_specs:
- filename: qwiet-ai-openapi-original.yml
  format: yaml
  label: Qwiet AI API v4
  slug: qwiet-ai-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwiet-ai/refs/heads/main/openapi/qwiet-ai-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Qwiet Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qwiet Ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qwiet Ai
provider_slug: qwiet-ai
scheme_count: 1
schemes:
- description: 'Use of the Qwiet API requires an access token, which is available via the Qwiet Dashboard (either under [Account Settings](https://app.shiftleft.io/user/profile) or [Integration Tokens](https://app.shiftleft.io/integrations)) or via the `/tokens` endpoints. You can pass an access token to the API using the HTTP `Authorization` Request header as follows:\

    `Authorization: Bearer {access token}`'
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/qwiet-ai-openapi-original.yml
  type: http
slug: qwiet-ai-authentication
source_filename: qwiet-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/qwiet-ai-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: |-\n    Use of the Qwiet API requires an access token, which is available via the Qwiet Dashboard (either under [Account Settings](https://app.shiftleft.io/user/profile) or [Integration Tokens](https://app.shiftleft.io/integrations)) or via the `/tokens` endpoints. You can pass an access token to the API using the HTTP `Authorization` Request header as follows:\\\n    `Authorization: Bearer {access token}`\n  sources:\n  - openapi/qwiet-ai-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwiet-ai/refs/heads/main/authentication/qwiet-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Application Security
- SAST
- SCA
- Code Security
- Vulnerability Management
- DevSecOps
- AutoFix
---
