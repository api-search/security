---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Detectify Authentication
name_suffix: Authentication
oauth_flows: []
overview: detectify secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: detectify
provider_slug: detectify
scheme_count: 1
schemes:
- format: API key (UUID) passed in the Authorization header. Keys are generated on the API keys page in the Detectify dashboard and scoped to a team.
  in: header
  name: ApiKeyAuth
  parameter_name: Authorization
  sources:
  - https://developer.detectify.com/
  type: apiKey
slug: detectify-authentication
source_filename: detectify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.detectify.com/developer/authentication\ndocs: https://docs.detectify.com/developer/authentication\nreference: https://developer.detectify.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: >-\n    API key (UUID) passed in the Authorization header. Keys are generated on the\n    API keys page in the Detectify dashboard and scoped to a team.\n  sources: [https://developer.detectify.com/]\nnotes: >-\n  The Detectify REST API (base https://api.detectify.com/rest/v3) authenticates\n  with a per-team API key supplied in the Authorization header. No OAuth2 / OIDC\n  surface is documented, so no scopes/ artifact is produced.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/detectify/refs/heads/main/authentication/detectify-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Attack Surface Management
- EASM
- Vulnerability Scanning
- DAST
- Application Security
- API Security
---
