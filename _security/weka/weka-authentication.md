---
api_key_in: []
api_specs:
- filename: weka-openapi-original.json
  format: json
  label: WEKA REST API
  slug: weka-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weka/refs/heads/main/openapi/weka-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Weka Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weka secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weka
provider_slug: weka
scheme_count: 1
schemes:
- bearerFormat: JWT
  docs: https://docs.weka.io/security/obtain-authentication-tokens.md
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/weka-openapi-original.json
  type: http
slug: weka-authentication
source_filename: weka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/weka-openapi-original.json\ndocs: https://docs.weka.io/security/obtain-authentication-tokens.md\nsummary:\n  types:\n  - http\n  model: JWT bearer token obtained from the cluster login endpoint\n  token_endpoint: POST /api/v2/login\n  refresh_endpoint: POST /api/v2/login/refresh\n  access_token_ttl: 5 minutes (default; configurable)\n  refresh_token_ttl: 1 month (default; configurable)\n  long_lived_tokens: supported for local users (GUI/CLI API Token)\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  docs: https://docs.weka.io/security/obtain-authentication-tokens.md\n  sources:\n  - openapi/weka-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weka/refs/heads/main/authentication/weka-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Storage
- Data Platform
- High Performance Computing
- File System
- Object Storage
- Kubernetes
- Cloud Infrastructure
---
