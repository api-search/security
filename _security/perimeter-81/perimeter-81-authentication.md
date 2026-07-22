---
api_key_in: []
api_specs:
- filename: perimeter-81-openapi-original.json
  format: json
  label: Harmony SASE Public API
  slug: harmony-sase-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perimeter-81/refs/heads/main/openapi/perimeter-81-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Perimeter 81 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perimeter 81 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Perimeter 81
provider_slug: perimeter-81
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/perimeter-81-openapi-original.json
  type: http
slug: perimeter-81-authentication
source_filename: perimeter-81-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/perimeter-81-openapi-original.json\ndocs: https://support.perimeter81.com/docs/api-getting-started\nsummary:\n  types:\n  - http\n  model: two-step (API key -> time-based JWT access token)\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/perimeter-81-openapi-original.json\nflow:\n  description: >-\n    Harmony SASE (Perimeter 81) uses two-step secure tokens. A long-lived API key is\n    generated in the Web Management Console (Settings -> API Support -> Generate New Key)\n    with a chosen expiration date and a set of selected key permissions (e.g. 'View list\n    of users', 'Add new members', 'Delete groups'). The API key is then exchanged for a\n    short-lived JWT access token that is sent as an HTTP bearer token on every request.\n  steps:\n  - step: 1\n    action: Generate an API key in the Web Management Console (Settings -> API Support).\n    note: Requires\
  \ Premium Plus or Enterprise plan; key carries selected permissions and an expiration date.\n  - step: 2\n    action: 'POST /v1/auth/authorize with body {grantType: \"api_key\", apiKey: <API_KEY>} to obtain an access token.'\n    endpoint: POST https://api.perimeter81.com/api/v1/auth/authorize\n    docs: https://support.perimeter81.com/docs/access-token-post\n  - step: 3\n    action: \"Send the access token as 'Authorization: Bearer <access_token>' on all API calls.\"\n    note: Access token expires 60 minutes after issue; regenerate via the authorize endpoint.\npermissions_model: >-\n  Key-scoped permissions are chosen at API-key generation time in the console (not OAuth2 scopes).\n  No oauth2 securityScheme is declared in the OpenAPI, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perimeter-81/refs/heads/main/authentication/perimeter-81-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cybersecurity
- SASE
- Zero Trust
- Networking
- VPN
- ZTNA
- Security
- Cloud Security
---
