---
api_key_in: []
api_specs:
- filename: capy-openapi-original.json
  format: json
  label: Capy API
  slug: capy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Capy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Capy
provider_slug: capy
scheme_count: 1
schemes:
- description: API token (capy_xxxx). Generate at capy.ai/settings/tokens
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/capy-openapi-original.json
  token_prefix: capy_
  type: http
slug: capy-authentication
source_filename: capy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/capy-openapi-original.json\ndocs: https://docs.capy.ai/api-reference/overview\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_format: capy_xxxx\n  header: 'Authorization: Bearer [example key]'\n  token_management: https://capy.ai/settings/tokens\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API token (capy_xxxx). Generate at capy.ai/settings/tokens\n  token_prefix: capy_\n  sources:\n  - openapi/capy-openapi-original.json\nnotes:\n- Session identity tokens (verifySession / getThreadSessionToken) are a separate,\n  short-lived token issued per captain session and written inside the VM at\n  /etc/capy/session-token (mode 0600); they are not API auth credentials but let\n  code prove a request came from a genuine Capy session.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/authentication/capy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- AI Coding Agent
- Software Engineering
- Developer Tools
- Automation
- Code Review
- DevOps
---
