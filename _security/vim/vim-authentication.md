---
api_key_in: []
api_specs:
- filename: vim-data-source-openapi-original.json
  format: json
  label: Vim Data Source
  slug: vim-data-source
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-data-source-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Vim Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Vim secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Vim
provider_slug: vim
scheme_count: 2
schemes:
- flows:
  - flow: implicit
    scopes: 0
  name: service
  sources:
  - openapi/vim-data-source-openapi-original.json
  type: oauth2
- bearerFormat: JWT
  description: Bearer authentication token obtained from the /oauth/token endpoint
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vim-data-source-openapi-original.json
  type: http
slug: vim-authentication
source_filename: vim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/vim-data-source-openapi-original.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: service\n  type: oauth2\n  flows:\n  - flow: implicit\n    scopes: 0\n  sources:\n  - openapi/vim-data-source-openapi-original.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer authentication token obtained from the /oauth/token endpoint\n  sources:\n  - openapi/vim-data-source-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/authentication/vim-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Healthcare
- United States
- Clinical AI
- EHR Integration
- Point of Care
- Interoperability
- Value-Based Care
- Care Gaps
- OAuth
---
